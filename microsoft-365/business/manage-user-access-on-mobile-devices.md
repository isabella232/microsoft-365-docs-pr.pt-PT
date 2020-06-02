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
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a>Gerir a forma como os utilizadores acedem a documentos do Office em dispositivos móveis

Este artigo aplica-se ao Microsoft 365 Business Premium.

Por predefinição, as definições de políticas que controlam a forma como os utilizadores acedem a ficheiros do Office a partir dos seus dispositivos móveis estão definidas como **Desativadas**. Recomendamos que aceite os valores padrão durante a configuração para criar políticas de aplicação para Android, iOS e Windows 10 que se aplicam a todos os utilizadores. Poderá criar políticas adicionais após a configuração estar concluída. 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Definições que controlam a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis

As seguintes definições estão disponíveis para gerir como os utilizadores acedem a ficheiros de trabalho do Office:
  
|||
|:-----|:-----|
|Definição  <br/> |Descrição  <br/> |
|Exigir um PIN ou uma impressão digital para aceder às aplicações do Office  <br/> |Se esta definição estiver **on**, os utilizadores devem fornecer outra forma de autenticação, além do seu nome de utilizador e senha, antes de poderem utilizar aplicações do Office no seu dispositivo móvel.  <br/> |
|Repor o PIN quando o início de sessão falha este número de vezes  <br/> |Para impedir um utilizador não autorizado de adivinhar um PIN aleatoriamente, o PIN será reposto após o número de tentativas incorretas que especificar.  <br/> |
|Exigir que o utilizador inicie a sessão novamente após as aplicações do Office estarem inativas durante  <br/> |Esta definição determina quanto tempo um utilizador pode ficar inativo antes de ser solicitado a iniciar novamente o seu sposição.  <br/> |
|Negar o acesso a ficheiros de trabalho em dispositivos desbloqueados por jailbreak ou rooting  <br/> |Alguns utilizadores podem ter um dispositivo desbloqueado através de jailbreak ou rooting. Isto significa que o utilizador pode modificar o sistema operativo, o que pode tornar o dispositivo mais suscetível a malware. Estes dispositivos são bloqueados quando esta definição se encontra **Ativada**.  <br/> |
|Não permita que os utilizadores copiem conteúdo de apps do Office em aplicações pessoais  <br/> |Quando a definição está **em Funcionamento,** o utilizador não pode copiar informações num ficheiro de trabalho para um ficheiro pessoal. Se a definição estiver **desligada,** o utilizador pode copiar informações de um ficheiro de trabalho para uma aplicação pessoal ou conta pessoal.  <br/> |
   

