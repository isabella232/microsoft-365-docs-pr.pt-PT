---
title: Configurar o Microsoft 365 Business
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
description: Saiba como configurar o Microsoft 365 Business.
ms.openlocfilehash: 1efb7379930f639cf10875cf5aa6731001bb41c8
ms.sourcegitcommit: 2e5ae52bb641ee1f72c077260b5d0f35622935fe
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/17/2019
ms.locfileid: "37005204"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="4b7b9-103">Configurar o Microsoft 365 Business no assistente de configuração</span><span class="sxs-lookup"><span data-stu-id="4b7b9-103">Set up Microsoft 365 Business in the setup wizard</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="4b7b9-104">Adicionar seu domínio, usuários e configurar políticas</span><span class="sxs-lookup"><span data-stu-id="4b7b9-104">Add your domain, users, and set up policies</span></span>

![Banner que apontam para https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

<span data-ttu-id="4b7b9-106">Quando você compra o Microsoft 365 Business, você tem a opção de usar um domínio que você possui ou comprar um durante a [inscrição](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="4b7b9-106">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="4b7b9-107">Se você adquiriu um novo domínio quando se inscreveu, seu domínio está configurado e você pode mover para [Adicionar usuários e atribuir licenças](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="4b7b9-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="4b7b9-108">Adicione seu domínio para personalizar o login</span><span class="sxs-lookup"><span data-stu-id="4b7b9-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="4b7b9-109">Entre no [centro de administração do Microsoft 365](https://admin.microsoft.com) usando suas credenciais de administrador global.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="4b7b9-110">Escolha **Adicionar um domínio** ou **Adicionar usuários** para iniciar o assistente.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-110">Choose **Add a domain** or **Add users** to start the wizard.</span></span>
    > [!IMPORTANT]
    > <span data-ttu-id="4b7b9-111">Se você adquiriu um domínio durante a inscrição, não verá **Adicionar uma etapa de domínio** aqui.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-111">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="4b7b9-112">Vá para [Adicionar usuários](#add-users-and-assign-licenses) em vez disso.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-112">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![Selecione Adicionar um domínio.](media/addadomainadmincenter.png)
    
3. <span data-ttu-id="4b7b9-114">No assistente, digite o nome de domínio que você deseja usar (como contoso.com).</span><span class="sxs-lookup"><span data-stu-id="4b7b9-114">In the wizard, enter the domain name you want to use (like contoso.com).</span></span>


    ![Screenshot do Personalize sua página de login.](media/personalizesignin.png)

    
4. <span data-ttu-id="4b7b9-116">Siga as etapas no Assistente para [criar registros DNS em qualquer provedor de hospedagem DNS para o Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) que verifica se você possui o domínio.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-116">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="4b7b9-117">Se você souber seu host de domínio, consulte também as [instruções específicas do host](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="4b7b9-117">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="4b7b9-118">Se o seu provedor de hospedagem é GoDaddy, ou outro host habilitado com o [domínio de conexão](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), o processo é fácil e você será automaticamente solicitado a entrar e permitir que a Microsoft autenticar em seu nome:</span><span class="sxs-lookup"><span data-stu-id="4b7b9-118">If your hosting provider is GoDaddy, or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect),the process is easy and you will be automatically asked to sign in and let Microsoft authenticate on your behalf:</span></span>

    ![Na página Confirmar acesso da GoDaddy, selecione autorizar.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="4b7b9-120">Adicionar utilizadores e atribuir licenças</span><span class="sxs-lookup"><span data-stu-id="4b7b9-120">Add users and assign licenses</span></span>

<span data-ttu-id="4b7b9-121">Você pode adicionar usuários no assistente, mas você também pode [Adicionar usuários posteriormente](add-users-m365b.md) no centro de administração.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-121">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="4b7b9-122">Além disso, se tiver um controlador de domínio local, pode adicionar utilizadores com o [Azure ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="4b7b9-122">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="4b7b9-123">Adicionar usuários no assistente</span><span class="sxs-lookup"><span data-stu-id="4b7b9-123">Add users in the wizard</span></span>

<span data-ttu-id="4b7b9-124">Todos os usuários que você adicionar no assistente recebem automaticamente uma licença do Microsoft 365 Business atribuída.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-124">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![Screenshot da página Adicionar novos usuários no assistente](media/addnewuserspage.png)

1. <span data-ttu-id="4b7b9-126">Se sua assinatura do Microsoft 365 Business tiver usuários existentes (por exemplo, se você usou o Azure AD Connect), você terá uma opção para atribuir licenças a eles agora.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-126">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you get an option to assign licenses to them now.</span></span> <span data-ttu-id="4b7b9-127">Continue o processo e adicione licenças aos utilizadores.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-127">Go ahead and add licenses to them as well.</span></span>

3. <span data-ttu-id="4b7b9-128">Depois de adicionar os usuários, você também receberá uma opção para compartilhar credenciais com os novos usuários que você adicionou.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-128">After you have added the users, you will also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="4b7b9-129">Pode optar por imprimir, transferir ou enviá-las por e-mail.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-129">You can choose to print them out, email them, or download them.</span></span>

4. <span data-ttu-id="4b7b9-130">Ignore a migração de mensagens de e-mail e selecione **Seguinte** na página **Migrar as mensagens de e-mail**.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-130">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 

    <span data-ttu-id="4b7b9-131">Se você estiver movendo de outro provedor de email e quiser copiar seus dados mais tarde, você pode [migrar emails e contatos para o Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span><span class="sxs-lookup"><span data-stu-id="4b7b9-131">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>


### <a name="connect-your-domain"></a><span data-ttu-id="4b7b9-132">Ligar o seu domínio</span><span class="sxs-lookup"><span data-stu-id="4b7b9-132">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="4b7b9-133">Se você optou por usar o domínio. onmicrosoft ou usou o Azure AD Connect para configurar usuários, você não verá esta etapa.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-133">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="4b7b9-134">Para configurar serviços, tem de atualizar alguns registos no seu anfitrião de DNS ou entidade de registo de domínios.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-134">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="4b7b9-135">Normalmente, o assistente de configuração deteta a sua entidade de registo e fornece-lhe uma ligação para instruções passo a passo de forma a atualizar os seus registos NS no site da entidade de registo de domínios.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-135">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="4b7b9-136">Se isso não for possível, altere os servidores [de nomes para configurar o Office 365 com qualquer registrador de domínio](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="4b7b9-136">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="4b7b9-137">Se você tiver registros DNS existentes, por exemplo, um site da Web existente, mas o host DNS estiver habilitado para [conexão de domínio](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), escolha **adicionar registros para mim**.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-137">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> 
    - <span data-ttu-id="4b7b9-138">Se você tiver registros DNS existentes com outros hosts DNS (não habilitados para conexão de domínio), você desejará gerenciar seus próprios registros DNS para garantir que os serviços existentes fiquem conectados.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-138">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you will want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="4b7b9-139">Consulte [noções básicas do domínio](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-139">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Conecte sua página de domínio com eu gerencio meus próprios registros DNS.](media/connectyourdomainpage.png)

2. <span data-ttu-id="4b7b9-141">Siga as etapas no assistente e e-mail e outros serviços serão configurados para você.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-141">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="set-up-security-policies-and-device-configurations"></a><span data-ttu-id="4b7b9-142">Configurar políticas de segurança e configurações de dispositivo</span><span class="sxs-lookup"><span data-stu-id="4b7b9-142">Set up security policies and device configurations</span></span> 

<span data-ttu-id="4b7b9-143">As diretivas configuradas no assistente são aplicadas automaticamente a um [grupo de segurança](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) chamado todos os *usuários*.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-143">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="4b7b9-144">Você também pode criar grupos adicionais para atribuir políticas no centro de administração.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-144">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="4b7b9-145">Na **proteger seus arquivos de trabalho em dispositivos móveis** a opção **proteger arquivos de trabalho quando os dispositivos são perdidos ou roubados** é selecionado por padrão.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-145">On the **Protect your work files on mobile devices** the option **Protect work files when devices are lost or stolen** is selected by default.</span></span> <span data-ttu-id="4b7b9-146">Você tem uma opção para ativar **gerenciar como os usuários acessam arquivos do Office em dispositivos móveis**, e isso é recomendado.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-146">You have an option to turn on **Manage how users access Office files on mobile devices**, and this is recommended.</span></span>

    ![Screenshot de proteger arquivos de trabalho na página de dispositivos móveis.](media/protectworkfilesondevices.png)

     - <span data-ttu-id="4b7b9-148">Expanda **proteger arquivos de trabalho quando os dispositivos são perdidos ou roubados** para exibir os [valores padrão](protect-work-files-on-lost-or-stolen-device.md):</span><span class="sxs-lookup"><span data-stu-id="4b7b9-148">Expand **Protect work files when devices are lost or stolen** to display the [default values](protect-work-files-on-lost-or-stolen-device.md):</span></span>

        ![Captura de tela de valores padrão para proteger arquivos em dispositivos perdidos.](media/protectworkfilesondevicesdefault.png)

    - <span data-ttu-id="4b7b9-150">Selecione **gerenciar como os usuários acessam arquivos do Office em dispositivos móveis** e expandi-lo para exibir os [valores padrão](manage-user-access-on-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="4b7b9-150">Select **Manage how users access Office files on mobile devices** and expand it to display the [default values](manage-user-access-on-mobile-devices.md).</span></span> <span data-ttu-id="4b7b9-151">Recomendamos que você aceite os valores padrão durante a instalação para criar diretivas de aplicativo para Android, iOS e Windows 10 que se aplicam a todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-151">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="4b7b9-152">Poderá criar políticas adicionais após a configuração estar concluída.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-152">You can create more policies after setup completes.</span></span>

        ![Screenshot de configurações de proteção para arquivos do Office no celular.](media/useraccessonmobile.png)

2. <span data-ttu-id="4b7b9-154">A última etapa na proteção de dados e dispositivos permite que você configure políticas para proteger dispositivos Windows 10.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-154">The last step on protect data and devices allows you to set up policies to secure Windows 10 devices.</span></span> <span data-ttu-id="4b7b9-155">Essas configurações são aplicadas automaticamente quando o Windows 10 de um usuário se conecta à sua organização.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-155">These settings are applied automatically when a user's Windows 10 connects to your organization.</span></span> <span data-ttu-id="4b7b9-156">Você pode expandir os **dispositivos Windows 10 seguros** para ver e modificar os [valores padrão](secure-windows-10-devices.md).</span><span class="sxs-lookup"><span data-stu-id="4b7b9-156">You can expand **Secure Windows 10 devices** to see and modify the [default values](secure-windows-10-devices.md).</span></span>
3. <span data-ttu-id="4b7b9-157">Você também pode optar por [instalar automaticamente o Office](install-office-on-windows-10-during-setup.md) em dispositivos Windows 10.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-157">You can also choose to [automatically install Office](install-office-on-windows-10-during-setup.md) on Windows 10 devices.</span></span>

    ![Screenshot do conjunto Windows 10 página de configuração do dispositivo.](media/setwin10config.png)



## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="4b7b9-159">Implantar aplicativos cliente do Office 365</span><span class="sxs-lookup"><span data-stu-id="4b7b9-159">Deploy Office 365 client apps</span></span>

<span data-ttu-id="4b7b9-160">Se você optou por instalar automaticamente os aplicativos do Office durante a instalação, os aplicativos serão instalado nos dispositivos Windows 10 depois que os usuários fizerem logon no Azure AD a partir de seus dispositivos Windows com suas credenciais de trabalho.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-160">If you chose to automatically install Office apps in during the set up, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices with their work credentials.</span></span>
<span data-ttu-id="4b7b9-161">Para instalar o Office em dispositivos móveis iOS ou Android, consulte [configurar dispositivos móveis para usuários do Microsoft 365 Business](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="4b7b9-161">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="4b7b9-162">Você também pode instalar o Office individualmente.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-162">You can also install Office individually.</span></span> <span data-ttu-id="4b7b9-163">Consulte [instalar o Office em um PC ou Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) para obter instruções.</span><span class="sxs-lookup"><span data-stu-id="4b7b9-163">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>
