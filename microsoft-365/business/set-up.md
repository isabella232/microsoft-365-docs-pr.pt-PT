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
ms.openlocfilehash: f3a9ad62f5ec8779296e800b9ecc8d6181d7aff7
ms.sourcegitcommit: f420a5cdedf3ec2babc6d8ad7e7c79da0b08e115
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/13/2019
ms.locfileid: "33966984"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="49f2f-103">Configurar o Microsoft 365 Business no Assistente de configuração</span><span class="sxs-lookup"><span data-stu-id="49f2f-103">Set up Microsoft 365 Business in the setup wizard</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="49f2f-104">Adicionar o domínio, utilizadores e configurar políticas</span><span class="sxs-lookup"><span data-stu-id="49f2f-104">Add your domain, users, and set up policies</span></span>

![Faixa que apontam para https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

<span data-ttu-id="49f2f-106">Quando adquirir o Microsoft 365 Business, tem a opção de utilização de um domínio que possui ou comprar uma durante a [inscrição](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="49f2f-106">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="49f2f-107">Se tiver adquirido um novo domínio, quando se inscreve, o domínio é o conjunto de todas as cópias e pode mover para [Adicionar utilizadores e atribuir licenças](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="49f2f-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="49f2f-108">Adicionar o domínio para personalizar o início de sessão</span><span class="sxs-lookup"><span data-stu-id="49f2f-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="49f2f-109">Iniciar sessão no [Centro de administração do Microsoft 365](https://admin.microsoft.com) utilizando as credenciais de administrador global.</span><span class="sxs-lookup"><span data-stu-id="49f2f-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="49f2f-110">Optar por **Adicionar um domínio** ou **Adicionar utilizadores** para iniciar o assistente.</span><span class="sxs-lookup"><span data-stu-id="49f2f-110">Choose **Add a domain** or **Add users** to start the wizard.</span></span>
    > [!IMPORTANT]
    > <span data-ttu-id="49f2f-111">Se tiver adquirido um domínio durante a inscrição, irá não consulte **Adicionar um domínio do** passo aqui.</span><span class="sxs-lookup"><span data-stu-id="49f2f-111">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="49f2f-112">Vá para [Adicionar utilizadores](#add-users-and-assign-licenses) em vez disso.</span><span class="sxs-lookup"><span data-stu-id="49f2f-112">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![Seleccione Adicionar um domínio.](media/addadomainadmincenter.png)
    
3. <span data-ttu-id="49f2f-114">No assistente, introduza o nome de domínio que pretende utilizar (por exemplo, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="49f2f-114">In the wizard, enter the domain name you want to use (like contoso.com).</span></span>


    ![Captura de ecrã de personalizar a página de início de sessão.](media/personalizesignin.png)

    
4. <span data-ttu-id="49f2f-116">Siga os passos no Assistente para [registos de DNS criar em qualquer fornecedor de alojamento de DNS para o Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) , que verifica que possui o domínio.</span><span class="sxs-lookup"><span data-stu-id="49f2f-116">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="49f2f-117">Se souber o anfitrião de domínio, consulte também as [instruções específicas do anfitrião](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="49f2f-117">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="49f2f-118">Se o fornecedor de alojamento de GoDaddy, o processo é fácil e será automaticamente solicitado para iniciar sessão e informar a Microsoft autenticar em seu nome:</span><span class="sxs-lookup"><span data-stu-id="49f2f-118">If your hosting provider is GoDaddy, the process is easy and you will be automatically asked to sign in and let Microsoft authenticate on your behalf:</span></span>

    ![Na página de acesso de confirmar GoDaddy, seleccione o autorizar.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="49f2f-120">Adicionar utilizadores e atribuir licenças</span><span class="sxs-lookup"><span data-stu-id="49f2f-120">Add users and assign licenses</span></span>

<span data-ttu-id="49f2f-121">Pode adicionar utilizadores no assistente, mas também pode [Adicionar utilizadores posteriormente](add-users-m365b.md) no Centro de administração.</span><span class="sxs-lookup"><span data-stu-id="49f2f-121">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="49f2f-122">Além disso, se tiver um controlador de domínio local, pode adicionar os utilizadores com [Azure AD ligar](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="49f2f-122">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="49f2f-123">Adicionar utilizadores no Assistente</span><span class="sxs-lookup"><span data-stu-id="49f2f-123">Add users in the wizard</span></span>

<span data-ttu-id="49f2f-124">Qualquer utilizador que adicione no assistente obter atribui automaticamente uma licença do Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="49f2f-124">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![Instantâneo da página Adicionar de utilizadores novo no Assistente](media/addnewuserspage.png)

1. <span data-ttu-id="49f2f-126">Se a sua subscrição do Microsoft 365 Business tem utilizadores existentes (por exemplo, se utilizou Azure ligar AD), receberá uma opção para atribuir-lhes licenças agora.</span><span class="sxs-lookup"><span data-stu-id="49f2f-126">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you get an option to assign licenses to them now.</span></span> <span data-ttu-id="49f2f-127">Continue o processo e adicione licenças aos utilizadores.</span><span class="sxs-lookup"><span data-stu-id="49f2f-127">Go ahead and add licenses to them as well.</span></span>

3. <span data-ttu-id="49f2f-128">Depois de ter adicionado os utilizadores, também terá a opção de partilhar as credenciais com os novos utilizadores que adicionou.</span><span class="sxs-lookup"><span data-stu-id="49f2f-128">After you have added the users, you will also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="49f2f-129">Pode optar por imprimir, transferir ou enviá-las por e-mail.</span><span class="sxs-lookup"><span data-stu-id="49f2f-129">You can choose to print them out, email them, or download them.</span></span>

4. <span data-ttu-id="49f2f-130">Ignore a migração de mensagens de e-mail e selecione **Seguinte** na página **Migrar as mensagens de e-mail**.</span><span class="sxs-lookup"><span data-stu-id="49f2f-130">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 

    <span data-ttu-id="49f2f-131">Se estiver a mover de outro fornecedor de correio electrónico e pretender copiar os dados mais tarde, pode [Migrar correio-electrónico e contactos para o Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span><span class="sxs-lookup"><span data-stu-id="49f2f-131">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>


### <a name="connect-your-domain"></a><span data-ttu-id="49f2f-132">Ligar o seu domínio</span><span class="sxs-lookup"><span data-stu-id="49f2f-132">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="49f2f-133">Se optou por utilizar o domínio de .onmicrosoft, ou utilizado Azure AD ligar para configurar utilizadores, não verá este passo.</span><span class="sxs-lookup"><span data-stu-id="49f2f-133">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="49f2f-134">Para configurar serviços, tem de atualizar alguns registos no seu anfitrião de DNS ou entidade de registo de domínios.</span><span class="sxs-lookup"><span data-stu-id="49f2f-134">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="49f2f-135">Normalmente, o assistente de configuração deteta a sua entidade de registo e fornece-lhe uma ligação para instruções passo a passo de forma a atualizar os seus registos NS no site da entidade de registo de domínios.</span><span class="sxs-lookup"><span data-stu-id="49f2f-135">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="49f2f-136">Caso contrário, [nameservers de alteração para configurar o Office 365 qualquer registo de domínio](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="49f2f-136">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="49f2f-137">Se tiver registos DNS existentes, por exemplo um web site existente, irá pretender gerir os seus próprios registos DNS para se certificar de que os serviços existentes permanecem ligados.</span><span class="sxs-lookup"><span data-stu-id="49f2f-137">If you have existing DNS records, for example an existing web site, you will want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="49f2f-138">Consulte [Noções básicas de domínio](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="49f2f-138">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Ligar o seu domínio página com irá gerir os meus próprios registos DNS.](media/connectyourdomainpage.png)

2. <span data-ttu-id="49f2f-140">Siga os passos no assistente e correio electrónico e outros serviços serão configurados para si.</span><span class="sxs-lookup"><span data-stu-id="49f2f-140">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="set-up-security-policies-and-device-configurations"></a><span data-ttu-id="49f2f-141">Configurar políticas de segurança e configurações de dispositivo</span><span class="sxs-lookup"><span data-stu-id="49f2f-141">Set up security policies and device configurations</span></span> 

<span data-ttu-id="49f2f-142">As políticas que configura no assistente são aplicadas automaticamente a um [grupo de segurança](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) denominado *Todos os utilizadores*.</span><span class="sxs-lookup"><span data-stu-id="49f2f-142">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="49f2f-143">Também pode criar grupos adicionais para atribuir políticas para no Centro de administração.</span><span class="sxs-lookup"><span data-stu-id="49f2f-143">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="49f2f-144">Na **proteger os ficheiros de trabalho em dispositivos móveis** a opção **proteger ficheiros de trabalho quando dispositivos perdidos ou roubados** está seleccionada por predefinição.</span><span class="sxs-lookup"><span data-stu-id="49f2f-144">On the **Protect your work files on mobile devices** the option **Protect work files when devices are lost or stolen** is selected by default.</span></span> <span data-ttu-id="49f2f-145">Tem uma opção para activar a **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis**, e este procedimento é recomendado.</span><span class="sxs-lookup"><span data-stu-id="49f2f-145">You have an option to turn on **Manage how users access Office files on mobile devices**, and this is recommended.</span></span>

    ![Captura de ecrã de proteger ficheiros de trabalho na página de dispositivos móveis.](media/protectworkfilesondevices.png)

     - <span data-ttu-id="49f2f-147">Expanda a **proteger ficheiros de trabalho quando dispositivos perdidos ou roubados** para apresentar os [valores predefinidos](protect-work-files-on-lost-or-stolen-device.md):</span><span class="sxs-lookup"><span data-stu-id="49f2f-147">Expand **Protect work files when devices are lost or stolen** to display the [default values](protect-work-files-on-lost-or-stolen-device.md):</span></span>

        ![Captura de ecrã de valores predefinidos para proteger ficheiros em dispositivos perdidos.](media/protectworkfilesondevicesdefault.png)

    - <span data-ttu-id="49f2f-149">Seleccione **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis** e expandi-lo para apresentar os [valores predefinidos](manage-user-access-on-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="49f2f-149">Select **Manage how users access Office files on mobile devices** and expand it to display the [default values](manage-user-access-on-mobile-devices.md).</span></span> <span data-ttu-id="49f2f-150">Recomendamos que aceite os valores predefinidos durante a configuração para criar políticas de aplicação para Android, iOS e 10 do Windows que se aplicam a todos os utilizadores.</span><span class="sxs-lookup"><span data-stu-id="49f2f-150">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="49f2f-151">Poderá criar políticas adicionais após a configuração estar concluída.</span><span class="sxs-lookup"><span data-stu-id="49f2f-151">You can create more policies after setup completes.</span></span>

        ![Captura de ecrã de definições de protecção de ficheiros do Office no telemóvel.](media/useraccessonmobile.png)

2. <span data-ttu-id="49f2f-153">O último passo no proteger os dados e dispositivos permite-lhe definir políticas para proteger o Windows 10 dispositivos.</span><span class="sxs-lookup"><span data-stu-id="49f2f-153">The last step on protect data and devices allows you to set up policies to secure Windows 10 devices.</span></span> <span data-ttu-id="49f2f-154">Estas definições são aplicadas automaticamente quando Windows 10 um utilizador liga a sua organização.</span><span class="sxs-lookup"><span data-stu-id="49f2f-154">These settings are applied automatically when a user's Windows 10 connects to your organization.</span></span> <span data-ttu-id="49f2f-155">Pode expandir **Secure Windows 10 dispositivos** para ver e modificar os [valores predefinidos](secure-windows-10-devices.md).</span><span class="sxs-lookup"><span data-stu-id="49f2f-155">You can expand **Secure Windows 10 devices** to see and modify the [default values](secure-windows-10-devices.md).</span></span>
3. <span data-ttu-id="49f2f-156">Também pode optar por [instalar automaticamente o Office](install-office-on-windows-10-during-setup.md) no Windows 10 dispositivos.</span><span class="sxs-lookup"><span data-stu-id="49f2f-156">You can also choose to [automatically install Office](install-office-on-windows-10-during-setup.md) on Windows 10 devices.</span></span>

    ![Instantâneo da Definir página de configuração do Windows 10 dispositivo.](media/setwin10config.png)



## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="49f2f-158">Implementar aplicações de cliente do Office 365</span><span class="sxs-lookup"><span data-stu-id="49f2f-158">Deploy Office 365 client apps</span></span>

<span data-ttu-id="49f2f-159">Se optar por instalar automaticamente aplicações do Office no durante o conjunto de cópias, as aplicações instalará nos dispositivos Windows 10 depois dos utilizadores têm sessão iniciada no Azure AD dos dispositivos do Windows com as respectivas credenciais de trabalho.</span><span class="sxs-lookup"><span data-stu-id="49f2f-159">If you chose to automatically install Office apps in during the set up, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices with their work credentials.</span></span>
<span data-ttu-id="49f2f-160">Para instalar o Office iOS móvel ou dispositivos Android, consulte [Configurar dispositivos móveis para utilizadores empresariais do Microsoft 365](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="49f2f-160">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="49f2f-161">Pode também instalar o Office individualmente.</span><span class="sxs-lookup"><span data-stu-id="49f2f-161">You can also install Office individually.</span></span> <span data-ttu-id="49f2f-162">Consulte a [instalar o Office num PC ou Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) para obter instruções.</span><span class="sxs-lookup"><span data-stu-id="49f2f-162">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) for instructions.</span></span>
