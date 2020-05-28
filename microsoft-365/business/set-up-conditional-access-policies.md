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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
description: Saiba como criar políticas de acesso condicional para as Campanhas Microsoft 365 para adicionar uma segurança adicional substancial.
ms.openlocfilehash: d7c9cfee2ef00e4ebe231a28ccca185c10f53c6b
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403024"
---
# <a name="set-up-conditional-access-policies"></a>Criar políticas de acesso condicional

[As](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) políticas de acesso condicional acrescentam uma segurança adicional substancial. A Microsoft fornece um conjunto de políticas de acesso condicional de base que são recomendadas para todos os clientes. As políticas de base são um conjunto de políticas predefinidas que ajudam a proteger as organizações contra muitos ataques comuns. Estes ataques comuns podem incluir spray de senha, repetição e phishing.

Estas políticas exigem que os administradores e utilizadores introduzam uma segunda forma de autenticação (chamada autenticação multifactor, ou MFA) quando determinadas condições são satisfeitas. Por exemplo, se um utilizador estiver a iniciar sessão a partir de um país diferente, o inserido pode ser considerado arriscado e o utilizador deve fornecer uma forma adicional de autenticação. 

Atualmente, as políticas de base incluem:
- **Exigir MFA para administradores** &ndash; Requer a autenticação de vários fatores para as funções de administrador mais privilegiadas, incluindo administrador global.
- Proteção do **utilizador final** &ndash; Requer a autenticação de vários fatores para os utilizadores apenas quando um inserido é arriscado. 
- Autenticação do **legado do bloco** &ndash; Aplicações de clientes mais antigas e algumas novas aplicações não usam protocolos de autenticação mais recentes, mais seguros e seguros. Estas aplicações mais antigas podem contornar as políticas de acesso condicional e obter acesso não autorizado ao seu ambiente. Esta política bloqueia o acesso de clientes que não suportam acesso condicional. 
- **Exigir MFA para gestão de serviços** &ndash; Requer a autenticação de vários fatores para o acesso a ferramentas de gestão, incluindo o portal Azure (onde configura as políticas de base). 

A Microsoft recomenda que ative todas estas políticas de base. Após a ativação destas políticas, os administradores e utilizadores serão solicitados a registar-se para autenticação Azure Multii-Factor.

Para obter mais informações sobre estas políticas, veja [quais são as políticas de base?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)


## <a name="set-up-baseline-policies"></a>Criar políticas de base

1. Vá ao [portal Azure,](https://portal.azure.com)e depois navegue até ao Acesso Condicional do **Diretório Ativo Azure.** \> **Conditional Access**
    
    As políticas de base estão listadas na página. <br/> <br/>
    ![Página que lista políticas de base para acesso condicional.](../media/baslinepolicies.png)
1. Consulte as seguintes instruções específicas para cada política:

  - [Exigir MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Exigir MFA para utilizadores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Autenticação do legado do bloco](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Exigir MFA para gestão de serviços](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Pode configurar muitas políticas adicionais, tais como exigir aplicações de clientes aprovadas. Para mais informações, consulte a Documentação de [Acesso Condicional.](https://docs.microsoft.com/azure/active-directory/conditional-access/)
