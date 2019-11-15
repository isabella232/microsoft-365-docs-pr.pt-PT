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
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a>Gerir a forma como os utilizadores acedem a documentos do Office em dispositivos móveis

 Por predefinição, as definições de políticas que controlam a forma como os utilizadores acedem a ficheiros do Office a partir dos seus dispositivos móveis estão definidas como **Desativadas**. Recomendamos que você aceite os valores padrão durante a configuração para criar políticas de aplicativos para Android, iOS e Windows 10 que se aplicam a todos os usuários. Poderá criar políticas adicionais após a configuração estar concluída. 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Definições que controlam a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis

As seguintes definições estão disponíveis para gerir como os utilizadores acedem a ficheiros de trabalho do Office:
  
|||
|:-----|:-----|
|Definição  <br/> |Descrição  <br/> |
|Exigir um PIN ou uma impressão digital para aceder às aplicações do Office  <br/> |Se essa configuração estiver **em campo,** os usuários devem fornecer outra forma de autenticação, além de seu nome de usuário e senha, antes que eles possam usar aplicativos do Office em seu dispositivo móvel.  <br/> |
|Repor o PIN quando o início de sessão falha este número de vezes  <br/> |Para impedir um utilizador não autorizado de adivinhar um PIN aleatoriamente, o PIN será reposto após o número de tentativas incorretas que especificar.  <br/> |
|Exigir que o utilizador inicie a sessão novamente após as aplicações do Office estarem inativas durante  <br/> |Essa configuração determina quanto tempo um usuário pode ficar ocioso antes de ser solicitado a entrar novamente.  <br/> |
|Negar o acesso a ficheiros de trabalho em dispositivos desbloqueados por jailbreak ou rooting  <br/> |Alguns utilizadores podem ter um dispositivo desbloqueado através de jailbreak ou rooting. Isso significa que o usuário pode modificar o sistema operacional, o que pode tornar o dispositivo mais suscetível a malware. Estes dispositivos são bloqueados quando esta definição se encontra **Ativada**.  <br/> |
|Não permita que os usuários copiem conteúdo de aplicativos do Office em aplicativos pessoais  <br/> |Quando a configuração está **on,** o usuário não pode copiar informações em um arquivo de trabalho para um arquivo pessoal. Se a configuração estiver **desligada,** o usuário poderá copiar informações de um arquivo de trabalho para um aplicativo pessoal ou conta pessoal.  <br/> |
   

