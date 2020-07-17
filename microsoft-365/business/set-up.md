---
title: Configurar o Microsoft 365 Business Premium
f1.keywords:
- NOCSH
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Descubra os passos de configuração do Microsoft 365 Business Premium, incluindo a adição de um domínio e utilizadores, configurando políticas de segurança, e muito mais.
ms.openlocfilehash: efa7934ece0dfeac3c4b20daa37da6f1160901e7
ms.sourcegitcommit: 5b769f74bcc76ac8d38aad815d1728824783cd9f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081901"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a><span data-ttu-id="0ac51-103">Configurar o Microsoft 365 Business Premium no assistente de configuração</span><span class="sxs-lookup"><span data-stu-id="0ac51-103">Set up Microsoft 365 Business Premium in the setup wizard</span></span>

<span data-ttu-id="0ac51-104">Veja este vídeo para uma visão geral da configuração do Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="0ac51-104">Watch this video for an overview of Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

<span data-ttu-id="0ac51-105">Caso tenha considerado este vídeo útil, veja a [série de formação completa para pequenas empresas e as novidades do Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="0ac51-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="0ac51-106">Adicione o seu domínio, utilizadores e configurar políticas</span><span class="sxs-lookup"><span data-stu-id="0ac51-106">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="0ac51-107">Ao comprar o Microsoft 365 Business Premium, tem a opção de utilizar um domínio que possui ou de comprar um durante a [inscrição](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="0ac51-107">When you purchase Microsoft 365 Business Premium, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="0ac51-108">Se adquiriu um novo domínio quando se inscreveu, o seu domínio está todo configurado e pode mudar-se para [Adicionar utilizadores e atribuir licenças](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="0ac51-108">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="0ac51-109">Adicione o seu domínio para personalizar o s-in</span><span class="sxs-lookup"><span data-stu-id="0ac51-109">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="0ac51-110">Inscreva-se no [Microsoft 365 admin center](https://admin.microsoft.com) usando as suas credenciais de administração global.</span><span class="sxs-lookup"><span data-stu-id="0ac51-110">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="0ac51-111">Escolha **Ir para a configuração** para iniciar o assistente.</span><span class="sxs-lookup"><span data-stu-id="0ac51-111">Choose **Go to setup** to start the wizard.</span></span>

    ![Selecione Ir para a configuração.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="0ac51-113">Na página **de aplicações do Office,** pode instalar opcionalmente as aplicações no seu próprio computador.</span><span class="sxs-lookup"><span data-stu-id="0ac51-113">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="0ac51-114">No passo de **domínio Adicionar,** insira o nome de domínio que pretende utilizar (como contoso.com).</span><span class="sxs-lookup"><span data-stu-id="0ac51-114">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="0ac51-115">Se adquiriu um domínio durante a inscrição, não verá **Adicionar um** passo de domínio aqui.</span><span class="sxs-lookup"><span data-stu-id="0ac51-115">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="0ac51-116">Vá a [Adicionar os utilizadores](#add-users-and-assign-licenses) em vez disso.</span><span class="sxs-lookup"><span data-stu-id="0ac51-116">Go to [Add users](#add-users-and-assign-licenses) instead.</span></span>

    ![Screenshot da página De Personalizar o seu sign-in.](../media/adddomain.png)

    
4. <span data-ttu-id="0ac51-118">Siga os passos no assistente para [criar registos DNS em qualquer fornecedor de hospedagem DNS para o Microsoft 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) que verifique que é dono do domínio.</span><span class="sxs-lookup"><span data-stu-id="0ac51-118">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Microsoft 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="0ac51-119">Se conhecer o seu anfitrião de domínio, consulte também as [instruções específicas](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)do anfitrião .</span><span class="sxs-lookup"><span data-stu-id="0ac51-119">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="0ac51-120">Se o seu fornecedor de hospedagem for o GoDaddy ou outro anfitrião ativado com [ligação de domínio,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)o processo é fácil e será automaticamente solicitado que faça sessão e deixe a Microsoft autenticar em seu nome.</span><span class="sxs-lookup"><span data-stu-id="0ac51-120">If your hosting provider is GoDaddy or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![Na página GoDaddy Confirm Access, selecione Authorize.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="0ac51-122">Adicionar utilizadores e atribuir licenças</span><span class="sxs-lookup"><span data-stu-id="0ac51-122">Add users and assign licenses</span></span>

<span data-ttu-id="0ac51-123">Pode adicionar utilizadores no assistente, mas também pode [adicionar utilizadores mais tarde](add-users-m365b.md) no centro de administração.</span><span class="sxs-lookup"><span data-stu-id="0ac51-123">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="0ac51-124">Além disso, se tiver um controlador de domínio local, pode adicionar utilizadores ao [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="0ac51-124">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="0ac51-125">Adicionar utilizadores no assistente</span><span class="sxs-lookup"><span data-stu-id="0ac51-125">Add users in the wizard</span></span>

<span data-ttu-id="0ac51-126">Qualquer utilizadores que adicione no assistente recebem automaticamente uma licença Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="0ac51-126">Any users you add in the wizard get automatically assigned a Microsoft 365 Business Premium license.</span></span>

![Screenshot da página de novos utilizadores adicionar no assistente](../media/addnewuserspage.png)

1. <span data-ttu-id="0ac51-128">Se a sua subscrição Microsoft 365 Business Premium tiver utilizadores existentes (por exemplo, se usou o Azure AD Connect), terá agora a opção de lhes atribuir licenças.</span><span class="sxs-lookup"><span data-stu-id="0ac51-128">If your Microsoft 365 Business Premium subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="0ac51-129">Continue o processo e adicione licenças aos utilizadores.</span><span class="sxs-lookup"><span data-stu-id="0ac51-129">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="0ac51-130">Depois de adicionar os utilizadores, também terá a opção de partilhar credenciais com os novos utilizadores que adicionou.</span><span class="sxs-lookup"><span data-stu-id="0ac51-130">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="0ac51-131">Pode optar por imprimir, transferir ou enviá-las por e-mail.</span><span class="sxs-lookup"><span data-stu-id="0ac51-131">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="0ac51-132">Ligar o seu domínio</span><span class="sxs-lookup"><span data-stu-id="0ac51-132">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="0ac51-133">Se optar por utilizar o domínio .onmicrosoft ou utilizar o Azure AD Connect para configurar os utilizadores, não verá este passo.</span><span class="sxs-lookup"><span data-stu-id="0ac51-133">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="0ac51-134">Para configurar serviços, tem de atualizar alguns registos no seu anfitrião de DNS ou entidade de registo de domínios.</span><span class="sxs-lookup"><span data-stu-id="0ac51-134">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="0ac51-135">Normalmente, o assistente de configuração deteta a sua entidade de registo e fornece-lhe uma ligação para instruções passo a passo de forma a atualizar os seus registos NS no site da entidade de registo de domínios.</span><span class="sxs-lookup"><span data-stu-id="0ac51-135">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="0ac51-136">Caso não o faça, [altere os serviçais para configurar o Microsoft 365 com qualquer registo de domínio](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar).</span><span class="sxs-lookup"><span data-stu-id="0ac51-136">If it doesn't, [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar).</span></span> 

    - <span data-ttu-id="0ac51-137">Se tiver registos DNS existentes, por exemplo, um web site existente, mas o seu anfitrião DNS está ativado para [a ligação de domínios](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), escolha **adicionar registos para mim**.</span><span class="sxs-lookup"><span data-stu-id="0ac51-137">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="0ac51-138">Na página **de serviços online,** aceite todas as predefinições e escolha **Seguinte**, e escolha **'Autorizo'** na página do seu anfitrião DNS.</span><span class="sxs-lookup"><span data-stu-id="0ac51-138">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="0ac51-139">Se tiver registos DNS existentes com outros anfitriões DNS (não habilitados para a ligação de domínios), irá querer gerir os seus próprios registos DNS para garantir que os serviços existentes se mantenham ligados.</span><span class="sxs-lookup"><span data-stu-id="0ac51-139">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="0ac51-140">Consulte [o básico do domínio](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="0ac51-140">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Ativar a página de registos.](../media/activaterecords.png)

2. <span data-ttu-id="0ac51-142">Siga os passos no assistente e o e-mail e outros serviços serão configurado para si.</span><span class="sxs-lookup"><span data-stu-id="0ac51-142">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="0ac51-143">Proteja a sua organização</span><span class="sxs-lookup"><span data-stu-id="0ac51-143">Protect your organization</span></span> 

<span data-ttu-id="0ac51-144">As políticas configuradas no assistente são aplicadas automaticamente a um [grupo de Segurança](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) chamado Todos os *Utilizadores*.</span><span class="sxs-lookup"><span data-stu-id="0ac51-144">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="0ac51-145">Também pode criar grupos adicionais para atribuir políticas no centro de administração.</span><span class="sxs-lookup"><span data-stu-id="0ac51-145">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="0ac51-146">Sobre a **proteção do Aumento contra ameaças cibernéticas avançadas,** recomenda-se que aceite os padrãos para permitir que os ficheiros e links [de proteção de ameaças avançadas do Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) e links nas aplicações do Office.</span><span class="sxs-lookup"><span data-stu-id="0ac51-146">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) scan files and links in Office apps.</span></span>

    ![Screenshot da página de proteção Aumentar.](../media/increasetreatprotection.png)


2. <span data-ttu-id="0ac51-148">Na página **Prevent leaks of sensitive data** page, aceite os predefinidos para ligar o Office 365 Data Loss Prevention (DLP) para rastrear dados sensíveis em aplicações do Office e impedir a partilha acidental destes fora da sua organização.</span><span class="sxs-lookup"><span data-stu-id="0ac51-148">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="0ac51-149">Nos **dados** protect in Office para página móvel, deixe a gestão de aplicações móveis, expanda as definições e reveja-as e, em seguida, **selecione Create mobile app management policy**.</span><span class="sxs-lookup"><span data-stu-id="0ac51-149">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Screenshot de Protect datas no Office para página móvel.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="0ac51-151">Secure Windows 10 PCs</span><span class="sxs-lookup"><span data-stu-id="0ac51-151">Secure Windows 10 PCs</span></span>

<span data-ttu-id="0ac51-152">No navegador esquerdo, selecione **Configuração** e, em seguida, **em 'Iniciar s-in e segurança',** escolha **Fixe os computadores Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="0ac51-152">On the left nav, select **Setup** and then, under **Sign-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="0ac51-153">Escolha **a Vista** para começar.</span><span class="sxs-lookup"><span data-stu-id="0ac51-153">Choose **View** to get started.</span></span> <span data-ttu-id="0ac51-154">Consulte [os computadores Windows 10 para](secure-win-10-pcs.md) obter instruções completas.</span><span class="sxs-lookup"><span data-stu-id="0ac51-154">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="0ac51-155">Implementar aplicações de clientes 365</span><span class="sxs-lookup"><span data-stu-id="0ac51-155">Deploy Office 365 client apps</span></span>

<span data-ttu-id="0ac51-156">Se optar por instalar automaticamente aplicações do Office durante a configuração, as aplicações serão instaladas nos dispositivos Windows 10 assim que os utilizadores tiverem assinado no Azure AD a partir dos seus dispositivos Windows, utilizando as suas credenciais de trabalho.</span><span class="sxs-lookup"><span data-stu-id="0ac51-156">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="0ac51-157">Para instalar o Office em dispositivos móveis iOS ou Android, consulte [Configurar dispositivos móveis para utilizadores Do Microsoft 365 Business Premium](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="0ac51-157">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="0ac51-158">Também pode instalar o Office individualmente.</span><span class="sxs-lookup"><span data-stu-id="0ac51-158">You can also install Office individually.</span></span> <span data-ttu-id="0ac51-159">Consulte [o Escritório de Instalação num PC ou Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) para obter instruções.</span><span class="sxs-lookup"><span data-stu-id="0ac51-159">See [install Office on a PC or Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="0ac51-160">Consulte também</span><span class="sxs-lookup"><span data-stu-id="0ac51-160">See also</span></span>

[<span data-ttu-id="0ac51-161">Microsoft 365 para vídeos de formação de negócios</span><span class="sxs-lookup"><span data-stu-id="0ac51-161">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
