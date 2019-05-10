---
title: Configurar o Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
description: Obter informações sobre como configurar o Microsoft 365 Business.
ms.openlocfilehash: e635b828609fc47cd8b92bb179a25bcc43cb0a1a
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660875"
---
# <a name="set-up-microsoft-365-business"></a><span data-ttu-id="dca65-103">Configurar o Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="dca65-103">Set up Microsoft 365 Business</span></span>

<span data-ttu-id="dca65-104">Antes de começar, consulte [Obter Microsoft 365 Business](get-microsoft-365-business.md) para detalhes de inscrição.</span><span class="sxs-lookup"><span data-stu-id="dca65-104">Before you get started, see [Get Microsoft 365 Business](get-microsoft-365-business.md) for sign-up details.</span></span>

<span data-ttu-id="dca65-105">Ver um [vídeo de curta duração sobre como configurar o Microsoft 365 Business](https://support.office.com/article/38003e30-9d10-44cf-b596-f1b5f662bfa1) utilizando o conjunto de cópias de segurança assistente e quando não tiver um local, Active Directory</span><span class="sxs-lookup"><span data-stu-id="dca65-105">Watch a [short video on how to set up Microsoft 365 Business](https://support.office.com/article/38003e30-9d10-44cf-b596-f1b5f662bfa1) by using the set up wizard, and when you don't have an on-premises Active Directory</span></span>
  

## <a name="overview"></a><span data-ttu-id="dca65-106">Descrição Geral</span><span class="sxs-lookup"><span data-stu-id="dca65-106">Overview</span></span>

<span data-ttu-id="dca65-107">A maior parte dos passos de configuração pode ser efectuado no Assistente de configuração, mas as outras opções também se encontram listadas.</span><span class="sxs-lookup"><span data-stu-id="dca65-107">Most of the set up steps can be done in the setup wizard, but the other options are also listed.</span></span>

1. <span data-ttu-id="dca65-108">[Adicionar o domínio](#add-your-domain-to-personalize-sign-in) (se adquiriu o seu domínio durante a [inscrição](sign-up.md), este passo já é efectuado.)</span><span class="sxs-lookup"><span data-stu-id="dca65-108">[Add your domain](#add-your-domain-to-personalize-sign-in) (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>
2. <span data-ttu-id="dca65-109">Adicione utilizadores.</span><span class="sxs-lookup"><span data-stu-id="dca65-109">Add users.</span></span> <span data-ttu-id="dca65-110">Pode fazê-lo em qualquer uma das três formas:</span><span class="sxs-lookup"><span data-stu-id="dca65-110">You can do this in any of the three ways:</span></span>
    - <span data-ttu-id="dca65-111">No [Assistente de configuração](#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="dca65-111">In the [setup wizard](#add-users-in-the-wizard).</span></span>
    - <span data-ttu-id="dca65-112">Utilize a sincronização de directório para [Adicionar utilizadores utilizando Azure AD ligar](#add-users-by-using-azure-ad-connect) se tiver no local do Active directory.</span><span class="sxs-lookup"><span data-stu-id="dca65-112">Use directory synchronization to [add users by using Azure AD Connect](#add-users-by-using-azure-ad-connect) if you have an on-premises Active directory.</span></span>
    - <span data-ttu-id="dca65-113">Também pode [Adicionar utilizadores posteriormente](add-users-m365b.md) no Centro de administração.</span><span class="sxs-lookup"><span data-stu-id="dca65-113">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
3. <span data-ttu-id="dca65-114">Configurar políticas de segurança e configurar dispositivos.</span><span class="sxs-lookup"><span data-stu-id="dca65-114">Set up security policies and configure devices.</span></span> <span data-ttu-id="dca65-115">Pode fazê-lo em qualquer uma das três formas:</span><span class="sxs-lookup"><span data-stu-id="dca65-115">You can do this in any of the three ways:</span></span>
    - <span data-ttu-id="dca65-116">No [Assistente de configuração](#set-up-policies-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="dca65-116">In the [setup wizard](#set-up-policies-in-the-wizard).</span></span>  
    - <span data-ttu-id="dca65-117">No [Centro de administração](#modify-or-add-policies-in-the-admin-center).</span><span class="sxs-lookup"><span data-stu-id="dca65-117">In the [admin center](#modify-or-add-policies-in-the-admin-center).</span></span>
    - <span data-ttu-id="dca65-118">No [Centro de administração de Intune](https://docs.microsoft.com/intune/what-is-device-management).</span><span class="sxs-lookup"><span data-stu-id="dca65-118">In the [Intune admin center](https://docs.microsoft.com/intune/what-is-device-management).</span></span>
4. <span data-ttu-id="dca65-119">Configurar e gerir os dispositivos Windows 10.</span><span class="sxs-lookup"><span data-stu-id="dca65-119">Set up and manage Windows 10 devices.</span></span>

    <span data-ttu-id="dca65-120">Quando associa um dispositivo WIndows 10 a Azure AD, todas as políticas são aplicadas ao mesmo.</span><span class="sxs-lookup"><span data-stu-id="dca65-120">When you join a WIndows 10 device to Azure AD, all the policies get applied to it.</span></span>
    - <span data-ttu-id="dca65-121">Defina configurações de dispositivo do Windows 10 no [Assistente de configuração](#set-up-policies-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="dca65-121">Set up Windows 10 device configurations in the [setup wizard](#set-up-policies-in-the-wizard).</span></span>
    - <span data-ttu-id="dca65-122">Associe um [novo dispositivo de Windows 10](set-up-windows-devices.md#for-a-brand-new-or-newly-upgraded-windows-10-pro-device) a Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dca65-122">Join a [new Windows 10 device](set-up-windows-devices.md#for-a-brand-new-or-newly-upgraded-windows-10-pro-device) to Azure AD.</span></span>
    - <span data-ttu-id="dca65-123">Associe um [dispositivo existente do Windows 10](set-up-windows-devices.md#for-a-device-already-set-up-and-running-windows-10-pro) a Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dca65-123">Join an [existing Windows 10 device](set-up-windows-devices.md#for-a-device-already-set-up-and-running-windows-10-pro) to Azure AD.</span></span>
1. <span data-ttu-id="dca65-124">Instale o Office 365 Business.</span><span class="sxs-lookup"><span data-stu-id="dca65-124">Install Office 365 Business.</span></span>
    - <span data-ttu-id="dca65-125">Pode instalar automaticamente o Office nos dispositivos Windows utilizando o [Assistente de configuração](#set-up-policies-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="dca65-125">You can automatically install Office in the Windows devices by using the [setup wizard](#set-up-policies-in-the-wizard).</span></span>
    - <span data-ttu-id="dca65-126">Automaticamente a [instalar o Office](auto-install-or-uninstall-office.md) partir do Centro de administração.</span><span class="sxs-lookup"><span data-stu-id="dca65-126">Automatically [install Office](auto-install-or-uninstall-office.md) from the admin center.</span></span>
    - <span data-ttu-id="dca65-127">Permitir que os utilizadores [instalar aplicações do Office](https://docs.microsoft.com/office365/admin/setup/install-applications) para o Windows e dispositivos.</span><span class="sxs-lookup"><span data-stu-id="dca65-127">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
1. <span data-ttu-id="dca65-128">Configure segurança adicional.</span><span class="sxs-lookup"><span data-stu-id="dca65-128">Set up additional security.</span></span>
    - <span data-ttu-id="dca65-129">O Assistente de configuração adiciona políticas para proteger os dispositivos, mas também pode tirar partido das capacidades de [segurança adicionais](#additional-security-settings) para ajuda a proteger os dados, contas e mensagens de correio electrónico.</span><span class="sxs-lookup"><span data-stu-id="dca65-129">The setup wizard adds policies to secure your devices, but you can also take advantage of [additional security](#additional-security-settings) capabilities to helps secure your data, accounts, and emails.</span></span> 

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="dca65-130">Adicionar o domínio, utilizadores e configurar políticas</span><span class="sxs-lookup"><span data-stu-id="dca65-130">Add your domain, users and set up policies</span></span>

![Faixa que apontam para https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

<span data-ttu-id="dca65-132">Quando adquirir o Microsoft 365 Business, tem a opção de utilização de um domínio que possui ou comprar uma durante a [inscrição](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="dca65-132">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="dca65-133">Se tiver adquirido um novo domínio, quando se inscreve, o domínio é o conjunto de todas as cópias e pode mover para [Adicionar utilizadores e atribuir licenças](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="dca65-133">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="dca65-134">Adicionar o domínio para personalizar o início de sessão</span><span class="sxs-lookup"><span data-stu-id="dca65-134">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="dca65-135">Iniciar sessão no [Centro de administração do Microsoft 365](https://admin.microsoft.com) utilizando as credenciais de administrador global.</span><span class="sxs-lookup"><span data-stu-id="dca65-135">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="dca65-136">Seleccione **Adicionar um domínio** para iniciar o assistente.</span><span class="sxs-lookup"><span data-stu-id="dca65-136">Choose **Add a domain** to start the wizard.</span></span>

    ![Seleccione Adicionar um domínio.](media/addadomainadmincenter.png)
    
3. <span data-ttu-id="dca65-138">No assistente, introduza o nome de domínio que pretende utilizar (por exemplo, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="dca65-138">In the wizard, enter the domain name you want to use (like contoso.com).</span></span>


    ![Captura de ecrã de personalizar a página de início de sessão.](media/personalizesignin.png)

    
4. <span data-ttu-id="dca65-140">Siga os passos no Assistente para [registos de DNS criar em qualquer fornecedor de alojamento de DNS para o Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) , que verifica que possui o domínio.</span><span class="sxs-lookup"><span data-stu-id="dca65-140">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="dca65-141">Se souber o anfitrião de domínio, consulte também as [instruções específicas do anfitrião](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="dca65-141">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="dca65-142">Se o fornecedor de alojamento de GoDaddy, o processo é fácil e será automaticamente solicitado para iniciar sessão e informar a Microsoft autenticar em seu nome:</span><span class="sxs-lookup"><span data-stu-id="dca65-142">If your hosting provider is GoDaddy, the process is easy and you will be automatically asked to sign in and let Microsoft authenticate on your behalf:</span></span>

    ![Na página de acesso de confirmar GoDaddy, seleccione o autorizar.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="dca65-144">Adicionar utilizadores e atribuir licenças</span><span class="sxs-lookup"><span data-stu-id="dca65-144">Add users and assign licenses</span></span>

<span data-ttu-id="dca65-145">Pode adicionar utilizadores no assistente, mas também pode [Adicionar utilizadores posteriormente](add-users-m365b.md) no Centro de administração.</span><span class="sxs-lookup"><span data-stu-id="dca65-145">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="dca65-146">Além disso, se tiver um controlador de domínio local, pode adicionar os utilizadores com [Azure AD ligar](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="dca65-146">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="dca65-147">Adicionar utilizadores no Assistente</span><span class="sxs-lookup"><span data-stu-id="dca65-147">Add users in the wizard</span></span>

<span data-ttu-id="dca65-148">Qualquer utilizador que adicione no assistente obter atribui automaticamente uma licença do Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="dca65-148">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>
<span data-ttu-id="dca65-149">Se tiver um controlador de domínio local e estiver a utilizar o Active Directory, consulte [como os utilizadores de ddd utilizando Azure AD ligar](#add-users-by-using-azure-ad-connect).</span><span class="sxs-lookup"><span data-stu-id="dca65-149">If you have a local domain controller, and are using Active Directory, see [how to ddd users by using Azure AD Connect](#add-users-by-using-azure-ad-connect).</span></span>

![Instantâneo da página Adicionar de utilizadores novo no Assistente](media/addnewuserspage.png)

1. <span data-ttu-id="dca65-p106">Se a sua subscrição do Microsoft 365 Business já tiver utilizadores existentes (por exemplo, se utilizou o Azure AD Connect), verá uma opção para atribuir licenças aos mesmos agora. Continue o processo e adicione licenças aos utilizadores.</span><span class="sxs-lookup"><span data-stu-id="dca65-p106">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you will get an option to assign licenses to them now. Go ahead and add licenses to them as well.</span></span>

3. <span data-ttu-id="dca65-153">Depois de ter adicionado os utilizadores, também terá a opção de partilhar as credenciais com os novos utilizadores que adicionou.</span><span class="sxs-lookup"><span data-stu-id="dca65-153">After you have added the users, you will also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="dca65-154">Pode optar por imprimir, transferir ou enviá-las por e-mail.</span><span class="sxs-lookup"><span data-stu-id="dca65-154">You can choose to print them out, email them, or download them.</span></span>

4. <span data-ttu-id="dca65-155">Ignore a migração de mensagens de e-mail e selecione **Seguinte** na página **Migrar as mensagens de e-mail**.</span><span class="sxs-lookup"><span data-stu-id="dca65-155">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 

    <span data-ttu-id="dca65-156">Se estiver a mover de outro fornecedor de correio electrónico e pretender copiar os dados mais tarde, pode [Migrar correio-electrónico e contactos para o Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span><span class="sxs-lookup"><span data-stu-id="dca65-156">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>

#### <a name="add-users-by-using-azure-ad-connect"></a><span data-ttu-id="dca65-157">Adicionar utilizadores utilizando Azure ligar AD</span><span class="sxs-lookup"><span data-stu-id="dca65-157">Add users by using Azure AD Connect</span></span>

 <span data-ttu-id="dca65-158">Se tiver um controlador de domínio local com o Active Directory, sincronizar os utilizadores com o Microsoft 365 Business utilizando [Azure AD ligar](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="dca65-158">If you have a local domain controller with Active Directory, you synchronize your users with Microsoft 365 Business by using [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span> <span data-ttu-id="dca65-159">Preencha esta opção antes de iniciar o Assistente de configuração.</span><span class="sxs-lookup"><span data-stu-id="dca65-159">Complete this before you start the setup wizard.</span></span> <span data-ttu-id="dca65-160">Pode transferi-lo no Centro de administração:</span><span class="sxs-lookup"><span data-stu-id="dca65-160">You can download it in the admin center:</span></span>

- <span data-ttu-id="dca65-161">Vá para **os utilizadores** \> **utilizadores activos**, seleccione nas reticências na parte superior da página e, em seguida, seleccione **sincronização de directórios** para transferir Azure AD ligar.</span><span class="sxs-lookup"><span data-stu-id="dca65-161">Go to **Users** \> **Active users**, select the ellipses on the top of the page and then select **Directory synchronization** to download Azure AD Connect.</span></span>

    ![Na página utilizadores do Active seleccione elipses > directório snchronization.](media/setupdirsync.png)

    > [!IMPORTANT]
    > <span data-ttu-id="dca65-163">Se criar os utilizadores desta forma, ainda terá de atribuir licenças aos mesmos no Centro de administração.</span><span class="sxs-lookup"><span data-stu-id="dca65-163">If you create users this way, you will still have to assign licenses to them in the admin center.</span></span>

##### <a name="continue-to-access-domain-joined-apps-and-devices"></a><span data-ttu-id="dca65-164">Continuar a aceder a dispositivos e aplicações associado ao domínio</span><span class="sxs-lookup"><span data-stu-id="dca65-164">Continue to access domain-joined apps and devices</span></span>

<span data-ttu-id="dca65-165">Se pretender continuar a aceder a dispositivos e aplicações associado ao domínio, consulte os seguintes artigos para dois outra forma de permitir que:</span><span class="sxs-lookup"><span data-stu-id="dca65-165">If you want to continue to access domain-joined apps and devices, read the following articles for two different way of enabling that:</span></span>
  
- [<span data-ttu-id="dca65-166">Ativar a gestão, por parte do Microsoft 365 Business, de dispositivos associados ao domínio Windows 10</span><span class="sxs-lookup"><span data-stu-id="dca65-166">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>](manage-windows-devices.md)
    - <span data-ttu-id="dca65-167">Esta é a forma recomendada.</span><span class="sxs-lookup"><span data-stu-id="dca65-167">This is the recommended way.</span></span>

- [<span data-ttu-id="dca65-168">Acesso local recursos a partir de um dispositivo associado AD Azure no Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="dca65-168">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>](access-resources.md)

### <a name="connect-your-domain"></a><span data-ttu-id="dca65-169">Ligar o seu domínio</span><span class="sxs-lookup"><span data-stu-id="dca65-169">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="dca65-170">Se optou por utilizar o domínio de .onmicrosoft, ou utilizado Azure AD ligar para configurar utilizadores, não verá este passo.</span><span class="sxs-lookup"><span data-stu-id="dca65-170">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="dca65-171">Para configurar serviços, tem de atualizar alguns registos no seu anfitrião de DNS ou entidade de registo de domínios.</span><span class="sxs-lookup"><span data-stu-id="dca65-171">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="dca65-172">Normalmente, o assistente de configuração deteta a sua entidade de registo e fornece-lhe uma ligação para instruções passo a passo de forma a atualizar os seus registos NS no site da entidade de registo de domínios.</span><span class="sxs-lookup"><span data-stu-id="dca65-172">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="dca65-173">Caso contrário, [nameservers de alteração para configurar o Office 365 qualquer registo de domínio](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="dca65-173">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="dca65-174">Se tiver registos DNS existentes, por exemplo um web site existente, irá pretender gerir os seus próprios registos DNS para se certificar de que os serviços existentes permanecem ligados.</span><span class="sxs-lookup"><span data-stu-id="dca65-174">If you have existing DNS records, for example an existing web site, you will want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="dca65-175">Consulte [Noções básicas de domínio](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="dca65-175">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Ligar o seu domínio página com irá gerir os meus próprios registos DNS.](media/connectyourdomainpage.png)

2. <span data-ttu-id="dca65-177">Siga os passos no assistente e correio electrónico e outros serviços serão configurados para si.</span><span class="sxs-lookup"><span data-stu-id="dca65-177">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="set-up-security-policies-and-device-configurations"></a><span data-ttu-id="dca65-178">Configurar políticas de segurança e configurações de dispositivo</span><span class="sxs-lookup"><span data-stu-id="dca65-178">Set up security policies and device configurations</span></span> 

<span data-ttu-id="dca65-179">Estas políticas aplicam-se para cada utilizador fornecer uma licença para ou a um grupo de utilizadores se optar por atribuir diferentes políticas a um conjunto de utilizadores.</span><span class="sxs-lookup"><span data-stu-id="dca65-179">These policies apply to every user you give a license to, or to a group of users if you decide to assign different policies to a set of users.</span></span>

#### <a name="set-up-policies-in-the-wizard"></a><span data-ttu-id="dca65-180">Configurar políticas no Assistente</span><span class="sxs-lookup"><span data-stu-id="dca65-180">Set up policies in the wizard</span></span>

<span data-ttu-id="dca65-181">As políticas que configura no assistente são aplicadas automaticamente a um [grupo de segurança](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) denominado *Todos os utilizadores*.</span><span class="sxs-lookup"><span data-stu-id="dca65-181">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span>

1. <span data-ttu-id="dca65-182">Na **proteger os ficheiros de trabalho em dispositivos móveis** a opção **proteger ficheiros de trabalho quando dispositivos perdidos ou roubados** está seleccionada por predefinição.</span><span class="sxs-lookup"><span data-stu-id="dca65-182">On the **Protect your work files on mobile devices** the option **Protect work files when devices are lost or stolen** is selected by default.</span></span> <span data-ttu-id="dca65-183">Tem uma opção para activar a **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis**, e este procedimento é recomendado.</span><span class="sxs-lookup"><span data-stu-id="dca65-183">You have an option to turn on **Manage how users access Office files on mobile devices**, and this is recommended.</span></span>

    ![Captura de ecrã de proteger ficheiros de trabalho na página de dispositivos móveis.](media/protectworkfilesondevices.png)

     - <span data-ttu-id="dca65-185">Se expandir **proteger ficheiros de trabalho quando dispositivos perdidos ou roubados**, os [valores predefinidos](protect-work-files-on-lost-or-stolen-device.md) estão pré-seleccionadas:</span><span class="sxs-lookup"><span data-stu-id="dca65-185">If you expand **Protect work files when devices are lost or stolen**, the [default values](protect-work-files-on-lost-or-stolen-device.md) are pre-selected:</span></span>

        ![Captura de ecrã de valores predefinidos para proteger ficheiros em dispositivos perdidos.](media/protectworkfilesondevicesdefault.png)

    - <span data-ttu-id="dca65-187">Se seleccionar a **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis** e expandi-lo, os [valores predefinidos](manage-user-access-on-mobile-devices.md) são apresentados.</span><span class="sxs-lookup"><span data-stu-id="dca65-187">If you select **Manage how users access Office files on mobile devices** and expand it, the [default values](manage-user-access-on-mobile-devices.md) are shown.</span></span> <span data-ttu-id="dca65-188">Recomendamos que aceite os valores predefinidos durante a configuração para criar políticas de aplicações para Android, iOS e Windows 10 que se apliquem a todos os utilizadores.</span><span class="sxs-lookup"><span data-stu-id="dca65-188">We recommend you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="dca65-189">Poderá criar políticas adicionais após a configuração estar concluída.</span><span class="sxs-lookup"><span data-stu-id="dca65-189">You can create more policies after setup completes.</span></span>

        ![Captura de ecrã de definições de protecção de ficheiros do Office no telemóvel.](media/useraccessonmobile.png)

2. <span data-ttu-id="dca65-191">O último passo no proteger os dados e dispositivos permite-lhe definir políticas para proteger o Windows 10 dispositivos.</span><span class="sxs-lookup"><span data-stu-id="dca65-191">The last step on protect data and devices allows you to set up policies to secure Windows 10 devices.</span></span> <span data-ttu-id="dca65-192">Estas definições são aplicadas automaticamente quando Windows 10 um utilizador liga a sua organização.</span><span class="sxs-lookup"><span data-stu-id="dca65-192">These settings are applied automatically when a user's Windows 10 connects to your organization.</span></span> <span data-ttu-id="dca65-193">Pode expandir **Secure Windows 10 dispositivos** para ver e modificar os [valores predefinidos](secure-windows-10-devices.md).</span><span class="sxs-lookup"><span data-stu-id="dca65-193">You can expand **Secure Windows 10 devices** to see and modify the [default values](secure-windows-10-devices.md).</span></span>
3. <span data-ttu-id="dca65-194">Também pode optar por [instalar automaticamente o Office](install-office-on-windows-10-during-setup.md) no Windows 10 dispositivos.</span><span class="sxs-lookup"><span data-stu-id="dca65-194">You can also choose to [automatically install Office](install-office-on-windows-10-during-setup.md) on Windows 10 devices.</span></span>

    ![Instantâneo da Definir página de configuração do Windows 10 dispositivo.](media/setwin10config.png)

#### <a name="modify-or-add-policies-in-the-admin-center"></a><span data-ttu-id="dca65-196">Modificar ou adicionar políticas no Centro de administração</span><span class="sxs-lookup"><span data-stu-id="dca65-196">Modify or add policies in the admin center</span></span>

<span data-ttu-id="dca65-197">Consulte [Gerir Microsoft 365 Business](manage.md) para ligações a tópicos sobre como visualizar e modificar a protecção de dispositivo e aplicação de políticas e como remover dados a partir de ou repor dispositivos de utilizador.</span><span class="sxs-lookup"><span data-stu-id="dca65-197">See [manage Microsoft 365 Business](manage.md) for links to topics on how to view and modify device and app protection polices, and how to remove data from, or reset user devices.</span></span>

## <a name="deploy-and-manage-windows-10"></a><span data-ttu-id="dca65-198">Implementar e gerir o Windows 10</span><span class="sxs-lookup"><span data-stu-id="dca65-198">Deploy and manage Windows 10</span></span>
<span data-ttu-id="dca65-199">Consulte [Configurar dispositivos do Windows para utilizadores empresariais do Microsoft 365](set-up-windows-devices.md) para ligar manualmente a Azure AD, quer durante a configuração para novos computadores, ou alterando o perfil de início de sessão para os computadores existentes.</span><span class="sxs-lookup"><span data-stu-id="dca65-199">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) to manually connect to Azure AD, either during setup for new computers, or by changing sign-in profile for existing computers.</span></span> 

### <a name="use-autopilot-to-set-up-new-devices"></a><span data-ttu-id="dca65-200">Utilizar o piloto automático para configurar novos dispositivos</span><span class="sxs-lookup"><span data-stu-id="dca65-200">Use Autopilot to set up new devices</span></span>

<span data-ttu-id="dca65-201">Pode utilizar o [Piloto automático do Windows](add-autopilot-devices-and-profile.md) para pré-configurar automaticamente **novos** dispositivos Windows 10 para um utilizador, mas poderá ser mais fácil obter um [parceiro](https://www.microsoft.com/solution-providers/search) que pode fazer isto por si.</span><span class="sxs-lookup"><span data-stu-id="dca65-201">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="dca65-202">Também pode ir para o [Arquivo do Microsoft](https://go.microsoft.com/fwlink/?linkid=874598) e peça um perito em tecnologia nuvem configurar novos dispositivos de compras para si.</span><span class="sxs-lookup"><span data-stu-id="dca65-202">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) and ask a cloud technology expert set up new devices you purchase for you.</span></span>

### <a name="access-on-premises-resources"></a><span data-ttu-id="dca65-203">Aceder a recursos no local</span><span class="sxs-lookup"><span data-stu-id="dca65-203">Access on-premises resources</span></span>

<span data-ttu-id="dca65-204">Se a organização utilizar o Windows Server Active Directory no local, pode configurar o Microsoft 365 Business para proteger os dispositivos Windows 10, mantendo o acesso a recursos locais que requerem autenticação local.</span><span class="sxs-lookup"><span data-stu-id="dca65-204">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="dca65-205">Siga os passos em [activar dispositivos associados ao domínio de Windows 10 para serem geridos pelo Microsoft 365 Business](manage-windows-devices.md) para configurar esta tarefa.</span><span class="sxs-lookup"><span data-stu-id="dca65-205">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="dca65-206">Este é o método preferido e dispositivos neste estado são denominados híbrido Azure AD associado dispositivos.</span><span class="sxs-lookup"><span data-stu-id="dca65-206">This is the preferred method and devices in this state are called Hybrid Azure AD joined devices.</span></span>

<span data-ttu-id="dca65-207">Se a empresa possui um local do Active Directory que contém alguns locais recursos (tais como partilhas de ficheiros e impressoras), pode conceder acesso a dispositivos Azure AD associados a estes recursos seguindo os passos aqui: [acesso local recursos de um Dispositivo Azure AD associados no Microsoft 365 Business](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="dca65-207">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers) , you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="dca65-208">Implementar aplicações de cliente do Office 365</span><span class="sxs-lookup"><span data-stu-id="dca65-208">Deploy Office 365 client apps</span></span>

<span data-ttu-id="dca65-209">Se optar por instalar automaticamente aplicações do Office no durante o conjunto de cópias, as aplicações instalará nos dispositivos Windows 10 depois dos utilizadores têm sessão iniciada no Azure AD dos dispositivos do Windows com as respectivas credenciais de trabalho.</span><span class="sxs-lookup"><span data-stu-id="dca65-209">If you chose to automatically install Office apps in during the set up, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices with their work credentials.</span></span>
<span data-ttu-id="dca65-210">Para instalar o Office iOS móvel ou dispositivos Android, consulte [Configurar dispositivos móveis para utilizadores empresariais do Microsoft 365](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="dca65-210">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="dca65-211">Pode também instalar o Office individualmente.</span><span class="sxs-lookup"><span data-stu-id="dca65-211">You can also install Office individually.</span></span> <span data-ttu-id="dca65-212">Consulte a [instalar o Office num PC ou Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) para obter instruções.</span><span class="sxs-lookup"><span data-stu-id="dca65-212">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) for instructions.</span></span>

## <a name="additional-security-settings"></a><span data-ttu-id="dca65-213">Definições de segurança adicionais</span><span class="sxs-lookup"><span data-stu-id="dca65-213">Additional security settings</span></span>

<span data-ttu-id="dca65-214">Para além da segurança e a definição de conformidade no Assistente de configuração, pode também configurar as seguintes definições adicionais:</span><span class="sxs-lookup"><span data-stu-id="dca65-214">In addition to the security and compliance setting in the setup wizard, you can also set up the following additional settings:</span></span>
  
- <span data-ttu-id="dca65-215">**Mensagem de correio electrónico de protecção contra malware**</span><span class="sxs-lookup"><span data-stu-id="dca65-215">**Email malware protection**</span></span>
- <span data-ttu-id="dca65-216">**Anexos seguros de protecção (ATP) ameaça avançadas**</span><span class="sxs-lookup"><span data-stu-id="dca65-216">**Advanced Threat Protection (ATP) Safe Attachments**</span></span>
- <span data-ttu-id="dca65-217">**Hiperligações de seguro de ATP**</span><span class="sxs-lookup"><span data-stu-id="dca65-217">**ATP Safe Links**</span></span>
- <span data-ttu-id="dca65-218">**APT anti-phishing**</span><span class="sxs-lookup"><span data-stu-id="dca65-218">**APT anti-phishing**</span></span>
- <span data-ttu-id="dca65-219">**Arquivo do Exchange Online**</span><span class="sxs-lookup"><span data-stu-id="dca65-219">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="dca65-220">**Prevenção de perda de dados (DLP)**</span><span class="sxs-lookup"><span data-stu-id="dca65-220">**Data loss prevention (DLP)**</span></span>
- <span data-ttu-id="dca65-221">**Protecção de informações Azure** (Planear 1)</span><span class="sxs-lookup"><span data-stu-id="dca65-221">**Azure Information Protection** (Plan 1)</span></span>
- <span data-ttu-id="dca65-222">**Disponibilidade de portal Intune**</span><span class="sxs-lookup"><span data-stu-id="dca65-222">**Intune portal availability**</span></span>

<span data-ttu-id="dca65-223">Para obter iniciado, consulte [Configurar políticas de segurança avançada](set-up-advanced-security.md).</span><span class="sxs-lookup"><span data-stu-id="dca65-223">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

<span data-ttu-id="dca65-224">Consulte também [10 principais formas de proteger o seu negócio de 365 da Microsoft](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) para obter um guia de procedimentos recomendados de segurança.</span><span class="sxs-lookup"><span data-stu-id="dca65-224">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>