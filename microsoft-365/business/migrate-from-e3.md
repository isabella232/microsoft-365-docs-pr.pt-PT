---
title: Migrar para o Microsoft 365 Business a partir do Office 365 E3
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
description: Saiba como mover o seu negócio para o Microsoft 365 Business Premium do Office 365 E3.
ms.openlocfilehash: d72f0c52a745ff973868b6fdaa95efa1a37a3dbd
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/18/2020
ms.locfileid: "45081880"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a><span data-ttu-id="91f12-103">Migrando do Office 365 E3 para o Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="91f12-103">Migrating from Office 365 E3 to Microsoft 365 Business Premium</span></span> 

<span data-ttu-id="91f12-104">O Microsoft 365 Business Premium tem tudo o que precisa para o seu pequeno negócio, combinando as melhores aplicações de produtividade baseadas na nuvem com uma simples gestão e segurança de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="91f12-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security.</span></span> <span data-ttu-id="91f12-105">Se atualmente tem uma subscrição do Office 365 E3, mas não tem mais de 300 funcionários, considere mudar para o Microsoft 365 Business Premium para funcionalidades de segurança adicionais.</span><span class="sxs-lookup"><span data-stu-id="91f12-105">If you currently have an Office 365 E3 subscription, but don't have more than 300 employees, consider switching to Microsoft 365 Business Premium for added security features.</span></span>

<span data-ttu-id="91f12-106">Migrar é fácil: Primeiro, troca licenças e mantém-se todos os seus dados e informações do utilizador na sua subscrição atual.</span><span class="sxs-lookup"><span data-stu-id="91f12-106">Migrating is easy: First you switch licenses and all your data and user information in your current subscription is maintained.</span></span> <span data-ttu-id="91f12-107">Após a migração, terá de configurar as funcionalidades que são adicionadas no Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="91f12-107">After the migration, you'll need to set up the features that are added in Microsoft 365 Business Premium.</span></span>

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a><span data-ttu-id="91f12-108">Diferenças entre o Office 365 E3 e o Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="91f12-108">Differences between Office 365 E3 and Microsoft 365 Business Premium</span></span>

<span data-ttu-id="91f12-109">Esta tabela mostra as diferenças entre o Microsoft 365 Business Premium e o Office 365 E3.</span><span class="sxs-lookup"><span data-stu-id="91f12-109">This table shows the differences between Microsoft 365 Business Premium and Office 365 E3.</span></span>

| <span data-ttu-id="91f12-110">Funcionalidade</span><span class="sxs-lookup"><span data-stu-id="91f12-110">Feature</span></span>    | <span data-ttu-id="91f12-111">Suporte no Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="91f12-111">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="91f12-112">Apoio no Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="91f12-112">Support in Office 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="91f12-113">**No local**</span><span class="sxs-lookup"><span data-stu-id="91f12-113">**On-premises**</span></span>        | | | 
| <span data-ttu-id="91f12-114">Aplicativos de escritório<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="91f12-114">Office apps<sup>1</sup></span></span>    | <span data-ttu-id="91f12-115">Microsoft 365 Apps para negócios</span><span class="sxs-lookup"><span data-stu-id="91f12-115">Microsoft 365 Apps for business</span></span>    | <span data-ttu-id="91f12-116">Microsoft 365 Apps para empresa</span><span class="sxs-lookup"><span data-stu-id="91f12-116">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="91f12-117">**Aplicativos de produtividade em nuvem**</span><span class="sxs-lookup"><span data-stu-id="91f12-117">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="91f12-118">Troca online e outlook</span><span class="sxs-lookup"><span data-stu-id="91f12-118">Exchange Online and Outlook</span></span>    | <span data-ttu-id="91f12-119">Limite de armazenamento de 50 GB por caixa de correio e arquivamento online ilimitado de trocas</span><span class="sxs-lookup"><span data-stu-id="91f12-119">50 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span>    | <span data-ttu-id="91f12-120">Limite de armazenamento de 100 GB por caixa de correio e arquivamento online ilimitado de trocas</span><span class="sxs-lookup"><span data-stu-id="91f12-120">100 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span> | 
| <span data-ttu-id="91f12-121">Equipas</span><span class="sxs-lookup"><span data-stu-id="91f12-121">Teams</span></span>    | ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | ![Incluído com Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="91f12-124">OneDrive para Empresas</span><span class="sxs-lookup"><span data-stu-id="91f12-124">OneDrive for Business</span></span>    | <span data-ttu-id="91f12-125">1 Limite de armazenamento de TB por utilizador</span><span class="sxs-lookup"><span data-stu-id="91f12-125">1 TB storage limit per user</span></span>    | <span data-ttu-id="91f12-126">Ilimitado</span><span class="sxs-lookup"><span data-stu-id="91f12-126">Unlimited</span></span> | 
| <span data-ttu-id="91f12-127">Yammer, SharePoint Online, Planner, Stream</span><span class="sxs-lookup"><span data-stu-id="91f12-127">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | ![Incluído com Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="91f12-130">StaffHub</span><span class="sxs-lookup"><span data-stu-id="91f12-130">StaffHub</span></span>    | ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | ![Incluído com Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="91f12-133">Outlook Customer Manager, MileIQ</span><span class="sxs-lookup"><span data-stu-id="91f12-133">Outlook Customer Manager, MileIQ</span></span>    | ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| <span data-ttu-id="91f12-135">**Proteção contra ameaças**</span><span class="sxs-lookup"><span data-stu-id="91f12-135">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="91f12-136">Office 365 Advanced Threat Protection (ATP) Plano 1</span><span class="sxs-lookup"><span data-stu-id="91f12-136">Office 365 Advanced Threat Protection (ATP) Plan 1</span></span> | ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | <span data-ttu-id="91f12-138">Não incluído, mas pode ser adicionado em</span><span class="sxs-lookup"><span data-stu-id="91f12-138">Not included, but can be added on</span></span> | 
| <span data-ttu-id="91f12-139">**Gestão de identidades**</span><span class="sxs-lookup"><span data-stu-id="91f12-139">**Identity management**</span></span>        | | | 
| <span data-ttu-id="91f12-140">Autosserviço de autosserviço reset para contas híbridas Azure Ative Directory (Azure AD), autenticação multi-factor Azure (MFA), Acesso Condicional, writeback de palavra-passe para identidades no local</span><span class="sxs-lookup"><span data-stu-id="91f12-140">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    |  | 
| <span data-ttu-id="91f12-142">**Gestão de dispositivos e aplicativos**</span><span class="sxs-lookup"><span data-stu-id="91f12-142">**Device and app management**</span></span>        | | |
| <span data-ttu-id="91f12-143">Microsoft Intune, Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="91f12-143">Microsoft Intune, Windows AutoPilot</span></span>|     ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| <span data-ttu-id="91f12-145">Ativação partilhada do computador</span><span class="sxs-lookup"><span data-stu-id="91f12-145">Shared computer activation</span></span>|     ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | ![Incluído com Office 365 E3](../media/check-mark.png)| 
| <span data-ttu-id="91f12-148">Direitos de upgrade para o Windows 10 Pro a partir de licenças Win 7/8.1 Pro</span><span class="sxs-lookup"><span data-stu-id="91f12-148">Upgrade rights to Windows 10 Pro from Win 7/8.1 Pro licenses</span></span>|     ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    || 
| <span data-ttu-id="91f12-150">**Proteção da informação**</span><span class="sxs-lookup"><span data-stu-id="91f12-150">**Information protection**</span></span>        | | |
|<span data-ttu-id="91f12-151">Gabinete 365 Prevenção de Perdas de Dados</span><span class="sxs-lookup"><span data-stu-id="91f12-151">Office 365 Data Loss Prevention</span></span>|    ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)|![Incluído com Office 365 E3](../media/check-mark.png)|
|<span data-ttu-id="91f12-154">Plano de Proteção de Informação Azure 1, aplicação bitlocker</span><span class="sxs-lookup"><span data-stu-id="91f12-154">Azure Information Protection Plan 1, Bitlocker enforcement</span></span>|![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="91f12-156">Plano de Proteção de Informação Azure 1, Etiquetas de sensibilidade</span><span class="sxs-lookup"><span data-stu-id="91f12-156">Azure Information Protection Plan 1, Sensitivity labels</span></span>|![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="91f12-158">**Licença de Acesso ao Cliente (direitos CAL)**</span><span class="sxs-lookup"><span data-stu-id="91f12-158">**Client Access License (CAL rights)**</span></span>|||
|<span data-ttu-id="91f12-159">Suíte Enterprise CAL (Bolsa, SharePoint, Skype)</span><span class="sxs-lookup"><span data-stu-id="91f12-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span></span>||![Incluído com Office 365 E3](../media/check-mark.png)|

<span data-ttu-id="91f12-161"><sup>1</sup> A versão Microsoft 365 Business Premium das aplicações office não inclui a ativação de volume através da Política de Grupo, telemetria de aplicações, controlos de atualização, comparação e consulta da folha de cálculo, ou Business Intelligence.</span><span class="sxs-lookup"><span data-stu-id="91f12-161"><sup>1</sup> The Microsoft 365 Business Premium version of the Office apps doesn't include volume activation through Group Policy, app telemetry, update controls, spreadsheet compare and inquire, or business Intelligence.</span></span>

## <a name="migration"></a><span data-ttu-id="91f12-162">Migração</span><span class="sxs-lookup"><span data-stu-id="91f12-162">Migration</span></span>

<span data-ttu-id="91f12-163">Para migrar a sua subscrição, consulte [os planos change manualmente](../commerce/subscriptions/change-plans-manually.md) para obter instruções se quiser mover apenas algumas pessoas para o Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="91f12-163">To migrate your subscription, see [Change plans manually](../commerce/subscriptions/change-plans-manually.md) for instructions if you want to move just a few people to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="91f12-164">Também pode [atualizar todos automaticamente,](../commerce/subscriptions/upgrade-to-different-plan.md)ou trabalhar com um parceiro para mover a subscrição e licenças E3 para uma subscrição Do Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="91f12-164">You can also [upgrade everyone automatically](../commerce/subscriptions/upgrade-to-different-plan.md), or work with a partner to move your E3 subscription and licenses to a Microsoft 365 Business Premium subscription.</span></span>
<span data-ttu-id="91f12-165">As secções seguintes descrevem as alterações que precisa de fazer, se houver, e o que pode fazer após a migração.</span><span class="sxs-lookup"><span data-stu-id="91f12-165">The following sections describe the changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="office-365-e3-subscription-configuration-and-data"></a><span data-ttu-id="91f12-166">Configuração e dados de subscrição do Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="91f12-166">Office 365 E3 subscription configuration and data</span></span>
<span data-ttu-id="91f12-167">Não precisa de fazer alterações na sua subscrição ou dados atuais antes de migrar, o que inclui:</span><span class="sxs-lookup"><span data-stu-id="91f12-167">You don't need to do any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="91f12-168">Configuração de subscrição, como registos DNS e nomes de domínio.</span><span class="sxs-lookup"><span data-stu-id="91f12-168">Subscription configuration, such as DNS records and domain names.</span></span>
- <span data-ttu-id="91f12-169">Contas de utilizador e grupo e configurações de autenticação, tais como a autenticação de vários fatores ou políticas de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="91f12-169">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="91f12-170">Configurações de serviço de produtividade e seus dados, tais como Equipas, Caixas de correio Exchange Online, sites SharePoint Online, OneDrive para pastas de negócios e cadernos OneNote.</span><span class="sxs-lookup"><span data-stu-id="91f12-170">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>
- <span data-ttu-id="91f12-171">As aplicações do office serão reduzidas automaticamente.</span><span class="sxs-lookup"><span data-stu-id="91f12-171">Office applications will scale automatically.</span></span> <span data-ttu-id="91f12-172">O licenciamento moderno do Office 365 verificará a atribuição da licença do utilizador a cada 72 horas e converterá as aplicações do Office para a versão que corresponde à subscrição do utilizador.</span><span class="sxs-lookup"><span data-stu-id="91f12-172">Office 365 modern licensing will check the user’s license assignment every 72 hours and will convert Office applications to the version that matches the user subscription.</span></span>

### <a name="windows-10"></a><span data-ttu-id="91f12-173">Windows 10</span><span class="sxs-lookup"><span data-stu-id="91f12-173">Windows 10</span></span>

<span data-ttu-id="91f12-174">Se o Windows ainda não estiver na atualização do Windows Pro Creator, [atualize-os para a Atualização de Criadores do Windows Pro](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="91f12-174">If your Windows aren't already on Windows Pro Creator update, [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

### <a name="set-up-policies-to-protect-user-devices-and-files"></a><span data-ttu-id="91f12-175">Configurar políticas para proteger dispositivos e ficheiros dos utilizadores</span><span class="sxs-lookup"><span data-stu-id="91f12-175">Set up policies to protect user devices and files</span></span>

> [!NOTE]
> <span data-ttu-id="91f12-176">Se configurar as políticas e dispositivos do Office 365 MDM, esses dispositivos serão listados na página **de Dispositivos** no centro de administração microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="91f12-176">If you set up Office 365 MDM policies and devices, those devices will be listed on the **Devices** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="91f12-177">Quaisquer políticas que tenha configurado aparecerão na lista de políticas clássicas no [portal Intune.](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)</span><span class="sxs-lookup"><span data-stu-id="91f12-177">Any policies you set up will show up in the list of classic policies in the [Intune portal](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span></span>

<span data-ttu-id="91f12-178">Depois de ter atribuído licenças ao Microsoft 365 Business Premium, pode começar a proteger os dispositivos e ficheiros dos utilizadores.</span><span class="sxs-lookup"><span data-stu-id="91f12-178">After you have assigned licenses to Microsoft 365 Business Premium, you can start protecting the users' devices and files.</span></span>

<span data-ttu-id="91f12-179">Se atualizar todos na sua organização para o Microsoft 365 Business Premium, verá o assistente de configuração na página Inicial e poderá seguir o [Microsoft 365 Business Premium nas](set-up.md) etapas do assistente de configuração para proteger ficheiros e dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="91f12-179">If you upgraded everyone in your organization to Microsoft 365 Business Premium, you'll see the setup wizard on the Home page, and can follow the [Set up Microsoft 365 Business Premium in the setup wizard](set-up.md) steps to protect files and mobile devices.</span></span>

<span data-ttu-id="91f12-180">Também pode completar estes passos na página dispositivos:</span><span class="sxs-lookup"><span data-stu-id="91f12-180">You can also complete these steps on the Devices page:</span></span>
  
1. <span data-ttu-id="91f12-181">No centro de administração, na navegação à esquerda, vá às Políticas **de Dispositivos.** \> **Policies**</span><span class="sxs-lookup"><span data-stu-id="91f12-181">In the admin center, in the left nav, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="91f12-182">Na página de políticas do **Dispositivo,** escolha **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="91f12-182">On the **Device policies** page, choose **Add**.</span></span>
    
3. <span data-ttu-id="91f12-183">No painel **de política Add** dê um nome à política e, em seguida, escolha um tipo de **Política** a partir do drop-down.</span><span class="sxs-lookup"><span data-stu-id="91f12-183">In the **Add policy** pane give the policy a name, and then choose a **Policy type** from the drop-down.</span></span> 
    
     <span data-ttu-id="91f12-184">Pode configurar políticas de aplicações para proteger ficheiros em dispositivos Android e iPhone, bem como windows 10, e pode configurar políticas de configuração de dispositivos para dispositivos do Windows 10 da empresa.</span><span class="sxs-lookup"><span data-stu-id="91f12-184">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="91f12-185">Consulte os seguintes links para mais detalhes:</span><span class="sxs-lookup"><span data-stu-id="91f12-185">See the following links for details:</span></span>
    
  - [<span data-ttu-id="91f12-186">Configurar as definições de proteção de aplicações para dispositivos Android ou iOS</span><span class="sxs-lookup"><span data-stu-id="91f12-186">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="91f12-187">Configurar as definições de proteção de aplicações para dispositivos Windows 10</span><span class="sxs-lookup"><span data-stu-id="91f12-187">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="91f12-188">Definir definições de proteção do dispositivo para PCs do Windows 10</span><span class="sxs-lookup"><span data-stu-id="91f12-188">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  
4. <span data-ttu-id="91f12-189">Assim que definir políticas, você e os seus colaboradores podem configurar dispositivos:</span><span class="sxs-lookup"><span data-stu-id="91f12-189">Once you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="91f12-190">Consulte [configurar dispositivos Windows para utilizadores Do Microsoft 365 Business Premium](set-up-windows-devices.md) para etapas para dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="91f12-190">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="91f12-191">Consulte [configurar dispositivos móveis para utilizadores Do Microsoft 365 Business Premium](set-up-mobile-devices.md) para passos para telemóveis e iPhones Android.</span><span class="sxs-lookup"><span data-stu-id="91f12-191">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 

### <a name="threat-protection"></a><span data-ttu-id="91f12-192">Proteção contra ameaças</span><span class="sxs-lookup"><span data-stu-id="91f12-192">Threat protection</span></span>

<span data-ttu-id="91f12-193">Depois de migrar para o Microsoft 365 Business Premium, tem o Office 365 ATP.</span><span class="sxs-lookup"><span data-stu-id="91f12-193">After migrating to Microsoft 365 Business Premium, you have Office 365 ATP.</span></span> <span data-ttu-id="91f12-194">Consulte [o Office 365 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) para uma visão geral.</span><span class="sxs-lookup"><span data-stu-id="91f12-194">See [Office 365 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) for an overview.</span></span> <span data-ttu-id="91f12-195">Para configurar, consulte [configurar links de segurança ATP,](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa) [configurar anexos seguros ATP](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)e [configurar anti-phishing ATP](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span><span class="sxs-lookup"><span data-stu-id="91f12-195">To set up, see [set up ATP safe links](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [set up ATP safe attachments](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), and [set up ATP anti-phishing](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span></span>

### <a name="sensitivity-labels"></a><span data-ttu-id="91f12-196">Etiquetas de confidencialidade</span><span class="sxs-lookup"><span data-stu-id="91f12-196">Sensitivity labels</span></span>

<span data-ttu-id="91f12-197">Para começar a utilizar rótulos de sensibilidade, consulte [a visão geral dos rótulos de sensibilidade](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) e crie e gere vídeos de [etiquetas de sensibilidade.](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)</span><span class="sxs-lookup"><span data-stu-id="91f12-197">To start using sensitivity labels, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) and [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>
