---
title: Configurar o Microsoft 365 Empresas Premium
f1.keywords:
- NOCSH
ms.author: kwekua
author: kwekua
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
description: Descubra os passos de configuração para o Microsoft 365 Empresas Premium, incluindo adicionar um domínio e utilizadores, configurar políticas de segurança e muito mais.
ms.openlocfilehash: 37607b483686fc12ac6253ae9f693ec86c073c4e
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/06/2021
ms.locfileid: "52245050"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a><span data-ttu-id="c4682-103">Configurar Microsoft 365 Empresas Premium no assistente de configuração</span><span class="sxs-lookup"><span data-stu-id="c4682-103">Set up Microsoft 365 Business Premium in the setup wizard</span></span>

<span data-ttu-id="c4682-104">Veja este vídeo para ver uma visão geral Microsoft 365 Empresas Premium configuração.</span><span class="sxs-lookup"><span data-stu-id="c4682-104">Watch this video for an overview of Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="c4682-105">Adicionar o seu domínio, utilizadores e configurar políticas</span><span class="sxs-lookup"><span data-stu-id="c4682-105">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="c4682-106">Quando compra um Microsoft 365 Empresas Premium, tem a opção de utilizar um domínio que possui ou de comprar um durante a [registo](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="c4682-106">When you purchase Microsoft 365 Business Premium, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="c4682-107">Se comprou um novo domínio quando se inscreveu, o seu domínio está configurado e pode aceder a Adicionar utilizadores e atribuir [licenças.](#add-users-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="c4682-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="c4682-108">Adicionar o seu domínio para personalizar o seu registo</span><span class="sxs-lookup"><span data-stu-id="c4682-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="c4682-109">Inscreva-se [no Microsoft 365 de administração](https://admin.microsoft.com) com as suas credenciais de administrador global.</span><span class="sxs-lookup"><span data-stu-id="c4682-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="c4682-110">**Selecionar Ir para a configuração** para iniciar o assistente.</span><span class="sxs-lookup"><span data-stu-id="c4682-110">Choose **Go to setup** to start the wizard.</span></span>

    ![Selecione Ir para a configuração.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="c4682-112">Na página **Instalar as Office aplicações,** pode instalar opcionalmente as aplicações no seu computador.</span><span class="sxs-lookup"><span data-stu-id="c4682-112">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="c4682-113">No passo **Adicionar domínio,** introduza o nome de domínio que pretende utilizar (como contoso.com).</span><span class="sxs-lookup"><span data-stu-id="c4682-113">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="c4682-114">Se comprou um domínio durante a inscrever-se, não verá **Adicionar um passo de** domínio aqui.</span><span class="sxs-lookup"><span data-stu-id="c4682-114">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="c4682-115">Em alternativa, [vá para Adicionar](#add-users-and-assign-licenses) utilizadores.</span><span class="sxs-lookup"><span data-stu-id="c4682-115">Go to [Add users](#add-users-and-assign-licenses) instead.</span></span>

    ![Captura de ecrã a mostra a página Personalizar o seu dia atual.](../media/adddomain.png)

    
4. <span data-ttu-id="c4682-117">Siga os passos no assistente para Criar registos DNS em qualquer fornecedor de anfitriões [DNS Microsoft 365](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) que verifique que é o propriedade do domínio.</span><span class="sxs-lookup"><span data-stu-id="c4682-117">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Microsoft 365](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="c4682-118">Se conhecer o seu anfitrião de domínio, consulte também as instruções [específicas do anfitrião.](/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)</span><span class="sxs-lookup"><span data-stu-id="c4682-118">If you know your domain host, see also the [host specific instructions](/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="c4682-119">Se o seu fornecedor de domínios for a GoDaddy ou outro anfitrião ativado com ligação de [domínio,](/office365/admin/get-help-with-domains/domain-connect)o processo é fácil e ser-lhe-á automaticamente pedido para o fazer e permitir que a Microsoft se autentique em seu nome.</span><span class="sxs-lookup"><span data-stu-id="c4682-119">If your hosting provider is GoDaddy or another host enabled with [domain connect](/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![Na página Confirmar Acesso da GoDaddy, selecione Autorizar.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="c4682-121">Adicionar utilizadores e atribuir licenças</span><span class="sxs-lookup"><span data-stu-id="c4682-121">Add users and assign licenses</span></span>

<span data-ttu-id="c4682-122">Pode adicionar utilizadores no assistente, mas também pode adicionar [utilizadores mais tarde](../admin/add-users/add-users.md) no centro de administração.</span><span class="sxs-lookup"><span data-stu-id="c4682-122">You can add users in the wizard, but you can also [add users later](../admin/add-users/add-users.md) in the admin center.</span></span> <span data-ttu-id="c4682-123">Além disso, se tiver um controlador de domínio local, pode adicionar utilizadores com o [Azure AD Ligação](/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="c4682-123">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="c4682-124">Adicionar utilizadores no assistente</span><span class="sxs-lookup"><span data-stu-id="c4682-124">Add users in the wizard</span></span>

<span data-ttu-id="c4682-125">Todos os utilizadores que adicionar no assistente receberão automaticamente uma Microsoft 365 Empresas Premium de licenciamento.</span><span class="sxs-lookup"><span data-stu-id="c4682-125">Any users you add in the wizard get automatically assigned a Microsoft 365 Business Premium license.</span></span>

![Captura de ecrã da página Adicionar novos utilizadores no assistente](../media/addnewuserspage.png)

1. <span data-ttu-id="c4682-127">Se a sua subscrição do Microsoft 365 Empresas Premium tiver utilizadores existentes (por exemplo, se tiver utilizado o Azure AD Ligação), terá uma opção para atribuir licenças aos utilizadores agora.</span><span class="sxs-lookup"><span data-stu-id="c4682-127">If your Microsoft 365 Business Premium subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="c4682-128">Continue o processo e adicione licenças aos utilizadores.</span><span class="sxs-lookup"><span data-stu-id="c4682-128">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="c4682-129">Depois de adicionar os utilizadores, também receberá uma opção para partilhar as credenciais com os novos utilizadores que adicionou.</span><span class="sxs-lookup"><span data-stu-id="c4682-129">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="c4682-130">Pode optar por imprimir, transferir ou enviá-las por e-mail.</span><span class="sxs-lookup"><span data-stu-id="c4682-130">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="c4682-131">Ligar o seu domínio</span><span class="sxs-lookup"><span data-stu-id="c4682-131">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="c4682-132">Se optou por utilizar o domínio .onmicrosoft ou tiver utilizado o Azure AD Ligação para configurar utilizadores, não verá este passo.</span><span class="sxs-lookup"><span data-stu-id="c4682-132">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="c4682-133">Para configurar serviços, tem de atualizar alguns registos no seu anfitrião de DNS ou entidade de registo de domínios.</span><span class="sxs-lookup"><span data-stu-id="c4682-133">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="c4682-134">Normalmente, o assistente de configuração deteta a sua entidade de registo e fornece-lhe uma ligação para instruções passo a passo de forma a atualizar os seus registos NS no site da entidade de registo de domínios.</span><span class="sxs-lookup"><span data-stu-id="c4682-134">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="c4682-135">Se isto não acontecer, altere os servidores de nomes para [configurar o Microsoft 365 de domínios.](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md)</span><span class="sxs-lookup"><span data-stu-id="c4682-135">If it doesn't, [Change nameservers to set up Microsoft 365 with any domain registrar](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md).</span></span> 

    - <span data-ttu-id="c4682-136">Se tiver registos DNS existentes, por exemplo um site existente, mas o seu anfitrião DNS estiver ativado para ligar o [domínio,](/office365/admin/get-help-with-domains/domain-connect)selecionar Adicionar **registos por mim.**</span><span class="sxs-lookup"><span data-stu-id="c4682-136">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="c4682-137">Na página **Escolher os seus serviços online,** aceite todas as  predefinições e selecionar Seguinte e selecionar Autorizar na página do seu anfitrião de DNS.</span><span class="sxs-lookup"><span data-stu-id="c4682-137">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="c4682-138">Se tiver registos DNS existentes com outros anfitriões de DNS (não ativado para ligação de domínio), é reflegado para gerir os seus próprios registos DNS para se certificar de que os serviços existentes permanecem ligados.</span><span class="sxs-lookup"><span data-stu-id="c4682-138">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="c4682-139">Consulte [as noções básicas de](/office365/admin/get-help-with-domains/dns-basics) domínios para mais informações.</span><span class="sxs-lookup"><span data-stu-id="c4682-139">See [domain basics](/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Página Ativar registos.](../media/activaterecords.png)

2. <span data-ttu-id="c4682-141">Siga os passos no assistente e o e-mail e outros serviços serão configurados para si.</span><span class="sxs-lookup"><span data-stu-id="c4682-141">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="c4682-142">Proteger a sua organização</span><span class="sxs-lookup"><span data-stu-id="c4682-142">Protect your organization</span></span> 

<span data-ttu-id="c4682-143">As políticas que configurar no assistente são aplicadas automaticamente a um Grupo [de segurança denominado](/office365/admin/create-groups/compare-groups#security-groups) *Todos os Utilizadores.*</span><span class="sxs-lookup"><span data-stu-id="c4682-143">The policies you set up in the wizard are applied automatically to a [Security group](/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="c4682-144">Também pode criar grupos adicionais para atribuir políticas no centro de administração.</span><span class="sxs-lookup"><span data-stu-id="c4682-144">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="c4682-145">Em Aumentar a proteção **contra ciberameaces avançadas**, [](../security/office-365-security/defender-for-office-365.md) recomendamos que aceite as predefinições para permitir que Office 365 a Proteção Avançada contra Ameaças analisa ficheiros e ligações em Office aplicações.</span><span class="sxs-lookup"><span data-stu-id="c4682-145">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](../security/office-365-security/defender-for-office-365.md) scan files and links in Office apps.</span></span>

    ![Captura de ecrã da página Aumentar proteção.](../media/increasetreatprotection.png)


2. <span data-ttu-id="c4682-147">Na página Impedir **fugas** de dados confidenciais, aceite as predefinições para ativo o Office 365 Prevenção de Perda de Dados (DLP) para controlar dados confidenciais em aplicações do Office e impedir a partilha acidental destes dados fora da sua organização.</span><span class="sxs-lookup"><span data-stu-id="c4682-147">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="c4682-148">Na página Proteger dados **no Office** para dispositivos móveis, deixe a gestão de aplicações móveis ativada, expanda as definições e reveja-as e, em seguida, selecione Criar política de gestão de aplicações **móveis**.</span><span class="sxs-lookup"><span data-stu-id="c4682-148">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Captura de ecrã da página Proteger dados no Office para dispositivos móveis.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="c4682-150">Proteger Windows 10 PCs</span><span class="sxs-lookup"><span data-stu-id="c4682-150">Secure Windows 10 PCs</span></span>

<span data-ttu-id="c4682-151">No navegador esquerdo,  selecione Configurar e, em seguida, em **Sign-in and security**, selecione Secure your **Windows 10 .**</span><span class="sxs-lookup"><span data-stu-id="c4682-151">On the left nav, select **Setup** and then, under **Sign-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="c4682-152">**Selecionar** Ver para começar.</span><span class="sxs-lookup"><span data-stu-id="c4682-152">Choose **View** to get started.</span></span> <span data-ttu-id="c4682-153">Consulte [Proteger os seus Windows 10 para obter](secure-win-10-pcs.md) instruções completas.</span><span class="sxs-lookup"><span data-stu-id="c4682-153">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="c4682-154">Implementar aplicações Office 365 cliente</span><span class="sxs-lookup"><span data-stu-id="c4682-154">Deploy Office 365 client apps</span></span>

<span data-ttu-id="c4682-155">Se optou por instalar automaticamente aplicações do Office durante a configuração, as aplicações serão instaladas nos dispositivos Windows 10 assim que os utilizadores tenham feito a loteamento no Azure AD a partir dos respetivos dispositivos Windows, com as respetivos credenciais de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c4682-155">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="c4682-156">Para instalar o Office dispositivos móveis iOS ou Android, consulte Configurar dispositivos [móveis para Microsoft 365 Empresas Premium utilizadores.](set-up-mobile-devices.md)</span><span class="sxs-lookup"><span data-stu-id="c4682-156">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="c4682-157">Também pode instalar o Office individualmente.</span><span class="sxs-lookup"><span data-stu-id="c4682-157">You can also install Office individually.</span></span> <span data-ttu-id="c4682-158">Consulte [Instalar Office num PC ou Mac para](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) obter instruções.</span><span class="sxs-lookup"><span data-stu-id="c4682-158">See [install Office on a PC or Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="c4682-159">Consulte também</span><span class="sxs-lookup"><span data-stu-id="c4682-159">See also</span></span>

[<span data-ttu-id="c4682-160">Microsoft 365 vídeos de formação para empresas</span><span class="sxs-lookup"><span data-stu-id="c4682-160">Microsoft 365 for business training videos</span></span>](../business-video/index.yml)
