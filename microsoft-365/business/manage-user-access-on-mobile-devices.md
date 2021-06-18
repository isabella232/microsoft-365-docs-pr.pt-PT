---
title: Gerir a forma como os utilizadores acedem a documentos do Office em dispositivos móveis
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: Saiba mais sobre as políticas de proteção que lhe permitem gerir a forma como os utilizadores acedem Office aplicações e ficheiros de trabalho a partir de dispositivos móveis.
ms.openlocfilehash: 7602b712f2dfc3ba369fd76979baaaa8d5da5c5c
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/14/2021
ms.locfileid: "52925285"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a>Gerir a forma como os utilizadores acedem a documentos do Office em dispositivos móveis

Este artigo aplica-se a Microsoft 365 Empresas Premium.

Por predefinição, as definições de políticas que controlam a forma como os utilizadores acedem a ficheiros do Office a partir dos seus dispositivos móveis estão definidas como **Desativadas**. Recomendamos que aceite os valores predefinido durante a configuração para criar políticas de aplicações para Android, iOS e Windows 10 que se apliquem a todos os utilizadores. Poderá criar políticas adicionais após a configuração estar concluída. 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Definições que controlam a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis

As seguintes definições estão disponíveis para gerir como os utilizadores acedem a ficheiros de trabalho do Office:

|Definição  <br/> |Descrição  <br/> |
|:-----|:-----|
|Exigir um PIN ou uma impressão digital para aceder às aplicações do Office  <br/> |Se esta definição estiver Ativada, os utilizadores têm de fornecer outra forma de autenticação, além do nome de utilizador e palavra-passe, antes de poderem utilizar aplicações Office nos respetivos dispositivos móveis.  <br/> |
|Repor o PIN quando o início de sessão falha este número de vezes  <br/> |Para impedir um utilizador não autorizado de adivinhar um PIN aleatoriamente, o PIN será reposto após o número de tentativas incorretas que especificar.  <br/> |
|Exigir que o utilizador inicie a sessão novamente após as aplicações do Office estarem inativas durante  <br/> |Esta definição determina durante quanto tempo um utilizador pode estar indisque antes de lhe ser pedido para voltar a entrar.  <br/> |
|Negar o acesso a ficheiros de trabalho em dispositivos desbloqueados por jailbreak ou rooting  <br/> |Alguns utilizadores podem ter um dispositivo desbloqueado através de jailbreak ou rooting. Isto significa que o utilizador pode modificar o sistema operativo, o que pode tornar o dispositivo mais suscetível a software malictivo. Estes dispositivos são bloqueados quando esta definição se encontra **Ativada**.  <br/> |
|Não permitir que os utilizadores copiem conteúdos de aplicações Office para aplicações pessoais  <br/> |Quando a definição está **Adada,** o utilizador não pode copiar informações num ficheiro de trabalho para um ficheiro pessoal. Se a definição estiver **Des desligada,** o utilizador pode copiar informações de um ficheiro de trabalho para uma aplicação pessoal ou conta pessoal.  <br/> |
   

