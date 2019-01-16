---
title: Gerir a forma como os utilizadores acedem a documentos do Office em dispositivos móveis
ms.author: sirkkuw
author: sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: overview
f1_keywords:
- 'O365E_BCSSetup4OfficeMobile '
ms.service: o365-administration
localization_priority: Normal
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
description: Obter informações sobre políticas de protecção que podem ajudar acesso seguro para aplicações do Office a partir de dispositivos móveis.
ms.openlocfilehash: 75dbe79acccabd851c43259a165e79bfe3c509c0
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/16/2019
ms.locfileid: "26983188"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="6874b-103">Gerir a forma como os utilizadores acedem a documentos do Office em dispositivos móveis</span><span class="sxs-lookup"><span data-stu-id="6874b-103">Manage how users access Office documents on mobile devices</span></span>

 <span data-ttu-id="6874b-p101">Por predefinição, as definições de políticas que controlam a forma como os utilizadores acedem a ficheiros do Office a partir dos seus dispositivos móveis estão definidas como **Desativadas**. Recomendamos que aceite os valores predefinidos durante a configuração para criar políticas de aplicações para Android, iOS e Windows 10 que se apliquem a todos os utilizadores. Poderá criar políticas adicionais após a configuração estar concluída.</span><span class="sxs-lookup"><span data-stu-id="6874b-p101">Policy settings that control how users access Office files from their mobile devices are **Off** by default. We recommend you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users. You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="6874b-107">Definições que controlam a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis</span><span class="sxs-lookup"><span data-stu-id="6874b-107">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="6874b-108">As seguintes definições estão disponíveis para gerir como os utilizadores acedem a ficheiros de trabalho do Office:</span><span class="sxs-lookup"><span data-stu-id="6874b-108">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="6874b-109">Definição</span><span class="sxs-lookup"><span data-stu-id="6874b-109">Setting</span></span>  <br/> |<span data-ttu-id="6874b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6874b-110">Description</span></span>  <br/> |
|<span data-ttu-id="6874b-111">Exigir um PIN ou uma impressão digital para aceder às aplicações do Office</span><span class="sxs-lookup"><span data-stu-id="6874b-111">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="6874b-112">Se esta definição se encontrar **Ativada**, os utilizadores terão de fornecer outro meio de autenticação, além do nome de utilizador e da palavra-passe, antes de poderem utilizar aplicações do Office nos respetivos dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="6874b-112">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="6874b-113">Repor o PIN quando o início de sessão falha este número de vezes</span><span class="sxs-lookup"><span data-stu-id="6874b-113">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="6874b-114">Para impedir um utilizador não autorizado de adivinhar um PIN aleatoriamente, o PIN será reposto após o número de tentativas incorretas que especificar.</span><span class="sxs-lookup"><span data-stu-id="6874b-114">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="6874b-115">Exigir que os utilizadores iniciem sessão novamente após as aplicações do Office terem estado inativas durante</span><span class="sxs-lookup"><span data-stu-id="6874b-115">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="6874b-116">Esta definição determina durante quanto tempo um utilizador pode estar inativo antes de ter de voltar a iniciar sessão.</span><span class="sxs-lookup"><span data-stu-id="6874b-116">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="6874b-117">Negar o acesso a ficheiros de trabalho em dispositivos desbloqueados por jailbreak ou rooting</span><span class="sxs-lookup"><span data-stu-id="6874b-117">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="6874b-p102">Alguns utilizadores podem ter um dispositivo desbloqueado através de jailbreak ou rooting. Isto significa que o utilizador pode modificar o sistema operativo, o que pode tornar o dispositivo mais suscetível a software maligno. Estes dispositivos são bloqueados quando esta definição se encontra **Ativada**.  </span><span class="sxs-lookup"><span data-stu-id="6874b-p102">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="6874b-121">Permitir que os utilizadores copiem conteúdos das aplicações do Office para aplicações pessoais</span><span class="sxs-lookup"><span data-stu-id="6874b-121">Allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="6874b-p103">Por predefinição, esta definição não é permitida. No entanto, se a mesma estiver definida como **Ativada**, o utilizador poderá copiar informações de um ficheiro de trabalho para um ficheiro pessoal. Se a definição estiver **Desativada**, o utilizador não pode copiar informações de um ficheiro de trabalho para uma aplicação ou conta pessoal.  </span><span class="sxs-lookup"><span data-stu-id="6874b-p103">We allow this by default, but when the setting is **On**, the user can copy information in a work file to a personal file. If the setting is **Off**, the user can't copy information from a work file to a personal app or personal account.  </span></span><br/> |
   

