---
title: Permitir que dispositivos Windows 10 unidos por domínio sejam geridos pela Microsoft 365 para negócios
f1.keywords:
- NOCSH
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
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Saiba como permitir que o Microsoft 365 proteja os dispositivos locais do Windows 10, aderidos ao Active-Directory, em apenas alguns passos.
ms.openlocfilehash: 7bfe5da8701a17712fa249eac99a22b8d5a1b2d1
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471053"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="d9fc1-103">Permitir que dispositivos Windows 10 unidos por domínio sejam geridos pelo Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="d9fc1-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="d9fc1-104">Se a sua organização utilizar o Windows Server Ative Directory no local, pode configurar o Microsoft 365 Business Premium para proteger os seus dispositivos Windows 10, mantendo ao mesmo tempo o acesso a recursos no local que requerem autenticação local.</span><span class="sxs-lookup"><span data-stu-id="d9fc1-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="d9fc1-105">Para configurar esta proteção, pode implementar **dispositivos híbridos Azure AD.**</span><span class="sxs-lookup"><span data-stu-id="d9fc1-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="d9fc1-106">Estes dispositivos estão ligados tanto ao seu Ative Directory como ao seu Diretório Ativo Azure.</span><span class="sxs-lookup"><span data-stu-id="d9fc1-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="d9fc1-107">Este vídeo descreve os passos para como configurar isto para o cenário mais comum, que também é detalhado nos passos que se seguem.</span><span class="sxs-lookup"><span data-stu-id="d9fc1-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="d9fc1-108">1. Preparar para a sincronização do diretório</span><span class="sxs-lookup"><span data-stu-id="d9fc1-108">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="d9fc1-109">Antes de sincronizar os seus utilizadores e computadores a partir do domínio do Diretório Ativo local, [reveja Prepare-se para sincronização de diretórios para o Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="d9fc1-109">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="d9fc1-110">Em particular:</span><span class="sxs-lookup"><span data-stu-id="d9fc1-110">In particular:</span></span>

   - <span data-ttu-id="d9fc1-111">Certifique-se de que não existem duplicados no seu diretório para os seguintes atributos: **correio,** **proxyAddresses**e **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="d9fc1-111">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="d9fc1-112">Estes valores devem ser únicos e quaisquer duplicados devem ser removidos.</span><span class="sxs-lookup"><span data-stu-id="d9fc1-112">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="d9fc1-113">Recomendamos que configuure o atributo **userPrincipalName** (UPN) para cada conta de utilizador local para corresponder ao endereço de e-mail primário que corresponde ao utilizador licenciado microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d9fc1-113">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="d9fc1-114">Por exemplo: *mary.shelley@contoso.com* em vez *de mary@contoso.local*</span><span class="sxs-lookup"><span data-stu-id="d9fc1-114">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="d9fc1-115">Se o domínio ative Directory terminar num sufixo não-encaminhável como *.local* ou *.lan*, em vez de um sufixo de internet rotable como *.com* ou *.org*, ajuste o sufixo UPN das contas de utilizador locais primeiro como descrito na [Prepare um domínio não-encaminhável para sincronização de diretórios](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="d9fc1-115">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="d9fc1-116">2. Instalar e configurar a Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="d9fc1-116">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="d9fc1-117">Para sincronizar os seus utilizadores, grupos e contactos do Diretório Ativo local no Azure Ative Directory, instale o Azure Ative Directory Connect e crie sincronização de diretórios.</span><span class="sxs-lookup"><span data-stu-id="d9fc1-117">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> <span data-ttu-id="d9fc1-118">Consulte [a sincronização do diretório configurado para o Office 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) para saber mais.</span><span class="sxs-lookup"><span data-stu-id="d9fc1-118">See [Set up directory synchronization for Office 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) to learn more.</span></span>

> [!NOTE]
> <span data-ttu-id="d9fc1-119">Os passos são exatamente os mesmos para o Microsoft 365 para negócios.</span><span class="sxs-lookup"><span data-stu-id="d9fc1-119">The steps are exactly the same for Microsoft 365 for business.</span></span> 

<span data-ttu-id="d9fc1-120">Ao configurar as suas opções para Azure AD Connect, recomendamos que ative a **sincronização de passwords**, **o Sign-On único sem emenda**e a funcionalidade de writeback de **palavra-passe,** que também é suportada no Microsoft 365 para negócios.</span><span class="sxs-lookup"><span data-stu-id="d9fc1-120">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="d9fc1-121">Existem alguns passos adicionais para a gravação de palavras-passe para além da caixa de verificação no Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="d9fc1-121">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="d9fc1-122">Para obter mais informações, consulte [Como-a-fazer: configurar a gravação da palavra-passe](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="d9fc1-122">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

## <a name="3-configure-hybrid-azure-ad-join"></a><span data-ttu-id="d9fc1-123">3. Configurar híbrido Azure Ad Join</span><span class="sxs-lookup"><span data-stu-id="d9fc1-123">3. Configure Hybrid Azure AD Join</span></span>

<span data-ttu-id="d9fc1-124">Antes de ativar os dispositivos do Windows 10 para serem híbridos Azure AD, certifique-se de que cumpre os seguintes requisitos:</span><span class="sxs-lookup"><span data-stu-id="d9fc1-124">Before you enable Windows 10 devices to be Hybrid Azure AD joined, make sure that you meet the following prerequisites:</span></span>

   - <span data-ttu-id="d9fc1-125">Estás a executar a versão mais recente do Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="d9fc1-125">You're running the latest version of Azure AD Connect.</span></span>

   - <span data-ttu-id="d9fc1-126">A ligação AD AD azure sincronizou todos os objetos de computador dos dispositivos que pretende ser híbrido Azure AD ligados.</span><span class="sxs-lookup"><span data-stu-id="d9fc1-126">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined.</span></span> <span data-ttu-id="d9fc1-127">Se os objetos do computador pertencerem a unidades organizacionais específicas (OU), certifique-se de que estas OUs estão definidas para sincronização em Azure AD connect também.</span><span class="sxs-lookup"><span data-stu-id="d9fc1-127">If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>

<span data-ttu-id="d9fc1-128">Para registar os dispositivos existentes do Windows 10 unidos como Híbrido Azure AD aderiu, siga os passos no [Tutorial: Configure híbrido Azure Ative Directy junte-se a domínios geridos](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span><span class="sxs-lookup"><span data-stu-id="d9fc1-128">To register existing domain-joined Windows 10 devices as Hybrid Azure AD joined, follow the steps in the [Tutorial: Configure hybrid Azure Active Directory join for managed domains](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span></span> <span data-ttu-id="d9fc1-129">Isto permite que o seu Ative Directory existente no local se junte aos computadores windows 10 e os torne em nuvem.</span><span class="sxs-lookup"><span data-stu-id="d9fc1-129">This hybrid-enables your existing on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a><span data-ttu-id="d9fc1-130">4. Permitir a inscrição automática para o Windows 10</span><span class="sxs-lookup"><span data-stu-id="d9fc1-130">4. Enable automatic enrollment for Windows 10</span></span>

 <span data-ttu-id="d9fc1-131">Para inscrever automaticamente dispositivos Windows 10 para gestão de dispositivos móveis no Intune, consulte [inscrever automaticamente um dispositivo Windows 10 utilizando a Política de Grupo](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy).</span><span class="sxs-lookup"><span data-stu-id="d9fc1-131">To automatically enroll Windows 10 devices for mobile device management in Intune, see [Enroll a Windows 10 device automatically using Group Policy](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy).</span></span> <span data-ttu-id="d9fc1-132">Pode definir a Política de Grupo a nível de computador local, ou para operações a granel, pode utilizar os modelos de Consola de Gestão de Políticas de Grupo e ADMX para criar esta definição de Política de Grupo no seu Controlador de Domínio.</span><span class="sxs-lookup"><span data-stu-id="d9fc1-132">You can set the Group Policy at a local computer level, or for bulk operations, you can use the Group Policy Management Console and ADMX templates to create this Group Policy setting on your Domain Controller.</span></span>

## <a name="5-configure-seamless-single-sign-on"></a><span data-ttu-id="d9fc1-133">5. Configurar um único sinal sem emenda</span><span class="sxs-lookup"><span data-stu-id="d9fc1-133">5. Configure Seamless Single Sign-On</span></span>

  <span data-ttu-id="d9fc1-134">O Seamless SSO assina automaticamente os utilizadores nos seus recursos em nuvem Microsoft 365 quando utilizam computadores corporativos.</span><span class="sxs-lookup"><span data-stu-id="d9fc1-134">Seamless SSO automatically signs users into their Microsoft 365 cloud resources when they use corporate computers.</span></span> <span data-ttu-id="d9fc1-135">Basta implementar uma das duas opções de Política de Grupo descritas no [Azure Ative Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature).</span><span class="sxs-lookup"><span data-stu-id="d9fc1-135">Simply deploy one of the two Group Policy options described in [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature).</span></span> <span data-ttu-id="d9fc1-136">A opção **Política de Grupo** não permite que os utilizadores alterem as suas definições, enquanto a opção De Preferência de Política de **Grupo** define os valores, mas também os deixa configuráveis pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="d9fc1-136">The **Group Policy** option doesn't allow users to change their settings, while the **Group Policy Preference** option sets the values but also leaves them user-configurable.</span></span>

## <a name="6-set-up-windows-hello-for-business"></a><span data-ttu-id="d9fc1-137">6. Configurar o Windows Hello para o Negócio</span><span class="sxs-lookup"><span data-stu-id="d9fc1-137">6. Set up Windows Hello for Business</span></span>

 <span data-ttu-id="d9fc1-138">O Windows Hello for Business substitui as palavras-passe por uma autenticação forte de dois fatores (2FA) para iniciar sessão num computador local.</span><span class="sxs-lookup"><span data-stu-id="d9fc1-138">Windows Hello for Business replaces passwords with strong two-factor authentication (2FA) for signing into a local computer.</span></span> <span data-ttu-id="d9fc1-139">Um fator é um par de chave assimétrica, e o outro é um PIN ou outro gesto local, como impressão digital ou reconhecimento facial se o seu dispositivo o suportar.</span><span class="sxs-lookup"><span data-stu-id="d9fc1-139">One factor is an asymmetric key pair, and the other is a PIN or other local gesture such as fingerprint or facial recognition if your device supports it.</span></span> <span data-ttu-id="d9fc1-140">Recomendamos que substitua as palavras-passe por 2FA e Windows Hello para Negócios sempre que possível.</span><span class="sxs-lookup"><span data-stu-id="d9fc1-140">We recommend that you replace passwords with 2FA and Windows Hello for Business where possible.</span></span>

<span data-ttu-id="d9fc1-141">Para configurar o Hybrid Windows Hello for Business, reveja o [fundo híbrido Windows Hello for Business Prerequisites](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs).</span><span class="sxs-lookup"><span data-stu-id="d9fc1-141">To configure Hybrid Windows Hello for Business, review the [Hybrid Key trust Windows Hello for Business Prerequisites](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs).</span></span> <span data-ttu-id="d9fc1-142">Em seguida, siga as instruções em [Configurar Híbrido Windows Hello for Business key trust settings](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings).</span><span class="sxs-lookup"><span data-stu-id="d9fc1-142">Then follow the instructions in [Configure Hybrid Windows Hello for Business key trust settings](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings).</span></span> 
