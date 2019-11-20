---
title: Criar políticas de acesso condicional para as campanhas da Microsoft 365
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
description: Saiba como configurar políticas de acesso condicional para as campanhas Microsoft 365.
ms.openlocfilehash: aebdb733c2dd9a05947335ad4f151104d801568e
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/19/2019
ms.locfileid: "38718835"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="ba2b8-103">Criar políticas de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="ba2b8-103">Set up conditional access policies</span></span>

<span data-ttu-id="ba2b8-104">[As](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) políticas de acesso condicional adicionam segurança adicional substancial.</span><span class="sxs-lookup"><span data-stu-id="ba2b8-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substantial additional security.</span></span> <span data-ttu-id="ba2b8-105">A Microsoft fornece um conjunto de políticas de acesso condicional de base que são recomendadas para todos os clientes.</span><span class="sxs-lookup"><span data-stu-id="ba2b8-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="ba2b8-106">As políticas de base são um conjunto de políticas predefinidas que ajudam a proteger as organizações contra muitos ataques comuns.</span><span class="sxs-lookup"><span data-stu-id="ba2b8-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="ba2b8-107">Esses ataques comuns podem incluir spray de senha, repetição e phishing.</span><span class="sxs-lookup"><span data-stu-id="ba2b8-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="ba2b8-108">Essas políticas exigem que os administradores e usuários insiram uma segunda forma de autenticação (chamada autenticação multifator, ou MFA) quando determinadas condições forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="ba2b8-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="ba2b8-109">Por exemplo, se um usuário estiver se inscrevendo de um país diferente, o login pode ser considerado arriscado e o usuário deve fornecer uma forma adicional de autenticação.</span><span class="sxs-lookup"><span data-stu-id="ba2b8-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="ba2b8-110">Atualmente, as políticas de base incluem o seguinte:</span><span class="sxs-lookup"><span data-stu-id="ba2b8-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="ba2b8-111">**Exigir mfa para administradores** &ndash; requer multi-fator de autenticação para as funções de administrador mais privilegiados, incluindo administrador global.</span><span class="sxs-lookup"><span data-stu-id="ba2b8-111">**Require MFA for admins** &ndash; Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="ba2b8-112">**A proteção** &ndash; do usuário final requer autenticação multifator para usuários somente quando um login é arriscado.</span><span class="sxs-lookup"><span data-stu-id="ba2b8-112">**End user protection** &ndash; Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="ba2b8-113">**Bloqueie aplicativos legados** &ndash; de autenticação de clientes mais antigos e alguns novos aplicativos não usam protocolos de autenticação mais novos e mais seguros.</span><span class="sxs-lookup"><span data-stu-id="ba2b8-113">**Block legacy authentication** &ndash; Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="ba2b8-114">Esses aplicativos mais antigos podem ignorar as políticas de acesso condicional e obter acesso não autorizado ao seu ambiente.</span><span class="sxs-lookup"><span data-stu-id="ba2b8-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="ba2b8-115">Esta política bloqueia o acesso de clientes que não suportam o acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="ba2b8-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="ba2b8-116">**Exigir o MFA para gerenciamento** &ndash; de serviços requer autenticação multifator para acesso a ferramentas de gerenciamento, incluindo o portal Azure (onde você configura as políticas de base).</span><span class="sxs-lookup"><span data-stu-id="ba2b8-116">**Require MFA for Service Management** &ndash; Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="ba2b8-117">A Microsoft recomenda que você habilite todas essas políticas básicas.</span><span class="sxs-lookup"><span data-stu-id="ba2b8-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="ba2b8-118">Depois que essas políticas forem ativadas, os administradores e os usuários serão solicitados a se cadastrar na autenticação do Azure Multii-Factor.</span><span class="sxs-lookup"><span data-stu-id="ba2b8-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="ba2b8-119">Para obter mais informações sobre essas políticas, veja quais são as políticas de [base?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)</span><span class="sxs-lookup"><span data-stu-id="ba2b8-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="ba2b8-120">Criar políticas de base</span><span class="sxs-lookup"><span data-stu-id="ba2b8-120">Set up baseline policies</span></span>

1. <span data-ttu-id="ba2b8-121">Vá para o [portal Azure](https://portal.azure.com)e, em seguida, navegue para o **Azure Active Directory** \> **Conditional Access**.</span><span class="sxs-lookup"><span data-stu-id="ba2b8-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="ba2b8-122">As políticas básicas estão listadas na página.</span><span class="sxs-lookup"><span data-stu-id="ba2b8-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="ba2b8-123">![Página que lista as políticas básicas para acesso condicional.](media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="ba2b8-123">![Page that lists baseline policies for conditional access.](media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="ba2b8-124">Veja as seguintes instruções específicas para cada política:</span><span class="sxs-lookup"><span data-stu-id="ba2b8-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="ba2b8-125">Exigir MFA para administradores</span><span class="sxs-lookup"><span data-stu-id="ba2b8-125">Require MFA for admins</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="ba2b8-126">Exigir MFA para usuários</span><span class="sxs-lookup"><span data-stu-id="ba2b8-126">Require MFA for users</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="ba2b8-127">Bloquear a autenticação herdada</span><span class="sxs-lookup"><span data-stu-id="ba2b8-127">Block legacy authentication</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="ba2b8-128">Exigir MFA para gestão de serviços</span><span class="sxs-lookup"><span data-stu-id="ba2b8-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="ba2b8-129">Você pode configurar muitas políticas adicionais, como a exigência de aplicativos de clientes aprovados.</span><span class="sxs-lookup"><span data-stu-id="ba2b8-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="ba2b8-130">Para mais informações, consulte a Documentação de [Acesso Condicional.](https://docs.microsoft.com/azure/active-directory/conditional-access/)</span><span class="sxs-lookup"><span data-stu-id="ba2b8-130">For more information, see the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>
