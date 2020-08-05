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
ms.openlocfilehash: 6275c6c4be9cd9631ab095f8b0e1b39683022bb2
ms.sourcegitcommit: d988faa292c2661ffea43c7161aef92b2b4b99bc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/04/2020
ms.locfileid: "46560849"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="a36b9-103">Permitir que dispositivos Windows 10 unidos por domínio sejam geridos pelo Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="a36b9-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="a36b9-104">Se a sua organização utilizar o Windows Server Ative Directory no local, pode configurar o Microsoft 365 Business Premium para proteger os seus dispositivos Windows 10, mantendo ao mesmo tempo o acesso a recursos no local que requerem autenticação local.</span><span class="sxs-lookup"><span data-stu-id="a36b9-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="a36b9-105">Para configurar esta proteção, pode implementar **dispositivos híbridos Azure AD.**</span><span class="sxs-lookup"><span data-stu-id="a36b9-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="a36b9-106">Estes dispositivos estão ligados tanto ao seu Ative Directory como ao seu Diretório Ativo Azure.</span><span class="sxs-lookup"><span data-stu-id="a36b9-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="a36b9-107">Este vídeo descreve os passos para como configurar isto para o cenário mais comum, que também é detalhado nos passos que se seguem.</span><span class="sxs-lookup"><span data-stu-id="a36b9-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="a36b9-108">Antes de começar, certifique-se de completar estes passos:</span><span class="sxs-lookup"><span data-stu-id="a36b9-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="a36b9-109">Sincronizar os utilizadores para Azure AD com Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="a36b9-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="a36b9-110">Sincronização completa da Unidade Organizacional de Ligação Azure (OU).</span><span class="sxs-lookup"><span data-stu-id="a36b9-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="a36b9-111">Certifique-se de que todos os utilizadores de domínio sincronizados têm licenças para o Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="a36b9-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="a36b9-112">Consulte [os utilizadores de domínio sincronizados com a Microsoft](manage-domain-users.md) para os passos.</span><span class="sxs-lookup"><span data-stu-id="a36b9-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="a36b9-113">1. Verificar a Autoridade MDM em Intune</span><span class="sxs-lookup"><span data-stu-id="a36b9-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="a36b9-114">Vá ao [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) e na página Microsoft Intune, selecione **a inscrição**do Dispositivo , em seguida, na página **'Vista Geral',** certifique-se de que **a autoridade MDM** está **Intune**.</span><span class="sxs-lookup"><span data-stu-id="a36b9-114">Go to [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) and on the Microsoft Intune page, select **Device enrollment**, then on the **Overview** page, make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="a36b9-115">Se **a autoridade do MDM** não for **nenhuma,** clique na **autoridade do MDM** para defini-la para **Intune**.</span><span class="sxs-lookup"><span data-stu-id="a36b9-115">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="a36b9-116">Se **a autoridade do MDM** for o Microsoft Office **365,** vá aos **Devices**  >  **dispositivos de inscrição** de dispositivos e use o diálogo **da autoridade Add MDM** no direito de adicionar a autoridade **Intune MDM** (o diálogo da Autoridade add **MDM** só está disponível se a **Autoridade MDM** estiver definida para o Microsoft Office 365).</span><span class="sxs-lookup"><span data-stu-id="a36b9-116">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="a36b9-117">2. Verifique se a Azure AD está ativada para unir computadores</span><span class="sxs-lookup"><span data-stu-id="a36b9-117">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="a36b9-118">Vá ao centro de administração <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> e selecione **Azure Ative Directory** (selecione Mostrar tudo se o Diretório Ativo Azure não estiver visível) na lista de **centros de administração.**</span><span class="sxs-lookup"><span data-stu-id="a36b9-118">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="a36b9-119">No **centro de administração Azure Ative,** vá ao **Azure Ative Directory,** escolha **Dispositivos** e, em seguida, **configurações do Dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="a36b9-119">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="a36b9-120">Verifique se**os utilizadores podem juntar-se a dispositivos para Azure AD** está ativado</span><span class="sxs-lookup"><span data-stu-id="a36b9-120">Verify**Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="a36b9-121">Para ativar todos os utilizadores, desa um pouco de **tudo**.</span><span class="sxs-lookup"><span data-stu-id="a36b9-121">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="a36b9-122">Para permitir utilizadores específicos, desatado para **selecionar** para permitir um grupo específico de utilizadores.</span><span class="sxs-lookup"><span data-stu-id="a36b9-122">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="a36b9-123">Adicione os utilizadores de domínio desejado sincronizados em Azure AD a um [grupo de segurança](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="a36b9-123">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="a36b9-124">Escolha **Grupos Selecionados** para ativar o âmbito do utilizador MDM para esse grupo de segurança.</span><span class="sxs-lookup"><span data-stu-id="a36b9-124">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="a36b9-125">3. Verifique se a Azure AD está ativada para o MDM</span><span class="sxs-lookup"><span data-stu-id="a36b9-125">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="a36b9-126">Vá ao centro de administração <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> e selecione **Endpoint Managemen**t (selecione **Mostrar tudo** se **o Endpoint Manager** não estiver visível)</span><span class="sxs-lookup"><span data-stu-id="a36b9-126">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen**t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="a36b9-127">No **centro de administração do Microsoft Endpoint Manager,** aceda a **Inscrições**  >  **Windows**  >  Automáticas de**Inscrição**  >  **no**Windows do Windows .</span><span class="sxs-lookup"><span data-stu-id="a36b9-127">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="a36b9-128">Verifique se o âmbito do utilizador DO MDM está ativado.</span><span class="sxs-lookup"><span data-stu-id="a36b9-128">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="a36b9-129">Para inscrever todos os computadores, descreva para **All** para inscrever automaticamente todos os computadores de utilizador que se unem ao Azure AD e aos novos computadores quando os utilizadores adicionarem uma conta de trabalho ao Windows.</span><span class="sxs-lookup"><span data-stu-id="a36b9-129">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="a36b9-130">Definir para **Alguns** para inscrever os computadores de um grupo específico de utilizadores.</span><span class="sxs-lookup"><span data-stu-id="a36b9-130">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="a36b9-131">Adicione os utilizadores de domínio desejado sincronizados em Azure AD a um [grupo de segurança](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="a36b9-131">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="a36b9-132">Escolha **Grupos Selecionados** para ativar o âmbito do utilizador MDM para esse grupo de segurança.</span><span class="sxs-lookup"><span data-stu-id="a36b9-132">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="a36b9-133">4. Criar os recursos necessários</span><span class="sxs-lookup"><span data-stu-id="a36b9-133">4. Create the required resources</span></span> 

<span data-ttu-id="a36b9-134">A execução das tarefas necessárias para configurar a [junção híbrida Azure AD](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) foi simplificada através da utilização do cmdlet [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) encontrado no módulo [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a36b9-134">Performing the required tasks to [configure hybrid Azure AD join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="a36b9-135">Quando invocar este cmdlet, criará e configurará o ponto de ligação de serviço e a política de grupo necessários.</span><span class="sxs-lookup"><span data-stu-id="a36b9-135">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="a36b9-136">Pode instalar este módulo invocando o seguinte a partir de uma instância do PowerShell:</span><span class="sxs-lookup"><span data-stu-id="a36b9-136">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="a36b9-137">Recomenda-se que instale este módulo no Servidor do Windows que executa o Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="a36b9-137">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="a36b9-138">Para criar o ponto de ligação de serviço e a política de grupo necessários, irá invocar o cmdlet [Initialize-SecMgmtHybirdDeviceEnrollment.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md)</span><span class="sxs-lookup"><span data-stu-id="a36b9-138">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="a36b9-139">Vai precisar das suas credenciais de administração global Microsoft 365 Business Premium ao realizar esta tarefa.</span><span class="sxs-lookup"><span data-stu-id="a36b9-139">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="a36b9-140">Quando estiver pronto para criar os recursos, invoque o seguinte:</span><span class="sxs-lookup"><span data-stu-id="a36b9-140">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="a36b9-141">O primeiro comando estabelecerá uma ligação com a nuvem microsoft, e quando for solicitado, especifique as suas credenciais de administração global Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="a36b9-141">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="a36b9-142">5. Ligue a Política de Grupo</span><span class="sxs-lookup"><span data-stu-id="a36b9-142">5. Link the Group Policy</span></span>

1. <span data-ttu-id="a36b9-143">Na Consola de Gestão de Políticas de Grupo (GPMC), clique à direita no local onde pretende ligar a política e selecione *Link um GPO existente...* a partir do menu de contexto.</span><span class="sxs-lookup"><span data-stu-id="a36b9-143">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="a36b9-144">Selecione a política criada no passo acima e, em seguida, clique **em OK**.</span><span class="sxs-lookup"><span data-stu-id="a36b9-144">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="a36b9-145">Obtenha os mais recentes modelos administrativos</span><span class="sxs-lookup"><span data-stu-id="a36b9-145">Get the latest Administrative Templates</span></span>

<span data-ttu-id="a36b9-146">Se não vir a política Ative a **inscrição automática de MDM utilizando credenciais AD predefinidas**, pode ser porque não tem o ADMX instalado para o Windows 10, a versão 1803, a versão 1809 ou a versão 1903.</span><span class="sxs-lookup"><span data-stu-id="a36b9-146">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, version 1809, or version 1903.</span></span> <span data-ttu-id="a36b9-147">Para corrigir o problema, siga estes passos (Nota: o mais recente MDM.admx é compatível com o contrário):</span><span class="sxs-lookup"><span data-stu-id="a36b9-147">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="a36b9-148">Download: [Modelos Administrativos (.admx) para Windows 10 May 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span><span class="sxs-lookup"><span data-stu-id="a36b9-148">Download: [Administrative Templates (.admx) for Windows 10 May 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span></span>
2.  <span data-ttu-id="a36b9-149">Instale a embalagem no Controlador de Domínio Primário (PDC).</span><span class="sxs-lookup"><span data-stu-id="a36b9-149">Install the package on the Primary Domain Controller (PDC).</span></span>
3.  <span data-ttu-id="a36b9-150">Navegar, dependendo da versão para a pasta: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 maio 2019 Update (1903) v3**.</span><span class="sxs-lookup"><span data-stu-id="a36b9-150">Navigate, depending on the version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span></span>
4.  <span data-ttu-id="a36b9-151">Rebatize a pasta **Definições de Política** no caminho acima para **Definições de Políticas**.</span><span class="sxs-lookup"><span data-stu-id="a36b9-151">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="a36b9-152">**Copiar Pasta dedefinições de cópia** para **C:\Windows\SYSVOL\domain\Policies**.</span><span class="sxs-lookup"><span data-stu-id="a36b9-152">Copy **PolicyDefinitions** folder to **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="a36b9-153">Se planeia utilizar uma loja de política central para todo o seu domínio, adicione o conteúdo das Definições de Política.</span><span class="sxs-lookup"><span data-stu-id="a36b9-153">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="a36b9-154">Reinicie o Controlador de Domínio Primário para que a política esteja disponível.</span><span class="sxs-lookup"><span data-stu-id="a36b9-154">Restart the Primary Domain Controller for the policy to be available.</span></span> <span data-ttu-id="a36b9-155">Este procedimento funcionará para qualquer versão futura também.</span><span class="sxs-lookup"><span data-stu-id="a36b9-155">This procedure will work for any future version as well.</span></span>

<span data-ttu-id="a36b9-156">Neste momento, deverá ser capaz de ver a política Ativar a **inscrição automática de MDM utilizando credenciais AD predefinidas** disponíveis.</span><span class="sxs-lookup"><span data-stu-id="a36b9-156">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>
