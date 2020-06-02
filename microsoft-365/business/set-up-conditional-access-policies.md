---
title: Configurar políticas de acesso condicional para campanhas microsoft 365
f1.keywords:
- NOCSH
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
description: Saiba como configurar políticas de acesso condicional para as Campanhas Microsoft 365 para adicionar segurança adicional substancial.
ms.openlocfilehash: 58ee760877ee2fd7e53ef9463242657ab66a2b6e
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/01/2020
ms.locfileid: "44470653"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="9c7f2-103">Configurar políticas de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="9c7f2-103">Set up conditional access policies</span></span>

<span data-ttu-id="9c7f2-104">Este artigo aplica-se ao Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="9c7f2-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="9c7f2-105">[As](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) políticas de acesso condicional adicionam uma segurança adicional substancial.</span><span class="sxs-lookup"><span data-stu-id="9c7f2-105">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substantial additional security.</span></span> <span data-ttu-id="9c7f2-106">A Microsoft fornece um conjunto de políticas de acesso condicional de base que são recomendadas para todos os clientes.</span><span class="sxs-lookup"><span data-stu-id="9c7f2-106">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="9c7f2-107">As políticas de base são um conjunto de políticas predefinidas que ajudam a proteger as organizações contra muitos ataques comuns.</span><span class="sxs-lookup"><span data-stu-id="9c7f2-107">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="9c7f2-108">Estes ataques comuns podem incluir spray de palavra-passe, repetição e phishing.</span><span class="sxs-lookup"><span data-stu-id="9c7f2-108">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="9c7f2-109">Estas políticas exigem que os administradores e utilizadores introduzam uma segunda forma de autenticação (chamada autenticação multifactor, ou MFA) quando determinadas condições são satisfeitas.</span><span class="sxs-lookup"><span data-stu-id="9c7f2-109">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="9c7f2-110">Por exemplo, se um utilizador estiver a iniciar sessão a partir de um país diferente, a inscrição pode ser considerada arriscada e o utilizador deve fornecer uma forma adicional de autenticação.</span><span class="sxs-lookup"><span data-stu-id="9c7f2-110">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="9c7f2-111">Atualmente, as políticas de base incluem o seguinte:</span><span class="sxs-lookup"><span data-stu-id="9c7f2-111">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="9c7f2-112">**Exigir MFA para administradores** &ndash; Requer autenticação multi-factor para as funções de administrador mais privilegiadas, incluindo administrador global.</span><span class="sxs-lookup"><span data-stu-id="9c7f2-112">**Require MFA for admins** &ndash; Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="9c7f2-113">Proteção final **do utilizador** &ndash; Requer autenticação multi-factor para os utilizadores apenas quando uma entrada é arriscada.</span><span class="sxs-lookup"><span data-stu-id="9c7f2-113">**End user protection** &ndash; Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="9c7f2-114">**Bloquear a autenticação do** &ndash; legado As aplicações de clientes mais antigas e algumas novas aplicações não utilizam protocolos de autenticação mais recentes, mais seguros.</span><span class="sxs-lookup"><span data-stu-id="9c7f2-114">**Block legacy authentication** &ndash; Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="9c7f2-115">Estas aplicações mais antigas podem contornar políticas de acesso condicional e obter acesso não autorizado ao seu ambiente.</span><span class="sxs-lookup"><span data-stu-id="9c7f2-115">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="9c7f2-116">Esta política bloqueia o acesso de clientes que não suportam acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="9c7f2-116">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="9c7f2-117">**Exigir MFA para gestão de serviços** &ndash; Requer autenticação multi-factor para acesso a ferramentas de gestão, incluindo o portal Azure (onde configura políticas de base).</span><span class="sxs-lookup"><span data-stu-id="9c7f2-117">**Require MFA for Service Management** &ndash; Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="9c7f2-118">A Microsoft recomenda que ative todas estas políticas de base.</span><span class="sxs-lookup"><span data-stu-id="9c7f2-118">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="9c7f2-119">Após estas políticas estarem ativadas, os administradores e utilizadores serão solicitados a registarem-se para a autenticação do Azure Multii-Factor.</span><span class="sxs-lookup"><span data-stu-id="9c7f2-119">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="9c7f2-120">Para obter mais informações sobre estas políticas, veja [o que são políticas de base?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)</span><span class="sxs-lookup"><span data-stu-id="9c7f2-120">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="9c7f2-121">Configurar políticas de base</span><span class="sxs-lookup"><span data-stu-id="9c7f2-121">Set up baseline policies</span></span>

1. <span data-ttu-id="9c7f2-122">Vá ao [portal Azure](https://portal.azure.com)e, em seguida, navegue para **O Azure Ative Directory** \> **Conditional Access**.</span><span class="sxs-lookup"><span data-stu-id="9c7f2-122">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="9c7f2-123">As políticas de base estão listadas na página.</span><span class="sxs-lookup"><span data-stu-id="9c7f2-123">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="9c7f2-124">![Página que lista políticas de base para acesso condicional.](../media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="9c7f2-124">![Page that lists baseline policies for conditional access.](../media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="9c7f2-125">Consulte as seguintes instruções específicas para cada política:</span><span class="sxs-lookup"><span data-stu-id="9c7f2-125">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="9c7f2-126">Exigir MFA para administradores</span><span class="sxs-lookup"><span data-stu-id="9c7f2-126">Require MFA for admins</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="9c7f2-127">Exigir MFA para utilizadores</span><span class="sxs-lookup"><span data-stu-id="9c7f2-127">Require MFA for users</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="9c7f2-128">Bloquear a autenticação do legado</span><span class="sxs-lookup"><span data-stu-id="9c7f2-128">Block legacy authentication</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="9c7f2-129">Exigir MFA para gestão de serviços</span><span class="sxs-lookup"><span data-stu-id="9c7f2-129">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="9c7f2-130">Pode configurar muitas políticas adicionais, tais como a necessidade de aplicações de clientes aprovadas.</span><span class="sxs-lookup"><span data-stu-id="9c7f2-130">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="9c7f2-131">Para mais informações, consulte a [Documentação de Acesso Condicional.](https://docs.microsoft.com/azure/active-directory/conditional-access/)</span><span class="sxs-lookup"><span data-stu-id="9c7f2-131">For more information, see the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>
