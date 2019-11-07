---
title: Aumentar a proteção contra ameaças para o Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
description: Configure recursos de conformidade para evitar a perda de dados e rotular dados confidenciais.
ms.openlocfilehash: 5213c55f4a8ce0e223896f1b960847714d6d06cb
ms.sourcegitcommit: 70e920f76526f47fc849df615de4569e0ac2f4be
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/07/2019
ms.locfileid: "38031421"
---
# <a name="set-up-compliance-features"></a>Configurar recursos de conformidade

Seu Microsoft 365 Business vem com recursos para proteger seus dados e dispositivos e ajudá-lo a manter as informações confidenciais dos seus clientes seguras.

## <a name="set-up-dlp-features"></a>Configurar recursos de DLP

Veja [criar uma política de DLP a partir de um modelo](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) para um exemplo sobre como criar uma política para proteger contra informações de identificação pessoal (PII). 
  
DLP vem com muitos modelos de política pronto-a-uso para muitos locais diferentes. Por exemplo, dados financeiros da Austrália, Canada Personal Information Act, Dados Financeiros dos EUA, etc. Veja [o que os modelos](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) de política do DLP incluem para uma lista completa. Todos esses modelos podem ser habilitados semelhante sagaz. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Configure retenção de e-mail com arquivamento on-line de intercâmbio

 Os recursos da licença **de arquivamento on-line** de intercâmbio ajudam a manter os padrões regulatórios e de conformidade, preservando o conteúdo de e-mail para o eDiscovery. Ele também ajuda a reduzir o risco em caso de uma ação judicial e fornece uma maneira de recuperar dados após uma violação de segurança, ou quando você precisa recuperar itens excluídos. Você pode usar o litígio para preservar todo o conteúdo de um usuário ou usar políticas de retenção para personalizar o que deseja preservar.
  
**Contenção:** Você pode preservar todo o conteúdo da caixa de correio, incluindo itens excluídos, colocando toda a caixa de correio de um usuário no porão de litígio. 
    
Para colocar uma caixa de correio em espera contencioso, no centro de administração:
    
1. No nav esquerdo, vá para **usuários** \> **ativos.**
    
2. Selecione um usuário cuja caixa de correio que você deseja colocar em espera de litígio e no painel do usuário expanda **as configurações** do Mail e, ao lado de **mais configurações,** escolha **as propriedades da Edit Exchange.**
    
3. Na página da caixa de correio para o usuário, escolha os recursos de caixa de correio ** ** na navegação esquerda e, em seguida, escolha o link **Habilitar** a **retenção de Litígio.**
    
4. No **litígio mantenha** a caixa de diálogo, você pode especificar a duração do litígio no campo de duração de **retenção de litígios,** deixar o campo vazio se você quiser colocar um porão infinito. Você também pode adicionar notas e direcionar o proprietário da caixa de \> correio para um site que você pode ter que explicar mais sobre o litígio hold **Save**.
    
**Retenção:** Você pode habilitar políticas de retenção personalizadas, por exemplo, preservar por um período de tempo específico ou excluir conteúdo permanentemente no final do período de retenção. Para saber mais, veja [a visão geral das políticas de retenção.](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423)

## <a name="set-up-sensitivity-labels"></a>Criar rótulos de sensibilidade

Os rótulos de sensibilidade vêm com o Plano 1 de Proteção de Informações Azure (AIP) e ajudam você a classificar e, opcionalmente, proteger seus documentos e e-mails, aplicando rótulos. Os rótulos podem ser aplicados automaticamente por administradores que definem regras e condições, manualmente pelos usuários ou usando uma combinação em que os usuários recebem recomendações.

Para configurar rótulos de sensibilidade, veja [criar e gerenciar vídeos](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) de rótulos de sensibilidade.



### <a name="install-the-azure-information-protection-client-manually"></a>Instale o cliente de Proteção de Informações do Azure manualmente

Para instalar manualmente o cliente AIP:

1. Baixe **AzinfoProtection_UL.exe** do centro de download da [Microsoft](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Você pode verificar se a instalação funcionou visualizando um documento do Word e certificando-se de que a opção **de sensibilidade** está disponível na guia **Home.**
<br/>![Guia de proteção drop-down em um documento do Word.](media/word-sensitivity.png)

Para mais informações ver, [instale o cliente.](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3)
