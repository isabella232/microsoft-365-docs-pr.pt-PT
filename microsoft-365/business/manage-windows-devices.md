---
title: Ativar a gestão, por parte do Microsoft 365 Business, de dispositivos associados ao domínio Windows 10
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
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Saiba como permitir que o Microsoft 365 proteja o Ative Directory local juntou-se aos dispositivos windows 10.
ms.openlocfilehash: 170703c7367f9c0e9cb4c10edbd81cb214aa1d3e
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593807"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="e0730-103">Ativar a gestão, por parte do Microsoft 365 Business, de dispositivos associados ao domínio Windows 10</span><span class="sxs-lookup"><span data-stu-id="e0730-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="e0730-104">Se a sua organização utilizar o Diretório Ativo do Windows Server no local, pode configurar o Microsoft 365 Business para proteger os seus dispositivos Windows 10, mantendo ao mesmo tempo o acesso aos recursos no local que requerem autenticação local.</span><span class="sxs-lookup"><span data-stu-id="e0730-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="e0730-105">Para configurar esta proteção, pode implementar **dispositivos ad ad ad híbridos Azure**.</span><span class="sxs-lookup"><span data-stu-id="e0730-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="e0730-106">Estes dispositivos juntam-se tanto ao diretório ativo no local como ao seu Diretório Ativo Azure.</span><span class="sxs-lookup"><span data-stu-id="e0730-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="e0730-107">Este vídeo descreve os passos para configurar isto para o cenário mais comum, que também é detalhado nos passos que se seguem.</span><span class="sxs-lookup"><span data-stu-id="e0730-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="e0730-108">1. Preparar para sincronização de diretório</span><span class="sxs-lookup"><span data-stu-id="e0730-108">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="e0730-109">Antes de sincronizar os seus utilizadores e computadores do domínio de diretório ativo local, reveja [prepare-se para sincronização de diretório sincronia para o Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="e0730-109">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="e0730-110">Em especial:</span><span class="sxs-lookup"><span data-stu-id="e0730-110">In particular:</span></span>

   - <span data-ttu-id="e0730-111">Certifique-se de que não existem duplicados no seu diretório para os seguintes atributos: **correio,** **proxyAddresss**, e **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="e0730-111">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="e0730-112">Estes valores devem ser únicos e quaisquer duplicados devem ser removidos.</span><span class="sxs-lookup"><span data-stu-id="e0730-112">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="e0730-113">Recomendamos que configure o atributo do **userPrincipalName** (UPN) para cada conta de utilizador local para corresponder ao endereço de e-mail primário que corresponde ao utilizador licenciado da Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e0730-113">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="e0730-114">Por exemplo: *mary.shelley@contoso.com* em vez de *mary@contoso.local*</span><span class="sxs-lookup"><span data-stu-id="e0730-114">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="e0730-115">Se o domínio do Diretório Ativo terminar num sufixo não repreensível como *.local* ou *.lan*, em vez de um sufixo resaída à Internet, como *.com* ou *.org,* ajuste primeiro o sufixo UPN das contas de utilizador local, tal como descrito na [Prepare um domínio não repreensível para sincronização](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization)de diretórios.</span><span class="sxs-lookup"><span data-stu-id="e0730-115">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="e0730-116">2. Instale e configure a Ligação AD Azure</span><span class="sxs-lookup"><span data-stu-id="e0730-116">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="e0730-117">Para sincronizar os seus utilizadores, grupos e contactos do Diretório Ativo local em Azure Ative Directory, instale o Azure Ative Directory Connect e instale sincronização de diretórios.</span><span class="sxs-lookup"><span data-stu-id="e0730-117">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> <span data-ttu-id="e0730-118">Consulte a [sincronização do diretório para o Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) para saber mais.</span><span class="sxs-lookup"><span data-stu-id="e0730-118">See [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) to learn more.</span></span>

> [!NOTE]
> <span data-ttu-id="e0730-119">Os passos são exatamente os mesmos para o Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="e0730-119">The steps are exactly the same for Microsoft 365 Business.</span></span> 

<span data-ttu-id="e0730-120">À medida que configura as suas opções para O Azure AD Connect, recomendamos que ative a **Sincronização**de Passwords, **Um Único Sinal**perfeito e a funcionalidade de redação de **palavra-passe,** que também é suportada no Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="e0730-120">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 Business.</span></span>

> [!NOTE]
> <span data-ttu-id="e0730-121">Existem alguns passos adicionais para a reescrita de palavra-passe para além da caixa de verificação no Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="e0730-121">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="e0730-122">Para mais informações, consulte [Como: configurar a reescrita da palavra-passe](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="e0730-122">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

## <a name="3-configure-hybrid-azure-ad-join"></a><span data-ttu-id="e0730-123">3. Configure Hybrid Azure AD Aderir</span><span class="sxs-lookup"><span data-stu-id="e0730-123">3. Configure Hybrid Azure AD Join</span></span>

<span data-ttu-id="e0730-124">Antes de ativar os dispositivos Do Windows 10 para ser Hybrid Azure AD, certifique-se de que cumpre os seguintes pré-requisitos:</span><span class="sxs-lookup"><span data-stu-id="e0730-124">Before you enable Windows 10 devices to be Hybrid Azure AD joined, make sure that you meet the following prerequisites:</span></span>

   - <span data-ttu-id="e0730-125">Estás a executar a versão mais recente do Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="e0730-125">You're running the latest version of Azure AD Connect.</span></span>

   - <span data-ttu-id="e0730-126">A ligação Azure AD sincronizou todos os objetos informáticos dos dispositivos que pretende ser híbrido Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e0730-126">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined.</span></span> <span data-ttu-id="e0730-127">Se os objetos informáticos pertencerem a unidades organizacionais específicas (OU), certifique-se de que estas OUs estão definidas para sincronização em Azure AD connect também.</span><span class="sxs-lookup"><span data-stu-id="e0730-127">If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>

<span data-ttu-id="e0730-128">Para registar os dispositivos Windows 10 existentes à medida que o Hybrid Azure AD se juntou, siga os passos no [Tutorial: Configure hybrid Azure Ative Directory juntam-se para domínios geridos](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span><span class="sxs-lookup"><span data-stu-id="e0730-128">To register existing domain-joined Windows 10 devices as Hybrid Azure AD joined, follow the steps in the [Tutorial: Configure hybrid Azure Active Directory join for managed domains](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span></span> <span data-ttu-id="e0730-129">Este diretório ativo no local permite que o seu Diretório Ativo no local se junte aos computadores Windows 10 e os torne em nuvem prontas.</span><span class="sxs-lookup"><span data-stu-id="e0730-129">This hybrid-enables your existing on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a><span data-ttu-id="e0730-130">4. Ativar a inscrição automática para o Windows 10</span><span class="sxs-lookup"><span data-stu-id="e0730-130">4. Enable automatic enrollment for Windows 10</span></span>

 <span data-ttu-id="e0730-131">Para inscrever automaticamente os dispositivos do Windows 10 para gestão de dispositivos móveis em Intune, consulte [Inscrever automaticamente um dispositivo Windows 10 utilizando automaticamente a Política de Grupo](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy).</span><span class="sxs-lookup"><span data-stu-id="e0730-131">To automatically enroll Windows 10 devices for mobile device management in Intune, see [Enroll a Windows 10 device automatically using Group Policy](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy).</span></span> <span data-ttu-id="e0730-132">Pode definir a Política de Grupo a nível de computador local, ou para operações a granel, pode utilizar os modelos de Consola de Gestão de Políticas de Grupo e DEM para criar esta definição de Política de Grupo no seu Controlador de Domínio.</span><span class="sxs-lookup"><span data-stu-id="e0730-132">You can set the Group Policy at a local computer level, or for bulk operations, you can use the Group Policy Management Console and ADMX templates to create this Group Policy setting on your Domain Controller.</span></span>

## <a name="5-configure-seamless-single-sign-on"></a><span data-ttu-id="e0730-133">5. Configurar um único signo sem emenda</span><span class="sxs-lookup"><span data-stu-id="e0730-133">5. Configure Seamless Single Sign-On</span></span>

  <span data-ttu-id="e0730-134">O SSO SSO sem emenda sintetmente assina automaticamente os utilizadores nos seus recursos na nuvem Microsoft 365 quando utilizam computadores corporativos.</span><span class="sxs-lookup"><span data-stu-id="e0730-134">Seamless SSO automatically signs users into their Microsoft 365 cloud resources when they use corporate computers.</span></span> <span data-ttu-id="e0730-135">Basta implementar uma das duas opções de Política de Grupo descritas no [Azure Ative Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature).</span><span class="sxs-lookup"><span data-stu-id="e0730-135">Simply deploy one of the two Group Policy options described in [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature).</span></span> <span data-ttu-id="e0730-136">A opção Política de **Grupo** não permite que os utilizadores alterem as suas definições, enquanto a opção **De Preferência** política do grupo define os valores, mas também os deixa configurados pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="e0730-136">The **Group Policy** option doesn't allow users to change their settings, while the **Group Policy Preference** option sets the values but also leaves them user-configurable.</span></span>

## <a name="6-set-up-windows-hello-for-business"></a><span data-ttu-id="e0730-137">6. Configurar o Windows Hello for Business</span><span class="sxs-lookup"><span data-stu-id="e0730-137">6. Set up Windows Hello for Business</span></span>

 <span data-ttu-id="e0730-138">O Windows Hello for Business substitui as palavras-passe por uma autenticação forte de dois fatores (2FA) para a assinatura num computador local.</span><span class="sxs-lookup"><span data-stu-id="e0730-138">Windows Hello for Business replaces passwords with strong two-factor authentication (2FA) for signing into a local computer.</span></span> <span data-ttu-id="e0730-139">Um fator é um par de chaves assimétrica, e o outro é um PIN ou outro gesto local, como impressão digital ou reconhecimento facial se o seu dispositivo o suportar.</span><span class="sxs-lookup"><span data-stu-id="e0730-139">One factor is an asymmetric key pair, and the other is a PIN or other local gesture such as fingerprint or facial recognition if your device supports it.</span></span> <span data-ttu-id="e0730-140">Recomendamos que substitua as palavras-passe por 2FA e Windows Hello for Business sempre que possível.</span><span class="sxs-lookup"><span data-stu-id="e0730-140">We recommend that you replace passwords with 2FA and Windows Hello for Business where possible.</span></span>

<span data-ttu-id="e0730-141">Para configurar o Hybrid Windows Hello for Business, reveja a [chave híbrida do Windows Hello for Business Pré-requisitos.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs)</span><span class="sxs-lookup"><span data-stu-id="e0730-141">To configure Hybrid Windows Hello for Business, review the [Hybrid Key trust Windows Hello for Business Prerequisites](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs).</span></span> <span data-ttu-id="e0730-142">Em seguida, siga as instruções em [Configurar as definições](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings)de confiança da chave Híbrida Configure Hello for Business .</span><span class="sxs-lookup"><span data-stu-id="e0730-142">Then follow the instructions in [Configure Hybrid Windows Hello for Business key trust settings](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings).</span></span> 
