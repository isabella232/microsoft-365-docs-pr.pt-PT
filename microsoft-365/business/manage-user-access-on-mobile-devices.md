---
title: Gerir a forma como os utilizadores acedem a documentos do Office em dispositivos móveis
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: aa31319c-9196-48c9-a90b-4057e0494c7a
description: Saiba mais sobre políticas de proteção que podem ajudar a proteger o acesso aos aplicativos do Office a partir de dispositivos móveis.
ms.openlocfilehash: c24dae7e0eea777e728ebead9a2abcc3785763dd
ms.sourcegitcommit: 9a057e70637dcfe06d4f729a96c02be989cf9e25
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/14/2019
ms.locfileid: "38633355"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="11c16-103">Gerir a forma como os utilizadores acedem a documentos do Office em dispositivos móveis</span><span class="sxs-lookup"><span data-stu-id="11c16-103">Manage how users access Office documents on mobile devices</span></span>

 <span data-ttu-id="11c16-104">Por predefinição, as definições de políticas que controlam a forma como os utilizadores acedem a ficheiros do Office a partir dos seus dispositivos móveis estão definidas como **Desativadas**.</span><span class="sxs-lookup"><span data-stu-id="11c16-104">Policy settings that control how users access Office files from their mobile devices are **Off** by default.</span></span> <span data-ttu-id="11c16-105">Recomendamos que você aceite os valores padrão durante a configuração para criar políticas de aplicativos para Android, iOS e Windows 10 que se aplicam a todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="11c16-105">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="11c16-106">Poderá criar políticas adicionais após a configuração estar concluída.</span><span class="sxs-lookup"><span data-stu-id="11c16-106">You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="11c16-107">Definições que controlam a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis</span><span class="sxs-lookup"><span data-stu-id="11c16-107">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="11c16-108">As seguintes definições estão disponíveis para gerir como os utilizadores acedem a ficheiros de trabalho do Office:</span><span class="sxs-lookup"><span data-stu-id="11c16-108">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="11c16-109">Definição</span><span class="sxs-lookup"><span data-stu-id="11c16-109">Setting</span></span>  <br/> |<span data-ttu-id="11c16-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="11c16-110">Description</span></span>  <br/> |
|<span data-ttu-id="11c16-111">Exigir um PIN ou uma impressão digital para aceder às aplicações do Office</span><span class="sxs-lookup"><span data-stu-id="11c16-111">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="11c16-112">Se essa configuração estiver **em campo,** os usuários devem fornecer outra forma de autenticação, além de seu nome de usuário e senha, antes que eles possam usar aplicativos do Office em seu dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="11c16-112">If this setting is **On**, users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="11c16-113">Repor o PIN quando o início de sessão falha este número de vezes</span><span class="sxs-lookup"><span data-stu-id="11c16-113">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="11c16-114">Para impedir um utilizador não autorizado de adivinhar um PIN aleatoriamente, o PIN será reposto após o número de tentativas incorretas que especificar.</span><span class="sxs-lookup"><span data-stu-id="11c16-114">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="11c16-115">Exigir que o utilizador inicie a sessão novamente após as aplicações do Office estarem inativas durante</span><span class="sxs-lookup"><span data-stu-id="11c16-115">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="11c16-116">Essa configuração determina quanto tempo um usuário pode ficar ocioso antes de ser solicitado a entrar novamente.</span><span class="sxs-lookup"><span data-stu-id="11c16-116">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="11c16-117">Negar o acesso a ficheiros de trabalho em dispositivos desbloqueados por jailbreak ou rooting</span><span class="sxs-lookup"><span data-stu-id="11c16-117">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="11c16-118">Alguns utilizadores podem ter um dispositivo desbloqueado através de jailbreak ou rooting.</span><span class="sxs-lookup"><span data-stu-id="11c16-118">Clever users may have a device that is jailbroken or rooted.</span></span> <span data-ttu-id="11c16-119">Isso significa que o usuário pode modificar o sistema operacional, o que pode tornar o dispositivo mais suscetível a malware.</span><span class="sxs-lookup"><span data-stu-id="11c16-119">This means that the user can modify the operating system, which can make the device more susceptible to malware.</span></span> <span data-ttu-id="11c16-120">Estes dispositivos são bloqueados quando esta definição se encontra **Ativada**.</span><span class="sxs-lookup"><span data-stu-id="11c16-120">These devices are blocked when this setting is **On**.</span></span>  <br/> |
|<span data-ttu-id="11c16-121">Não permita que os usuários copiem conteúdo de aplicativos do Office em aplicativos pessoais</span><span class="sxs-lookup"><span data-stu-id="11c16-121">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="11c16-122">Quando a configuração está **on,** o usuário não pode copiar informações em um arquivo de trabalho para um arquivo pessoal.</span><span class="sxs-lookup"><span data-stu-id="11c16-122">When the setting is **On**, the user can't copy information in a work file to a personal file.</span></span> <span data-ttu-id="11c16-123">Se a configuração estiver **desligada,** o usuário poderá copiar informações de um arquivo de trabalho para um aplicativo pessoal ou conta pessoal.</span><span class="sxs-lookup"><span data-stu-id="11c16-123">If the setting is **Off**, the user can copy information from a work file to a personal app or personal account.</span></span>  <br/> |
   

