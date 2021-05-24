---
title: Ativar a gestão Windows 10 dispositivos associados ao domínio pelo Microsoft 365 para empresas
f1.keywords:
- CSH
ms.author: efrene
author: efrene
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
description: Saiba como ativar Microsoft 365 proteger dispositivos associados ao Active-Directory Windows 10 dispositivos associados ao Active Directory em apenas alguns passos.
ms.openlocfilehash: f16962dd3c33c3c228da507bc5c4a902d76a8a08
ms.sourcegitcommit: b0d3abbccf4dd37e32d69664d3ebc9ab8dea760d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/21/2021
ms.locfileid: "52593899"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="05a7b-103">Ativar a gestão Windows 10 dispositivos associados ao domínio pelo Microsoft 365 Empresas Premium</span><span class="sxs-lookup"><span data-stu-id="05a7b-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="05a7b-104">Se a sua organização utilizar o Windows Server Active Directory no local, pode configurar o Microsoft 365 Empresas Premium para proteger os seus dispositivos do Windows 10, mantendo o acesso a recursos no local que exigem autenticação local.</span><span class="sxs-lookup"><span data-stu-id="05a7b-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="05a7b-105">Para configurar esta proteção, pode implementar dispositivos **associados ao Azure AD Híbrido.**</span><span class="sxs-lookup"><span data-stu-id="05a7b-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="05a7b-106">Estes dispositivos estão associados ao Active Directory no local e à sua Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="05a7b-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="05a7b-107">Este vídeo descreve os passos sobre como configurar esta configuração para o cenário mais comum, que também está detalhado nos passos que se seguem.</span><span class="sxs-lookup"><span data-stu-id="05a7b-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="05a7b-108">Antes de começar, certifique-se de que conclui estes passos:</span><span class="sxs-lookup"><span data-stu-id="05a7b-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="05a7b-109">Sincronize os utilizadores com o Azure AD com o Azure AD Ligação.</span><span class="sxs-lookup"><span data-stu-id="05a7b-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="05a7b-110">Conclua a sincronização Ligação do Azure AD para Organizações (OU).</span><span class="sxs-lookup"><span data-stu-id="05a7b-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="05a7b-111">Certifique-se de que todos os utilizadores do domínio que sincroniza têm licenças para Microsoft 365 Empresas Premium.</span><span class="sxs-lookup"><span data-stu-id="05a7b-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="05a7b-112">Consulte [Sincronizar utilizadores de domínio com a Microsoft](manage-domain-users.md) para ver os passos.</span><span class="sxs-lookup"><span data-stu-id="05a7b-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="05a7b-113">1. Verificar a Autoridade de MDM no Intune</span><span class="sxs-lookup"><span data-stu-id="05a7b-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="05a7b-114">Vá para [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) na página Microsoft Intune, selecione Inscrição de dispositivos **e,** em seguida, na página **Overview,** certifique-se de que a autoridade **de MDM** é **o Intune.**</span><span class="sxs-lookup"><span data-stu-id="05a7b-114">Go to [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) and on the Microsoft Intune page, select **Device enrollment**, then on the **Overview** page, make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="05a7b-115">Se **a autoridade MDM** for **Nenhuma**, clique na autoridade **de MDM** para a definir como **Intune.**</span><span class="sxs-lookup"><span data-stu-id="05a7b-115">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="05a7b-116">Se a **autoridade MDM** for **Microsoft Office 365,** vá a Dispositivos Inscrever dispositivos e utilize a caixa de diálogo Adicionar autoridade MDM à direita para adicionar autoridade MDM do  >   **Intune** (a caixa de diálogo Adicionar Autoridade **de MDM** só está disponível se a Autoridade de **MDM** estiver definida como Microsoft Office 365). </span><span class="sxs-lookup"><span data-stu-id="05a7b-116">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="05a7b-117">2. Verificar se o Azure AD está ativado para aderir a computadores</span><span class="sxs-lookup"><span data-stu-id="05a7b-117">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="05a7b-118">Vá para o centro de administração em e selecione Azure Active Directory (selecione Mostrar tudo se Azure Active Directory não estiver visível) na lista <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **Centros de** administração. </span><span class="sxs-lookup"><span data-stu-id="05a7b-118">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="05a7b-119">No centro **de Azure Active Directory, vá para** o centro de **Azure Active Directory** , selecionar **Dispositivos e,** em **seguida, Definições do dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="05a7b-119">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="05a7b-120">Verificar se os **utilizadores podem associar dispositivos ao Azure AD** está ativado</span><span class="sxs-lookup"><span data-stu-id="05a7b-120">Verify **Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="05a7b-121">Para ativar todos os utilizadores, defina para **Todos.**</span><span class="sxs-lookup"><span data-stu-id="05a7b-121">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="05a7b-122">Para ativar utilizadores específicos, defina para **Selecionado** para ativar um grupo específico de utilizadores.</span><span class="sxs-lookup"><span data-stu-id="05a7b-122">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="05a7b-123">Adicione os utilizadores de domínio pretendidos sincronizados no Azure AD a um grupo [de segurança](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="05a7b-123">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="05a7b-124">**Selecione Selecionar** grupos para ativar o âmbito de utilizador da MDM para esse grupo de segurança.</span><span class="sxs-lookup"><span data-stu-id="05a7b-124">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="05a7b-125">3. Verificar se o Azure AD está ativado para a MDM</span><span class="sxs-lookup"><span data-stu-id="05a7b-125">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="05a7b-126">Vá para o centro de administração em e selecione <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **Endpoint Managemen** t (selecione Mostrar todos se  **Endpoint Manager** não estiver visível)</span><span class="sxs-lookup"><span data-stu-id="05a7b-126">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen** t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="05a7b-127">No centro **de Microsoft Endpoint Manager,** vá a **Dispositivos**  >  **e, em Windows** Windows  >  **Inscrição**  >  **Automática.**</span><span class="sxs-lookup"><span data-stu-id="05a7b-127">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="05a7b-128">Verifique se o âmbito de utilizador da MDM está ativado.</span><span class="sxs-lookup"><span data-stu-id="05a7b-128">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="05a7b-129">Para inscrever todos  os computadores, defina para Todos para inscrever automaticamente todos os computadores dos utilizadores associados ao Azure AD e a novos computadores quando os utilizadores adicionarem uma conta Windows.</span><span class="sxs-lookup"><span data-stu-id="05a7b-129">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="05a7b-130">Defina **para Alguns** para inscrever os computadores de um grupo de utilizadores específico.</span><span class="sxs-lookup"><span data-stu-id="05a7b-130">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="05a7b-131">Adicione os utilizadores de domínio pretendidos sincronizados no Azure AD a um grupo [de segurança](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="05a7b-131">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="05a7b-132">**Selecione Selecionar** grupos para ativar o âmbito de utilizador da MDM para esse grupo de segurança.</span><span class="sxs-lookup"><span data-stu-id="05a7b-132">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="05a7b-133">4. Crie os recursos necessários</span><span class="sxs-lookup"><span data-stu-id="05a7b-133">4. Create the required resources</span></span> 

<span data-ttu-id="05a7b-134">O desempenho das tarefas necessárias para configurar a associação híbrida do [Azure AD](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) foi simplificado através da utilização do cmdlet [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) que se encontra no módulo [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) powerShell.</span><span class="sxs-lookup"><span data-stu-id="05a7b-134">Performing the required tasks to [configure hybrid Azure AD join](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="05a7b-135">Ao invocar este cmdlet, este irá criar e configurar a política de grupo e o ponto de ligação de serviço necessários.</span><span class="sxs-lookup"><span data-stu-id="05a7b-135">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="05a7b-136">Pode instalar este módulo ao invocar o seguinte a partir de uma instância do PowerShell:</span><span class="sxs-lookup"><span data-stu-id="05a7b-136">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="05a7b-137">Recomendamos que instale este módulo no servidor de Windows a executar o Azure AD Ligação.</span><span class="sxs-lookup"><span data-stu-id="05a7b-137">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="05a7b-138">Para criar a política de grupo e o ponto de ligação de serviço necessários, invoque o cmdlet [Initialize-SecMgmtHybirdDeviceEnrollment.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md)</span><span class="sxs-lookup"><span data-stu-id="05a7b-138">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="05a7b-139">Precisará das Microsoft 365 Empresas Premium administrador global quando efetuar esta tarefa.</span><span class="sxs-lookup"><span data-stu-id="05a7b-139">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="05a7b-140">Quando estiver pronto para criar os recursos, invoque o seguinte:</span><span class="sxs-lookup"><span data-stu-id="05a7b-140">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="05a7b-141">O primeiro comando estabelecerá uma ligação com a nuvem da Microsoft e, quando lhe for pedido, especifique as Microsoft 365 Empresas Premium de administrador global.</span><span class="sxs-lookup"><span data-stu-id="05a7b-141">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="05a7b-142">5. Associar a Política de Grupo</span><span class="sxs-lookup"><span data-stu-id="05a7b-142">5. Link the Group Policy</span></span>

1. <span data-ttu-id="05a7b-143">Na Consola de Gestão da Política de Grupo (GPMC), clique com o botão direito do rato na localização onde quer ligar a política e selecione Ligar um *GPO existente...* no menu de contexto.</span><span class="sxs-lookup"><span data-stu-id="05a7b-143">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="05a7b-144">Selecione a política criada no passo acima e, em seguida, clique **em OK.**</span><span class="sxs-lookup"><span data-stu-id="05a7b-144">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="05a7b-145">Obter os Modelos Administrativos mais recentes</span><span class="sxs-lookup"><span data-stu-id="05a7b-145">Get the latest Administrative Templates</span></span>

<span data-ttu-id="05a7b-146">Se não vir a política Ativar a inscrição automática da MDM com as credenciais predefinida do **Azure AD,** é possível que não tenha o ADMX instalado para o Windows 10, versão 1803 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="05a7b-146">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, or later.</span></span> <span data-ttu-id="05a7b-147">Para corrigir o problema, siga estes passos (Nota: a MDM.admx mais recente é retrocompatível):</span><span class="sxs-lookup"><span data-stu-id="05a7b-147">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="05a7b-148">Transferir: [Modelos Administrativos (.admx) para Windows 10 de outubro de 2020 Atualização (20H2).](https://www.microsoft.com/download/102157)</span><span class="sxs-lookup"><span data-stu-id="05a7b-148">Download: [Administrative Templates (.admx) for Windows 10 October 2020 Update (20H2)](https://www.microsoft.com/download/102157).</span></span>
2.  <span data-ttu-id="05a7b-149">Instale o pacote num Controlador de Domínio.</span><span class="sxs-lookup"><span data-stu-id="05a7b-149">Install the package on a Domain Controller.</span></span>
3.  <span data-ttu-id="05a7b-150">Navegue, consoante a versão Modelos Administrativos para a pasta: C:\Programas (x86)\Política de Grupo da Microsoft\Windows 10 Atualização de Outubro **de 2020 (20H2).**</span><span class="sxs-lookup"><span data-stu-id="05a7b-150">Navigate, depending on the Administrative Templates version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 October 2020 Update (20H2)**.</span></span>
4.  <span data-ttu-id="05a7b-151">Rename **the Policy Definitions** folder in the above path to **PolicyDefinitions.**</span><span class="sxs-lookup"><span data-stu-id="05a7b-151">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="05a7b-152">Copie a pasta **PolicyDefinitions** para a sua partilha SYSVOL, por predefinição localizada em **C:\Windows\SYSVOL\domain\Policies.**</span><span class="sxs-lookup"><span data-stu-id="05a7b-152">Copy the **PolicyDefinitions** folder to your SYSVOL share, by default located at **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="05a7b-153">Se tenciona utilizar um loja de políticas central para todo o domínio, adicione os conteúdos da PolicyDefinitions aí.</span><span class="sxs-lookup"><span data-stu-id="05a7b-153">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="05a7b-154">Caso tenha vários Controladores de Domínio, aguarde até que a replicação do SYSVOL esteja disponível para que as políticas sejam disponibilizadas.</span><span class="sxs-lookup"><span data-stu-id="05a7b-154">In case you have several Domain Controllers, wait for SYSVOL to replicate for the policies to be available.</span></span> <span data-ttu-id="05a7b-155">Este procedimento também funcionará em qualquer versão futura dos Modelos Administrativos.</span><span class="sxs-lookup"><span data-stu-id="05a7b-155">This procedure will work for any future version of the Administrative Templates as well.</span></span>

<span data-ttu-id="05a7b-156">Neste momento, deverá conseguir ver a política Ativar a inscrição automática de MDM utilizando **as credenciais do Azure AD predefinida** disponíveis.</span><span class="sxs-lookup"><span data-stu-id="05a7b-156">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>

## <a name="related-content"></a><span data-ttu-id="05a7b-157">Conteúdos relacionados</span><span class="sxs-lookup"><span data-stu-id="05a7b-157">Related content</span></span>

<span data-ttu-id="05a7b-158">[Sincronizar utilizadores do domínio com Microsoft 365](manage-domain-users.md) (artigo)</span><span class="sxs-lookup"><span data-stu-id="05a7b-158">[Synchronize domain users to Microsoft 365](manage-domain-users.md) (article)</span></span>

<span data-ttu-id="05a7b-159">[Criar um grupo no centro de administração](../admin/create-groups/create-groups.md) (artigo)</span><span class="sxs-lookup"><span data-stu-id="05a7b-159">[Create a group in the admin center](../admin/create-groups/create-groups.md) (article)</span></span>

<span data-ttu-id="05a7b-160">[Tutorial: Configurar uma associação Azure Active Directory híbrida para domínios geridos](/azure/active-directory/devices/hybrid-azuread-join-managed-domains.md) (artigo)</span><span class="sxs-lookup"><span data-stu-id="05a7b-160">[Tutorial: Configure hybrid Azure Active Directory join for managed domains](/azure/active-directory/devices/hybrid-azuread-join-managed-domains.md) (article)</span></span>