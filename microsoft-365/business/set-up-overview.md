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
ms.openlocfilehash: 3447f06d031462a7bebc6f129238de9f0c5dee41
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/19/2019
ms.locfileid: "38721565"
---
# <a name="overview-of-setup"></a><span data-ttu-id="66221-103">Visão geral da configuração</span><span class="sxs-lookup"><span data-stu-id="66221-103">Overview of setup</span></span>

<span data-ttu-id="66221-104">A maioria das etapas de configuração pode ser feita no assistente de configuração, mas as outras opções também estão listadas.</span><span class="sxs-lookup"><span data-stu-id="66221-104">Most of the setup steps can be done in the setup wizard, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="66221-105">Etapa 1: Adicione seu domínio e usuários</span><span class="sxs-lookup"><span data-stu-id="66221-105">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="66221-106">**[Adicione o seu domínio](set-up.md#add-your-domain-to-personalize-sign-in)** (se você comprou o seu domínio durante a [inscrição,](sign-up.md)esta etapa já está feito.)</span><span class="sxs-lookup"><span data-stu-id="66221-106">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="66221-107">**Adicionar usuários.**</span><span class="sxs-lookup"><span data-stu-id="66221-107">**Add users**.</span></span> <span data-ttu-id="66221-108">Você pode adicionar usuários de qualquer uma das três maneiras:</span><span class="sxs-lookup"><span data-stu-id="66221-108">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="66221-109">No [mago.](set-up.md#add-users-in-the-wizard)</span><span class="sxs-lookup"><span data-stu-id="66221-109">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="66221-110">Use sincronização do diretório para adicionar usuários usando o AD Connect do [Azure](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) se você tiver um diretório ativo no local.</span><span class="sxs-lookup"><span data-stu-id="66221-110">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="66221-111">Você também pode [adicionar usuários mais tarde](add-users-m365b.md) no centro de administração.</span><span class="sxs-lookup"><span data-stu-id="66221-111">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="66221-112">Etapa 2: Configurar políticas de segurança e configurar dispositivos</span><span class="sxs-lookup"><span data-stu-id="66221-112">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="66221-113">Use o assistente de [configuração](set-up.md#protect-data-and-devices) para configurar políticas de dispositivo e segurança.</span><span class="sxs-lookup"><span data-stu-id="66221-113">Use the [Setup wizard](set-up.md#protect-data-and-devices) to configure device and security policies.</span></span> 
  - <span data-ttu-id="66221-114">Você também pode adicionar mais ou editá-los mais tarde no centro de [administração](view-policies-and-devices.md) e no [portal Intune.](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)</span><span class="sxs-lookup"><span data-stu-id="66221-114">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="66221-115">Além das configurações de segurança no assistente de configuração, você pode aumentar sua segurança adicionando as seguintes configurações:</span><span class="sxs-lookup"><span data-stu-id="66221-115">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

      - <span data-ttu-id="66221-116">**Proteção de malware por e-mail**</span><span class="sxs-lookup"><span data-stu-id="66221-116">**Email malware protection**</span></span>
      - <span data-ttu-id="66221-117">**Ligações seguras de Proteção a Ameaças Avançadas (ATP)**</span><span class="sxs-lookup"><span data-stu-id="66221-117">**Advanced Threat Protection (ATP) Safe links**</span></span>
      - <span data-ttu-id="66221-118">**Anexos seguros ATP**</span><span class="sxs-lookup"><span data-stu-id="66221-118">**ATP Safe Attachments**</span></span>
      - <span data-ttu-id="66221-119">**Atp anti-phishing ATP anti-phishing**</span><span class="sxs-lookup"><span data-stu-id="66221-119">**ATP anti-phishing**</span></span>
      - <span data-ttu-id="66221-120">**Arquivo do Exchange Online**</span><span class="sxs-lookup"><span data-stu-id="66221-120">**Exchange Online Archiving**</span></span>
      - <span data-ttu-id="66221-121">**Prevenção de Perdas de Dados (DLP)**</span><span class="sxs-lookup"><span data-stu-id="66221-121">**Data Loss Prevention (DLP)**</span></span>
      - <span data-ttu-id="66221-122">**Proteção da Informação Azure (Plan1**)</span><span class="sxs-lookup"><span data-stu-id="66221-122">**Azure Information Protection (Plan1**)</span></span>

          <span data-ttu-id="66221-123">Para começar a ver, criar políticas de [segurança avançadas](set-up-advanced-security.md).</span><span class="sxs-lookup"><span data-stu-id="66221-123">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

        <span data-ttu-id="66221-124">Veja também [as 10 principais maneiras de proteger seu Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) para um roteiro das melhores práticas de segurança.</span><span class="sxs-lookup"><span data-stu-id="66221-124">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="66221-125">Etapa 3: Configurar e gerenciar dispositivos Windows 10</span><span class="sxs-lookup"><span data-stu-id="66221-125">Step 3: Set up and manage Windows 10 devices</span></span>

   <span data-ttu-id="66221-126">Quando você junta um dispositivo Windows 10 ao AD do Azure, as políticas que você configura no [Passo 2](#step-2-set-up-security-policies-and-configure-devices) são aplicadas a ele.</span><span class="sxs-lookup"><span data-stu-id="66221-126">When you join a Windows 10 device to Azure AD, the policies you set up in [Step 2](#step-2-set-up-security-policies-and-configure-devices) get applied to it.</span></span>

   - <span data-ttu-id="66221-127">O Windows 10 Pro é um [pré-requisito](pre-requisites-for-data-protection.md) para o Microsoft 365 Business, mas se você tiver o Windows 7 Pro, o Windows 8 Pro ou o Windows 8.1 Pro, sua assinatura lhe dá direito a uma atualização para o [Windows 10 Pro.](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update)</span><span class="sxs-lookup"><span data-stu-id="66221-127">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
    - <span data-ttu-id="66221-128">Use o assistente de [configuração](set-up.md#protect-data-and-devices) para configurar políticas para dispositivos Windows 10.</span><span class="sxs-lookup"><span data-stu-id="66221-128">Use the [Setup wizard](set-up.md#protect-data-and-devices) to configure policies for Windows 10 devices.</span></span>

## <a name="step-4-install-office-365-business"></a><span data-ttu-id="66221-129">Etapa 4: Instale o escritório 365 negócio</span><span class="sxs-lookup"><span data-stu-id="66221-129">Step 4: Install Office 365 Business</span></span>
- <span data-ttu-id="66221-130">Você pode instalar automaticamente o Office nos dispositivos Windows usando o assistente de [configuração.](set-up.md#deploy-office-365-client-apps)</span><span class="sxs-lookup"><span data-stu-id="66221-130">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="66221-131">Permita que os usuários [instalem aplicativos do Office](https://docs.microsoft.com/office365/admin/setup/install-applications) para Windows e dispositivos.</span><span class="sxs-lookup"><span data-stu-id="66221-131">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="66221-132">Avançado</span><span class="sxs-lookup"><span data-stu-id="66221-132">Advanced</span></span>
- <span data-ttu-id="66221-133">**Use o piloto automático para configurar novos dispositivos**</span><span class="sxs-lookup"><span data-stu-id="66221-133">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="66221-134">Você pode usar o [Windows Autopilot](add-autopilot-devices-and-profile.md) para pré-configurar automaticamente **novos** dispositivos Windows 10 para um usuário, mas pode ser mais fácil conseguir um [parceiro](https://www.microsoft.com/solution-providers/search) que possa fazer isso por você.</span><span class="sxs-lookup"><span data-stu-id="66221-134">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="66221-135">Você também pode ir à [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598)e pedir a um especialista em tecnologia de nuvem para configurar novos dispositivos que você compra.</span><span class="sxs-lookup"><span data-stu-id="66221-135">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="66221-136">**Acesso a recursos no local**</span><span class="sxs-lookup"><span data-stu-id="66221-136">**Access on-premises resources**</span></span>

     - <span data-ttu-id="66221-137">Se a sua organização usar o Diretório Ativo do Windows Server no local, você poderá configurar o Microsoft 365 Business para proteger seus dispositivos Windows 10, mantendo o acesso a recursos no local que exigem autenticação local.</span><span class="sxs-lookup"><span data-stu-id="66221-137">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="66221-138">Siga as etapas dos [dispositivos Windows 10 incluídos no domínio habilitado para serem gerenciados pelo Microsoft 365 Business](manage-windows-devices.md) para configurar isso.</span><span class="sxs-lookup"><span data-stu-id="66221-138">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="66221-139">Este é o método preferido, e os dispositivos neste estado são chamados dispositivos unidos a Anúncio híbrido sucateado a AD.</span><span class="sxs-lookup"><span data-stu-id="66221-139">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="66221-140">Se a sua empresa tiver um Diretório Ativo local que contém alguns recursos no local (como compartilhamentos de arquivos e impressoras), você poderá dar aos dispositivos vinculados a Azure a dispositivos vinculados a esses recursos seguindo os passos aqui: [acesse recursos locais de um dispositivo azure vinculado a AD no Microsoft 365 Business](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="66221-140">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

  