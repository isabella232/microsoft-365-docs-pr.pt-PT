---
title: Configurar políticas de acesso condicional para campanhas de Microsoft 365
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
search.appverid:
- BCS160
- MET150
- MOE150
description: Obter informações sobre como configurar políticas de acesso condicional para Microsoft 365 campanhas.
ms.openlocfilehash: 7d8e1f16019d151478aae57b1593b0e0758e5b19
ms.sourcegitcommit: 7e46db0b35c188ee6a7b40ab3eb2d76ff6c101c5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/19/2019
ms.locfileid: "35086391"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="37c18-103">Configurar políticas de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="37c18-103">Set up conditional access policies</span></span>

<span data-ttu-id="37c18-104">Políticas de [acesso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) adicionar segurança adicional substancial.</span><span class="sxs-lookup"><span data-stu-id="37c18-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substancial additional security.</span></span> <span data-ttu-id="37c18-105">A Microsoft fornece um conjunto de políticas de acesso condicional do plano base que são recomendadas para todos os clientes.</span><span class="sxs-lookup"><span data-stu-id="37c18-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="37c18-106">As políticas do plano base são um conjunto de políticas predefinidas que ajudam a proteger organizações contra muitos ataques comuns.</span><span class="sxs-lookup"><span data-stu-id="37c18-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="37c18-107">Estes ataques comuns podem incluir pulverização de palavra-passe, de reprodução e de phishing.</span><span class="sxs-lookup"><span data-stu-id="37c18-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="37c18-108">Estas políticas requerem admins e os utilizadores introduzam uma segunda forma de autenticação (denominada autenticação multifactor ou AMF) quando forem cumpridas determinadas condições.</span><span class="sxs-lookup"><span data-stu-id="37c18-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="37c18-109">Por exemplo, se um utilizador é iniciada a sessão de outro país, a inscrição no possa ser considerada perigoso e o utilizador tem de fornecer uma forma adicional de autenticação.</span><span class="sxs-lookup"><span data-stu-id="37c18-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="37c18-110">Actualmente, as políticas do plano base incluem o seguinte:</span><span class="sxs-lookup"><span data-stu-id="37c18-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="37c18-111">**Exigir AMF para admins** — requer autenticação multi-factores para as funções de administrador mais privilegiadas, incluindo o administrador global.</span><span class="sxs-lookup"><span data-stu-id="37c18-111">**Require MFA for admins** — Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="37c18-112">**Protecção do utilizador final** — requer autenticação multi-factores para os utilizadores apenas quando um início de sessão-in é arriscado.</span><span class="sxs-lookup"><span data-stu-id="37c18-112">**End user protection** — Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="37c18-113">**Autenticação de legado bloco** — aplicações mais antigas do cliente e algumas novas aplicações não utilizam protocolos de autenticação mais seguro, mais recente.</span><span class="sxs-lookup"><span data-stu-id="37c18-113">**Block legacy authentication** — Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="37c18-114">Estas aplicações mais antigas, podem ignorar políticas de acesso condicional e obter acesso não autorizado ao seu ambiente.</span><span class="sxs-lookup"><span data-stu-id="37c18-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="37c18-115">Esta política bloqueia o acesso de clientes que não suportam acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="37c18-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="37c18-116">**Exigir AMF gestão de serviços de** — requer autenticação multi-factores para aceder a ferramentas de gestão, incluindo Azure portal (onde a configurar políticas de plano base).</span><span class="sxs-lookup"><span data-stu-id="37c18-116">**Require MFA for Service Management** — Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="37c18-117">A Microsoft recomenda que activa todas as políticas do plano base.</span><span class="sxs-lookup"><span data-stu-id="37c18-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="37c18-118">Depois destas políticas forem activadas, administradores e utilizadores serão pedidos para registar para a autenticação de factores Multii Azure.</span><span class="sxs-lookup"><span data-stu-id="37c18-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="37c18-119">Para mais informações sobre estas políticas, consulte [o que são as políticas do plano base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span><span class="sxs-lookup"><span data-stu-id="37c18-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="37c18-120">Configurar políticas de plano base</span><span class="sxs-lookup"><span data-stu-id="37c18-120">Set up baseline policies</span></span>

1. <span data-ttu-id="37c18-121">Vá para o [Azure portal](https://portal.azure.com)e, em seguida, navegue para o **Active Directory de Azure** \> **Acesso condicional**.</span><span class="sxs-lookup"><span data-stu-id="37c18-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="37c18-122">As políticas do plano base são listadas na página.</span><span class="sxs-lookup"><span data-stu-id="37c18-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="37c18-123">![Página de lista do plano base políticas de acesso condicional.](media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="37c18-123">![Page that lists baseline policies for conditional access.](media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="37c18-124">Consulte as seguintes instruções específicas para cada política:</span><span class="sxs-lookup"><span data-stu-id="37c18-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="37c18-125">Exigir AMF para admins</span><span class="sxs-lookup"><span data-stu-id="37c18-125">Require MFA for admins</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="37c18-126">Reequire AMF para utilizadores</span><span class="sxs-lookup"><span data-stu-id="37c18-126">Reequire MFA for users</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="37c18-127">Autenticação de legado do bloco</span><span class="sxs-lookup"><span data-stu-id="37c18-127">Block legacy authentication</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="37c18-128">Requerer AMF para gestão de serviços</span><span class="sxs-lookup"><span data-stu-id="37c18-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="37c18-129">Pode configurar várias políticas adicionais, como requerer aplicações de cliente aprovado.</span><span class="sxs-lookup"><span data-stu-id="37c18-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="37c18-130">Consulte a [Documentação de acesso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="37c18-130">See the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/) for more information.</span></span>