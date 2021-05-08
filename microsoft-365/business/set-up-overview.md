---
title: Visão geral da configuração
f1.keywords:
- NOCSH
ms.author: kwekua
author: kwekua
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Saiba os passos de configuração Microsoft 365 Empresas Premium, desde subscrever, adicionar um domínio e utilizadores, configurar políticas de segurança e muito mais.
ms.openlocfilehash: 008a5c51698589667acc0d01649f67dab33b4c58
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/06/2021
ms.locfileid: "52245070"
---
# <a name="overview-of-setup"></a><span data-ttu-id="782bf-103">Visão geral da configuração</span><span class="sxs-lookup"><span data-stu-id="782bf-103">Overview of setup</span></span>

<span data-ttu-id="782bf-104">Veja um breve vídeo sobre como Microsoft 365 Empresas Premium configuração.</span><span class="sxs-lookup"><span data-stu-id="782bf-104">Watch a short video about Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

<span data-ttu-id="782bf-105">Caso tenha considerado este vídeo útil, veja a [série de formação completa para pequenas empresas e as novidades do Microsoft 365](../business-video/index.yml).</span><span class="sxs-lookup"><span data-stu-id="782bf-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](../business-video/index.yml).</span></span>

<span data-ttu-id="782bf-106">A maioria dos passos de configuração pode ser feita na configuração guiada, mas as outras opções também são listadas.</span><span class="sxs-lookup"><span data-stu-id="782bf-106">Most of the setup steps can be done in the guided setup, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="782bf-107">Passo 1: adicionar o seu domínio e utilizadores</span><span class="sxs-lookup"><span data-stu-id="782bf-107">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="782bf-108">**[Adicione o seu domínio](set-up.md#add-your-domain-to-personalize-sign-in)** (se comprou o seu domínio durante a [registo](sign-up.md), este passo já está feito).)</span><span class="sxs-lookup"><span data-stu-id="782bf-108">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

   - <span data-ttu-id="782bf-109">**Adicionar utilizadores.**</span><span class="sxs-lookup"><span data-stu-id="782bf-109">**Add users**.</span></span> <span data-ttu-id="782bf-110">Pode adicionar utilizadores de uma das três formas:</span><span class="sxs-lookup"><span data-stu-id="782bf-110">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="782bf-111">Na [configuração guiada](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="782bf-111">In the [guided setup](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="782bf-112">Utilize a sincronização de diretórios para adicionar utilizadores com o [Azure AD Ligação](../enterprise/set-up-directory-synchronization.md) se tiver um Active Directory no local.</span><span class="sxs-lookup"><span data-stu-id="782bf-112">Use directory synchronization to [add users by using Azure AD Connect](../enterprise/set-up-directory-synchronization.md) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="782bf-113">Também pode [adicionar utilizadores mais tarde](../admin/add-users/add-users.md) no centro de administração.</span><span class="sxs-lookup"><span data-stu-id="782bf-113">You can also [add users later](../admin/add-users/add-users.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="782bf-114">Passo 2: Configurar políticas de segurança e configurar dispositivos</span><span class="sxs-lookup"><span data-stu-id="782bf-114">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="782bf-115">Utilize a [configuração guiada para](set-up.md#protect-your-organization) configurar políticas de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="782bf-115">Use the [guided setup](set-up.md#protect-your-organization) to configure device policies.</span></span> 
  - <span data-ttu-id="782bf-116">Também pode adicionar mais ou editá-los mais tarde [no centro de administração e](view-policies-and-devices.md) no portal do [Intune.](/intune/tutorial-walkthrough-intune-portal)</span><span class="sxs-lookup"><span data-stu-id="782bf-116">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="782bf-117">O assistente de configuração também irá configurar definições básicas de proteção contra ameaças e prevenção de perda de dados.</span><span class="sxs-lookup"><span data-stu-id="782bf-117">The setup wizard will also set up basic threat protection and data loss prevention settings.</span></span>
  
  <span data-ttu-id="782bf-118">Além das definições de segurança no assistente de configuração, pode aumentar a segurança ao adicionar as seguintes definições:</span><span class="sxs-lookup"><span data-stu-id="782bf-118">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

- <span data-ttu-id="782bf-119">**Proteção contra software malicónico de e-mail**</span><span class="sxs-lookup"><span data-stu-id="782bf-119">**Email malware protection**</span></span>
- <span data-ttu-id="782bf-120">**Anti phishing no Defender para Office 365**</span><span class="sxs-lookup"><span data-stu-id="782bf-120">**Anti-phishing in Defender for Office 365**</span></span>
- <span data-ttu-id="782bf-121">**Arquivo do Exchange Online**</span><span class="sxs-lookup"><span data-stu-id="782bf-121">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="782bf-122">**Azure Information Protection (Plano1)**</span><span class="sxs-lookup"><span data-stu-id="782bf-122">**Azure Information Protection (Plan1**)</span></span>

<span data-ttu-id="782bf-123">Para começar, consulte Aumentar [a proteção contra ameaças](increase-threat-protection.md) e [configurar funcionalidades de conformidade.](set-up-compliance.md)</span><span class="sxs-lookup"><span data-stu-id="782bf-123">To get started, see [increase threat protection](increase-threat-protection.md) and [set up compliance features](set-up-compliance.md).</span></span>

<span data-ttu-id="782bf-124">Consulte também [as 10 principais formas de proteger](/office365/admin/security-and-compliance/secure-your-business-data) o Microsoft 365 Empresas Premium para saber mais sobre as melhores práticas de segurança.</span><span class="sxs-lookup"><span data-stu-id="782bf-124">See also [top 10 ways to secure your Microsoft 365 Business Premium](/office365/admin/security-and-compliance/secure-your-business-data) for a road-map of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="782bf-125">Passo 3: configurar e gerir dispositivos Windows 10 dispositivos</span><span class="sxs-lookup"><span data-stu-id="782bf-125">Step 3: Set up and manage Windows 10 devices</span></span>

<span data-ttu-id="782bf-126">Após concluir a configuração guiada, irá querer proteger todos os Windows 10 da sua organização.</span><span class="sxs-lookup"><span data-stu-id="782bf-126">After you complete the guided setup, you will want to protect all the Windows 10 computers in your organization.</span></span>
  
- <span data-ttu-id="782bf-127">Windows 10 Pro é um [](pre-requisites-for-data-protection.md) pré-requisito para o Microsoft 365 Empresas Premium, mas se tiver o Windows 7 Pro, Windows 8 Pro ou Windows 8.1 Pro, a sua subscrição dá-lhe direito a uma atualização para o [Windows 10 Pro.](./upgrade-to-windows-pro-creators-update.md)</span><span class="sxs-lookup"><span data-stu-id="782bf-127">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business Premium, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](./upgrade-to-windows-pro-creators-update.md).</span></span>
- <span data-ttu-id="782bf-128">Siga os passos em [PCs Windows 10 segurança](secure-win-10-pcs.md) para configurar políticas para Windows 10 dispositivos.</span><span class="sxs-lookup"><span data-stu-id="782bf-128">Follow the steps in [secure Windows 10 PCs](secure-win-10-pcs.md) to set up policies for Windows 10 devices.</span></span>

<span data-ttu-id="782bf-129">Quando adere a um Windows 10 Azure AD, as políticas que definir para Windows 10 seus computadores são aplicadas ao mesmo.</span><span class="sxs-lookup"><span data-stu-id="782bf-129">When you join a Windows 10 device to Azure AD, the policies you set for Windows 10 computers get applied to it.</span></span> <span data-ttu-id="782bf-130">Para obter mais informações, consulte [Configurar o Windows dispositivos para Microsoft 365 utilizadores.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="782bf-130">For more information, see [Set up Windows devices for Microsoft 365 users](set-up-windows-devices.md).</span></span>

## <a name="step-4-install-microsoft-365-apps-for-business"></a><span data-ttu-id="782bf-131">Passo 4: instale o Microsoft 365 Apps para Pequenas e Médias Empresas</span><span class="sxs-lookup"><span data-stu-id="782bf-131">Step 4: Install Microsoft 365 Apps for business</span></span>
- <span data-ttu-id="782bf-132">Pode instalar automaticamente os Office dispositivos Windows com o assistente [de configuração.](set-up.md#deploy-office-365-client-apps)</span><span class="sxs-lookup"><span data-stu-id="782bf-132">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="782bf-133">Permita que [os utilizadores instalem Office](/office365/admin/setup/install-applications) aplicações para Windows dispositivos e dispositivos.</span><span class="sxs-lookup"><span data-stu-id="782bf-133">Let users [install Office apps](/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="782bf-134">Advanced</span><span class="sxs-lookup"><span data-stu-id="782bf-134">Advanced</span></span>
- <span data-ttu-id="782bf-135">**Utilizar o Autopilot para configurar novos dispositivos**</span><span class="sxs-lookup"><span data-stu-id="782bf-135">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="782bf-136">Pode utilizar o [Windows Autopilot](add-autopilot-devices-and-profile.md) para pré-configurar automaticamente novos dispositivos **Windows 10** para um utilizador, [](https://www.microsoft.com/solution-providers/search) mas será mais fácil obter um parceiro que o possa fazer por si.</span><span class="sxs-lookup"><span data-stu-id="782bf-136">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="782bf-137">Também pode entrar no Microsoft Store e [pedir](https://go.microsoft.com/fwlink/?linkid=874598)a um especialista em tecnologia da nuvem para configurar os novos dispositivos que comprar.</span><span class="sxs-lookup"><span data-stu-id="782bf-137">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="782bf-138">**Recursos do Access no local**</span><span class="sxs-lookup"><span data-stu-id="782bf-138">**Access on-premises resources**</span></span>

     - <span data-ttu-id="782bf-139">Se a sua organização utilizar o Windows Server Active Directory no local, pode configurar o Microsoft 365 Empresas Premium para proteger os seus dispositivos do Windows 10, mantendo o acesso a recursos no local que exigem autenticação local.</span><span class="sxs-lookup"><span data-stu-id="782bf-139">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="782bf-140">Siga os passos em [Ativar a gestão Windows 10 dispositivos associados](manage-windows-devices.md) ao domínio Microsoft 365 Empresas Premium configuração.</span><span class="sxs-lookup"><span data-stu-id="782bf-140">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="782bf-141">Este é o método preferido e os dispositivos neste estado denominam-se dispositivos associados ao Azure AD Híbrido.</span><span class="sxs-lookup"><span data-stu-id="782bf-141">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="782bf-142">Se a sua empresa tiver um Active Directory local que contenha alguns recursos no local (como partilhas de ficheiros e impressoras), pode dar aos seus dispositivos associados ao Azure AD acesso a estes recursos ao seguir os passos aqui: Aceder a recursos no local a partir de um dispositivo associado ao [Azure AD](access-resources.md)no Microsoft 365 Empresas Premium .</span><span class="sxs-lookup"><span data-stu-id="782bf-142">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium](access-resources.md).</span></span>

## <a name="related-content"></a><span data-ttu-id="782bf-143">Conteúdo relacionado</span><span class="sxs-lookup"><span data-stu-id="782bf-143">Related content</span></span>

<span data-ttu-id="782bf-144">[Microsoft 365 vídeos de formação para empresas](../business-video/index.yml) (página de ligação)</span><span class="sxs-lookup"><span data-stu-id="782bf-144">[Microsoft 365 for business training videos](../business-video/index.yml) (link page)</span></span>