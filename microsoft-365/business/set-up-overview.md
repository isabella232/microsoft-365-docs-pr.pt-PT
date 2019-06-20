---
title: Descrição geral da configuração
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Descrição geral do conjunto de passos para o Microsoft 365 Business.
ms.openlocfilehash: ae7ed0aab36a6e759e0f0c1fbc3d3183273a284e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/15/2019
ms.locfileid: "35086382"
---
# <a name="overview-of-setup"></a><span data-ttu-id="3b028-103">Descrição geral do programa de configuração</span><span class="sxs-lookup"><span data-stu-id="3b028-103">Overview of setup</span></span>

<span data-ttu-id="3b028-104">A maior parte dos passos de configuração pode ser efectuado no Assistente de configuração, mas as outras opções também se encontram listadas.</span><span class="sxs-lookup"><span data-stu-id="3b028-104">Most of the set up steps can be done in the setup wizard, but the other options are also listed.</span></span>


## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="3b028-105">Passo 1: Adicionar o domínio e utilizadores</span><span class="sxs-lookup"><span data-stu-id="3b028-105">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="3b028-106">**[Adicionar o domínio](set-up.md#add-your-domain-to-personalize-sign-in)** (se adquiriu o seu domínio durante a [inscrição](sign-up.md), este passo já é efectuado.)</span><span class="sxs-lookup"><span data-stu-id="3b028-106">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="3b028-107">**Adicionar utilizadores**.</span><span class="sxs-lookup"><span data-stu-id="3b028-107">**Add users**.</span></span> <span data-ttu-id="3b028-108">Pode fazê-lo em qualquer uma das três formas:</span><span class="sxs-lookup"><span data-stu-id="3b028-108">You can do this in any of the three ways:</span></span>
        - <span data-ttu-id="3b028-109">No [Assistente](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="3b028-109">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="3b028-110">Utilize a sincronização de directório para [Adicionar utilizadores utilizando Azure AD ligar](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) se tiver no local do Active directory.</span><span class="sxs-lookup"><span data-stu-id="3b028-110">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="3b028-111">Também pode [Adicionar utilizadores posteriormente](add-users-m365b.md) no Centro de administração.</span><span class="sxs-lookup"><span data-stu-id="3b028-111">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="3b028-112">Passo 2: Definir políticas de segurança e configurar dispositivos</span><span class="sxs-lookup"><span data-stu-id="3b028-112">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="3b028-113">Utilize o [Assistente de configuração](set-up.md#set-up-security-policies-and-device-configurations) para configurar políticas de segurança e dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3b028-113">Use the [Setup wizard](set-up.md#set-up-security-policies-and-device-configurations) to configure device and security policies.</span></span> 
  - <span data-ttu-id="3b028-114">Também pode adicionar mais ou editá-los mais tarde no [Centro de administração](view-policies-and-devices.md) e no [portal de Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span><span class="sxs-lookup"><span data-stu-id="3b028-114">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="3b028-115">Além das definições de segurança no Assistente de configuração, pode aumentar a segurança, adicionando as seguintes definições:</span><span class="sxs-lookup"><span data-stu-id="3b028-115">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

      - <span data-ttu-id="3b028-116">**Mensagem de correio electrónico de protecção contra malware**</span><span class="sxs-lookup"><span data-stu-id="3b028-116">**Email malware protection**</span></span>
      - <span data-ttu-id="3b028-117">**Avançadas hiperligações de seguro de protecção de ameaças (ATP)**</span><span class="sxs-lookup"><span data-stu-id="3b028-117">**Advanced Threat Protection (ATP) Safe links**</span></span>
      - <span data-ttu-id="3b028-118">**Anexos de segurança de ATP**</span><span class="sxs-lookup"><span data-stu-id="3b028-118">**ATP Safe Attachments**</span></span>
      - <span data-ttu-id="3b028-119">**ATP anti-phishing**</span><span class="sxs-lookup"><span data-stu-id="3b028-119">**ATP anti-phishing**</span></span>
      - <span data-ttu-id="3b028-120">**Arquivo do Exchange Online**</span><span class="sxs-lookup"><span data-stu-id="3b028-120">**Exchange Online Archiving**</span></span>
      - <span data-ttu-id="3b028-121">**Data Loss Prevention (DLP)**</span><span class="sxs-lookup"><span data-stu-id="3b028-121">**Data Loss Prevention (DLP)**</span></span>
      - <span data-ttu-id="3b028-122">**a protecção de informações azure (Plan1**)</span><span class="sxs-lookup"><span data-stu-id="3b028-122">**Azure Information Protection (Plan1**)</span></span>

          <span data-ttu-id="3b028-123">Para obter iniciado, consulte [Configurar políticas de segurança avançada](set-up-advanced-security.md).</span><span class="sxs-lookup"><span data-stu-id="3b028-123">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

        <span data-ttu-id="3b028-124">Consulte também [10 principais formas de proteger o seu negócio de 365 da Microsoft](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) para obter um guia de procedimentos recomendados de segurança.</span><span class="sxs-lookup"><span data-stu-id="3b028-124">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="3b028-125">Passo 3: Configurar e gerir os dispositivos Windows 10</span><span class="sxs-lookup"><span data-stu-id="3b028-125">Step 3: Set up and manage Windows 10 devices</span></span>

   <span data-ttu-id="3b028-126">Quando associa um dispositivo Windows 10 a Azure AD, as políticas que configurar no [passo 2](#step-2-set-up-security-policies-and-configure-devices) são aplicadas ao mesmo.</span><span class="sxs-lookup"><span data-stu-id="3b028-126">When you join a Windows 10 device to Azure AD, the policies you set up in [Step 2](#step-2-set-up-security-policies-and-configure-devices) get applied to it.</span></span>

   - <span data-ttu-id="3b028-127">Windows 10 Pro é um [requisito prévio](pre-requisites-for-data-protection.md) para Microsoft 365 Business, mas se tiver o Windows 7 Pro, o Windows 8 Pro ou o Windows 8.1 Pro, sua subscrição lhe permitir para uma [actualização para o Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span><span class="sxs-lookup"><span data-stu-id="3b028-127">Windows 10 Pro is a [pre-requisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
    - <span data-ttu-id="3b028-128">Utilize o [Assistente de configuração](set-up.md#set-up-security-policies-and-device-configurations) para configurar políticas para Windows 10 dispositivos.</span><span class="sxs-lookup"><span data-stu-id="3b028-128">Use the [setup wizard](set-up.md#set-up-security-policies-and-device-configurations) to configure policies for Windows 10 devices.</span></span>

## <a name="stes-4-install-office-365-business"></a><span data-ttu-id="3b028-129">Stes 4: Instalar o Office 365 Business</span><span class="sxs-lookup"><span data-stu-id="3b028-129">Stes 4: Install Office 365 Business</span></span>
- <span data-ttu-id="3b028-130">Pode instalar automaticamente o Office nos dispositivos Windows utilizando o [Assistente de configuração](set-up.md#deploy-office-365-client-apps).</span><span class="sxs-lookup"><span data-stu-id="3b028-130">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="3b028-131">Automaticamente a [instalar o Office](auto-install-or-uninstall-office.md) partir do Centro de administração.</span><span class="sxs-lookup"><span data-stu-id="3b028-131">Automatically [install Office](auto-install-or-uninstall-office.md) from the admin center.</span></span>
- <span data-ttu-id="3b028-132">Permitir que os utilizadores [instalar aplicações do Office](https://docs.microsoft.com/office365/admin/setup/install-applications) para o Windows e dispositivos.</span><span class="sxs-lookup"><span data-stu-id="3b028-132">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="3b028-133">Avançadas</span><span class="sxs-lookup"><span data-stu-id="3b028-133">Advanced</span></span>
- <span data-ttu-id="3b028-134">**Utilizar o piloto automático para configurar novos dispositivos**</span><span class="sxs-lookup"><span data-stu-id="3b028-134">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="3b028-135">Pode utilizar o [Piloto automático do Windows](add-autopilot-devices-and-profile.md) para pré-configurar automaticamente **novos** dispositivos Windows 10 para um utilizador, mas poderá ser mais fácil obter um [parceiro](https://www.microsoft.com/solution-providers/search) que pode fazer isto por si.</span><span class="sxs-lookup"><span data-stu-id="3b028-135">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="3b028-136">Também pode ir para o [Arquivo do Microsoft](https://go.microsoft.com/fwlink/?linkid=874598) e peça um perito em tecnologia nuvem configurar novos dispositivos de compras para si.</span><span class="sxs-lookup"><span data-stu-id="3b028-136">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) and ask a cloud technology expert set up new devices you purchase for you.</span></span>

- <span data-ttu-id="3b028-137">**Aceder a recursos no local**</span><span class="sxs-lookup"><span data-stu-id="3b028-137">**Access on-premises resources**</span></span>

     - <span data-ttu-id="3b028-138">Se a organização utilizar o Windows Server Active Directory no local, pode configurar o Microsoft 365 Business para proteger os dispositivos Windows 10, mantendo o acesso a recursos locais que requerem autenticação local.</span><span class="sxs-lookup"><span data-stu-id="3b028-138">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="3b028-139">Siga os passos em [activar dispositivos associados ao domínio de Windows 10 para serem geridos pelo Microsoft 365 Business](manage-windows-devices.md) para configurar esta tarefa.</span><span class="sxs-lookup"><span data-stu-id="3b028-139">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="3b028-140">Este é o método preferido e dispositivos neste estado são denominados híbrido Azure AD associado dispositivos.</span><span class="sxs-lookup"><span data-stu-id="3b028-140">This is the preferred method and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="3b028-141">Se a empresa possui um local do Active Directory que contém alguns locais recursos (tais como partilhas de ficheiros e impressoras), pode conceder acesso a dispositivos Azure AD associados a estes recursos seguindo os passos aqui: [acesso local recursos de um Dispositivo Azure AD associados no Microsoft 365 Business](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="3b028-141">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers) , you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

  