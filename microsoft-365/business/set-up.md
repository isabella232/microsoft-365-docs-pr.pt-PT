---
title: Configurar o Microsoft 365 Business através do assistente de configuração
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
description: Obter informações sobre como configurar o Microsoft 365 Business, concluindo os quatro passos.
ms.openlocfilehash: a1c8a41c3e291983276280a063248bdd10a7f85a
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32283941"
---
# <a name="set-up-microsoft-365-business-by-using-the-setup-wizard"></a><span data-ttu-id="6df63-103">Configurar o Microsoft 365 Business através do assistente de configuração</span><span class="sxs-lookup"><span data-stu-id="6df63-103">Set up Microsoft 365 Business by using the setup wizard</span></span>

<span data-ttu-id="6df63-104">Conclua os passos 1 a 4 abaixo.</span><span class="sxs-lookup"><span data-stu-id="6df63-104">Complete steps 1-4 below.</span></span>
  
### <a name="set-up-microsoft-365-business"></a><span data-ttu-id="6df63-105">Configurar o Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="6df63-105">Set up Microsoft 365 Business</span></span>

<span data-ttu-id="6df63-106">Ver um vídeo sobre como configurar o Microsoft 365 Business quando não tiver um local, Active Directory:</span><span class="sxs-lookup"><span data-stu-id="6df63-106">Watch a video on how to set up Microsoft 365 Business when you don't have an on-premises Active Directory:</span></span>
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/0705c337-f3e8-4d28-bb6c-530cd28e99f2?autoplay=false]
  
<span data-ttu-id="6df63-107">Os passos de configuração incluem informações sobre configurações que incluem o local do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6df63-107">The set-up steps include information for setups that include local Active Directory.</span></span> <span data-ttu-id="6df63-108">Se pretender continuar a aceder a dispositivos associados ao domínio, leia os seguintes artigos para dois outra forma de permitir que e conclua os passos antes de executar o Assistente de configuração:</span><span class="sxs-lookup"><span data-stu-id="6df63-108">If you want to continue to access domain-joined devices, read the following articles for two different way of enabling that, and complete the steps before you run the Setup wizard:</span></span>
  
- [<span data-ttu-id="6df63-109">Ativar a gestão, por parte do Microsoft 365 Business, de dispositivos associados ao domínio Windows 10</span><span class="sxs-lookup"><span data-stu-id="6df63-109">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>](manage-windows-devices.md)
    
    <span data-ttu-id="6df63-110">-Esta é a forma recomendada.</span><span class="sxs-lookup"><span data-stu-id="6df63-110">-This is the recommended way.</span></span>
    
- [<span data-ttu-id="6df63-111">Acesso local recursos a partir de um dispositivo associado AD Azure no Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="6df63-111">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>](access-resources.md)
    
### <a name="step-1-personalize-sign-in"></a><span data-ttu-id="6df63-112">Passo 1: Personalizar o início de sessão</span><span class="sxs-lookup"><span data-stu-id="6df63-112">Step 1: Personalize sign-in</span></span>

1. <span data-ttu-id="6df63-p102">Inicie sessão no [Microsoft 365 Business](https://portal.microsoft.com) com as suas credenciais de administrador global. Selecione o mosaico **Administrador** para aceder ao centro de administração.</span><span class="sxs-lookup"><span data-stu-id="6df63-p102">Sign in to [Microsoft 365 Business](https://portal.microsoft.com) by using your global admin credentials. Choose the **Admin** tile to go to the admin center.</span></span> 
    
2. <span data-ttu-id="6df63-115">Selecione **Iniciar a configuração** (consoante o seu estado, poderá ver a opção **Continuar configuração**) no centro de administração para iniciar o assistente.</span><span class="sxs-lookup"><span data-stu-id="6df63-115">Choose **Start setup** (depending on your state you may see **Continue setup** instead) in the admin center to start the wizard.</span></span> 
    
3. <span data-ttu-id="6df63-116">Introduza o nome do domínio que pretende utilizar (como contoso.com)</span><span class="sxs-lookup"><span data-stu-id="6df63-116">Enter the domain name you want to use (like contoso.com).</span></span>
    
    <span data-ttu-id="6df63-117">Continue o processo e introduza o seu domínio mesmo que já o tenha verificado quando utilizou o Azure AD Connect, por exemplo.</span><span class="sxs-lookup"><span data-stu-id="6df63-117">Go ahead and enter your domain even if you have verified it while using Azure AD Connect, for example.</span></span> <span data-ttu-id="6df63-118">Os dois passos seguintes não se aplicam ao utilizador se tiver utilizado Azure AD ligar para verificar se o domínio.</span><span class="sxs-lookup"><span data-stu-id="6df63-118">The following two steps do not apply to you if you used Azure AD Connect to verify your domain.</span></span>
    
4. <span data-ttu-id="6df63-119">Siga os passos no Assistente para [registos de DNS criar em qualquer fornecedor de alojamento de DNS para o Office 365](https://support.office.com/article/7b7b075d-79f9-4e37-8a9e-fb60c1d95166) , que verifica que possui o domínio.</span><span class="sxs-lookup"><span data-stu-id="6df63-119">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://support.office.com/article/7b7b075d-79f9-4e37-8a9e-fb60c1d95166) that verifies you own the domain.</span></span> 
    
    <span data-ttu-id="6df63-120">Pode ver um vídeo de exemplo do [vídeo: configuração do Office 365 no novo Centro de administração do](https://support.office.com/article/a8c2002a-34bc-4ab3-93d8-9b5156c48bf8).</span><span class="sxs-lookup"><span data-stu-id="6df63-120">You can view an example video of [Video: Setup Office 365 in the new Admin Center](https://support.office.com/article/a8c2002a-34bc-4ab3-93d8-9b5156c48bf8).</span></span> <span data-ttu-id="6df63-121">Tenha em atenção que este vídeo não inclui os passos de proteção de dados do Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="6df63-121">Note that this video does not include the data protection steps of Microsoft 365 Business.</span></span>
    
    ![Screenshot of the Business Cloud Suite setup wizard.](media/3c4fd40c-2de1-4a87-8ee0-78d3928c7bb7.png)
  
### <a name="step-2-add-users-and-assign-licenses"></a><span data-ttu-id="6df63-123">Passo 2: Adicionar utilizadores e atribuir licenças</span><span class="sxs-lookup"><span data-stu-id="6df63-123">Step 2: Add users and assign licenses</span></span>

1. <span data-ttu-id="6df63-124">Pode adicionar utilizadores aqui ou [adicionar utilizadores mais tarde](add-users-m365b.md) no centro de administração.</span><span class="sxs-lookup"><span data-stu-id="6df63-124">You can add users here, or you can [add users later](add-users-m365b.md) in the admin center.</span></span> 
    
    <span data-ttu-id="6df63-125">Será atribuída automaticamente uma licença do Microsoft 365 Business a todos os utilizadores que adicionar.</span><span class="sxs-lookup"><span data-stu-id="6df63-125">Any users you add get automatically assigned a Microsoft 365 Business license.</span></span>
    
2. <span data-ttu-id="6df63-p105">Se a sua subscrição do Microsoft 365 Business já tiver utilizadores existentes (por exemplo, se utilizou o Azure AD Connect), verá uma opção para atribuir licenças aos mesmos agora. Continue o processo e adicione licenças aos utilizadores.</span><span class="sxs-lookup"><span data-stu-id="6df63-p105">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you will get an option to assign licenses to them now. Go ahead and add licenses to them as well.</span></span>
    
3. <span data-ttu-id="6df63-p106">Também verá uma opção para partilhar credenciais com os novos utilizadores adicionados. Pode optar por imprimir, transferir ou enviá-las por e-mail.</span><span class="sxs-lookup"><span data-stu-id="6df63-p106">You will also get an option to share credentials with the new users you added. You can choose to print them out, email them, or download them.</span></span>
    
4. <span data-ttu-id="6df63-130">Ignore a migração de mensagens de e-mail e selecione **Seguinte** na página **Migrar as mensagens de e-mail**.</span><span class="sxs-lookup"><span data-stu-id="6df63-130">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 
    
    <span data-ttu-id="6df63-131">Se estiver a mover de outro fornecedor de correio electrónico e pretender copiar os dados mais tarde, pode [Migrar correio-electrónico e contactos para o Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span><span class="sxs-lookup"><span data-stu-id="6df63-131">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>
    
    ![Screenshot of two new users added in the setup wizard](media/8f729967-5c65-4ceb-b737-18119db40564.png)
  
### <a name="step-3-connect-your-domain"></a><span data-ttu-id="6df63-133">Passo 3: Ligar ao domínio</span><span class="sxs-lookup"><span data-stu-id="6df63-133">Step 3: Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="6df63-134">Se optou por utilizar o domínio de .onmicrosoft, ou utilizado Azure AD ligar, não verá este passo.</span><span class="sxs-lookup"><span data-stu-id="6df63-134">If you chose to use the .onmicrosoft domain, or used Azure AD Connect, you will not see this step.</span></span> 
  
<span data-ttu-id="6df63-135">Para configurar serviços, tem de atualizar alguns registos no seu anfitrião de DNS ou entidade de registo de domínios.</span><span class="sxs-lookup"><span data-stu-id="6df63-135">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="6df63-136">Normalmente, o assistente de configuração deteta a sua entidade de registo e fornece-lhe uma ligação para instruções passo a passo de forma a atualizar os seus registos NS no site da entidade de registo de domínios.</span><span class="sxs-lookup"><span data-stu-id="6df63-136">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="6df63-137">Caso contrário, [nameservers de alteração para configurar o Office 365 qualquer registo de domínio](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="6df63-137">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span>
    
2. <span data-ttu-id="6df63-138">O e-mail e os restantes serviços serão configurados automaticamente</span><span class="sxs-lookup"><span data-stu-id="6df63-138">Email and other services will be set up for you</span></span>
    
### <a name="step-4-manage-devices-and-work-files"></a><span data-ttu-id="6df63-139">Passo 4: Gerir dispositivos e ficheiros de trabalho</span><span class="sxs-lookup"><span data-stu-id="6df63-139">Step 4: Manage devices and work files</span></span>

1. <span data-ttu-id="6df63-140">Na página **Proteger ficheiros de trabalho nos seus dispositivos móveis**, altere as definições **Proteger os ficheiros de trabalho se os dispositivos forem perdidos ou roubados** e **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis** para **Ativada**.</span><span class="sxs-lookup"><span data-stu-id="6df63-140">On the **Protect work files on your mobile devices** page set both **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** settings to **On**.</span></span> <span data-ttu-id="6df63-141">Também pode aceder a cada sub definição clicando em divisas ao lado de cada definição.</span><span class="sxs-lookup"><span data-stu-id="6df63-141">You can also access each sub-setting by clicking the chevrons next to each setting.</span></span>
  
  <span data-ttu-id="6df63-142">Todos os ficheiros de trabalho dos utilizadores licenciados estão agora protegidos iOS e dos dispositivos Android, logo [instalar aplicações do Office](set-up-mobile-devices.md) (e autenticar com as respectivas credenciais de Microsoft 365 Business).</span><span class="sxs-lookup"><span data-stu-id="6df63-142">All of your licensed users' work files are now protected on iOS and Android devices, as soon as they [install Office apps](set-up-mobile-devices.md) (and authenticate with their Microsoft 365 Business credentials).</span></span> 
  
  ![Screenshot of protect work files on your mobile devices page](media/3139a9aa-6228-4e74-8166-c6a886d7319f.PNG)
  
2. <span data-ttu-id="6df63-144">Na página **configuração do dispositivo Windows 10 definido** , defina **Proteger dispositivos 10 do Windows** como **no**.</span><span class="sxs-lookup"><span data-stu-id="6df63-144">On the **Set Windows 10 device configuration** page, set **Secure Windows 10 Devices** setting to **On**.</span></span>
  
   <span data-ttu-id="6df63-145">Também pode aceder a cada sub definição clicando nas divisas junto da mesma.</span><span class="sxs-lookup"><span data-stu-id="6df63-145">You can also access each sub-setting by clicking the chevron next to it.</span></span>
  
3. <span data-ttu-id="6df63-146">Altere a definição **Instalar o Office em dispositivos Windows 10** para **Sim** se todos os seus utilizadores tiverem computadores com o Windows 10, mas sem uma instalação do Office ou uma instalação do Office com tecnologia Clique-e-Use.</span><span class="sxs-lookup"><span data-stu-id="6df63-146">Set the **Install Office on Windows 10 Devices** setting to **Yes** if all of your users have Windows 10 computers, and either no existing Office installs, or click-to-run Office installs.</span></span> <span data-ttu-id="6df63-147">Se este não for o caso, defina esta opção para **Não**.</span><span class="sxs-lookup"><span data-stu-id="6df63-147">If this is not the case, set this option to **No**.</span></span> <span data-ttu-id="6df63-148">Pode [instalar automaticamente o Office](auto-install-or-uninstall-office.md) mais tarde a partir do centro de administração após ter preparado os computadores dos utilizadores.</span><span class="sxs-lookup"><span data-stu-id="6df63-148">You can [automatically install Office](auto-install-or-uninstall-office.md) later from the admin center after you have prepared the user computers.</span></span> <span data-ttu-id="6df63-149">Para obter instruções, consulte a [preparar a instalação de cliente do Office](prepare-for-office-client-deployment.md).</span><span class="sxs-lookup"><span data-stu-id="6df63-149">For instructions, see [prepare for Office client installation](prepare-for-office-client-deployment.md).</span></span>
  
    <span data-ttu-id="6df63-150">Ficheiros de trabalho dos utilizadores licenciados em dispositivos de Windows 10 vão ser projectados, logo a [associar o seu dispositivo Windows 10](set-up-windows-devices.md) a um domínio do Microsoft 365 Business Azure AD ou, em seguida, [instalar o Windows 10 num novo computador](https://support.office.com/article/c654bd23-d256-4ac7-8fba-0c993bf5a771.aspx) ao aderir ao mesmo tempo o Microsoft 365 Domínio de Azure AD de negócio.</span><span class="sxs-lookup"><span data-stu-id="6df63-150">The licensed users' work files on Windows 10 devices will be projected as soon as they [join their Windows 10 device](set-up-windows-devices.md) to a Microsoft 365 Business Azure AD domain or [install Windows 10 on a new computer](https://support.office.com/article/c654bd23-d256-4ac7-8fba-0c993bf5a771.aspx) while simultaneously joining the Microsoft 365 Business Azure AD domain.</span></span> 
  
4. <span data-ttu-id="6df63-151">Clique em **Seguinte** para terminar a configuração.</span><span class="sxs-lookup"><span data-stu-id="6df63-151">Click **Next** and you are done with setup.</span></span> 
  
    <span data-ttu-id="6df63-152">Dê-nos o seu feedback neste passo para nos ajudar a melhorar a experiência.</span><span class="sxs-lookup"><span data-stu-id="6df63-152">Please leave us feedback at this step to help us improve the experience.</span></span>
  
    ![Screenshot of Prepare Windows 10 devices page](media/bff701c1-48a3-44f4-aa95-9d959d57c85b.PNG)
  
## <a name="additional-security-settings"></a><span data-ttu-id="6df63-154">Definições de segurança adicionais</span><span class="sxs-lookup"><span data-stu-id="6df63-154">Additional security settings</span></span>

<span data-ttu-id="6df63-155">Para além da segurança e a definição de conformidade no Assistente de configuração, pode também configurar as seguintes definições adicionais:</span><span class="sxs-lookup"><span data-stu-id="6df63-155">In addition to the security and compliance setting in the setup wizard, you can also set up the following additional settings:</span></span>
  
- <span data-ttu-id="6df63-156">Configure a protecção contra anexos não seguros.</span><span class="sxs-lookup"><span data-stu-id="6df63-156">Set up protection against unsafe attachments.</span></span> <span data-ttu-id="6df63-157">**Avançada protecção contra ameaças** (ATP) identifica o conteúdo malicioso e, em seguida, bloqueia a entrega de anexos inseguros, ajudando a proteger o computador contra infecções de ransomware e esquemas de phishing.</span><span class="sxs-lookup"><span data-stu-id="6df63-157">**Advanced Threat Protection** (ATP) identifies malicious content and then blocks delivery of unsafe attachments, helping protect you against phishing schemes and ransomware infections.</span></span> <span data-ttu-id="6df63-158">Para activar a protecção do anexo, consulte [Configurar políticas de anexos seguros do Office 365 ATP](https://support.office.com/article/078eb946-819a-4e13-8673-fe0c0ad3a775#setpolicy).</span><span class="sxs-lookup"><span data-stu-id="6df63-158">To activate attachment protection, see [Set up Office 365 ATP Safe Attachments policies](https://support.office.com/article/078eb946-819a-4e13-8673-fe0c0ad3a775#setpolicy).</span></span>
    
- <span data-ttu-id="6df63-159">Proteger o ambiente, quando os utilizadores clicam em hiperligações maliciosas.</span><span class="sxs-lookup"><span data-stu-id="6df63-159">Protect your environment when users click malicious links.</span></span> <span data-ttu-id="6df63-160">ATP examina hiperligações na mensagem de correio electrónico quando que um utilizador clica-los.</span><span class="sxs-lookup"><span data-stu-id="6df63-160">ATP examines links in email at the time a user clicks them.</span></span> <span data-ttu-id="6df63-161">Se uma hiperligação não é segura, o utilizador é avisado não a visitar o site ou informado que o site foi bloqueado.</span><span class="sxs-lookup"><span data-stu-id="6df63-161">If a link is unsafe, the user is warned not to visit the site or informed that the site has been blocked.</span></span> <span data-ttu-id="6df63-162">Isto ajuda a proteger contra esquemas de phishing.</span><span class="sxs-lookup"><span data-stu-id="6df63-162">This helps protect against phishing schemes.</span></span> <span data-ttu-id="6df63-163">[Configurar políticas de segurança ligações do Office 365 ATP](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#reveddefaultscc) ou [configurar as políticas de segurança ligações do Office 365 ATP](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#addemailpolscc).</span><span class="sxs-lookup"><span data-stu-id="6df63-163">[Set up Office 365 ATP Safe Links policies](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#reveddefaultscc) or [Set up Office 365 ATP Safe Links policies](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#addemailpolscc).</span></span>
    
- <span data-ttu-id="6df63-164">Pode preservar incluindo itens eliminados, colocando o correio todo um utilizador no **litígio mantenha**todo o conteúdo da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6df63-164">You can preserve all mailbox content including deleted items by putting a user's entire mailbox on **litigation hold**.</span></span> <span data-ttu-id="6df63-165">Para obter instruções, consulte</span><span class="sxs-lookup"><span data-stu-id="6df63-165">For instructions, see</span></span> 
- <span data-ttu-id="6df63-166">[Configurar a retenção de correio electrónico com o arquivo Online do Exchange](security-features.md#set-up-email-retention-with-exchange-online-archiving).</span><span class="sxs-lookup"><span data-stu-id="6df63-166">[Set up email retention with Exchange Online Archiving](security-features.md#set-up-email-retention-with-exchange-online-archiving).</span></span>
    
- <span data-ttu-id="6df63-167">Configurar **políticas de retenção**de personalizadas, por exemplo, para manter durante um período específico de tempo ou eliminar permanentemente o conteúdo no final do período de retenção.</span><span class="sxs-lookup"><span data-stu-id="6df63-167">Set up customized **retention policies**, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="6df63-168">Pode activar políticas de retenção personalizada no Centro de conformidade, vá para a **governação de dados** de valores mobiliários e \> **retenção**e, em seguida, siga os passos no assistente.</span><span class="sxs-lookup"><span data-stu-id="6df63-168">You can enable customized retention policies in the Securities and compliance center, go to **Data governance** \> **Retention**, and then follow the steps in the wizard.</span></span> <span data-ttu-id="6df63-169">Para obter mais informações, consulte [Descrição geral de políticas de retenção](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span><span class="sxs-lookup"><span data-stu-id="6df63-169">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>
    
## <a name="next-steps"></a><span data-ttu-id="6df63-170">Next steps</span><span class="sxs-lookup"><span data-stu-id="6df63-170">Next steps</span></span>

<span data-ttu-id="6df63-171">Para os utilizadores que têm licenças, o próximo passo é configurar os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="6df63-171">For the users that have their licenses, the next step is to set up devices.</span></span><br/> <span data-ttu-id="6df63-172">Consulte [Configurar dispositivos Windows para utilizadores do Microsoft 365 Business](set-up-windows-devices.md) e [Configurar dispositivos móveis para utilizadores do Microsoft 365 Business](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="6df63-172">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) and [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span> <br/><span data-ttu-id="6df63-173">Consulte [Gerir o Microsoft 365 Business](manage.md) para obter ligações para tópicos sobre como definir políticas de proteção de aplicações e de dispositivos e como remover dados de dispositivos do utilizador.</span><span class="sxs-lookup"><span data-stu-id="6df63-173">See [Manage Microsoft 365 Business](manage.md) for links to topics on how to set device and app protection polices, and how to remove data from user devices.</span></span> 
  


