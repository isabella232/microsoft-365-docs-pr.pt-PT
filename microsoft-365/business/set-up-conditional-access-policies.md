---
title: Configurar políticas de acesso condicional para campanhas microsoft 365
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
description: Saiba como configurar políticas de acesso condicional para as Campanhas Microsoft 365 para adicionar segurança adicional substancial.
ms.openlocfilehash: 58ee760877ee2fd7e53ef9463242657ab66a2b6e
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/01/2020
ms.locfileid: "44470653"
---
# <a name="set-up-conditional-access-policies"></a>Configurar políticas de acesso condicional

Este artigo aplica-se ao Microsoft 365 Business Premium.

[As](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) políticas de acesso condicional adicionam uma segurança adicional substancial. A Microsoft fornece um conjunto de políticas de acesso condicional de base que são recomendadas para todos os clientes. As políticas de base são um conjunto de políticas predefinidas que ajudam a proteger as organizações contra muitos ataques comuns. Estes ataques comuns podem incluir spray de palavra-passe, repetição e phishing.

Estas políticas exigem que os administradores e utilizadores introduzam uma segunda forma de autenticação (chamada autenticação multifactor, ou MFA) quando determinadas condições são satisfeitas. Por exemplo, se um utilizador estiver a iniciar sessão a partir de um país diferente, a inscrição pode ser considerada arriscada e o utilizador deve fornecer uma forma adicional de autenticação. 

Atualmente, as políticas de base incluem o seguinte:
- **Exigir MFA para administradores** &ndash; Requer autenticação multi-factor para as funções de administrador mais privilegiadas, incluindo administrador global.
- Proteção final **do utilizador** &ndash; Requer autenticação multi-factor para os utilizadores apenas quando uma entrada é arriscada. 
- **Bloquear a autenticação do** &ndash; legado As aplicações de clientes mais antigas e algumas novas aplicações não utilizam protocolos de autenticação mais recentes, mais seguros. Estas aplicações mais antigas podem contornar políticas de acesso condicional e obter acesso não autorizado ao seu ambiente. Esta política bloqueia o acesso de clientes que não suportam acesso condicional. 
- **Exigir MFA para gestão de serviços** &ndash; Requer autenticação multi-factor para acesso a ferramentas de gestão, incluindo o portal Azure (onde configura políticas de base). 

A Microsoft recomenda que ative todas estas políticas de base. Após estas políticas estarem ativadas, os administradores e utilizadores serão solicitados a registarem-se para a autenticação do Azure Multii-Factor.

Para obter mais informações sobre estas políticas, veja [o que são políticas de base?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)


## <a name="set-up-baseline-policies"></a>Configurar políticas de base

1. Vá ao [portal Azure](https://portal.azure.com)e, em seguida, navegue para **O Azure Ative Directory** \> **Conditional Access**.
    
    As políticas de base estão listadas na página. <br/> <br/>
    ![Página que lista políticas de base para acesso condicional.](../media/baslinepolicies.png)
1. Consulte as seguintes instruções específicas para cada política:

  - [Exigir MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Exigir MFA para utilizadores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Bloquear a autenticação do legado](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Exigir MFA para gestão de serviços](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Pode configurar muitas políticas adicionais, tais como a necessidade de aplicações de clientes aprovadas. Para mais informações, consulte a [Documentação de Acesso Condicional.](https://docs.microsoft.com/azure/active-directory/conditional-access/)
