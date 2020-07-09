---
title: Migrar do Microsoft 365 Business para o Microsoft 365 E3
f1.keywords:
- NOCSH
ms.author: josephd
author: JoeDavies-MSFT
manager: laurawi
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Saiba como mover o seu negócio de Microsoft 365 Business Premium para o Microsoft 365 E3.
ms.openlocfilehash: 6a795d96ccae7e054e7e52d4fd60a4e73b3c71dd
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/27/2020
ms.locfileid: "45081871"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Migrar do Microsoft 365 Business Premium para o Microsoft 365 E3

O Microsoft 365 Business Premium tem tudo o que precisa para o seu pequeno negócio, combinando as melhores aplicações de produtividade baseadas na nuvem com uma simples gestão e segurança de dispositivos que permitem aos seus colaboradores fazer o seu melhor trabalho. Em alguns casos, no entanto, poderá ter de migrar a sua subscrição Microsoft 365 Business Premium para o Microsoft 365 E3. 

Por exemplo, o seu negócio cresceu e precisa de mais de 300 licenças (parabéns, a propósito).

Ou, o seu negócio precisa de funcionalidades empresariais, como aplicações microsoft 365 para empresas, Windows 10 Enterprise E3 ou Licenças de Acesso a Clientes Empresariais (CALs).

A atualização é fácil: pode iniciar a atualização [a partir do centro de administração.](../commerce/subscriptions/upgrade-to-different-plan.md) Todos os seus dados e configuração na sua subscrição atual são mantidos. Não há nada que possa fazer para se preparar para a migração e nada para fazer depois, a não ser aproveitar as novas funcionalidades.

>[!Note]
>Também pode utilizar uma subscrição Microsoft 365 Business Premium para até 300 lugares e obter uma subscrição Microsoft 365 E3 para mais de 300 lugares. No entanto, o Office 365 ATP não está incluído no Microsoft 365 E3. Para uma proteção contínua de ameaças, deve adicionar licenças ATP adicionais do Office 365 para que todos os utilizadores no âmbito do seu Office 365 polícias ATP sejam licenciados.
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>Diferenças entre o Microsoft 365 Business Premium e a Microsoft 365 Enterprise

Esta tabela mostra as diferenças entre o Microsoft 365 Business Premium e o Microsoft 365 E3.

| Funcionalidade    | Suporte no Microsoft 365 Business Premium    | Suporte na Microsoft 365 E3 | 
|:-------|:-----|:-----|
| **No local**        | | | 
| Windows 10    | Negócios windows 10  |     Windows 10 Enterprise E3| 
| Aplicativos de escritório*    | [Microsoft 365 Apps para negócios](#office-365-business)    | Microsoft 365 Apps para empresa | 
| **Aplicativos de produtividade em nuvem**        | | | 
| Troca online e outlook    | Limite de armazenamento de 50 GB por caixa de correio e arquivamento ilimitado da Exchange Online    | Limite de armazenamento de 100 GB por caixa de correio e arquivamento ilimitado da Exchange Online | 
| Equipas    | ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | ![Incluído com Microsoft 365 E3](../media/check-mark.png) | 
| OneDrive para Empresas    | 1 Limite de armazenamento de TB por utilizador    | Ilimitado | 
| Yammer, SharePoint Online, Planner, Stream    | ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | ![Incluído com Microsoft 365 E3](../media/check-mark.png) | 
| Outlook Customer Manager, MileIQ    | ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| **Proteção contra ameaças**        | | | 
| Capacidades de redução de superfície de ataque    | [Consulte esta lista](#threat-protection) | Gestão empresarial do isolamento baseado em hardware para o Microsoft Edge | 
| Office 365 Advanced Threat Protection (ATP) Plano 1 | ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | Não incluído, mas pode ser adicionado em | 
| **Gestão de identidades**        | | | 
| Autosserviço de autosserviço reset para contas híbridas Azure Ative Directory (Azure AD), autenticação multi-factor Azure (MFA), Acesso Condicional, writeback de palavra-passe para identidades no local|     ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | ![Incluído com Microsoft 365 E3](../media/check-mark.png) | 
| Cloud App Discovery, Azure AD Connect Health    |     | ![Incluído com Microsoft 365 E3](../media/check-mark.png) | 
| Azure AD Office 365 apps Single Sign-On (SSO): 10 apps por utilizador (apps Da Gallery SaaS como Salesforce)* | ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | ![Incluído com Microsoft 365 E3](../media/check-mark.png) | 
| Azure AD Premium 1 SSO: sem limite (aplicações no local através de aplicações AZure AD Application Proxy e aplicações não-galeria usando modelos de integração de aplicativos de self-service)    |     | ![Incluído com Microsoft 365 E3](../media/check-mark.png) | 
| **Gestão de dispositivos e aplicativos**        | | | 
| Microsoft Intune, Windows Autopilot|     ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | ![Incluído com Microsoft 365 E3](../media/check-mark.png) | 
|Acesso virtual ao ambiente de trabalho (VDA)    |  |     ![Incluído com Microsoft 365 E3](../media/check-mark.png) | 
|Windows Virtual Desktop (WVD)    | ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png) |     ![Incluído com Microsoft 365 E3](../media/check-mark.png) | 
|Ativação partilhada do computador (SCA)    | ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png) |     ![Incluído com Microsoft 365 E3](../media/check-mark.png) | 
| Pacote de otimização do ambiente de trabalho da Microsoft    | |     ![Incluído com Microsoft 365 E3](../media/check-mark.png) | 
| **Proteção da informação**        | | | 
| Office 365 Data Loss Prevention, Plano de Proteção de Informação Azure 1    | ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | ![Incluído com Microsoft 365 E3](../media/check-mark.png) | 
| Proteção de informação de janela para dLP de ponto final    | ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | ![Incluído com Microsoft 365 E3](../media/check-mark.png) | 
| **Licença de Acesso ao Cliente (direitos CAL)**    | | |     
| Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)| |         ![Incluído com Microsoft 365 E3](../media/check-mark.png) | 
| **Conformidade**        | | | 
| Arquivo ilimitado de e-mails    | ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | ![Incluído com Microsoft 365 E3](../media/check-mark.png) | 
| Compliance Score/Compliance Manager    | ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | ![Incluído com Microsoft 365 E3](../media/check-mark.png) | 
| eDiscovery    | ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | ![Incluído com Microsoft 365 E3](../media/check-mark.png) | 
| Em espera e contencioso    | ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | ![Incluído com Microsoft 365 E3](../media/check-mark.png) | 
| Etiquetas de retenção de registos de mensagens (MRM) e políticas de retenção    | ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | ![Incluído com Microsoft 365 E3](../media/check-mark.png) | 
||||

\*Os utilizadores que tenham sido atribuídos a acesso a aplicações SaaS podem ter acesso SSO a até 10 aplicações. Os administradores podem configurar o SSO e alterar o acesso dos utilizadores a diferentes aplicações SaaS, mas o acesso SSO só é permitido para 10 aplicações por utilizador de cada vez. Todas as aplicações do Office 365 são contadas como uma única aplicação.

## <a name="migration"></a>Migração

Para migrar, trabalhe com o seu parceiro para mover a subscrição microsoft 365 Business Premium e licenças para uma subscrição adequada do Microsoft 365 E3 com as suas licenças.

As seguintes secções descrevem as mudanças que precisa de fazer, se houver, e o que pode fazer após a migração.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Configuração e dados de subscrição microsoft 365

Não precisa de fazer alterações na sua subscrição ou dados atuais antes de migrar, o que inclui:

- Configuração de subscrição, como nomes de domínio DNS.
- Contas de utilizador e grupo e configurações de autenticação, tais como a autenticação de vários fatores ou políticas de acesso condicional.
- Configurações de serviço de produtividade e seus dados, tais como Equipas, Caixas de correio Exchange Online, sites SharePoint Online, OneDrive para pastas de negócios e cadernos OneNote.

Os seus utilizadores podem agora usufruir de armazenamento ilimitado nas caixas de correio Exchange Online e No OneDrive para pastas Business.

Pode começar a usar cloud App Discovery, Azure AD Connect Health e SSO para mais de 10 aplicações.

>[!Note]
>Os utilizadores migrados para o Microsoft 365 E3 já não podem utilizar o Outlook Customer Manager e o MileIQ.
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Proteção contra ameaças

O Windows 10 Business inclui estas proteções:

- Aplicação da integridade do processo de arranque do sistema operativo
- Aplicação da integridade de componentes operacionais sensíveis
- Vulnerabilidade avançada e mitigação de exploração de zero dias
- Proteção de rede baseada na reputação para Microsoft Edge, Internet Explorer e Chrome
- Firewall baseada em hospedeiro
- Mitigações do ransomware
- Isolamento baseado em hardware para o Microsoft Edge
- Controlo de aplicações alimentado pelo Gráfico de Segurança Inteligente
- Controlo do dispositivo (USB)
- Proteção da rede para ameaças baseadas na Web
- Regras de prevenção de intrusões de hospedeiro

O Windows 10 Enterprise E3 também inclui a gestão empresarial do isolamento baseado em hardware para o Microsoft Edge.

>[!Note]
>Os utilizadores migrados para o Microsoft 365 E3 precisarão cada um de uma licença ATP do Office 365 para uma proteção contínua de ameaças. Certifique-se de comprar licenças ATP adicionais do Office 365 para que todos os utilizadores no âmbito do seu Office 365 polícias ATP sejam licenciados. 
>

### <a name="device-management-with-intune"></a>Gestão de dispositivos com Intune

Não precisa de fazer alterações na sua configuração atual do Intune antes de migrar, que inclui dispositivos matriculados e configurações de dispositivos e aplicações.

### <a name="windows-10"></a>Windows 10

O Microsoft 365 Business Premium inclui o Windows 10 Business, que pode instalar com o Windows AutoPilot. Quando migra para o Microsoft 365 E3, cada licença de utilizador inclui o Windows 10 Enterprise E3, que também pode instalar com o Windows Autopilot.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>Microsoft 365 Apps para negócios

As aplicações microsoft 365 para clientes empresariais instaladas nos seus dispositivos começarão automaticamente a utilizar as funcionalidades das Aplicações Microsoft 365 para empresas. Após a migração, pode agora utilizar:

 - Ativação de volume através da Política de Grupo
 - Telemetria de aplicações
 - Atualização de controlos
 - Folha de cálculo compara e inquiri
 - Inteligência empresarial

