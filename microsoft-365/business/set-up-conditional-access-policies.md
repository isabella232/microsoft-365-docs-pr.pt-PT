---
title: Configurar políticas de acesso condicional para campanhas do Microsoft 365
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
description: Saiba como configurar políticas de acesso condicional para campanhas do Microsoft 365.
ms.openlocfilehash: 31f3b7f3678671af3b5ca3947dec37041b226fac
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575644"
---
# <a name="set-up-conditional-access-policies"></a>Configurar políticas de acesso condicional

Políticas de [acesso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) adicionam substancial segurança adicional. A Microsoft fornece um conjunto de diretivas de acesso condicional de linha de base que são recomendadas para todos os clientes. As diretivas de linha de base são um conjunto de diretivas predefinidas que ajudam a proteger as organizações contra muitos ataques comuns. Esses ataques comuns podem incluir spray de senha, repetição e phishing.

Essas diretivas exigem que os administradores e usuários entrem em uma segunda forma de autenticação (chamada de autenticação multifator ou MFA) quando determinadas condições forem atendidas. Por exemplo, se um usuário está entrando em um país diferente, o logon pode ser considerado arriscado e o usuário deve fornecer uma forma adicional de autenticação. 

Atualmente, as diretivas de linha de base incluem o seguinte:
- **Exigir MFA para administradores** — requer autenticação multifator para as funções de administrador mais privilegiadas, incluindo o administrador global.
- **Proteção do usuário final** — requer autenticação multifator para usuários somente quando um logon é arriscado. 
- **Bloquear a autenticação herdada** — os aplicativos de cliente mais antigos e alguns novos aplicativos não usam protocolos de autenticação mais novos e mais seguros. Esses aplicativos mais antigos podem ignorar políticas de acesso condicional e obter acesso não autorizado ao seu ambiente. Esta política bloqueia o acesso de clientes que não suportam o acesso condicional. 
- **Exigir MFA para gerenciamento de serviços** — requer autenticação multifator para acesso a ferramentas de gerenciamento, incluindo o portal do Azure (onde você configura as diretivas de linha de base). 

A Microsoft recomenda que você habilite todas essas diretivas de linha de base. Depois que essas diretivas estiverem habilitadas, administradores e usuários serão solicitados a se registrar para a autenticação do Azure Multii-factor.

Para obter mais informações sobre essas diretivas, consulte [o que são diretivas de linha de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?


## <a name="set-up-baseline-policies"></a>Configurar políticas de linha de base

1. Vá para o [portal do Azure](https://portal.azure.com)e navegue até o **acesso condicional** **do Azure Active Directory** \> .
    
    As diretivas de linha de base são listadas na página. <br/> <br/>
    ![Página que lista as diretivas de linha de base para acesso condicional.](media/baslinepolicies.png)
1. Consulte as seguintes instruções específicas para cada política:

  - [Exigir MFA para administradores](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Exigir MFA para usuários](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Bloquear a autenticação herdada](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Exigir MFA para gerenciamento de serviços](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Você pode configurar várias diretivas adicionais, como a necessidade de aplicativos cliente aprovados. Consulte a [documentação de acesso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/) para obter mais informações.