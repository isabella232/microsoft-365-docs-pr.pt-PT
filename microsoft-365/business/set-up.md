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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Saiba como configurar o Microsoft 365 Business.
ms.openlocfilehash: f29dbdb61636fdfe573a1a6920d0aed963b737ad
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/19/2019
ms.locfileid: "38721495"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="a3859-103">Configurar o Microsoft 365 Business no assistente de configuração</span><span class="sxs-lookup"><span data-stu-id="a3859-103">Set up Microsoft 365 Business in the setup wizard</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="a3859-104">Adicione seu domínio, usuários e configure políticas</span><span class="sxs-lookup"><span data-stu-id="a3859-104">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="a3859-105">[![Etiqueta que informa que o centro de administração está a mudar e que pode encontrar mais detalhes em aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="a3859-105">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="a3859-106">Quando você compra o Microsoft 365 Business, você tem a opção de usar um domínio que possui ou comprar um durante a [inscrição.](sign-up.md)</span><span class="sxs-lookup"><span data-stu-id="a3859-106">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="a3859-107">Se você comprou um novo domínio quando se inscreveu, seu domínio está tudo configurado e você pode passar para [adicionar usuários e atribuir licenças.](#add-users-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="a3859-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="a3859-108">Adicione o seu domínio para personalizar a entrada</span><span class="sxs-lookup"><span data-stu-id="a3859-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="a3859-109">Entre no [centro de administração da Microsoft 365](https://admin.microsoft.com) usando suas credenciais de administração global.</span><span class="sxs-lookup"><span data-stu-id="a3859-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="a3859-110">Escolha **Adicionar um domínio** ou adicionar **usuários** para iniciar o assistente.</span><span class="sxs-lookup"><span data-stu-id="a3859-110">Choose **Add a domain** or **Add users** to start the wizard.</span></span>
    > [!IMPORTANT]
    > <span data-ttu-id="a3859-111">Se você comprou um domínio durante a inscrição, você não verá **adicionar um** passo de domínio aqui.</span><span class="sxs-lookup"><span data-stu-id="a3859-111">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="a3859-112">Ir para [adicionar usuários](#add-users-and-assign-licenses) em seu lugar.</span><span class="sxs-lookup"><span data-stu-id="a3859-112">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![Selecione Vá para a configuração.](media/gotosetupinadmincenter.png)
    
3. <span data-ttu-id="a3859-114">No mago, digite o nome de domínio que você deseja usar (como contoso.com).</span><span class="sxs-lookup"><span data-stu-id="a3859-114">In the wizard, enter the domain name you want to use (like contoso.com).</span></span>


    ![Captura de tela do Personalize sua página de login.](media/personalizesignin.png)

    
4. <span data-ttu-id="a3859-116">Siga os passos no mago para [criar registros DeNS em qualquer provedor de hospedagem dns para o Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) que verifica o seu próprio domínio.</span><span class="sxs-lookup"><span data-stu-id="a3859-116">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="a3859-117">Se você conhece o seu anfitrião de domínio, consulte também as instruções específicas do [anfitrião.](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)</span><span class="sxs-lookup"><span data-stu-id="a3859-117">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="a3859-118">Se o seu provedor de hospedagem é GoDaddy ou outro host habilitado com [conectar domínio,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)o processo é fácil e você será automaticamente solicitado a entrar e deixar microsoft autenticar em seu nome.</span><span class="sxs-lookup"><span data-stu-id="a3859-118">If your hosting provider is GoDaddy or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![Na página GoDaddy Confirm Access, selecione Authorize.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="a3859-120">Adicionar utilizadores e atribuir licenças</span><span class="sxs-lookup"><span data-stu-id="a3859-120">Add users and assign licenses</span></span>

<span data-ttu-id="a3859-121">Você pode adicionar usuários no mago, mas você também pode [adicionar usuários mais tarde](add-users-m365b.md) no centro de administração.</span><span class="sxs-lookup"><span data-stu-id="a3859-121">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="a3859-122">Além disso, se você tiver um controlador de domínio local, você pode adicionar usuários ao [Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="a3859-122">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="a3859-123">Adicionar usuários no mago</span><span class="sxs-lookup"><span data-stu-id="a3859-123">Add users in the wizard</span></span>

<span data-ttu-id="a3859-124">Todos os usuários que você adicionar no assistente obter automaticamente atribuído uma licença de negócios Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a3859-124">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![Screenshot da página adicionar novos usuários no mago](media/addnewuserspage.png)

1. <span data-ttu-id="a3859-126">Se sua assinatura Microsoft 365 Business tiver usuários existentes (por exemplo, se você usar o AD Connect do Azure), você receberá uma opção para atribuir licenças a eles agora.</span><span class="sxs-lookup"><span data-stu-id="a3859-126">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="a3859-127">Continue o processo e adicione licenças aos utilizadores.</span><span class="sxs-lookup"><span data-stu-id="a3859-127">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="a3859-128">Depois de adicionar os usuários, você também terá a opção de compartilhar credenciais com os novos usuários que você adicionou.</span><span class="sxs-lookup"><span data-stu-id="a3859-128">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="a3859-129">Pode optar por imprimir, transferir ou enviá-las por e-mail.</span><span class="sxs-lookup"><span data-stu-id="a3859-129">You can choose to print them out, email them, or download them.</span></span>

3. <span data-ttu-id="a3859-130">Nas Equipes de Criação para sua organização, você pode optar por adicionar equipes e adicionar usuários a elas.</span><span class="sxs-lookup"><span data-stu-id="a3859-130">On the Create Teams for your organization, you can choose to add Teams and add users to them.</span></span> <span data-ttu-id="a3859-131">Você também pode fazer isso mais tarde.</span><span class="sxs-lookup"><span data-stu-id="a3859-131">You can also do this later.</span></span> <span data-ttu-id="a3859-132">Para mais informações, veja [criar uma equipe em toda a empresa.](https://support.office.com/article/037bb27a-bcc9-48fe-8d72-44d9482420a3)</span><span class="sxs-lookup"><span data-stu-id="a3859-132">For more information, see [create a company-wide Team](https://support.office.com/article/037bb27a-bcc9-48fe-8d72-44d9482420a3).</span></span>

4. <span data-ttu-id="a3859-133">Ignore a migração de mensagens de e-mail e selecione **Seguinte** na página **Migrar as mensagens de e-mail**.</span><span class="sxs-lookup"><span data-stu-id="a3859-133">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 

    <span data-ttu-id="a3859-134">Se você estiver se movendo de outro provedor de e-mail e quiser copiar seus dados mais tarde, poderá [migrar e-mails e contatos para o Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span><span class="sxs-lookup"><span data-stu-id="a3859-134">If you're moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>


### <a name="connect-your-domain"></a><span data-ttu-id="a3859-135">Ligar o seu domínio</span><span class="sxs-lookup"><span data-stu-id="a3859-135">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="a3859-136">Se você optar por usar o domínio .onmicrosoft ou usar o AD Connect do Azure para configurar usuários, não verá essa etapa.</span><span class="sxs-lookup"><span data-stu-id="a3859-136">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="a3859-137">Para configurar serviços, tem de atualizar alguns registos no seu anfitrião de DNS ou entidade de registo de domínios.</span><span class="sxs-lookup"><span data-stu-id="a3859-137">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="a3859-138">Normalmente, o assistente de configuração deteta a sua entidade de registo e fornece-lhe uma ligação para instruções passo a passo de forma a atualizar os seus registos NS no site da entidade de registo de domínios.</span><span class="sxs-lookup"><span data-stu-id="a3859-138">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="a3859-139">Se isso não o fazer, [alterar nameservers para configurar o Office 365 com qualquer registrador](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2)de domínio .</span><span class="sxs-lookup"><span data-stu-id="a3859-139">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="a3859-140">Se você tiver registros DNS existentes, por exemplo, um site existente, mas seu host DNS está habilitado para [conectar domínio,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)escolha **adicionar registros para mim**.</span><span class="sxs-lookup"><span data-stu-id="a3859-140">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="a3859-141">Na página **de serviços on-line Escolha,** aceite todos os padrões e escolha **em seguida**e escolha **autorizar** na página do seu host DNS.</span><span class="sxs-lookup"><span data-stu-id="a3859-141">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="a3859-142">Se você tiver registros DNS existentes com outros hosts DNS (não habilitados para conexão de domínio), você deseja gerenciar seus próprios registros de DNS para garantir que os serviços existentes permaneçam conectados.</span><span class="sxs-lookup"><span data-stu-id="a3859-142">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="a3859-143">Veja o [básico de domínio](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="a3859-143">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Conecte sua página de domínio com eu gerenciarei meus próprios registros de DNS.](media/connectyourdomainpage.png)

2. <span data-ttu-id="a3859-145">Siga os passos no assistente e e-mail e outros serviços serão configurados para você.</span><span class="sxs-lookup"><span data-stu-id="a3859-145">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-data-and-devices"></a><span data-ttu-id="a3859-146">Proteger dados e dispositivos</span><span class="sxs-lookup"><span data-stu-id="a3859-146">Protect data and devices</span></span> 

<span data-ttu-id="a3859-147">As políticas que você configura no mago são aplicadas automaticamente a um grupo de [segurança](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) chamado *All Users.*</span><span class="sxs-lookup"><span data-stu-id="a3859-147">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="a3859-148">Você também pode criar grupos adicionais para atribuir políticas no centro de administração.</span><span class="sxs-lookup"><span data-stu-id="a3859-148">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="a3859-149">No **Protect your work files em dispositivos móveis,** a opção Protect arquivos de trabalho quando os **dispositivos são perdidos ou roubados** é selecionada por padrão.</span><span class="sxs-lookup"><span data-stu-id="a3859-149">On the **Protect your work files on mobile devices**, the option **Protect work files when devices are lost or stolen** is selected by default.</span></span> <span data-ttu-id="a3859-150">Você tem a opção de ativar **gerenciar como os usuários acessam os arquivos do Office em dispositivos móveis,** e isso é recomendado.</span><span class="sxs-lookup"><span data-stu-id="a3859-150">You have an option to turn on **Manage how users access Office files on mobile devices**, and this is recommended.</span></span>

    ![Captura de tela dos arquivos de trabalho Protect na página de dispositivos móveis.](media/protectworkfilesondevices.png)

     - <span data-ttu-id="a3859-152">Expanda os arquivos de trabalho protect quando os **dispositivos são perdidos ou roubados** para exibir os [valores padrão:](protect-work-files-on-lost-or-stolen-device.md)</span><span class="sxs-lookup"><span data-stu-id="a3859-152">Expand **Protect work files when devices are lost or stolen** to display the [default values](protect-work-files-on-lost-or-stolen-device.md):</span></span>

        ![Captura de tela dos valores padrão para proteger arquivos em dispositivos perdidos.](media/protectworkfilesondevicesdefault.png)

    - <span data-ttu-id="a3859-154">Selecione **Gerenciar como os usuários acessam arquivos do Office em dispositivos móveis** e expandi-los para exibir os [valores padrão](manage-user-access-on-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="a3859-154">Select **Manage how users access Office files on mobile devices** and expand it to display the [default values](manage-user-access-on-mobile-devices.md).</span></span> <span data-ttu-id="a3859-155">Recomendamos que você aceite os valores padrão durante a configuração para criar políticas de aplicativos para Android, iOS e Windows 10 que se aplicam a todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="a3859-155">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="a3859-156">Poderá criar políticas adicionais após a configuração estar concluída.</span><span class="sxs-lookup"><span data-stu-id="a3859-156">You can create more policies after setup completes.</span></span>

        ![Captura de tela das configurações de proteção para arquivos do Office em dispositivos móveis.](media/useraccessonmobile.png)

2. <span data-ttu-id="a3859-158">A última etapa para proteger dados e dispositivos permite configurar políticas para proteger os dispositivos Windows 10.</span><span class="sxs-lookup"><span data-stu-id="a3859-158">The last step on protect data and devices allows you to set up policies to secure Windows 10 devices.</span></span> <span data-ttu-id="a3859-159">Essas configurações são aplicadas automaticamente quando o Windows 10 de um usuário se conecta à sua organização.</span><span class="sxs-lookup"><span data-stu-id="a3859-159">These settings are applied automatically when a user's Windows 10 connects to your organization.</span></span> <span data-ttu-id="a3859-160">Você pode expandir **dispositivos Secure Windows 10** para ver e modificar os [valores padrão.](secure-windows-10-devices.md)</span><span class="sxs-lookup"><span data-stu-id="a3859-160">You can expand **Secure Windows 10 devices** to see and modify the [default values](secure-windows-10-devices.md).</span></span>
3. <span data-ttu-id="a3859-161">Você também pode optar por [instalar automaticamente](install-office-on-windows-10-during-setup.md) o Office em dispositivos Windows 10.</span><span class="sxs-lookup"><span data-stu-id="a3859-161">You can also choose to [automatically install Office](install-office-on-windows-10-during-setup.md) on Windows 10 devices.</span></span>

    ![Captura de tela da página de configuração do dispositivo Conjunto Windows 10.](media/setwin10config.png)


## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="a3859-163">Implantar aplicativos para clientes do Office 365</span><span class="sxs-lookup"><span data-stu-id="a3859-163">Deploy Office 365 client apps</span></span>

<span data-ttu-id="a3859-164">Se você optar por instalar aplicativos do Office automaticamente durante a configuração, os aplicativos serão instalados nos dispositivos Do Windows 10 assim que os usuários entrarem no AD do Azure a partir de seus dispositivos Windows, usando suas credenciais de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a3859-164">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="a3859-165">Para instalar o Office em dispositivos iOS ou Android móveis, [consulte a configuração de dispositivos móveis para usuários do Microsoft 365 Business.](set-up-mobile-devices.md)</span><span class="sxs-lookup"><span data-stu-id="a3859-165">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="a3859-166">Você também pode instalar o Office individualmente.</span><span class="sxs-lookup"><span data-stu-id="a3859-166">You can also install Office individually.</span></span> <span data-ttu-id="a3859-167">Consulte [o Office em um PC ou Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) para obter instruções.</span><span class="sxs-lookup"><span data-stu-id="a3859-167">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>
