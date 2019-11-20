---
title: Criar políticas de acesso condicional para as campanhas da Microsoft 365
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
description: Saiba como configurar políticas de acesso condicional para as campanhas Microsoft 365.
ms.openlocfilehash: aebdb733c2dd9a05947335ad4f151104d801568e
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/19/2019
ms.locfileid: "38718835"
---
# <a name="set-up-conditional-access-policies"></a>Criar políticas de acesso condicional

[As](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) políticas de acesso condicional adicionam segurança adicional substancial. A Microsoft fornece um conjunto de políticas de acesso condicional de base que são recomendadas para todos os clientes. As políticas de base são um conjunto de políticas predefinidas que ajudam a proteger as organizações contra muitos ataques comuns. Esses ataques comuns podem incluir spray de senha, repetição e phishing.

Essas políticas exigem que os administradores e usuários insiram uma segunda forma de autenticação (chamada autenticação multifator, ou MFA) quando determinadas condições forem atendidas. Por exemplo, se um usuário estiver se inscrevendo de um país diferente, o login pode ser considerado arriscado e o usuário deve fornecer uma forma adicional de autenticação. 

Atualmente, as políticas de base incluem o seguinte:
- **Exigir mfa para administradores** &ndash; requer multi-fator de autenticação para as funções de administrador mais privilegiados, incluindo administrador global.
- **A proteção** &ndash; do usuário final requer autenticação multifator para usuários somente quando um login é arriscado. 
- **Bloqueie aplicativos legados** &ndash; de autenticação de clientes mais antigos e alguns novos aplicativos não usam protocolos de autenticação mais novos e mais seguros. Esses aplicativos mais antigos podem ignorar as políticas de acesso condicional e obter acesso não autorizado ao seu ambiente. Esta política bloqueia o acesso de clientes que não suportam o acesso condicional. 
- **Exigir o MFA para gerenciamento** &ndash; de serviços requer autenticação multifator para acesso a ferramentas de gerenciamento, incluindo o portal Azure (onde você configura as políticas de base). 

A Microsoft recomenda que você habilite todas essas políticas básicas. Depois que essas políticas forem ativadas, os administradores e os usuários serão solicitados a se cadastrar na autenticação do Azure Multii-Factor.

Para obter mais informações sobre essas políticas, veja quais são as políticas de [base?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)


## <a name="set-up-baseline-policies"></a>Criar políticas de base

1. Vá para o [portal Azure](https://portal.azure.com)e, em seguida, navegue para o **Azure Active Directory** \> **Conditional Access**.
    
    As políticas básicas estão listadas na página. <br/> <br/>
    ![Página que lista as políticas básicas para acesso condicional.](media/baslinepolicies.png)
1. Veja as seguintes instruções específicas para cada política:

  - [Exigir MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Exigir MFA para usuários](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Bloquear a autenticação herdada](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Exigir MFA para gestão de serviços](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Você pode configurar muitas políticas adicionais, como a exigência de aplicativos de clientes aprovados. Para mais informações, consulte a Documentação de [Acesso Condicional.](https://docs.microsoft.com/azure/active-directory/conditional-access/)
