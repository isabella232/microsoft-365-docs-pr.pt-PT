---
title: Gerir a forma como os utilizadores acedem a documentos do Office em dispositivos móveis
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4OfficeMobile
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: aa31319c-9196-48c9-a90b-4057e0494c7a
description: Saiba mais sobre políticas de proteção que lhe permitem gerir a forma como os utilizadores acedem a aplicações do Office e trabalham ficheiros a partir de dispositivos móveis.
ms.openlocfilehash: b2b828cf2e201360f12b8fadcb395e72958230f6
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471073"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="cfb1a-103">Gerir a forma como os utilizadores acedem a documentos do Office em dispositivos móveis</span><span class="sxs-lookup"><span data-stu-id="cfb1a-103">Manage how users access Office documents on mobile devices</span></span>

<span data-ttu-id="cfb1a-104">Este artigo aplica-se ao Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="cfb1a-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="cfb1a-105">Por predefinição, as definições de políticas que controlam a forma como os utilizadores acedem a ficheiros do Office a partir dos seus dispositivos móveis estão definidas como **Desativadas**.</span><span class="sxs-lookup"><span data-stu-id="cfb1a-105">Policy settings that control how users access Office files from their mobile devices are **Off** by default.</span></span> <span data-ttu-id="cfb1a-106">Recomendamos que aceite os valores padrão durante a configuração para criar políticas de aplicação para Android, iOS e Windows 10 que se aplicam a todos os utilizadores.</span><span class="sxs-lookup"><span data-stu-id="cfb1a-106">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="cfb1a-107">Poderá criar políticas adicionais após a configuração estar concluída.</span><span class="sxs-lookup"><span data-stu-id="cfb1a-107">You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="cfb1a-108">Definições que controlam a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis</span><span class="sxs-lookup"><span data-stu-id="cfb1a-108">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="cfb1a-109">As seguintes definições estão disponíveis para gerir como os utilizadores acedem a ficheiros de trabalho do Office:</span><span class="sxs-lookup"><span data-stu-id="cfb1a-109">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="cfb1a-110">Definição</span><span class="sxs-lookup"><span data-stu-id="cfb1a-110">Setting</span></span>  <br/> |<span data-ttu-id="cfb1a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfb1a-111">Description</span></span>  <br/> |
|<span data-ttu-id="cfb1a-112">Exigir um PIN ou uma impressão digital para aceder às aplicações do Office</span><span class="sxs-lookup"><span data-stu-id="cfb1a-112">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="cfb1a-113">Se esta definição estiver **on**, os utilizadores devem fornecer outra forma de autenticação, além do seu nome de utilizador e senha, antes de poderem utilizar aplicações do Office no seu dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="cfb1a-113">If this setting is **On**, users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="cfb1a-114">Repor o PIN quando o início de sessão falha este número de vezes</span><span class="sxs-lookup"><span data-stu-id="cfb1a-114">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="cfb1a-115">Para impedir um utilizador não autorizado de adivinhar um PIN aleatoriamente, o PIN será reposto após o número de tentativas incorretas que especificar.</span><span class="sxs-lookup"><span data-stu-id="cfb1a-115">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="cfb1a-116">Exigir que o utilizador inicie a sessão novamente após as aplicações do Office estarem inativas durante</span><span class="sxs-lookup"><span data-stu-id="cfb1a-116">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="cfb1a-117">Esta definição determina quanto tempo um utilizador pode ficar inativo antes de ser solicitado a iniciar novamente o seu sposição.</span><span class="sxs-lookup"><span data-stu-id="cfb1a-117">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="cfb1a-118">Negar o acesso a ficheiros de trabalho em dispositivos desbloqueados por jailbreak ou rooting</span><span class="sxs-lookup"><span data-stu-id="cfb1a-118">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="cfb1a-119">Alguns utilizadores podem ter um dispositivo desbloqueado através de jailbreak ou rooting.</span><span class="sxs-lookup"><span data-stu-id="cfb1a-119">Clever users may have a device that is jailbroken or rooted.</span></span> <span data-ttu-id="cfb1a-120">Isto significa que o utilizador pode modificar o sistema operativo, o que pode tornar o dispositivo mais suscetível a malware.</span><span class="sxs-lookup"><span data-stu-id="cfb1a-120">This means that the user can modify the operating system, which can make the device more susceptible to malware.</span></span> <span data-ttu-id="cfb1a-121">Estes dispositivos são bloqueados quando esta definição se encontra **Ativada**.</span><span class="sxs-lookup"><span data-stu-id="cfb1a-121">These devices are blocked when this setting is **On**.</span></span>  <br/> |
|<span data-ttu-id="cfb1a-122">Não permita que os utilizadores copiem conteúdo de apps do Office em aplicações pessoais</span><span class="sxs-lookup"><span data-stu-id="cfb1a-122">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="cfb1a-123">Quando a definição está **em Funcionamento,** o utilizador não pode copiar informações num ficheiro de trabalho para um ficheiro pessoal.</span><span class="sxs-lookup"><span data-stu-id="cfb1a-123">When the setting is **On**, the user can't copy information in a work file to a personal file.</span></span> <span data-ttu-id="cfb1a-124">Se a definição estiver **desligada,** o utilizador pode copiar informações de um ficheiro de trabalho para uma aplicação pessoal ou conta pessoal.</span><span class="sxs-lookup"><span data-stu-id="cfb1a-124">If the setting is **Off**, the user can copy information from a work file to a personal app or personal account.</span></span>  <br/> |
   

