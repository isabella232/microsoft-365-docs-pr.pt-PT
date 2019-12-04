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
- TRN_SMB
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Saiba como configurar o Microsoft 365 Business.
ms.openlocfilehash: 0001c2b9962f6cce0be1f77cbf427c68f9ee3249
ms.sourcegitcommit: c5ca71d6feb0f033b50ccd4de816fd59b0925007
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/04/2019
ms.locfileid: "39831309"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="96020-103">Configurar o Microsoft 365 Business no assistente de configuração</span><span class="sxs-lookup"><span data-stu-id="96020-103">Set up Microsoft 365 Business in the setup wizard</span></span>

<span data-ttu-id="96020-104">Assista a este vídeo para uma visão geral da configuração do Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="96020-104">Watch this video for an overview of Microsoft 365 Business setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

<span data-ttu-id="96020-105">Se você achou este vídeo útil, confira a série de [treinamento completo para pequenas empresas e as novas para a Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="96020-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="96020-106">Adicione seu domínio, usuários e configure políticas</span><span class="sxs-lookup"><span data-stu-id="96020-106">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="96020-107">[![Etiqueta que informa que o centro de administração está a mudar e que pode encontrar mais detalhes em aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="96020-107">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="96020-108">Quando você compra o Microsoft 365 Business, você tem a opção de usar um domínio que possui ou comprar um durante a [inscrição.](sign-up.md)</span><span class="sxs-lookup"><span data-stu-id="96020-108">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="96020-109">Se você comprou um novo domínio quando se inscreveu, seu domínio está tudo configurado e você pode passar para [adicionar usuários e atribuir licenças.](#add-users-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="96020-109">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="96020-110">Adicione o seu domínio para personalizar a entrada</span><span class="sxs-lookup"><span data-stu-id="96020-110">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="96020-111">Entre no [centro de administração da Microsoft 365](https://admin.microsoft.com) usando suas credenciais de administração global.</span><span class="sxs-lookup"><span data-stu-id="96020-111">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="96020-112">Escolha **Vá para a configuração** para iniciar o mago.</span><span class="sxs-lookup"><span data-stu-id="96020-112">Choose **Go to setup** to start the wizard.</span></span>

    ![Selecione Vá para a configuração.](media/gotosetupinadmincenter.png)

3. <span data-ttu-id="96020-114">Na página **de aplicativos install your office,** você pode instalar opcionalmente os aplicativos em seu próprio computador.</span><span class="sxs-lookup"><span data-stu-id="96020-114">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="96020-115">Na etapa de **domínio Adicionar,** digite o nome de domínio que deseja usar (como contoso.com).</span><span class="sxs-lookup"><span data-stu-id="96020-115">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="96020-116">Se você comprou um domínio durante a inscrição, você não verá **adicionar um** passo de domínio aqui.</span><span class="sxs-lookup"><span data-stu-id="96020-116">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="96020-117">Ir para [adicionar usuários](#add-users-and-assign-licenses) em seu lugar.</span><span class="sxs-lookup"><span data-stu-id="96020-117">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![Captura de tela do Personalize sua página de login.](media/adddomain.png)

    
4. <span data-ttu-id="96020-119">Siga os passos no mago para [criar registros DeNS em qualquer provedor de hospedagem dns para o Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) que verifica o seu próprio domínio.</span><span class="sxs-lookup"><span data-stu-id="96020-119">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="96020-120">Se você conhece o seu anfitrião de domínio, consulte também as instruções específicas do [anfitrião.](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)</span><span class="sxs-lookup"><span data-stu-id="96020-120">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="96020-121">Se o seu provedor de hospedagem é GoDaddy ou outro host habilitado com [conectar domínio,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)o processo é fácil e você será automaticamente solicitado a entrar e deixar microsoft autenticar em seu nome.</span><span class="sxs-lookup"><span data-stu-id="96020-121">If your hosting provider is GoDaddy or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![Na página GoDaddy Confirm Access, selecione Authorize.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="96020-123">Adicionar utilizadores e atribuir licenças</span><span class="sxs-lookup"><span data-stu-id="96020-123">Add users and assign licenses</span></span>

<span data-ttu-id="96020-124">Você pode adicionar usuários no mago, mas você também pode [adicionar usuários mais tarde](add-users-m365b.md) no centro de administração.</span><span class="sxs-lookup"><span data-stu-id="96020-124">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="96020-125">Além disso, se você tiver um controlador de domínio local, você pode adicionar usuários ao [Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="96020-125">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="96020-126">Adicionar usuários no mago</span><span class="sxs-lookup"><span data-stu-id="96020-126">Add users in the wizard</span></span>

<span data-ttu-id="96020-127">Todos os usuários que você adicionar no assistente obter automaticamente atribuído uma licença de negócios Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="96020-127">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![Screenshot da página adicionar novos usuários no mago](media/addnewuserspage.png)

1. <span data-ttu-id="96020-129">Se sua assinatura Microsoft 365 Business tiver usuários existentes (por exemplo, se você usar o AD Connect do Azure), você receberá uma opção para atribuir licenças a eles agora.</span><span class="sxs-lookup"><span data-stu-id="96020-129">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="96020-130">Continue o processo e adicione licenças aos utilizadores.</span><span class="sxs-lookup"><span data-stu-id="96020-130">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="96020-131">Depois de adicionar os usuários, você também terá a opção de compartilhar credenciais com os novos usuários que você adicionou.</span><span class="sxs-lookup"><span data-stu-id="96020-131">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="96020-132">Pode optar por imprimir, transferir ou enviá-las por e-mail.</span><span class="sxs-lookup"><span data-stu-id="96020-132">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="96020-133">Ligar o seu domínio</span><span class="sxs-lookup"><span data-stu-id="96020-133">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="96020-134">Se você optar por usar o domínio .onmicrosoft ou usar o AD Connect do Azure para configurar usuários, não verá essa etapa.</span><span class="sxs-lookup"><span data-stu-id="96020-134">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="96020-135">Para configurar serviços, tem de atualizar alguns registos no seu anfitrião de DNS ou entidade de registo de domínios.</span><span class="sxs-lookup"><span data-stu-id="96020-135">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="96020-136">Normalmente, o assistente de configuração deteta a sua entidade de registo e fornece-lhe uma ligação para instruções passo a passo de forma a atualizar os seus registos NS no site da entidade de registo de domínios.</span><span class="sxs-lookup"><span data-stu-id="96020-136">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="96020-137">Se isso não o fazer, [alterar nameservers para configurar o Office 365 com qualquer registrador](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2)de domínio .</span><span class="sxs-lookup"><span data-stu-id="96020-137">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="96020-138">Se você tiver registros DNS existentes, por exemplo, um site existente, mas seu host DNS está habilitado para [conectar domínio,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)escolha **adicionar registros para mim**.</span><span class="sxs-lookup"><span data-stu-id="96020-138">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="96020-139">Na página **de serviços on-line Escolha,** aceite todos os padrões e escolha **em seguida**e escolha **autorizar** na página do seu host DNS.</span><span class="sxs-lookup"><span data-stu-id="96020-139">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="96020-140">Se você tiver registros DNS existentes com outros hosts DNS (não habilitados para conexão de domínio), você deseja gerenciar seus próprios registros de DNS para garantir que os serviços existentes permaneçam conectados.</span><span class="sxs-lookup"><span data-stu-id="96020-140">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="96020-141">Veja o [básico de domínio](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="96020-141">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Ativar a página de registros.](media/activaterecords.png)

2. <span data-ttu-id="96020-143">Siga os passos no assistente e e-mail e outros serviços serão configurados para você.</span><span class="sxs-lookup"><span data-stu-id="96020-143">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="96020-144">Proteger sua organização</span><span class="sxs-lookup"><span data-stu-id="96020-144">Protect your organization</span></span> 

<span data-ttu-id="96020-145">As políticas que você configura no mago são aplicadas automaticamente a um grupo de [segurança](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) chamado *All Users.*</span><span class="sxs-lookup"><span data-stu-id="96020-145">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="96020-146">Você também pode criar grupos adicionais para atribuir políticas no centro de administração.</span><span class="sxs-lookup"><span data-stu-id="96020-146">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="96020-147">Sobre a **proteção de aumento contra ameaças cibernéticas avançadas,** recomenda-se que você aceite os padrões para permitir que o Office [365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) escaneie arquivos e links em aplicativos do Office.</span><span class="sxs-lookup"><span data-stu-id="96020-147">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) scan files and links in Office apps.</span></span>

    ![Página de proteção de captura de tela do aumento.](media/increasetreatprotection.png)


2. <span data-ttu-id="96020-149">No **Prevent vazamentos de página de dados confidenciais,** aceite os padrões para ativar a Prevenção de Perdas de Dados (DLP) do Office 365 para rastrear dados confidenciais em aplicativos do Office e evitar o compartilhamento acidental desses fora de sua organização.</span><span class="sxs-lookup"><span data-stu-id="96020-149">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="96020-150">Nos **dados protect in Office para** página móvel, deixe o gerenciamento de aplicativos móveis, expanda as configurações e os revise e selecione a política de gerenciamento de **aplicativos móveis**do Create.</span><span class="sxs-lookup"><span data-stu-id="96020-150">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Captura de tela dos dados de Proteger no Office para página móvel.](media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="96020-152">PCs seguros do Windows 10</span><span class="sxs-lookup"><span data-stu-id="96020-152">Secure Windows 10 PCs</span></span>

<span data-ttu-id="96020-153">No nav esquerdo, selecione **a configuração** e, em seguida, **sing-in e segurança,** escolha **proteger seus computadores do Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="96020-153">On the left nav, select **Setup** and then, under **Sing-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="96020-154">Escolha **o View** para começar.</span><span class="sxs-lookup"><span data-stu-id="96020-154">Choose **View** to get started.</span></span> <span data-ttu-id="96020-155">Veja [proteger seus computadores do Windows 10](secure-win-10-pcs.md) para instruções completas.</span><span class="sxs-lookup"><span data-stu-id="96020-155">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="96020-156">Implantar aplicativos para clientes do Office 365</span><span class="sxs-lookup"><span data-stu-id="96020-156">Deploy Office 365 client apps</span></span>

<span data-ttu-id="96020-157">Se você optar por instalar aplicativos do Office automaticamente durante a configuração, os aplicativos serão instalados nos dispositivos Do Windows 10 assim que os usuários entrarem no AD do Azure a partir de seus dispositivos Windows, usando suas credenciais de trabalho.</span><span class="sxs-lookup"><span data-stu-id="96020-157">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="96020-158">Para instalar o Office em dispositivos iOS ou Android móveis, [consulte a configuração de dispositivos móveis para usuários do Microsoft 365 Business.](set-up-mobile-devices.md)</span><span class="sxs-lookup"><span data-stu-id="96020-158">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="96020-159">Você também pode instalar o Office individualmente.</span><span class="sxs-lookup"><span data-stu-id="96020-159">You can also install Office individually.</span></span> <span data-ttu-id="96020-160">Consulte [o Office em um PC ou Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) para obter instruções.</span><span class="sxs-lookup"><span data-stu-id="96020-160">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="96020-161">See also</span><span class="sxs-lookup"><span data-stu-id="96020-161">See also</span></span>

[<span data-ttu-id="96020-162">Microsoft 365 Vídeos de treinamento de negócios</span><span class="sxs-lookup"><span data-stu-id="96020-162">Microsoft 365 Business training videos</span></span>](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
