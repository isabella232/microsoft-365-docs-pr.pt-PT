---
title: Migrar para o Microsoft 365 Business a partir do Office 365 E3
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
description: Saiba como mover o seu negócio para o Microsoft 365 Business Premium do Office 365 E3.
ms.openlocfilehash: d72f0c52a745ff973868b6fdaa95efa1a37a3dbd
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/18/2020
ms.locfileid: "45081880"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>Migrando do Office 365 E3 para o Microsoft 365 Business Premium 

O Microsoft 365 Business Premium tem tudo o que precisa para o seu pequeno negócio, combinando as melhores aplicações de produtividade baseadas na nuvem com uma simples gestão e segurança de dispositivos. Se atualmente tem uma subscrição do Office 365 E3, mas não tem mais de 300 funcionários, considere mudar para o Microsoft 365 Business Premium para funcionalidades de segurança adicionais.

Migrar é fácil: Primeiro, troca licenças e mantém-se todos os seus dados e informações do utilizador na sua subscrição atual. Após a migração, terá de configurar as funcionalidades que são adicionadas no Microsoft 365 Business Premium.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>Diferenças entre o Office 365 E3 e o Microsoft 365 Business Premium

Esta tabela mostra as diferenças entre o Microsoft 365 Business Premium e o Office 365 E3.

| Funcionalidade    | Suporte no Microsoft 365 Business Premium    | Apoio no Office 365 E3 | 
|:-------|:-----|:-----|
| **No local**        | | | 
| Aplicativos de escritório<sup>1</sup>    | Microsoft 365 Apps para negócios    | Microsoft 365 Apps para empresa | 
| **Aplicativos de produtividade em nuvem**        | | | 
| Troca online e outlook    | Limite de armazenamento de 50 GB por caixa de correio e arquivamento online ilimitado de trocas    | Limite de armazenamento de 100 GB por caixa de correio e arquivamento online ilimitado de trocas | 
| Equipas    | ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | ![Incluído com Office 365 E3](../media/check-mark.png) | 
| OneDrive para Empresas    | 1 Limite de armazenamento de TB por utilizador    | Ilimitado | 
| Yammer, SharePoint Online, Planner, Stream    | ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | ![Incluído com Office 365 E3](../media/check-mark.png) | 
| StaffHub    | ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | ![Incluído com Office 365 E3](../media/check-mark.png) | 
| Outlook Customer Manager, MileIQ    | ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| **Proteção contra ameaças**        | | | 
| Office 365 Advanced Threat Protection (ATP) Plano 1 | ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | Não incluído, mas pode ser adicionado em | 
| **Gestão de identidades**        | | | 
| Autosserviço de autosserviço reset para contas híbridas Azure Ative Directory (Azure AD), autenticação multi-factor Azure (MFA), Acesso Condicional, writeback de palavra-passe para identidades no local|     ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    |  | 
| **Gestão de dispositivos e aplicativos**        | | |
| Microsoft Intune, Windows AutoPilot|     ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| Ativação partilhada do computador|     ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    | ![Incluído com Office 365 E3](../media/check-mark.png)| 
| Direitos de upgrade para o Windows 10 Pro a partir de licenças Win 7/8.1 Pro|     ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)    || 
| **Proteção da informação**        | | |
|Gabinete 365 Prevenção de Perdas de Dados|    ![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)|![Incluído com Office 365 E3](../media/check-mark.png)|
|Plano de Proteção de Informação Azure 1, aplicação bitlocker|![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)||
|Plano de Proteção de Informação Azure 1, Etiquetas de sensibilidade|![Incluído com Microsoft 365 Business Premium](../media/check-mark.png)||
|**Licença de Acesso ao Cliente (direitos CAL)**|||
|Suíte Enterprise CAL (Bolsa, SharePoint, Skype)||![Incluído com Office 365 E3](../media/check-mark.png)|

<sup>1</sup> A versão Microsoft 365 Business Premium das aplicações office não inclui a ativação de volume através da Política de Grupo, telemetria de aplicações, controlos de atualização, comparação e consulta da folha de cálculo, ou Business Intelligence.

## <a name="migration"></a>Migração

Para migrar a sua subscrição, consulte [os planos change manualmente](../commerce/subscriptions/change-plans-manually.md) para obter instruções se quiser mover apenas algumas pessoas para o Microsoft 365 Business Premium. Também pode [atualizar todos automaticamente,](../commerce/subscriptions/upgrade-to-different-plan.md)ou trabalhar com um parceiro para mover a subscrição e licenças E3 para uma subscrição Do Microsoft 365 Business Premium.
As secções seguintes descrevem as alterações que precisa de fazer, se houver, e o que pode fazer após a migração.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Configuração e dados de subscrição do Office 365 E3
Não precisa de fazer alterações na sua subscrição ou dados atuais antes de migrar, o que inclui:

- Configuração de subscrição, como registos DNS e nomes de domínio.
- Contas de utilizador e grupo e configurações de autenticação, tais como a autenticação de vários fatores ou políticas de acesso condicional.
- Configurações de serviço de produtividade e seus dados, tais como Equipas, Caixas de correio Exchange Online, sites SharePoint Online, OneDrive para pastas de negócios e cadernos OneNote.
- As aplicações do office serão reduzidas automaticamente. O licenciamento moderno do Office 365 verificará a atribuição da licença do utilizador a cada 72 horas e converterá as aplicações do Office para a versão que corresponde à subscrição do utilizador.

### <a name="windows-10"></a>Windows 10

Se o Windows ainda não estiver na atualização do Windows Pro Creator, [atualize-os para a Atualização de Criadores do Windows Pro](upgrade-to-windows-pro-creators-update.md).

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Configurar políticas para proteger dispositivos e ficheiros dos utilizadores

> [!NOTE]
> Se configurar as políticas e dispositivos do Office 365 MDM, esses dispositivos serão listados na página **de Dispositivos** no centro de administração microsoft 365. Quaisquer políticas que tenha configurado aparecerão na lista de políticas clássicas no [portal Intune.](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)

Depois de ter atribuído licenças ao Microsoft 365 Business Premium, pode começar a proteger os dispositivos e ficheiros dos utilizadores.

Se atualizar todos na sua organização para o Microsoft 365 Business Premium, verá o assistente de configuração na página Inicial e poderá seguir o [Microsoft 365 Business Premium nas](set-up.md) etapas do assistente de configuração para proteger ficheiros e dispositivos móveis.

Também pode completar estes passos na página dispositivos:
  
1. No centro de administração, na navegação à esquerda, vá às Políticas **de Dispositivos.** \> **Policies**
    
2. Na página de políticas do **Dispositivo,** escolha **Adicionar**.
    
3. No painel **de política Add** dê um nome à política e, em seguida, escolha um tipo de **Política** a partir do drop-down. 
    
     Pode configurar políticas de aplicações para proteger ficheiros em dispositivos Android e iPhone, bem como windows 10, e pode configurar políticas de configuração de dispositivos para dispositivos do Windows 10 da empresa. Consulte os seguintes links para mais detalhes:
    
  - [Configurar as definições de proteção de aplicações para dispositivos Android ou iOS](app-protection-settings-for-android-and-ios.md)
    
  - [Configurar as definições de proteção de aplicações para dispositivos Windows 10](protection-settings-for-windows-10-devices.md)
    
  - [Definir definições de proteção do dispositivo para PCs do Windows 10](protection-settings-for-windows-10-pcs.md)
  
4. Assim que definir políticas, você e os seus colaboradores podem configurar dispositivos:
    
  - Consulte [configurar dispositivos Windows para utilizadores Do Microsoft 365 Business Premium](set-up-windows-devices.md) para etapas para dispositivos Windows. 
    
  - Consulte [configurar dispositivos móveis para utilizadores Do Microsoft 365 Business Premium](set-up-mobile-devices.md) para passos para telemóveis e iPhones Android. 

### <a name="threat-protection"></a>Proteção contra ameaças

Depois de migrar para o Microsoft 365 Business Premium, tem o Office 365 ATP. Consulte [o Office 365 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) para uma visão geral. Para configurar, consulte [configurar links de segurança ATP,](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa) [configurar anexos seguros ATP](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)e [configurar anti-phishing ATP](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).

### <a name="sensitivity-labels"></a>Etiquetas de confidencialidade

Para começar a utilizar rótulos de sensibilidade, consulte [a visão geral dos rótulos de sensibilidade](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) e crie e gere vídeos de [etiquetas de sensibilidade.](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)
