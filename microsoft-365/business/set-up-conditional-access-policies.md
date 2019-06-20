---
title: Configurar políticas de acesso condicional para campanhas de Microsoft 365
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
search.appverid:
- BCS160
- MET150
- MOE150
description: Obter informações sobre como configurar políticas de acesso condicional para Microsoft 365 campanhas.
ms.openlocfilehash: 7d8e1f16019d151478aae57b1593b0e0758e5b19
ms.sourcegitcommit: 7e46db0b35c188ee6a7b40ab3eb2d76ff6c101c5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/19/2019
ms.locfileid: "35086391"
---
# <a name="set-up-conditional-access-policies"></a>Configurar políticas de acesso condicional

Políticas de [acesso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) adicionar segurança adicional substancial. A Microsoft fornece um conjunto de políticas de acesso condicional do plano base que são recomendadas para todos os clientes. As políticas do plano base são um conjunto de políticas predefinidas que ajudam a proteger organizações contra muitos ataques comuns. Estes ataques comuns podem incluir pulverização de palavra-passe, de reprodução e de phishing.

Estas políticas requerem admins e os utilizadores introduzam uma segunda forma de autenticação (denominada autenticação multifactor ou AMF) quando forem cumpridas determinadas condições. Por exemplo, se um utilizador é iniciada a sessão de outro país, a inscrição no possa ser considerada perigoso e o utilizador tem de fornecer uma forma adicional de autenticação. 

Actualmente, as políticas do plano base incluem o seguinte:
- **Exigir AMF para admins** — requer autenticação multi-factores para as funções de administrador mais privilegiadas, incluindo o administrador global.
- **Protecção do utilizador final** — requer autenticação multi-factores para os utilizadores apenas quando um início de sessão-in é arriscado. 
- **Autenticação de legado bloco** — aplicações mais antigas do cliente e algumas novas aplicações não utilizam protocolos de autenticação mais seguro, mais recente. Estas aplicações mais antigas, podem ignorar políticas de acesso condicional e obter acesso não autorizado ao seu ambiente. Esta política bloqueia o acesso de clientes que não suportam acesso condicional. 
- **Exigir AMF gestão de serviços de** — requer autenticação multi-factores para aceder a ferramentas de gestão, incluindo Azure portal (onde a configurar políticas de plano base). 

A Microsoft recomenda que activa todas as políticas do plano base. Depois destas políticas forem activadas, administradores e utilizadores serão pedidos para registar para a autenticação de factores Multii Azure.

Para mais informações sobre estas políticas, consulte [o que são as políticas do plano base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?


## <a name="set-up-baseline-policies"></a>Configurar políticas de plano base

1. Vá para o [Azure portal](https://portal.azure.com)e, em seguida, navegue para o **Active Directory de Azure** \> **Acesso condicional**.
    
    As políticas do plano base são listadas na página. <br/> <br/>
    ![Página de lista do plano base políticas de acesso condicional.](media/baslinepolicies.png)
1. Consulte as seguintes instruções específicas para cada política:

  - [Exigir AMF para admins](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Reequire AMF para utilizadores](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Autenticação de legado do bloco](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Requerer AMF para gestão de serviços](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Pode configurar várias políticas adicionais, como requerer aplicações de cliente aprovado. Consulte a [Documentação de acesso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/) para obter mais informações.