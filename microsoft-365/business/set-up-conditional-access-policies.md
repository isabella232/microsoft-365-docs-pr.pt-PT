---
title: Criar políticas de acesso condicional para campanhas da Microsoft 365
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
search.appverid:
- BCS160
- MET150
- MOE150
description: Saiba como criar políticas de acesso condicional para as Campanhas Microsoft 365 para adicionar uma segurança adicional substancial.
ms.openlocfilehash: eda65e335df2a7c2c443d7095f7b35b5c1cf27e4
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561226"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="0f8b1-103">Criar políticas de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="0f8b1-103">Set up conditional access policies</span></span>

<span data-ttu-id="0f8b1-104">[As](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) políticas de acesso condicional acrescentam uma segurança adicional substancial.</span><span class="sxs-lookup"><span data-stu-id="0f8b1-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substantial additional security.</span></span> <span data-ttu-id="0f8b1-105">A Microsoft fornece um conjunto de políticas de acesso condicional de base que são recomendadas para todos os clientes.</span><span class="sxs-lookup"><span data-stu-id="0f8b1-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="0f8b1-106">As políticas de base são um conjunto de políticas predefinidas que ajudam a proteger as organizações contra muitos ataques comuns.</span><span class="sxs-lookup"><span data-stu-id="0f8b1-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="0f8b1-107">Estes ataques comuns podem incluir spray de senha, repetição e phishing.</span><span class="sxs-lookup"><span data-stu-id="0f8b1-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="0f8b1-108">Estas políticas exigem que os administradores e utilizadores introduzam uma segunda forma de autenticação (chamada autenticação multifactor, ou MFA) quando determinadas condições são satisfeitas.</span><span class="sxs-lookup"><span data-stu-id="0f8b1-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="0f8b1-109">Por exemplo, se um utilizador estiver a iniciar sessão a partir de um país diferente, o inserido pode ser considerado arriscado e o utilizador deve fornecer uma forma adicional de autenticação.</span><span class="sxs-lookup"><span data-stu-id="0f8b1-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="0f8b1-110">Atualmente, as políticas de base incluem:</span><span class="sxs-lookup"><span data-stu-id="0f8b1-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="0f8b1-111">**Exigir MFA para administradores** &ndash; requer autenticação multi-factor para as funções de administrador mais privilegiada, incluindo administrador global.</span><span class="sxs-lookup"><span data-stu-id="0f8b1-111">**Require MFA for admins** &ndash; Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="0f8b1-112">**A proteção** &ndash; final do utilizador requer a autenticação de vários fatores para os utilizadores apenas quando um inseri-lo é arriscado.</span><span class="sxs-lookup"><span data-stu-id="0f8b1-112">**End user protection** &ndash; Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="0f8b1-113">**Autenticação** &ndash; legado O legado das aplicações de clientes mais antigos e algumas novas aplicações não utilizam protocolos de autenticação mais recentes, mais seguros e seguros.</span><span class="sxs-lookup"><span data-stu-id="0f8b1-113">**Block legacy authentication** &ndash; Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="0f8b1-114">Estas aplicações mais antigas podem contornar as políticas de acesso condicional e obter acesso não autorizado ao seu ambiente.</span><span class="sxs-lookup"><span data-stu-id="0f8b1-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="0f8b1-115">Esta política bloqueia o acesso de clientes que não suportam acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="0f8b1-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="0f8b1-116">**Exigir MFA para gestão** &ndash; de serviçorequer autenticação de vários fatores para o acesso a ferramentas de gestão, incluindo portal Azure (onde configura políticas de base).</span><span class="sxs-lookup"><span data-stu-id="0f8b1-116">**Require MFA for Service Management** &ndash; Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="0f8b1-117">A Microsoft recomenda que ative todas estas políticas de base.</span><span class="sxs-lookup"><span data-stu-id="0f8b1-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="0f8b1-118">Após a ativação destas políticas, os administradores e utilizadores serão solicitados a registar-se para autenticação Azure Multii-Factor.</span><span class="sxs-lookup"><span data-stu-id="0f8b1-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="0f8b1-119">Para obter mais informações sobre estas políticas, veja [quais são as políticas de base?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)</span><span class="sxs-lookup"><span data-stu-id="0f8b1-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="0f8b1-120">Criar políticas de base</span><span class="sxs-lookup"><span data-stu-id="0f8b1-120">Set up baseline policies</span></span>

1. <span data-ttu-id="0f8b1-121">Vá ao [portal Azure,](https://portal.azure.com)e depois navegue até ao **Acesso Condicional**do **Diretório** \> Ativo Azure.</span><span class="sxs-lookup"><span data-stu-id="0f8b1-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="0f8b1-122">As políticas de base estão listadas na página.</span><span class="sxs-lookup"><span data-stu-id="0f8b1-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="0f8b1-123">![Página que lista políticas de base para acesso condicional.](../media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="0f8b1-123">![Page that lists baseline policies for conditional access.](../media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="0f8b1-124">Consulte as seguintes instruções específicas para cada política:</span><span class="sxs-lookup"><span data-stu-id="0f8b1-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="0f8b1-125">Exigir MFA para administradores</span><span class="sxs-lookup"><span data-stu-id="0f8b1-125">Require MFA for admins</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="0f8b1-126">Exigir MFA para utilizadores</span><span class="sxs-lookup"><span data-stu-id="0f8b1-126">Require MFA for users</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="0f8b1-127">Autenticação do legado do bloco</span><span class="sxs-lookup"><span data-stu-id="0f8b1-127">Block legacy authentication</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="0f8b1-128">Exigir MFA para gestão de serviços</span><span class="sxs-lookup"><span data-stu-id="0f8b1-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="0f8b1-129">Pode configurar muitas políticas adicionais, tais como exigir aplicações de clientes aprovadas.</span><span class="sxs-lookup"><span data-stu-id="0f8b1-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="0f8b1-130">Para mais informações, consulte a Documentação de [Acesso Condicional.](https://docs.microsoft.com/azure/active-directory/conditional-access/)</span><span class="sxs-lookup"><span data-stu-id="0f8b1-130">For more information, see the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>
