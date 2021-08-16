---
title: Aumentar a proteção contra ameaças Microsoft 365 Empresas Premium
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Defina funcionalidades de conformidade para impedir a perda de dados e ajudar a manter as informações confidenciais dos seus clientes e dos seus clientes seguras.
ms.openlocfilehash: ae5e5727db1f372c40aa4468329021525b6dfc8c5ebbf34705184e461df069e5
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53881851"
---
# <a name="set-up-compliance-features"></a>Configurar funcionalidades de conformidade

Os Microsoft 365 Empresas Premium são fornecidos com funcionalidades para proteger os seus dados e dispositivos e ajudá-lo a manter as informações confidenciais dos seus clientes e dos seus clientes seguras.

## <a name="set-up-dlp-features"></a>Configurar funcionalidades DLP

Consulte [Criar uma política DLP a partir](../compliance/create-a-dlp-policy-from-a-template.md) de um modelo para saber como configurar uma política para proteger contra a perda de dados pessoais. 
  
O DLP vem com vários modelos de políticas prontos a utilizar para várias localidades diferentes. Por exemplo, Dados Financeiros da Austrália, Lei de Informações Pessoais do Canadá, Dados Financeiros dos EUA, entre outros. Consulte [O que os modelos de políticas DLP incluem](../compliance/what-the-dlp-policy-templates-include.md) para uma lista completa. Todos estes modelos podem ser ativados de forma semelhante ao exemplo do modelo PII. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Configurar a retenção de e-mail com Arquivo de Exchange Online

 **Arquivo de Exchange Online funcionalidades** de licença ajudam a manter as normas de conformidade e regulamentação ao preservar conteúdos de e-mail para Deteção de Dados Eletrónicos. Também ajuda a reduzir o risco se houver uma ação judicial e fornece uma forma de recuperar dados após uma violação de segurança ou quando necessitar de recuperar itens eliminados. Pode utilizar a retenção de litigações para preservar todos os conteúdos de um utilizador ou utilizar políticas de retenção para personalizar o que pretende preservar.
  
**Retenção de litigações:** Pode preservar todo o conteúdo da caixa de correio, incluindo itens eliminados, colocando toda a caixa de correio de um utilizador em espera de litígios. 
    
Para colocar uma caixa de correio em espera de litigação, no Centro de administração:
    
1. No navegador esquerdo, aceda a **Utilizadores** \> **Ativos.**
    
2. Selecione um utilizador cuja caixa de correio pretende colocar em espera de litigação. No painel de utilizador, **expanda** Definições de correio e, junto a Mais definições, selecionar **Editar Exchange propriedades**.
    
3. Na página da caixa de correio do utilizador, selecionar ** funcionalidades  da caixa de correio ** no navegador esquerdo e, em seguida, selecionar a ligação Ativar em Retenção **de litígios**.
    
4. Na caixa **de diálogo litigação,** pode especificar a duração da retenção de litigações no campo Duração da **litigação.** Deixe o campo em branco se quiser colocar uma posição infinita. Também pode adicionar notas e direcionar o proprietário da caixa de correio para um site poderá ter de explicar mais sobre a retenção de litígios. \>**Guardar**.
    
**Retenção:** Pode ativar políticas de retenção personalizadas, por exemplo, para preservar durante um período de tempo específico ou eliminar conteúdo permanentemente no final do período de retenção. Para saber mais, consulte [o resumo das políticas de retenção.](../compliance/retention.md)

## <a name="set-up-sensitivity-labels"></a>Configurar etiquetas de sensibilidade

As etiquetas de confidencialidade vêm com o Plano 1 do Azure Information Protection (AIP) e ajudam-no a classificar e a proteger opcionalmente os seus documentos e e-mails ao aplicar etiquetas. As etiquetas podem ser aplicadas automaticamente por administradores que definam regras e condições, manualmente pelos utilizadores ou através de uma combinação em que os utilizadores recebem recomendações.

Para configurar etiquetas de Sensibilidade, veja o vídeo Criar e [gerir etiquetas de](../business-video/create-sensitivity-labels.md) sensibilidade.



### <a name="install-the-azure-information-protection-client-manually"></a>Instalar manualmente o cliente do Azure Information Protection

Para instalar manualmente o cliente AIP:

1. **Transfira oAzinfoProtection_UL.exe** centro de [transferências da Microsoft.](https://www.microsoft.com/download/details.aspx?id=53018)
 
2. Pode verificar se a instalação funcionou ao ver um  documento do Word e ao certificar-se de que a opção Confidencialidade está disponível no **separador** Base.
<br/>![Separador Proteção num documento Word.](../media/word-sensitivity.png)

Para obter mais informações, consulte [Instalar o cliente.](/azure/information-protection/infoprotect-tutorial-step3)