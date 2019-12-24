---
title: Visão geral da configuração
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Visão geral das etapas de configuração para o Microsoft 365 Business.
ms.openlocfilehash: 4aca617015cceb85ca35c8d8ada7b83d1416d959
ms.sourcegitcommit: 178ecb21cacdeaf440f3df2fe6e539e9127fcf15
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/23/2019
ms.locfileid: "40850810"
---
# <a name="overview-of-setup"></a><span data-ttu-id="22bc2-103">Visão geral da configuração</span><span class="sxs-lookup"><span data-stu-id="22bc2-103">Overview of setup</span></span>

<span data-ttu-id="22bc2-104">Assista a um pequeno vídeo sobre a configuração do Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="22bc2-104">Watch a short video about Microsoft 365 Business setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

<span data-ttu-id="22bc2-105">Se você achou este vídeo útil, confira a série de [treinamento completo para pequenas empresas e as novas para a Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="22bc2-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

<span data-ttu-id="22bc2-106">A maioria das etapas de configuração pode ser feita no assistente de configuração, mas as outras opções também estão listadas.</span><span class="sxs-lookup"><span data-stu-id="22bc2-106">Most of the setup steps can be done in the setup wizard, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="22bc2-107">Etapa 1: Adicione seu domínio e usuários</span><span class="sxs-lookup"><span data-stu-id="22bc2-107">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="22bc2-108">**[Adicione o seu domínio](set-up.md#add-your-domain-to-personalize-sign-in)** (se você comprou o seu domínio durante a [inscrição,](sign-up.md)esta etapa já está feito.)</span><span class="sxs-lookup"><span data-stu-id="22bc2-108">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="22bc2-109">**Adicionar usuários.**</span><span class="sxs-lookup"><span data-stu-id="22bc2-109">**Add users**.</span></span> <span data-ttu-id="22bc2-110">Você pode adicionar usuários de qualquer uma das três maneiras:</span><span class="sxs-lookup"><span data-stu-id="22bc2-110">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="22bc2-111">No [mago.](set-up.md#add-users-in-the-wizard)</span><span class="sxs-lookup"><span data-stu-id="22bc2-111">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="22bc2-112">Use sincronização do diretório para adicionar usuários usando o AD Connect do [Azure](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) se você tiver um diretório ativo no local.</span><span class="sxs-lookup"><span data-stu-id="22bc2-112">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="22bc2-113">Você também pode [adicionar usuários mais tarde](add-users-m365b.md) no centro de administração.</span><span class="sxs-lookup"><span data-stu-id="22bc2-113">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="22bc2-114">Etapa 2: Configurar políticas de segurança e configurar dispositivos</span><span class="sxs-lookup"><span data-stu-id="22bc2-114">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="22bc2-115">Use o assistente de [configuração](set-up.md#protect-your-organization) para configurar as políticas do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22bc2-115">Use the [Setup wizard](set-up.md#protect-your-organization) to configure device policies.</span></span> 
  - <span data-ttu-id="22bc2-116">Você também pode adicionar mais ou editá-los mais tarde no centro de [administração](view-policies-and-devices.md) e no [portal Intune.](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)</span><span class="sxs-lookup"><span data-stu-id="22bc2-116">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="22bc2-117">O assistente de configuração também criará configurações básicas de proteção contra ameaças e prevenção de perdas de dados.</span><span class="sxs-lookup"><span data-stu-id="22bc2-117">The setup wizard will also set up basic threat protection and data loss prevention settings.</span></span>
  
  <span data-ttu-id="22bc2-118">Além das configurações de segurança no assistente de configuração, você pode aumentar sua segurança adicionando as seguintes configurações:</span><span class="sxs-lookup"><span data-stu-id="22bc2-118">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

- <span data-ttu-id="22bc2-119">**Proteção de malware por e-mail**</span><span class="sxs-lookup"><span data-stu-id="22bc2-119">**Email malware protection**</span></span>
- <span data-ttu-id="22bc2-120">**Atp anti-phishing ATP anti-phishing**</span><span class="sxs-lookup"><span data-stu-id="22bc2-120">**ATP anti-phishing**</span></span>
- <span data-ttu-id="22bc2-121">**Arquivo do Exchange Online**</span><span class="sxs-lookup"><span data-stu-id="22bc2-121">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="22bc2-122">**Proteção da Informação Azure (Plan1**)</span><span class="sxs-lookup"><span data-stu-id="22bc2-122">**Azure Information Protection (Plan1**)</span></span>

<span data-ttu-id="22bc2-123">Para começar, veja a criação de políticas de [segurança avançadas.](set-up-advanced-security.md)</span><span class="sxs-lookup"><span data-stu-id="22bc2-123">To get started, see [set up advanced security policies](set-up-advanced-security.md).</span></span>

<span data-ttu-id="22bc2-124">Veja também [as 10 principais maneiras de proteger seu Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) para um roteiro das melhores práticas de segurança.</span><span class="sxs-lookup"><span data-stu-id="22bc2-124">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="22bc2-125">Etapa 3: Configurar e gerenciar dispositivos Windows 10</span><span class="sxs-lookup"><span data-stu-id="22bc2-125">Step 3: Set up and manage Windows 10 devices</span></span>

<span data-ttu-id="22bc2-126">Depois de executar o assistente configurar, você vai querer proctect todos os windwos 10 computadores em sua organização.</span><span class="sxs-lookup"><span data-stu-id="22bc2-126">After you run the set up wizard, you will want to proctect all the Windwos 10 computers in your organization.</span></span>
  
- <span data-ttu-id="22bc2-127">O Windows 10 Pro é um [pré-requisito](pre-requisites-for-data-protection.md) para o Microsoft 365 Business, mas se você tiver o Windows 7 Pro, o Windows 8 Pro ou o Windows 8.1 Pro, sua assinatura lhe dá direito a uma atualização para o [Windows 10 Pro.](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update)</span><span class="sxs-lookup"><span data-stu-id="22bc2-127">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
- <span data-ttu-id="22bc2-128">Siga as etapas em [PCs do Windows 10 seguros](secure-win-10-pcs.md) para configurar políticas para dispositivos Windows 10.</span><span class="sxs-lookup"><span data-stu-id="22bc2-128">Follow the steps in [secure Windows 10 PCs](secure-win-10-pcs.md) to set up policies for Windows 10 devices.</span></span>

<span data-ttu-id="22bc2-129">Quando você junta um dispositivo Windows 10 ao AD do Azure, as políticas que você define para computadores Windows 10 são aplicadas a ele.</span><span class="sxs-lookup"><span data-stu-id="22bc2-129">When you join a Windows 10 device to Azure AD, the policies you set for Windows 10 computers get applied to it.</span></span> <span data-ttu-id="22bc2-130">Para mais informações, consulte [dispositivos Windows para usuários do Microsoft 365 Business.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="22bc2-130">For more information, see [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md).</span></span>

## <a name="step-4-install-office-365-business"></a><span data-ttu-id="22bc2-131">Etapa 4: Instale o escritório 365 negócio</span><span class="sxs-lookup"><span data-stu-id="22bc2-131">Step 4: Install Office 365 Business</span></span>
- <span data-ttu-id="22bc2-132">Você pode instalar automaticamente o Office nos dispositivos Windows usando o assistente de [configuração.](set-up.md#deploy-office-365-client-apps)</span><span class="sxs-lookup"><span data-stu-id="22bc2-132">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="22bc2-133">Permita que os usuários [instalem aplicativos do Office](https://docs.microsoft.com/office365/admin/setup/install-applications) para Windows e dispositivos.</span><span class="sxs-lookup"><span data-stu-id="22bc2-133">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="22bc2-134">Avançado</span><span class="sxs-lookup"><span data-stu-id="22bc2-134">Advanced</span></span>
- <span data-ttu-id="22bc2-135">**Use o piloto automático para configurar novos dispositivos**</span><span class="sxs-lookup"><span data-stu-id="22bc2-135">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="22bc2-136">Você pode usar o [Windows Autopilot](add-autopilot-devices-and-profile.md) para pré-configurar automaticamente **novos** dispositivos Windows 10 para um usuário, mas pode ser mais fácil conseguir um [parceiro](https://www.microsoft.com/solution-providers/search) que possa fazer isso por você.</span><span class="sxs-lookup"><span data-stu-id="22bc2-136">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="22bc2-137">Você também pode ir à [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598)e pedir a um especialista em tecnologia de nuvem para configurar novos dispositivos que você compra.</span><span class="sxs-lookup"><span data-stu-id="22bc2-137">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="22bc2-138">**Acesso a recursos no local**</span><span class="sxs-lookup"><span data-stu-id="22bc2-138">**Access on-premises resources**</span></span>

     - <span data-ttu-id="22bc2-139">Se a sua organização usar o Diretório Ativo do Windows Server no local, você poderá configurar o Microsoft 365 Business para proteger seus dispositivos Windows 10, mantendo o acesso a recursos no local que exigem autenticação local.</span><span class="sxs-lookup"><span data-stu-id="22bc2-139">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="22bc2-140">Siga as etapas dos [dispositivos Windows 10 incluídos no domínio habilitado para serem gerenciados pelo Microsoft 365 Business](manage-windows-devices.md) para configurar isso.</span><span class="sxs-lookup"><span data-stu-id="22bc2-140">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="22bc2-141">Este é o método preferido, e os dispositivos neste estado são chamados dispositivos unidos a Anúncio híbrido sucateado a AD.</span><span class="sxs-lookup"><span data-stu-id="22bc2-141">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="22bc2-142">Se a sua empresa tiver um Diretório Ativo local que contém alguns recursos no local (como compartilhamentos de arquivos e impressoras), você poderá dar aos dispositivos vinculados a Azure a dispositivos vinculados a esses recursos seguindo os passos aqui: [acesse recursos locais de um dispositivo azure vinculado a AD no Microsoft 365 Business](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="22bc2-142">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="22bc2-143">See also</span><span class="sxs-lookup"><span data-stu-id="22bc2-143">See also</span></span>

[<span data-ttu-id="22bc2-144">Microsoft 365 Vídeos de treinamento de negócios</span><span class="sxs-lookup"><span data-stu-id="22bc2-144">Microsoft 365 Business training videos</span></span>](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
