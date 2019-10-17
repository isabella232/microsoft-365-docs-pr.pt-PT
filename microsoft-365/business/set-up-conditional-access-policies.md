---
title: Configurar políticas de acesso condicional para campanhas do Microsoft 365
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
description: Saiba como configurar políticas de acesso condicional para campanhas do Microsoft 365.
ms.openlocfilehash: 31f3b7f3678671af3b5ca3947dec37041b226fac
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575644"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="24d19-103">Configurar políticas de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="24d19-103">Set up conditional access policies</span></span>

<span data-ttu-id="24d19-104">Políticas de [acesso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) adicionam substancial segurança adicional.</span><span class="sxs-lookup"><span data-stu-id="24d19-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substancial additional security.</span></span> <span data-ttu-id="24d19-105">A Microsoft fornece um conjunto de diretivas de acesso condicional de linha de base que são recomendadas para todos os clientes.</span><span class="sxs-lookup"><span data-stu-id="24d19-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="24d19-106">As diretivas de linha de base são um conjunto de diretivas predefinidas que ajudam a proteger as organizações contra muitos ataques comuns.</span><span class="sxs-lookup"><span data-stu-id="24d19-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="24d19-107">Esses ataques comuns podem incluir spray de senha, repetição e phishing.</span><span class="sxs-lookup"><span data-stu-id="24d19-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="24d19-108">Essas diretivas exigem que os administradores e usuários entrem em uma segunda forma de autenticação (chamada de autenticação multifator ou MFA) quando determinadas condições forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="24d19-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="24d19-109">Por exemplo, se um usuário está entrando em um país diferente, o logon pode ser considerado arriscado e o usuário deve fornecer uma forma adicional de autenticação.</span><span class="sxs-lookup"><span data-stu-id="24d19-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="24d19-110">Atualmente, as diretivas de linha de base incluem o seguinte:</span><span class="sxs-lookup"><span data-stu-id="24d19-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="24d19-111">**Exigir MFA para administradores** — requer autenticação multifator para as funções de administrador mais privilegiadas, incluindo o administrador global.</span><span class="sxs-lookup"><span data-stu-id="24d19-111">**Require MFA for admins** — Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="24d19-112">**Proteção do usuário final** — requer autenticação multifator para usuários somente quando um logon é arriscado.</span><span class="sxs-lookup"><span data-stu-id="24d19-112">**End user protection** — Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="24d19-113">**Bloquear a autenticação herdada** — os aplicativos de cliente mais antigos e alguns novos aplicativos não usam protocolos de autenticação mais novos e mais seguros.</span><span class="sxs-lookup"><span data-stu-id="24d19-113">**Block legacy authentication** — Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="24d19-114">Esses aplicativos mais antigos podem ignorar políticas de acesso condicional e obter acesso não autorizado ao seu ambiente.</span><span class="sxs-lookup"><span data-stu-id="24d19-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="24d19-115">Esta política bloqueia o acesso de clientes que não suportam o acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="24d19-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="24d19-116">**Exigir MFA para gerenciamento de serviços** — requer autenticação multifator para acesso a ferramentas de gerenciamento, incluindo o portal do Azure (onde você configura as diretivas de linha de base).</span><span class="sxs-lookup"><span data-stu-id="24d19-116">**Require MFA for Service Management** — Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="24d19-117">A Microsoft recomenda que você habilite todas essas diretivas de linha de base.</span><span class="sxs-lookup"><span data-stu-id="24d19-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="24d19-118">Depois que essas diretivas estiverem habilitadas, administradores e usuários serão solicitados a se registrar para a autenticação do Azure Multii-factor.</span><span class="sxs-lookup"><span data-stu-id="24d19-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="24d19-119">Para obter mais informações sobre essas diretivas, consulte [o que são diretivas de linha de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span><span class="sxs-lookup"><span data-stu-id="24d19-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="24d19-120">Configurar políticas de linha de base</span><span class="sxs-lookup"><span data-stu-id="24d19-120">Set up baseline policies</span></span>

1. <span data-ttu-id="24d19-121">Vá para o [portal do Azure](https://portal.azure.com)e navegue até o **acesso condicional** **do Azure Active Directory** \> .</span><span class="sxs-lookup"><span data-stu-id="24d19-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="24d19-122">As diretivas de linha de base são listadas na página.</span><span class="sxs-lookup"><span data-stu-id="24d19-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="24d19-123">![Página que lista as diretivas de linha de base para acesso condicional.](media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="24d19-123">![Page that lists baseline policies for conditional access.](media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="24d19-124">Consulte as seguintes instruções específicas para cada política:</span><span class="sxs-lookup"><span data-stu-id="24d19-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="24d19-125">Exigir MFA para administradores</span><span class="sxs-lookup"><span data-stu-id="24d19-125">Require MFA for admins</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="24d19-126">Exigir MFA para usuários</span><span class="sxs-lookup"><span data-stu-id="24d19-126">Require MFA for users</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="24d19-127">Bloquear a autenticação herdada</span><span class="sxs-lookup"><span data-stu-id="24d19-127">Block legacy authentication</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="24d19-128">Exigir MFA para gerenciamento de serviços</span><span class="sxs-lookup"><span data-stu-id="24d19-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="24d19-129">Você pode configurar várias diretivas adicionais, como a necessidade de aplicativos cliente aprovados.</span><span class="sxs-lookup"><span data-stu-id="24d19-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="24d19-130">Consulte a [documentação de acesso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="24d19-130">See the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/) for more information.</span></span>