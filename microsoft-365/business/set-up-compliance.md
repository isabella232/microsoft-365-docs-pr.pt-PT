---
title: Aumentar a proteção contra ameaças para o Microsoft 365 Business Premium
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
description: Crie funcionalidades de conformidade para evitar a perda de dados e ajude a manter as informações sensíveis dos seus e dos seus clientes seguras.
ms.openlocfilehash: 2c95ad3f36df28af2c68cd11192bcfe92dfe29e3
ms.sourcegitcommit: e56894917d2aae05705c3b9447388d10e2156183
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/03/2020
ms.locfileid: "48841179"
---
# <a name="set-up-compliance-features"></a>Configurar funcionalidades de conformidade

O Microsoft 365 Business Premium vem com funcionalidades para proteger os seus dados e dispositivos e ajudá-lo a manter as informações sensíveis dos seus clientes e dos seus clientes seguras.

## <a name="set-up-dlp-features"></a>Configurar funcionalidades DLP

Consulte [Criar uma política DLP a partir de um modelo](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) para um exemplo sobre como configurar uma política para proteger contra a perda de dados pessoais. 
  
DLP vem com muitos modelos de política prontos a usar para muitos locais diferentes. Por exemplo, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, e assim por diante. Veja [o que os modelos de política do DLP incluem](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) para uma lista completa. Todos estes modelos podem ser ativados semelhantes ao exemplo do modelo PII. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Configurar retenção de e-mail com o Arquivo Online da Bolsa

 As funcionalidades de licença **de arquivamento online de intercâmbio** ajudam a manter os padrões de conformidade e regulamentares, preservando o conteúdo de e-mail para eDiscovery. Também ajuda a reduzir o seu risco se houver um processo judicial, e fornece uma forma de recuperar dados após uma falha de segurança ou quando precisa de recuperar itens eliminados. Pode utilizar o porão de litígios para preservar todo o conteúdo de um utilizador, ou usar políticas de retenção para personalizar o que pretende preservar.
  
**Detenção de litígios:** Pode preservar todos os conteúdos da caixa de correio, incluindo itens eliminados, colocando toda a caixa de correio de um utilizador em porão de litígio. 
    
Para colocar uma caixa de correio em porão de litígio, no centro de administração:
    
1. No navegador esquerdo, vá aos **Users** \> **utilizadores Utilizadores Ativos**.
    
2. Selecione um utilizador cuja caixa de correio pretende colocar em espera de litígio. No painel de utilizador, expanda as **definições de Correio** , e ao lado **de mais definições,** escolha **propriedades de Edit Exchange**.
    
3. Na página da caixa de correio para o utilizador, escolha as funcionalidades da caixa de correio ** na navegação esquerda e, em seguida, escolha o link **Enable** no **porão de Contencioso**.
    
4. Na caixa de diálogo **de detenção de litígios,** pode especificar a duração da duração do litígio no campo de **duração do litígio.** Deixe o campo vazio se quiser colocar um domínio infinito. Também pode adicionar notas e dirigir o proprietário da caixa de correio para um site que poderá ter de explicar mais sobre o porão de litígios. \>**Guardar.**
    
**Retenção:** Pode ativar políticas de retenção personalizadas, por exemplo, para preservar por um determinado período de tempo ou eliminar o conteúdo permanentemente no final do período de retenção. Para saber mais, consulte [a visão geral das políticas de retenção.](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

## <a name="set-up-sensitivity-labels"></a>Configurar rótulos de sensibilidade

As etiquetas de sensibilidade vêm com o Plano 1 de Proteção de Informação (AIP) do Azure, e ajudam-no a classificar e a proteger opcionalmente os seus documentos e e-mails, aplicando etiquetas. As etiquetas podem ser aplicadas automaticamente por administradores que definem regras e condições, manualmente pelos utilizadores, ou através de uma combinação em que os utilizadores recebem recomendações.

Para configurar rótulos de sensibilidade, ver [criar e gerir vídeos de etiquetas de sensibilidade.](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)



### <a name="install-the-azure-information-protection-client-manually"></a>Instale manualmente o cliente Azure Information Protection

Para instalar manualmente o cliente AIP:

1. Descarregue **AzinfoProtection_UL.exe** do [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Pode verificar se a instalação funcionou visualizando um documento Word e certificando-se de que a opção **Sensibilidade** está disponível no **separador 'Casa'.**
<br/>![Aba de proteção num documento do Word.](../media/word-sensitivity.png)

Para mais informações, consulte [instalar o cliente.](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3)
