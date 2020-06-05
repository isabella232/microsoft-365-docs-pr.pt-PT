---
title: Permitir que dispositivos Windows 10 unidos por domínio sejam geridos pela Microsoft 365 para negócios
f1.keywords:
- CSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Saiba como permitir que o Microsoft 365 proteja os dispositivos locais do Windows 10, aderidos ao Active-Directory, em apenas alguns passos.
ms.openlocfilehash: 857651081fb10856d28dd419333ebef655388407
ms.sourcegitcommit: e6e704cbd9a50fc7db1e6a0cf5d3f8c6cbb94363
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/04/2020
ms.locfileid: "44564958"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="ca979-103">Permitir que dispositivos Windows 10 unidos por domínio sejam geridos pelo Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="ca979-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="ca979-104">Se a sua organização utilizar o Windows Server Ative Directory no local, pode configurar o Microsoft 365 Business Premium para proteger os seus dispositivos Windows 10, mantendo ao mesmo tempo o acesso a recursos no local que requerem autenticação local.</span><span class="sxs-lookup"><span data-stu-id="ca979-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="ca979-105">Para configurar esta proteção, pode implementar **dispositivos híbridos Azure AD.**</span><span class="sxs-lookup"><span data-stu-id="ca979-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="ca979-106">Estes dispositivos estão ligados tanto ao seu Ative Directory como ao seu Diretório Ativo Azure.</span><span class="sxs-lookup"><span data-stu-id="ca979-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="ca979-107">Este vídeo descreve os passos para como configurar isto para o cenário mais comum, que também é detalhado nos passos que se seguem.</span><span class="sxs-lookup"><span data-stu-id="ca979-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="ca979-108">Antes de começar, certifique-se de completar estes passos:</span><span class="sxs-lookup"><span data-stu-id="ca979-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="ca979-109">Sincronizar os utilizadores para Azure AD com Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="ca979-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="ca979-110">Sincronização completa da Unidade Organizacional de Ligação Azure (OU).</span><span class="sxs-lookup"><span data-stu-id="ca979-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="ca979-111">Certifique-se de que todos os utilizadores de domínio sincronizados têm licenças para o Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="ca979-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="ca979-112">Consulte [os utilizadores de domínio sincronizados com a Microsoft](manage-domain-users.md) para os passos.</span><span class="sxs-lookup"><span data-stu-id="ca979-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="ca979-113">1. Verificar a Autoridade MDM em Intune</span><span class="sxs-lookup"><span data-stu-id="ca979-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="ca979-114">Vá a portal.azure.com e no topo da pesquisa de página para Intune.</span><span class="sxs-lookup"><span data-stu-id="ca979-114">Go to portal.azure.com and on the top of the page search for Intune.</span></span>
<span data-ttu-id="ca979-115">Na página Microsoft Intune, selecione **a inscrição** do Dispositivo e na página **'Vista Geral'** certifique-se de que **a autoridade MDM** é **Intune**.</span><span class="sxs-lookup"><span data-stu-id="ca979-115">On the Microsoft Intune page, select **Device enrollment** and on the **Overview** page make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="ca979-116">Se **a autoridade do MDM** não for **nenhuma,** clique na **autoridade do MDM** para defini-la para **Intune**.</span><span class="sxs-lookup"><span data-stu-id="ca979-116">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="ca979-117">Se **a autoridade do MDM** for o Microsoft Office **365,** vá aos **Devices**  >  **dispositivos de inscrição** de dispositivos e use o diálogo **da autoridade Add MDM** no direito de adicionar a autoridade **Intune MDM** (o diálogo da Autoridade add **MDM** só está disponível se a **Autoridade MDM** estiver definida para o Microsoft Office 365).</span><span class="sxs-lookup"><span data-stu-id="ca979-117">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="ca979-118">2. Verifique se a Azure AD está ativada para unir computadores</span><span class="sxs-lookup"><span data-stu-id="ca979-118">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="ca979-119">Vá ao centro de administração <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> e selecione **Azure Ative Directory** (selecione Mostrar tudo se o Diretório Ativo Azure não estiver visível) na lista de **centros de administração.**</span><span class="sxs-lookup"><span data-stu-id="ca979-119">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="ca979-120">No **centro de administração Azure Ative,** vá ao **Azure Ative Directory,** escolha **Dispositivos** e, em seguida, **configurações do Dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="ca979-120">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="ca979-121">Verifique se**os utilizadores podem juntar-se a dispositivos para Azure AD** está ativado</span><span class="sxs-lookup"><span data-stu-id="ca979-121">Verify**Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="ca979-122">Para ativar todos os utilizadores, desa um pouco de **tudo**.</span><span class="sxs-lookup"><span data-stu-id="ca979-122">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="ca979-123">Para permitir utilizadores específicos, desatado para **selecionar** para permitir um grupo específico de utilizadores.</span><span class="sxs-lookup"><span data-stu-id="ca979-123">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="ca979-124">Adicione os utilizadores de domínio desejado sincronizados em Azure AD a um [grupo de segurança](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="ca979-124">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="ca979-125">Escolha **Grupos Selecionados** para ativar o âmbito do utilizador MDM para esse grupo de segurança.</span><span class="sxs-lookup"><span data-stu-id="ca979-125">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="ca979-126">3. Verifique se a Azure AD está ativada para o MDM</span><span class="sxs-lookup"><span data-stu-id="ca979-126">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="ca979-127">Vá ao centro de administração <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> e selecione **Endpoint Managemen**t (selecione **Mostrar tudo** se **o Endpoint Manager** não estiver visível)</span><span class="sxs-lookup"><span data-stu-id="ca979-127">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen**t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="ca979-128">No **centro de administração do Microsoft Endpoint Manager,** aceda a **Inscrições**  >  **Windows**  >  Automáticas de**Inscrição**  >  **no**Windows do Windows .</span><span class="sxs-lookup"><span data-stu-id="ca979-128">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="ca979-129">Verifique se o âmbito do utilizador DO MDM está ativado.</span><span class="sxs-lookup"><span data-stu-id="ca979-129">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="ca979-130">Para inscrever todos os computadores, descreva para **All** para inscrever automaticamente todos os computadores de utilizador que se unem ao Azure AD e aos novos computadores quando os utilizadores adicionarem uma conta de trabalho ao Windows.</span><span class="sxs-lookup"><span data-stu-id="ca979-130">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="ca979-131">Definir para **Alguns** para inscrever os computadores de um grupo específico de utilizadores.</span><span class="sxs-lookup"><span data-stu-id="ca979-131">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="ca979-132">Adicione os utilizadores de domínio desejado sincronizados em Azure AD a um [grupo de segurança](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="ca979-132">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="ca979-133">Escolha **Grupos Selecionados** para ativar o âmbito do utilizador MDM para esse grupo de segurança.</span><span class="sxs-lookup"><span data-stu-id="ca979-133">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-set-up-service-connection-point-scp"></a><span data-ttu-id="ca979-134">4. Configurar o ponto de ligação de serviço (SCP)</span><span class="sxs-lookup"><span data-stu-id="ca979-134">4. Set up Service connection point (SCP)</span></span>

<span data-ttu-id="ca979-135">Estes passos são simplificados a partir da [configuração híbrida azure ad join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span><span class="sxs-lookup"><span data-stu-id="ca979-135">These steps are simplified from [configure hybrid azure AD join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span></span> <span data-ttu-id="ca979-136">Para completar os passos, precisa de utilizar o Azure AD Connect e as suas palavras-passe de administração global e de administração de administração do Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="ca979-136">To complete the steps you need to use Azure AD Connect and your Microsoft 365 Business Premium global admin and Active Directory admin passwords.</span></span>

1.  <span data-ttu-id="ca979-137">Inicie o Azure AD Connect e, em seguida, selecione **Configure**.</span><span class="sxs-lookup"><span data-stu-id="ca979-137">Start Azure AD Connect, and then select **Configure**.</span></span>
2.  <span data-ttu-id="ca979-138">Na página **de tarefas adicionais,** selecione **opções do dispositivo configurar**e, em seguida, selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="ca979-138">On the **Additional tasks**  page, select **Configure device options**, and then select **Next**.</span></span>
3.  <span data-ttu-id="ca979-139">Na página **'Vista Geral',** selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="ca979-139">On the **Overview** page, select **Next**.</span></span>
4.  <span data-ttu-id="ca979-140">Na página **Connect to Azure AD,** insira as credenciais de um administrador global para o Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="ca979-140">On the **Connect to Azure AD** page, enter the credentials of a global administrator for Microsoft 365 Business Premium.</span></span>
5.  <span data-ttu-id="ca979-141">Na página de opções do **Dispositivo,** selecione **Configure Hybrid Azure AD ,** e, em seguida, selecione **Next**.</span><span class="sxs-lookup"><span data-stu-id="ca979-141">On the **Device options** page, select **Configure Hybrid Azure AD join**, and then select **Next**.</span></span>
6.  <span data-ttu-id="ca979-142">Na página **SCP,** para cada floresta onde deseja Azure AD Connect para configurar o SCP, complete os seguintes passos e, em seguida, selecione **Seguinte**:</span><span class="sxs-lookup"><span data-stu-id="ca979-142">On the **SCP** page, for each forest where you want Azure AD Connect to configure the SCP, complete the following steps, and then select **Next**:</span></span>
    - <span data-ttu-id="ca979-143">Verifique a caixa ao lado do nome da floresta.</span><span class="sxs-lookup"><span data-stu-id="ca979-143">Check the box beside the forest name.</span></span> <span data-ttu-id="ca979-144">A floresta deve ser o seu nome de domínio AD.</span><span class="sxs-lookup"><span data-stu-id="ca979-144">The forest should be your AD domain name.</span></span>
    - <span data-ttu-id="ca979-145">Sob a coluna **Serviço de Autenticação,** abra o dropdown e selecione o nome de domínio correspondente (deve haver apenas uma opção).</span><span class="sxs-lookup"><span data-stu-id="ca979-145">Under the **Authentication Service** column, open the dropdown and select matching domain name (there should only be one only option).</span></span>
    - <span data-ttu-id="ca979-146">**Selecione Adicionar** para introduzir as credenciais de administrador de domínio.</span><span class="sxs-lookup"><span data-stu-id="ca979-146">Select **Add** to enter the domain administrator credentials.</span></span>  
7.  <span data-ttu-id="ca979-147">Na página de **sistemas operativos do Dispositivo,** selecione apenas dispositivos ligados ao domínio do Windows 10 ou posteriormente ligados ao domínio.</span><span class="sxs-lookup"><span data-stu-id="ca979-147">On the **Device operating systems** page, select Windows 10 or later domain-joined devices only.</span></span>
8.  <span data-ttu-id="ca979-148">Na página **Pronto para configurar,** selecione **Configurar**.</span><span class="sxs-lookup"><span data-stu-id="ca979-148">On the **Ready to configure** page, select **Configure**.</span></span>
9.  <span data-ttu-id="ca979-149">Na página completa da **Configuração,** selecione **Sair**.</span><span class="sxs-lookup"><span data-stu-id="ca979-149">On the **Configuration complete** page, select **Exit**.</span></span>


## <a name="5-create-a-gpo-for-intune-enrollment--admx-method"></a><span data-ttu-id="ca979-150">5. Criar um GPO para inscrição intune – método ADMX</span><span class="sxs-lookup"><span data-stu-id="ca979-150">5. Create a GPO for Intune Enrollment – ADMX method</span></span>

<span data-ttu-id="ca979-151">Utilização . Arquivo de modelo ADMX.</span><span class="sxs-lookup"><span data-stu-id="ca979-151">Use .ADMX template file.</span></span>

1.  <span data-ttu-id="ca979-152">Inicie sessão no servidor AD, procure e abra **Server Manager**  >  **Tools**  >  **gestão de políticas do Grupo**de Ferramentas do Gestor do Servidor .</span><span class="sxs-lookup"><span data-stu-id="ca979-152">Log on to AD server, search and open **Server Manager** > **Tools** > **Group Policy Management**.</span></span>
2.  <span data-ttu-id="ca979-153">Selecione o nome de domínio em **Domínios** e clique com o botão direito **Objetos de Política** de Grupo para selecionar **Novos**.</span><span class="sxs-lookup"><span data-stu-id="ca979-153">Select your domain name under **Domains** and right-click **Group Policy Objects** to select **New**.</span></span>
3.  <span data-ttu-id="ca979-154">Dê ao novo GPO um nome, por exemplo , "*Cloud_Enrollment*" e, em seguida, selecione **OK**.</span><span class="sxs-lookup"><span data-stu-id="ca979-154">Give the new GPO an name, for example “*Cloud_Enrollment*” and then select **OK**.</span></span>
4.  <span data-ttu-id="ca979-155">Clique com o botão direito no novo GPO em **Objetos de Política de Grupo** e selecione **Editar**.</span><span class="sxs-lookup"><span data-stu-id="ca979-155">Right-click the new GPO under **Group Policy Objects** and select **Edit**.</span></span>
5.  <span data-ttu-id="ca979-156">No Editor de **Gestão de Políticas**de Grupo, aceda a políticas **de configuração de computador**  >  **Policies**  >  **Modelos Administrativos**De Componentes do  >  **Windows**  >  **.**</span><span class="sxs-lookup"><span data-stu-id="ca979-156">In the **Group Policy Management Editor**, go to **Computer Configuration** > **Policies** > **Administrative Templates** > **Windows Components** > **MDM**.</span></span>
6. <span data-ttu-id="ca979-157">Clique com o botão direito **Ativar a inscrição automática de MDM utilizando credenciais AD Ad predefinidas** e, em seguida, selecione **Enabled**  >  **Enabled OK**.</span><span class="sxs-lookup"><span data-stu-id="ca979-157">Right-click **Enable automatic MDM enrollment using default Azure AD credentials** and then select **Enabled** > **OK**.</span></span> <span data-ttu-id="ca979-158">Feche a janela do editor.</span><span class="sxs-lookup"><span data-stu-id="ca979-158">Close the editor window.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="ca979-159">Se não vir a política Ative a **inscrição automática de MDM utilizando credenciais AD predefinidas**, consulte [obter os modelos administrativos mais recentes](#get-the-latest-administrative-templates).</span><span class="sxs-lookup"><span data-stu-id="ca979-159">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, see [Get the latest Administrative Templates](#get-the-latest-administrative-templates).</span></span>

## <a name="6-deploy-the-group-policy"></a><span data-ttu-id="ca979-160">6. Implementar a Política de Grupo</span><span class="sxs-lookup"><span data-stu-id="ca979-160">6. Deploy the Group Policy</span></span>

1.  <span data-ttu-id="ca979-161">No Gestor do Servidor, em **"Domínios** > objetos de Política de Grupo", selecione o GPO do Passo 3 acima, por exemplo "Cloud_Enrollment".</span><span class="sxs-lookup"><span data-stu-id="ca979-161">In the Server Manager, under **Domains** > Group Policy objects, select the GPO from Step 3 above, for example “Cloud_Enrollment”.</span></span>
2.  <span data-ttu-id="ca979-162">Selecione o **separador Âmbito** para o seu GPO.</span><span class="sxs-lookup"><span data-stu-id="ca979-162">Select the **Scope** tab for your GPO.</span></span>
3.  <span data-ttu-id="ca979-163">No separador Scope da GPO, clique com o botão direito no link para o domínio em **Links**.</span><span class="sxs-lookup"><span data-stu-id="ca979-163">In the GPO’s Scope tab, right-click the link to the domain under **Links**.</span></span>
4.  <span data-ttu-id="ca979-164">Selecione **Aplicada** para implementar o GPO e, em seguida, **OK** no ecrã de confirmação.</span><span class="sxs-lookup"><span data-stu-id="ca979-164">Select **Enforced** to deploy the GPO and then **OK** in the confirmation screen.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="ca979-165">Obtenha os mais recentes modelos administrativos</span><span class="sxs-lookup"><span data-stu-id="ca979-165">Get the latest Administrative Templates</span></span>

<span data-ttu-id="ca979-166">Se não vir a política Ative a **inscrição automática de MDM utilizando credenciais AD predefinidas**, pode ser porque não tem o ADMX instalado para o Windows 10, a versão 1803, a versão 1809 ou a versão 1903.</span><span class="sxs-lookup"><span data-stu-id="ca979-166">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, version 1809, or version 1903.</span></span> <span data-ttu-id="ca979-167">Para corrigir o problema, siga estes passos (Nota: o mais recente MDM.admx é compatível com o contrário):</span><span class="sxs-lookup"><span data-stu-id="ca979-167">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="ca979-168">Download: [Modelos Administrativos (.admx) para Windows 10 May 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span><span class="sxs-lookup"><span data-stu-id="ca979-168">Download: [Administrative Templates (.admx) for Windows 10 May 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span></span>
2.  <span data-ttu-id="ca979-169">Instale a embalagem no Controlador de Domínio Primário (PDC).</span><span class="sxs-lookup"><span data-stu-id="ca979-169">Install the package on the Primary Domain Controller (PDC).</span></span>
3.  <span data-ttu-id="ca979-170">Navegar, dependendo da versão para a pasta: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 maio 2019 Update (1903) v3**.</span><span class="sxs-lookup"><span data-stu-id="ca979-170">Navigate, depending on the version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span></span>
4.  <span data-ttu-id="ca979-171">Rebatize a pasta **Definições de Política** no caminho acima para **Definições de Políticas**.</span><span class="sxs-lookup"><span data-stu-id="ca979-171">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="ca979-172">**Copiar Pasta dedefinições de cópia** para **C:\Windows\SYSVOL\domain\Policies**.</span><span class="sxs-lookup"><span data-stu-id="ca979-172">Copy **PolicyDefinitions** folder to **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="ca979-173">Se planeia utilizar uma loja de política central para todo o seu domínio, adicione o conteúdo das Definições de Política.</span><span class="sxs-lookup"><span data-stu-id="ca979-173">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="ca979-174">Reinicie o Controlador de Domínio Primário para que a política esteja disponível.</span><span class="sxs-lookup"><span data-stu-id="ca979-174">Restart the Primary Domain Controller for the policy to be available.</span></span> <span data-ttu-id="ca979-175">Este procedimento funcionará para qualquer versão futura também.</span><span class="sxs-lookup"><span data-stu-id="ca979-175">This procedure will work for any future version as well.</span></span>

<span data-ttu-id="ca979-176">Neste momento, deverá ser capaz de ver a política Ativar a **inscrição automática de MDM utilizando credenciais AD predefinidas** disponíveis.</span><span class="sxs-lookup"><span data-stu-id="ca979-176">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>

