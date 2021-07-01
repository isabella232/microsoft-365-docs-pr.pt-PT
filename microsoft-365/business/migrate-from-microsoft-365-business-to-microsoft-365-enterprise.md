---
title: Migrar do Microsoft 365 Empresas para o Microsoft 365 E3
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
description: Saiba como mover a sua empresa de Microsoft 365 Empresas Premium para Microsoft 365 E3.
ms.openlocfilehash: 6502d79dbb283db37b00e4fccf89b15ab4291ce5
ms.sourcegitcommit: 48195345b21b409b175d68acdc25d9f2fc4fc5f1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/30/2021
ms.locfileid: "53227625"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Migrar do Microsoft 365 Empresas Premium para o Microsoft 365 E3

Microsoft 365 Empresas Premium tem tudo o que precisa para a sua pequena empresa, combinando as melhores aplicações de produtividade baseadas na nuvem na classe, com uma gestão e segurança simples de dispositivos que permitem que os seus funcionários façam o seu melhor trabalho. No entanto, em alguns casos, poderá ter de migrar a sua subscrição Microsoft 365 Empresas Premium para a Microsoft 365 E3.

Por exemplo, a sua empresa cresceu e precisa de mais de 300 licenças (já agora, parabéns).

A sua empresa também precisa de funcionalidades empresariais, como o Microsoft 365 Apps para Grandes Empresas, Windows 10 Enterprise E3 ou LICENÇAS de Acesso de Cliente para Empresas (CALs).

A atualização é fácil: pode iniciar a atualização [a partir do Centro de administração.](../commerce/subscriptions/upgrade-to-different-plan.md) Todos os seus dados e configuração na sua subscrição atual são mantidos. Não tem de fazer nada para se preparar para a migração e nada a fazer posteriormente, exceto tirar partido das novas funcionalidades.

> [!NOTE]
> Também pode utilizar uma subscrição Microsoft 365 Empresas Premium de até 300 licenças e obter uma subscrição de Microsoft 365 E3 de mais de 300 licenças. No entanto, o Microsoft Defender para Office 365 não está incluído na Microsoft 365 E3. Para uma proteção contínua contra ameaças, deve adicionar mais o Defender Office 365 licenças para que todos os utilizadores no âmbito do seu Defender para Office 365 de segurança sejam licenciados.

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>Diferenças entre Microsoft 365 Empresas Premium e Microsoft 365 Enterprise

Esta tabela mostra as diferenças entre Microsoft 365 Empresas Premium e Microsoft 365 E3.

| Funcionalidade    | Suporte no Microsoft 365 Empresas Premium    | Suporte no Microsoft 365 E3 |
|:-------|:-----|:-----|
| **No local**        | | |
| Windows 10    | Windows 10 Business  |     Windows 10 Enterprise E3|
| Office aplicações*    | [Microsoft 365 Apps para Pequenas e Médias Empresas](#office-365-business)    | Aplicações Microsoft 365 para empresas |
| **Aplicações de produtividade na nuvem**        | | |
| Exchange Online e Outlook    | Limite de armazenamento de 50 GB por caixa de correio e arquivo Exchange Online ilimitado    | Limite de armazenamento de 100 GB por caixa de correio e arquivo Exchange Online ilimitado |
| Teams    | ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    | ![Incluído com Microsoft 365 E3](../media/check-mark.png) |
| OneDrive para Empresas    | 1 limite de armazenamento TB por utilizador    | Ilimitado |
| Yammer, SharePoint Online, Planner, Stream    | ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    | ![Incluído com Microsoft 365 E3](../media/check-mark.png) |
| **Proteção Contra Ameaças**        | | |
| Capacidades de redução da superfície de ataque    | [Ver esta lista](#threat-protection) | Gestão empresarial do isolamento baseado em hardware para Microsoft Edge |
| Defender para Office 365 Plano 1 | ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    | Não incluído, mas pode ser adicionado a |
| **Gestão de identidades**        | | |
| Reposição de palavra-passe self-service para contas híbridas do Azure Active Directory (Azure AD), Autenticação multifatores (MFA) do Azure AD, Acesso Condicional, writeback de palavra-passe para identidades no local|     ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    | ![Incluído com Microsoft 365 E3](../media/check-mark.png) |
| Deteção da Aplicação Cloud, Azure AD Ligação Health    |     | ![Incluído com Microsoft 365 E3](../media/check-mark.png) |
| Azure AD Office 365 aplicações Single Sign-On (SSO): 10 aplicações por utilizador (aplicações Gallery SaaS, como o Salesforce)* | ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    | ![Incluído com Microsoft 365 E3](../media/check-mark.png) |
| Azure AD Premium 1 SSO: sem limite (aplicações no local através do Proxy de Aplicações do Azure AD e de aplicações que não utilizem Self-Service Integração de Aplicações)    |     | ![Incluído com Microsoft 365 E3](../media/check-mark.png) |
| **Gestão de dispositivos e aplicações**        | | |
| Microsoft Intune, Windows Autopilot|     ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    | ![Incluído com Microsoft 365 E3](../media/check-mark.png) |
|VDA (Virtual Desktop Access)    |  |     ![Incluído com Microsoft 365 E3](../media/check-mark.png) |
|Windows Ambiente de Trabalho Virtual (WVD)    | ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png) |     ![Incluído com Microsoft 365 E3](../media/check-mark.png) |
|Ativação do Computador Partilhado (SCA)    | ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png) |     ![Incluído com Microsoft 365 E3](../media/check-mark.png) |
| Pacote de Otimização do Ambiente de Trabalho da Microsoft    | |     ![Incluído com Microsoft 365 E3](../media/check-mark.png) |
| **Proteção de informações**        | | |
| Office 365 Prevenção de Perda de Dados, Plano 1 do Azure Information Protection    | ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    | ![Incluído com Microsoft 365 E3](../media/check-mark.png) |
| Window Information Protection para DLP de ponto final    | ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    | ![Incluído com Microsoft 365 E3](../media/check-mark.png) |
| **Licença de Acesso de Cliente (direitos CAL)**    | | |
| Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Gestão de Direitos)| |         ![Incluído com Microsoft 365 E3](../media/check-mark.png) |
| **Conformidade**        | | |
| Arquivo de e-mail ilimitado    | ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    | ![Incluído com Microsoft 365 E3](../media/check-mark.png) |
| Gestor de Conformidade    | ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    | ![Incluído com Microsoft 365 E3](../media/check-mark.png) |
| Deteção de E-s    | ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    | ![Incluído com Microsoft 365 E3](../media/check-mark.png) |
| Retenção no local e retenção de litígios    | ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    | ![Incluído com Microsoft 365 E3](../media/check-mark.png) |
| Etiquetas de retenção e políticas de retenção de Mensagens de Gestão de Registos (MRM)    | ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    | ![Incluído com Microsoft 365 E3](../media/check-mark.png) |
||||

\* Os utilizadores a quem foi atribuído acesso a aplicações SaaS podem obter acesso ao SSO até 10 aplicações. Os administradores podem configurar o SSO e alterar o acesso de utilizador a diferentes aplicações SaaS, mas o acesso ao SSO só é permitido para 10 aplicações por utilizador de cada vez. Todas Office 365 aplicações únicas são contabiladas como uma única aplicação.

## <a name="migration"></a>Migração

Para migrar, trabalhe com o seu parceiro para mover a sua subscrição e licenças do Microsoft 365 Empresas Premium para uma subscrição de e-Microsoft 365 E3 adequada com as licenças do mesmo.

As secções seguintes descrevem as alterações que precisa de fazer, se tiver alguma, e o que pode fazer após a migração.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Microsoft 365 dados e a configuração da subscrição

Não precisa de fazer alterações à sua subscrição ou dados atuais antes da migração, o que inclui:

- Configuração da subscrição, como nomes de domínio DNS.
- Contas de utilizador e grupo e definições de autenticação, como a autenticação multifatores ou políticas de acesso condicional.
- As configurações do serviço de produtividade e os respetivos dados, como o Teams, caixas de correio Exchange Online, sites do SharePoint Online, pastas OneDrive para Empresas e blocos OneNote notas.

Os seus utilizadores podem agora desfrutar de armazenamento ilimitado nas caixas de Exchange Online correio e pastas OneDrive para Empresas ilimitadas.

Pode começar a utilizar a Deteção de Aplicações na Nuvem, o Azure AD Ligação Health e o SSO para mais de 10 aplicações.

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Proteção contra ameaças

Windows 10 Business inclui estas proteções:

- Imposição da integridade do processo de arranque do sistema operativo
- Imposição da integridade dos componentes operativos confidenciais
- Vulnerabilidade avançada e mitigações de exploração de zero dias
- Proteção de rede baseada na reputação para Microsoft Edge, Internet Explorer e Chrome
- Firewall baseada em Anfitrião
- Mitigações de ransomware
- Isolamento baseado em hardware para Microsoft Edge
- O controlo da aplicação é alimentado pela Equipa de Segurança inteligente Graph
- Controlo do dispositivo (USB)
- Proteção de rede para ameaças baseadas na Web
- Regras de prevenção de intrusões do anfitrião

Windows 10 Enterprise O E3 também inclui a gestão empresarial de isolamento baseado em hardware para Microsoft Edge.

> [!NOTE]
> Os utilizadores migrados para Microsoft 365 E3 precisam de uma licença do Microsoft Defender Office 365 para uma proteção contínua contra ameaças. Certifique-se de que compra mais o Defender Office 365 licenças de utilizador para que todos os utilizadores no âmbito do seu Defender Office 365 de segurança sejam licenciados.

### <a name="device-management-with-intune"></a>Gestão de dispositivos com o Intune

Não precisa de efetuar alterações à sua configuração atual do Intune antes de migrar, que inclui as definições de dispositivos e aplicações e dispositivos inscritos.

### <a name="windows-10"></a>Windows 10

Microsoft 365 Empresas Premium inclui Windows 10 Business, que pode instalar com o Windows AutoPilot. Ao migrar para o Microsoft 365 E3, cada licença de utilizador inclui o Windows 10 Enterprise E3, que também pode instalar com o Windows Autopilot.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>Microsoft 365 Apps para Pequenas e Médias Empresas

O Microsoft 365 Apps para Pequenas e Médias Empresas cliente instalado nos seus dispositivos começará automaticamente a utilizar as funcionalidades do Microsoft 365 Apps para Grandes Empresas. Após a migração, pode agora utilizar:

- Suporte da Política de Grupo
- Comparação de páginas e consultas de uma só vez
- Business Intelligence
