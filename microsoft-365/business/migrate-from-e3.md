---
title: Migrar para o Microsoft 365 Empresas do Office 365 E3
f1.keywords:
- NOCSH
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
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
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Saiba como mover a sua empresa para Microsoft 365 Empresas Premium do Office 365 E3.
ms.openlocfilehash: 990ca8bdae979f1efb8a60a3460add2953a51892
ms.sourcegitcommit: 68383240ef7a673d5f28e2ecfab9f105bf1d8c8f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/11/2021
ms.locfileid: "52327176"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>Migrar do Office 365 E3 para o Microsoft 365 Empresas Premium

Microsoft 365 Empresas Premium tem tudo o que precisa para a sua pequena empresa, combinando as melhores aplicações de produtividade baseadas na nuvem na classe, com gestão e segurança de dispositivos simples. Se tiver atualmente uma subscrição do Office 365 E3, mas não tiver mais de 300 funcionários, considere mudar para o Microsoft 365 Empresas Premium para ter funcionalidades de segurança adicionais.

A migração é fácil: Primeiro, muda de licenças e todas as suas informações de utilizador e dados na sua subscrição atual são mantidos. Após a migração, terá de configurar as funcionalidades adicionadas às Microsoft 365 Empresas Premium.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>Diferenças entre Office 365 E3 e Microsoft 365 Empresas Premium

Esta tabela mostra as diferenças entre Microsoft 365 Empresas Premium e Office 365 E3.

| Funcionalidade    | Suporte no Microsoft 365 Empresas Premium    | Suporte no Office 365 E3 |
|:-------|:-----|:-----|
| **No local**        | | |
| Office aplicações<sup>1</sup>    | Microsoft 365 Apps para Pequenas e Médias Empresas    | Aplicações Microsoft 365 para empresas |
| **Aplicações de produtividade na nuvem**        | | |
| Exchange Online e Outlook    | Limite de armazenamento de 50 GB por caixa de correio e limite de Arquivo de Exchange Online    | Limite de armazenamento de 100 GB por caixa de correio e limite de Arquivo de Exchange Online |
| Teams    | ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    | ![Incluído com o Office 365 E3](../media/check-mark.png) | 
| OneDrive para Empresas    | 1 limite de armazenamento TB por utilizador    | Ilimitado | 
| Yammer, SharePoint Online, Planner, Stream    | ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    | ![Incluído com o Office 365 E3](../media/check-mark.png) | 
| StaffHub    | ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    | ![Incluído com o Office 365 E3](../media/check-mark.png) |
| **Proteção Contra Ameaças**        | | |
| Defender para Office 365 Plano 1 | ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    | Não incluído, mas pode ser adicionado a |
| **Gestão de identidades**        | | |
| Reposição de palavra-passe self-service para contas híbridas do Azure Active Directory (Azure AD), Autenticação multifatores (MFA) do Azure AD, Acesso Condicional, writeback de palavra-passe para identidades no local|     ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    |  |
| **Gestão de dispositivos e aplicações**        | | |
| Microsoft Intune, Windows AutoPilot|     ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    |  |
| Ativação de computador partilhado|     ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    | ![Incluído com o Office 365 E3](../media/check-mark.png)| 
| Direitos de atualização para Windows 10 Pro das licenças de e-Pro Win 7/8.1|     ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)    ||
| **Proteção de informações**        | | |
|Office 365 Prevenção de Perda de Dados|    ![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)|![Incluído com o Office 365 E3](../media/check-mark.png)|
|Azure Information Protection Plano 1, BitLocker imposição|![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)||
|Azure Information Protection Plano 1, etiquetas de confidencialidade|![Incluído com Microsoft 365 Empresas Premium](../media/check-mark.png)||
|**Licença de Acesso de Cliente (direitos CAL)**|||
|Enterprise CAL Suite (Exchange, SharePoint, Skype)||![Incluído com o Office 365 E3](../media/check-mark.png)|

<sup>1</sup> A Microsoft 365 Empresas Premium das aplicações do Office não inclui a ativação em volume através da Política de Grupo, telemetria de aplicações, controlos de atualização, comparação de páginas de páginas e consultas ou business Intelligence.

## <a name="migration"></a>Migração

Para migrar a sua subscrição, consulte Alterar planos [manualmente](../commerce/subscriptions/change-plans-manually.md) para obter instruções se quiser mover apenas algumas pessoas para Microsoft 365 Empresas Premium. Também pode [atualizar todas](../commerce/subscriptions/upgrade-to-different-plan.md)as pessoas automaticamente ou trabalhar com um parceiro para mover a sua subscrição e licenças do E3 para uma subscrição Microsoft 365 Empresas Premium empresa.
As secções seguintes descrevem as alterações que precisa de fazer, se necessário, e o que pode fazer após a migração.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Office 365 Configuração e dados da subscrição E3
Não precisa de fazer alterações à sua subscrição ou dados atuais antes da migração, o que inclui:

- Configuração da subscrição, como registos DNS e nomes de domínio.
- Contas de utilizador e grupo e definições de autenticação, como a autenticação multifatores ou políticas de acesso condicional.
- As configurações do serviço de produtividade e os respetivos dados, como o Teams, caixas de correio Exchange Online, sites do SharePoint Online, pastas OneDrive para Empresas e blocos OneNote notas.
- Office aplicações serão dimensionadas automaticamente. Office 365 licenciamento moderno irá verificar a atribuição de licenças do utilizador a cada 72 horas e irá converter as Office para a versão que corresponde à subscrição de utilizador.

### <a name="windows-10"></a>Windows 10

Se a Windows ainda não se encontrar na atualização Windows Pro Criador, atualize-os para a [Atualização para Windows Pro Criadores.](upgrade-to-windows-pro-creators-update.md)

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Configurar políticas para proteger dispositivos e ficheiros de utilizador

> [!NOTE]
> Se configurar políticas e dispositivos Office 365 MDM, esses dispositivos serão listados na página Dispositivos no Microsoft 365 de administração.  Todas as políticas que configurar serão mostradas na lista de políticas clássicas no [portal do Intune.](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)

Após ter atribuído licenças à Microsoft 365 Empresas Premium, pode começar a proteger os dispositivos e ficheiros dos utilizadores.

Se atualizou todas as pessoas na sua organização para o Microsoft 365 Empresas Premium, verá o assistente de configuração na home page e poderá seguir o passo Configurar [Microsoft 365 Empresas Premium](set-up.md) nos passos do assistente de configuração para proteger ficheiros e dispositivos móveis.

Também pode concluir estes passos na página Dispositivos:
  
1. No centro de administração, no navegador esquerdo,  aceda a Políticas de \> **Dispositivos.**

2. Na página **Políticas de dispositivos,** selecionar **Adicionar.**

3. No painel **Adicionar política,** dê um nome à política e, em seguida, escolha um Tipo de **política** a partir do painel de pastas.

     Pode configurar políticas de aplicação para proteger ficheiros em dispositivos Android e iPhone, bem como Windows 10, e pode configurar políticas de configuração de dispositivos para dispositivos Windows 10 empresa. Consulte as seguintes ligações para obter detalhes:

  - [Configurar as definições de proteção de aplicações para dispositivos Android ou iOS](app-protection-settings-for-android-and-ios.md)

  - [Configurar as definições de proteção de aplicações para dispositivos Windows 10](protection-settings-for-windows-10-devices.md)

  - [Definir as definições de proteção de dispositivos Windows 10 PCs](protection-settings-for-windows-10-pcs.md)
  
4. Assim que configurar políticas, você e os seus funcionários podem configurar dispositivos:

  - Consulte [Configurar dispositivos Windows para utilizadores Microsoft 365 Empresas Premium passos](set-up-windows-devices.md) para os Windows dispositivos. 

  - Consulte [Configurar dispositivos móveis para Microsoft 365 Empresas Premium para](set-up-mobile-devices.md) os passos para telemóveis e iPhones Android. 
  
### <a name="mailbox-size"></a>Tamanho da Caixa de Correio

Microsoft 365 Empresas Premium um limite de armazenamento de 50 GB à medida que Exchange Online Plano 1. Ao migrar para o Microsoft 365 Empresas Premium, se algum dos seus utilizadores exceder os 50 GB de armazenamento da caixa de correio, recomendamos que designe um Plano 2 do Exchange Online a este utilizador e remova o Plano Exchange Online 1, uma vez que não é exequecível atribuir ambas as informações.

### <a name="threat-protection"></a>Proteção contra ameaças

Após migrar para o Microsoft 365 Empresas Premium, tem o Defender para Office 365. Consulte [o Microsoft Defender para Office 365](../security/office-365-security/defender-for-office-365.md) uma visão geral. Para configurar, consulte Configurar ligações de Cofre , [configurar](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5) [anexos](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)Cofre e configurar o [Anti phishing](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)no Defender para Office 365 .

### <a name="sensitivity-labels"></a>Etiquetas de confidencialidade

Para começar a utilizar etiquetas de sensibilidade, consulte o vídeo Visão geral das [etiquetas](../compliance/sensitivity-labels.md) de sensibilidade e criar e gerir [etiquetas de](../business-video/create-sensitivity-labels.md) sensibilidade.
