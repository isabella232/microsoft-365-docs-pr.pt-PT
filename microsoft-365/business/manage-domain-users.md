---
title: Sincronizar os utilizadores de domínio para o Microsoft 365
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
description: Sincronizar os utilizadores controlados pelo domínio com o Microsoft 365 para o negócio.
ms.openlocfilehash: af9cb7c9b2b639edc2375679a73ab41c4cf6de71
ms.sourcegitcommit: 5b769f74bcc76ac8d38aad815d1728824783cd9f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081909"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a><span data-ttu-id="1ff6b-103">Sincronizar os utilizadores de domínio para o Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="1ff6b-103">Synchronize domain users to Microsoft 365</span></span>

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="1ff6b-104">1. Preparar para a sincronização do diretório</span><span class="sxs-lookup"><span data-stu-id="1ff6b-104">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="1ff6b-105">Antes de sincronizar os seus utilizadores e computadores a partir do domínio do Diretório Ativo local, [reveja Prepare-se para sincronização de diretórios para o Microsoft 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="1ff6b-105">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Microsoft 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="1ff6b-106">Em particular:</span><span class="sxs-lookup"><span data-stu-id="1ff6b-106">In particular:</span></span>

   - <span data-ttu-id="1ff6b-107">Certifique-se de que não existem duplicados no seu diretório para os seguintes atributos: **correio,** **proxyAddresses**e **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-107">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="1ff6b-108">Estes valores devem ser únicos e quaisquer duplicados devem ser removidos.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-108">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="1ff6b-109">Recomendamos que configuure o atributo **userPrincipalName** (UPN) para cada conta de utilizador local para corresponder ao endereço de e-mail primário que corresponde ao utilizador licenciado microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-109">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="1ff6b-110">Por exemplo: *mary.shelley@contoso.com* em vez *de mary@contoso.local*</span><span class="sxs-lookup"><span data-stu-id="1ff6b-110">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="1ff6b-111">Se o domínio ative Directory terminar num sufixo não-encaminhável como *.local* ou *.lan*, em vez de um sufixo de internet rotable como *.com* ou *.org*, ajuste o sufixo UPN das contas de utilizador locais primeiro como descrito na [Prepare um domínio não-encaminhável para sincronização de diretórios](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="1ff6b-111">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

<span data-ttu-id="1ff6b-112">O **Run IdFix** no quarto passo (4) abaixo, também certificar-se-á de que o seu Ative Directory está pronto para sincronização de dir.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-112">The **Run IdFix** in step four (4) below, will also make sure your on-premises Active Directory is ready for dir sync.</span></span>

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="1ff6b-113">2. Instalar e configurar a Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="1ff6b-113">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="1ff6b-114">Para sincronizar os seus utilizadores, grupos e contactos do Diretório Ativo local no Azure Ative Directory, instale o Azure Ative Directory Connect e crie sincronização de diretórios.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-114">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> 

 1. <span data-ttu-id="1ff6b-115">No centro de administração <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> em seleção **Configurar** no navegador esquerdo.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-115">In the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> select **Setup** in the left nav.</span></span>

 2. <span data-ttu-id="1ff6b-116">Em **Iniciar sposição e segurança,** escolha **Ver** os **utilizadores do Sync a partir do diretório do seu org.**</span><span class="sxs-lookup"><span data-stu-id="1ff6b-116">Under **Sign-in and security**, choose **View**  under **Sync users from your org's directory**.</span></span>

 3. <span data-ttu-id="1ff6b-117">No **Sync dos utilizadores da página de diretório do seu org,** escolha **Começar a trabalhar**.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-117">On the **Sync users from your org's directory** page, choose **Get started**.</span></span>

 4. <span data-ttu-id="1ff6b-118">No primeiro passo, a ferramenta IdFix para preparar a sincronização do Diretório.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-118">In the first step  run IdFix tool to prepare for Directory sync.</span></span>

 5. <span data-ttu-id="1ff6b-119">Siga os passos do assistente para descarregar o Azure AD Connect e use-o para sincronizar os seus utilizadores controlados pelo domínio para o Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-119">Follow the wizard steps to download Azure AD Connect and use it to synchronize your domain-controlled users to Microsoft 365.</span></span>


<span data-ttu-id="1ff6b-120">Consulte [a sincronização de diretórios configurar para o Microsoft 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) para saber mais.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-120">See [Set up directory synchronization for Microsoft 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) to learn more.</span></span>

<span data-ttu-id="1ff6b-121">Ao configurar as suas opções para Azure AD Connect, recomendamos que ative a **sincronização de passwords**, **o Sign-On único sem emenda**e a funcionalidade de writeback de **palavra-passe,** que também é suportada no Microsoft 365 para negócios.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-121">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="1ff6b-122">Existem alguns passos adicionais para a gravação de palavras-passe para além da caixa de verificação no Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-122">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="1ff6b-123">Para obter mais informações, consulte [Como-a-fazer: configurar a gravação da palavra-passe](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="1ff6b-123">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

<span data-ttu-id="1ff6b-124">Se pretender gerir também dispositivos do Windows 10 unidos por domínios, consulte [ativar dispositivos Windows 10 que se juntem ao domínio para serem geridos pelo Microsoft 365 Business Premium](manage-windows-devices.md) para criar um AD AD AD Híbrido.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-124">If you want to manage domain-joined Windows 10 devices also, see [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set up a hybrid Azure AD Join.</span></span> 