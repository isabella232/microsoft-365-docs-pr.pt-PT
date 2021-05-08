---
title: Migrar para o Microsoft 365 Empresas do Office 365 E3
f1.keywords:
- NOCSH
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Saiba como mover a sua empresa para Microsoft 365 Empresas Premium do Office 365 E3.
ms.openlocfilehash: f08b054473fdd63ec2372e81c776a1b64f89fe9d
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/06/2021
ms.locfileid: "52244842"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a><span data-ttu-id="e263c-103">Migrar do Office 365 E3 para o Microsoft 365 Empresas Premium</span><span class="sxs-lookup"><span data-stu-id="e263c-103">Migrating from Office 365 E3 to Microsoft 365 Business Premium</span></span>

<span data-ttu-id="e263c-104">Microsoft 365 Empresas Premium tem tudo o que precisa para a sua pequena empresa, combinando as melhores aplicações de produtividade baseadas na nuvem na classe, com gestão e segurança de dispositivos simples.</span><span class="sxs-lookup"><span data-stu-id="e263c-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security.</span></span> <span data-ttu-id="e263c-105">Se tiver atualmente uma subscrição do Office 365 E3, mas não tiver mais de 300 funcionários, considere mudar para o Microsoft 365 Empresas Premium para ter funcionalidades de segurança adicionais.</span><span class="sxs-lookup"><span data-stu-id="e263c-105">If you currently have an Office 365 E3 subscription, but don't have more than 300 employees, consider switching to Microsoft 365 Business Premium for added security features.</span></span>

<span data-ttu-id="e263c-106">A migração é fácil: Primeiro, muda de licenças e todas as suas informações de utilizador e dados na sua subscrição atual são mantidos.</span><span class="sxs-lookup"><span data-stu-id="e263c-106">Migrating is easy: First you switch licenses and all your data and user information in your current subscription is maintained.</span></span> <span data-ttu-id="e263c-107">Após a migração, terá de configurar as funcionalidades adicionadas às Microsoft 365 Empresas Premium.</span><span class="sxs-lookup"><span data-stu-id="e263c-107">After the migration, you'll need to set up the features that are added in Microsoft 365 Business Premium.</span></span>

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a><span data-ttu-id="e263c-108">Diferenças entre Office 365 E3 e Microsoft 365 Empresas Premium</span><span class="sxs-lookup"><span data-stu-id="e263c-108">Differences between Office 365 E3 and Microsoft 365 Business Premium</span></span>

<span data-ttu-id="e263c-109">Esta tabela mostra as diferenças entre Microsoft 365 Empresas Premium e Office 365 E3.</span><span class="sxs-lookup"><span data-stu-id="e263c-109">This table shows the differences between Microsoft 365 Business Premium and Office 365 E3.</span></span>

| <span data-ttu-id="e263c-110">Funcionalidade</span><span class="sxs-lookup"><span data-stu-id="e263c-110">Feature</span></span>    | <span data-ttu-id="e263c-111">Suporte no Microsoft 365 Empresas Premium</span><span class="sxs-lookup"><span data-stu-id="e263c-111">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="e263c-112">Suporte no Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="e263c-112">Support in Office 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="e263c-113">**No local**</span><span class="sxs-lookup"><span data-stu-id="e263c-113">**On-premises**</span></span>        | | | 
| <span data-ttu-id="e263c-114">Office aplicações<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="e263c-114">Office apps<sup>1</sup></span></span>    | <span data-ttu-id="e263c-115">Microsoft 365 Apps para Pequenas e Médias Empresas</span><span class="sxs-lookup"><span data-stu-id="e263c-115">Microsoft 365 Apps for business</span></span>    | <span data-ttu-id="e263c-116">Aplicações Microsoft 365 para empresas</span><span class="sxs-lookup"><span data-stu-id="e263c-116">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="e263c-117">**Aplicações de produtividade na nuvem**</span><span class="sxs-lookup"><span data-stu-id="e263c-117">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="e263c-118">Exchange Online e Outlook</span><span class="sxs-lookup"><span data-stu-id="e263c-118">Exchange Online and Outlook</span></span>    | <span data-ttu-id="e263c-119">Limite de armazenamento de 50 GB por caixa de correio e limite de Arquivo de Exchange Online</span><span class="sxs-lookup"><span data-stu-id="e263c-119">50 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span>    | <span data-ttu-id="e263c-120">Limite de armazenamento de 100 GB por caixa de correio e limite de Arquivo de Exchange Online</span><span class="sxs-lookup"><span data-stu-id="e263c-120">100 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span> | 
| <span data-ttu-id="e263c-121">Teams</span><span class="sxs-lookup"><span data-stu-id="e263c-121">Teams</span></span>    | ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    | ![Incluído com o Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="e263c-124">OneDrive para Empresas</span><span class="sxs-lookup"><span data-stu-id="e263c-124">OneDrive for Business</span></span>    | <span data-ttu-id="e263c-125">1 limite de armazenamento TB por utilizador</span><span class="sxs-lookup"><span data-stu-id="e263c-125">1 TB storage limit per user</span></span>    | <span data-ttu-id="e263c-126">Ilimitado</span><span class="sxs-lookup"><span data-stu-id="e263c-126">Unlimited</span></span> | 
| <span data-ttu-id="e263c-127">Yammer, SharePoint Online, Planner, Stream</span><span class="sxs-lookup"><span data-stu-id="e263c-127">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    | ![Incluído com o Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="e263c-130">StaffHub</span><span class="sxs-lookup"><span data-stu-id="e263c-130">StaffHub</span></span>    | ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    | ![Incluído com o Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="e263c-133">MileIQ</span><span class="sxs-lookup"><span data-stu-id="e263c-133">MileIQ</span></span>    | ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    | | 
| <span data-ttu-id="e263c-135">**Proteção Contra Ameaças**</span><span class="sxs-lookup"><span data-stu-id="e263c-135">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="e263c-136">Defender para Office 365 Plano 1</span><span class="sxs-lookup"><span data-stu-id="e263c-136">Defender for Office 365 Plan 1</span></span> | ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    | <span data-ttu-id="e263c-138">Não incluído, mas pode ser adicionado a</span><span class="sxs-lookup"><span data-stu-id="e263c-138">Not included, but can be added on</span></span> | 
| <span data-ttu-id="e263c-139">**Gestão de identidades**</span><span class="sxs-lookup"><span data-stu-id="e263c-139">**Identity management**</span></span>        | | | 
| <span data-ttu-id="e263c-140">Reposição de palavra-passe self-service para contas híbridas do Azure Active Directory (Azure AD), Autenticação multifatores (MFA) do Azure AD, Acesso Condicional, writeback de palavra-passe para identidades no local</span><span class="sxs-lookup"><span data-stu-id="e263c-140">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure AD multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    |  | 
| <span data-ttu-id="e263c-142">**Gestão de dispositivos e aplicações**</span><span class="sxs-lookup"><span data-stu-id="e263c-142">**Device and app management**</span></span>        | | |
| <span data-ttu-id="e263c-143">Microsoft Intune, Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="e263c-143">Microsoft Intune, Windows AutoPilot</span></span>|     ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    |  |
| <span data-ttu-id="e263c-145">Ativação de computador partilhado</span><span class="sxs-lookup"><span data-stu-id="e263c-145">Shared computer activation</span></span>|     ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    | ![Incluído com o Office 365 E3](../media/check-mark.png)| 
| <span data-ttu-id="e263c-148">Direitos de atualização para Windows 10 Pro das licenças de e-Pro Win 7/8.1</span><span class="sxs-lookup"><span data-stu-id="e263c-148">Upgrade rights to Windows 10 Pro from Win 7/8.1 Pro licenses</span></span>|     ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    || 
| <span data-ttu-id="e263c-150">**Proteção de informações**</span><span class="sxs-lookup"><span data-stu-id="e263c-150">**Information protection**</span></span>        | | |
|<span data-ttu-id="e263c-151">Office 365 Prevenção de Perda de Dados</span><span class="sxs-lookup"><span data-stu-id="e263c-151">Office 365 Data Loss Prevention</span></span>|    ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)|![Incluído com o Office 365 E3](../media/check-mark.png)|
|<span data-ttu-id="e263c-154">Azure Information Protection Plano 1, BitLocker imposição</span><span class="sxs-lookup"><span data-stu-id="e263c-154">Azure Information Protection Plan 1, BitLocker enforcement</span></span>|![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)||
|<span data-ttu-id="e263c-156">Azure Information Protection Plano 1, etiquetas de confidencialidade</span><span class="sxs-lookup"><span data-stu-id="e263c-156">Azure Information Protection Plan 1, Sensitivity labels</span></span>|![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)||
|<span data-ttu-id="e263c-158">**Licença de Acesso de Cliente (direitos CAL)**</span><span class="sxs-lookup"><span data-stu-id="e263c-158">**Client Access License (CAL rights)**</span></span>|||
|<span data-ttu-id="e263c-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span><span class="sxs-lookup"><span data-stu-id="e263c-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span></span>||![Incluído com o Office 365 E3](../media/check-mark.png)|

<span data-ttu-id="e263c-161"><sup>1</sup> A Microsoft 365 Empresas Premium das aplicações do Office não inclui a ativação em volume através da Política de Grupo, telemetria de aplicações, controlos de atualização, comparação de páginas de páginas e consultas ou business Intelligence.</span><span class="sxs-lookup"><span data-stu-id="e263c-161"><sup>1</sup> The Microsoft 365 Business Premium version of the Office apps doesn't include volume activation through Group Policy, app telemetry, update controls, spreadsheet compare and inquire, or business Intelligence.</span></span>

## <a name="migration"></a><span data-ttu-id="e263c-162">Migração</span><span class="sxs-lookup"><span data-stu-id="e263c-162">Migration</span></span>

<span data-ttu-id="e263c-163">Para migrar a sua subscrição, consulte Alterar planos [manualmente](../commerce/subscriptions/change-plans-manually.md) para obter instruções se quiser mover apenas algumas pessoas para Microsoft 365 Empresas Premium.</span><span class="sxs-lookup"><span data-stu-id="e263c-163">To migrate your subscription, see [Change plans manually](../commerce/subscriptions/change-plans-manually.md) for instructions if you want to move just a few people to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="e263c-164">Também pode [atualizar todas](../commerce/subscriptions/upgrade-to-different-plan.md)as pessoas automaticamente ou trabalhar com um parceiro para mover a sua subscrição e licenças do E3 para uma subscrição Microsoft 365 Empresas Premium empresa.</span><span class="sxs-lookup"><span data-stu-id="e263c-164">You can also [upgrade everyone automatically](../commerce/subscriptions/upgrade-to-different-plan.md), or work with a partner to move your E3 subscription and licenses to a Microsoft 365 Business Premium subscription.</span></span>
<span data-ttu-id="e263c-165">As secções seguintes descrevem as alterações que precisa de fazer, se necessário, e o que pode fazer após a migração.</span><span class="sxs-lookup"><span data-stu-id="e263c-165">The following sections describe the changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="office-365-e3-subscription-configuration-and-data"></a><span data-ttu-id="e263c-166">Office 365 Configuração e dados da subscrição E3</span><span class="sxs-lookup"><span data-stu-id="e263c-166">Office 365 E3 subscription configuration and data</span></span>
<span data-ttu-id="e263c-167">Não precisa de fazer alterações à sua subscrição ou dados atuais antes da migração, o que inclui:</span><span class="sxs-lookup"><span data-stu-id="e263c-167">You don't need to do any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="e263c-168">Configuração da subscrição, como registos DNS e nomes de domínio.</span><span class="sxs-lookup"><span data-stu-id="e263c-168">Subscription configuration, such as DNS records and domain names.</span></span>
- <span data-ttu-id="e263c-169">Contas de utilizador e grupo e definições de autenticação, como a autenticação multifatores ou políticas de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="e263c-169">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="e263c-170">As configurações do serviço de produtividade e os respetivos dados, como o Teams, caixas de correio Exchange Online, sites do SharePoint Online, pastas OneDrive para Empresas e blocos OneNote notas.</span><span class="sxs-lookup"><span data-stu-id="e263c-170">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>
- <span data-ttu-id="e263c-171">Office aplicações serão dimensionadas automaticamente.</span><span class="sxs-lookup"><span data-stu-id="e263c-171">Office applications will scale automatically.</span></span> <span data-ttu-id="e263c-172">Office 365 licenciamento moderno irá verificar a atribuição de licenças do utilizador a cada 72 horas e irá converter as Office para a versão que corresponde à subscrição de utilizador.</span><span class="sxs-lookup"><span data-stu-id="e263c-172">Office 365 modern licensing will check the user’s license assignment every 72 hours and will convert Office applications to the version that matches the user subscription.</span></span>

### <a name="windows-10"></a><span data-ttu-id="e263c-173">Windows 10</span><span class="sxs-lookup"><span data-stu-id="e263c-173">Windows 10</span></span>

<span data-ttu-id="e263c-174">Se a Windows ainda não se encontrar na atualização Windows Pro Criador, atualize-os para a [Atualização para Windows Pro Criadores.](upgrade-to-windows-pro-creators-update.md)</span><span class="sxs-lookup"><span data-stu-id="e263c-174">If your Windows aren't already on Windows Pro Creator update, [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

### <a name="set-up-policies-to-protect-user-devices-and-files"></a><span data-ttu-id="e263c-175">Configurar políticas para proteger dispositivos e ficheiros de utilizador</span><span class="sxs-lookup"><span data-stu-id="e263c-175">Set up policies to protect user devices and files</span></span>

> [!NOTE]
> <span data-ttu-id="e263c-176">Se configurar políticas e dispositivos Office 365 MDM, esses dispositivos serão listados na página Dispositivos no Microsoft 365 de administração. </span><span class="sxs-lookup"><span data-stu-id="e263c-176">If you set up Office 365 MDM policies and devices, those devices will be listed on the **Devices** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="e263c-177">Todas as políticas que configurar serão mostradas na lista de políticas clássicas no [portal do Intune.](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)</span><span class="sxs-lookup"><span data-stu-id="e263c-177">Any policies you set up will show up in the list of classic policies in the [Intune portal](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span></span>

<span data-ttu-id="e263c-178">Após ter atribuído licenças à Microsoft 365 Empresas Premium, pode começar a proteger os dispositivos e ficheiros dos utilizadores.</span><span class="sxs-lookup"><span data-stu-id="e263c-178">After you have assigned licenses to Microsoft 365 Business Premium, you can start protecting the users' devices and files.</span></span>

<span data-ttu-id="e263c-179">Se atualizou todas as pessoas na sua organização para o Microsoft 365 Empresas Premium, verá o assistente de configuração na home page e poderá seguir o passo Configurar [Microsoft 365 Empresas Premium](set-up.md) nos passos do assistente de configuração para proteger ficheiros e dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="e263c-179">If you upgraded everyone in your organization to Microsoft 365 Business Premium, you'll see the setup wizard on the Home page, and can follow the [Set up Microsoft 365 Business Premium in the setup wizard](set-up.md) steps to protect files and mobile devices.</span></span>

<span data-ttu-id="e263c-180">Também pode concluir estes passos na página Dispositivos:</span><span class="sxs-lookup"><span data-stu-id="e263c-180">You can also complete these steps on the Devices page:</span></span>
  
1. <span data-ttu-id="e263c-181">No centro de administração, no navegador esquerdo,  aceda a Políticas de \> **Dispositivos.**</span><span class="sxs-lookup"><span data-stu-id="e263c-181">In the admin center, in the left nav, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="e263c-182">Na página **Políticas de dispositivos,** selecionar **Adicionar.**</span><span class="sxs-lookup"><span data-stu-id="e263c-182">On the **Device policies** page, choose **Add**.</span></span>
    
3. <span data-ttu-id="e263c-183">No painel **Adicionar política,** dê um nome à política e, em seguida, escolha um Tipo de **política** a partir do painel de pastas.</span><span class="sxs-lookup"><span data-stu-id="e263c-183">In the **Add policy** pane give the policy a name, and then choose a **Policy type** from the drop-down.</span></span> 
    
     <span data-ttu-id="e263c-184">Pode configurar políticas de aplicação para proteger ficheiros em dispositivos Android e iPhone, bem como Windows 10, e pode configurar políticas de configuração de dispositivos para dispositivos Windows 10 empresa.</span><span class="sxs-lookup"><span data-stu-id="e263c-184">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="e263c-185">Consulte as seguintes ligações para obter detalhes:</span><span class="sxs-lookup"><span data-stu-id="e263c-185">See the following links for details:</span></span>
    
  - [<span data-ttu-id="e263c-186">Configurar as definições de proteção de aplicações para dispositivos Android ou iOS</span><span class="sxs-lookup"><span data-stu-id="e263c-186">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="e263c-187">Configurar as definições de proteção de aplicações para dispositivos Windows 10</span><span class="sxs-lookup"><span data-stu-id="e263c-187">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="e263c-188">Definir as definições de proteção de dispositivos Windows 10 PCs</span><span class="sxs-lookup"><span data-stu-id="e263c-188">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  
4. <span data-ttu-id="e263c-189">Assim que configurar políticas, você e os seus funcionários podem configurar dispositivos:</span><span class="sxs-lookup"><span data-stu-id="e263c-189">Once you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="e263c-190">Consulte [Configurar dispositivos Windows para utilizadores Microsoft 365 Empresas Premium passos](set-up-windows-devices.md) para os Windows dispositivos.</span><span class="sxs-lookup"><span data-stu-id="e263c-190">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="e263c-191">Consulte [Configurar dispositivos móveis para Microsoft 365 Empresas Premium para](set-up-mobile-devices.md) os passos para telemóveis e iPhones Android.</span><span class="sxs-lookup"><span data-stu-id="e263c-191">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 
  
### <a name="mailbox-size"></a><span data-ttu-id="e263c-192">Tamanho da Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="e263c-192">Mailbox Size</span></span>

<span data-ttu-id="e263c-193">Microsoft 365 Empresas Premium um limite de armazenamento de 50 GB à medida que Exchange Online Plano 1.</span><span class="sxs-lookup"><span data-stu-id="e263c-193">Microsoft 365 Business Premium has a 50 GB storage limit as it uses Exchange Online Plan 1.</span></span> <span data-ttu-id="e263c-194">Ao migrar para o Microsoft 365 Empresas Premium, se algum dos seus utilizadores exceder os 50 GB de armazenamento da caixa de correio, recomendamos que designe um Plano 2 do Exchange Online a este utilizador e remova o Plano Exchange Online 1, uma vez que não é exequecível atribuir ambas as informações.</span><span class="sxs-lookup"><span data-stu-id="e263c-194">While migrating to Microsoft 365 Business Premium, if any of your users exceed 50 GB of mailbox storage, it is recommended that you assign this user an Exchange Online Plan 2 and remove the Exchange Online Plan 1 as it's not feasible to assign both.</span></span>


### <a name="threat-protection"></a><span data-ttu-id="e263c-195">Proteção contra ameaças</span><span class="sxs-lookup"><span data-stu-id="e263c-195">Threat protection</span></span>

<span data-ttu-id="e263c-196">Após migrar para o Microsoft 365 Empresas Premium, tem o Defender para Office 365.</span><span class="sxs-lookup"><span data-stu-id="e263c-196">After migrating to Microsoft 365 Business Premium, you have Defender for Office 365.</span></span> <span data-ttu-id="e263c-197">Consulte [o Microsoft Defender para Office 365](../security/office-365-security/defender-for-office-365.md) uma visão geral.</span><span class="sxs-lookup"><span data-stu-id="e263c-197">See [Microsoft Defender for Office 365](../security/office-365-security/defender-for-office-365.md) for an overview.</span></span> <span data-ttu-id="e263c-198">Para configurar, consulte Configurar ligações de Cofre , [configurar](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5) [anexos](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)Cofre e configurar o [Anti phishing](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)no Defender para Office 365 .</span><span class="sxs-lookup"><span data-stu-id="e263c-198">To set up, see [set up Safe Links](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [set up Safe Attachments](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), and [set up Anti-phishing in Defender for Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span></span>

### <a name="sensitivity-labels"></a><span data-ttu-id="e263c-199">Etiquetas de confidencialidade</span><span class="sxs-lookup"><span data-stu-id="e263c-199">Sensitivity labels</span></span>

<span data-ttu-id="e263c-200">Para começar a utilizar etiquetas de sensibilidade, consulte o vídeo Visão geral das [etiquetas](../compliance/sensitivity-labels.md) de sensibilidade e criar e gerir [etiquetas de](../business-video/create-sensitivity-labels.md) sensibilidade.</span><span class="sxs-lookup"><span data-stu-id="e263c-200">To start using sensitivity labels, see [Overview of sensitivity labels](../compliance/sensitivity-labels.md) and [create and manage sensitivity labels](../business-video/create-sensitivity-labels.md) video.</span></span>
