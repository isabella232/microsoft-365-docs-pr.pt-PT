---
title: Aumente a proteção contra ameaças para o Microsoft 365 Business
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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
description: Configure os recursos de conformidade para evitar perda de dados e rótulos de dados confidenciais.
ms.openlocfilehash: a0ba2fa6dbe7c786d577ad7098c1790f569f5acc
ms.sourcegitcommit: 255e8194bb5767a9983d54d16e79d628732a1d97
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/11/2019
ms.locfileid: "37453928"
---
# <a name="set-up-compliance-features"></a>Configurar recursos de conformidade

Seu Microsoft 365 Business vem com recursos para proteger seus dados e dispositivos, e ajudá-lo a manter a sua e as informações confidenciais dos seus clientes seguras.

## <a name="set-up-dlp-features"></a>Configurar recursos de DLP

Consulte [criar uma política de DLP a partir de um modelo](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) para obter um exemplo de como configurar uma política para proteger contra informações de identificação pessoal (PII). 
  
O DLP vem com muitos modelos de política prontos para uso para muitas localidades diferentes. Por exemplo, dados financeiros da Austrália, lei de informações pessoais do Canadá, dados financeiros dos EUA, etc. Consulte [o que os modelos de política de DLP incluem](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) para obter uma lista completa. Todos esses modelos podem ser habilitados semelhante ao exemplo de modelo de PII. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Configurar a retenção de email com o arquivamento do Exchange Online

 Os recursos **de licença de arquivamento do Exchange Online** ajudam a manter padrões normativos e de conformidade preservando conteúdo de email para eDiscovery. Ele também ajuda a reduzir o risco no caso de uma ação judicial e fornece uma maneira de recuperar dados após uma violação de segurança, ou quando você precisa recuperar itens excluídos. Você pode usar o litígio para preservar todo o conteúdo de um usuário ou usar políticas de retenção para personalizar o que deseja preservar.
  
Retenção de **litígio:** Você pode preservar todo o conteúdo da caixa de correio incluindo itens excluídos colocando a caixa de correio inteira de um usuário em retenção de litígio. 
    
Para colocar uma caixa de correio em retenção de litígio, no centro de administração:
    
1. No NAV esquerdo, **aceda a** \> utilizadores **activos**.
    
2. Selecione um usuário cuja caixa de correio você deseja colocar na retenção de litígio e no painel do usuário expanda **configurações de email** e, ao lado de **mais configurações** , escolha **Editar propriedades do Exchange**.
    
3. Na página de caixa de correio do usuário, escolha * * recursos de caixa de correio * * no NAV esquerdo e, em seguida, escolha o link **Enable** em retenção de **litígio**.
    
4. Na caixa de diálogo retenção de **litígio** , você pode especificar a duração da retenção de litígio no campo duração da retenção de **litígio** , deixar o campo vazio se desejar colocar uma retenção infinita. Você também pode adicionar anotações e direcionar o proprietário da caixa de correio para um site que talvez você tenha que explicar mais sobre \> a retenção de litígio **salvar**.
    
**Retenção:** Você pode habilitar políticas de retenção personalizadas, por exemplo, para preservar um determinado período de tempo ou excluir conteúdo permanentemente no final do período de retenção. Para saber mais, consulte [visão geral das políticas de retenção](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).

## <a name="set-up-sensitivity-labels"></a>Configurar rótulos de sensibilidade

Rótulos de sensibilidade vêm com o plano de proteção de informações do Azure (AIP) 1 e ajudam a classificar e, opcionalmente, proteger seus documentos e emails, aplicando rótulos. Os rótulos podem ser aplicados automaticamente por administradores que definem regras e condições, manualmente por usuários, ou usando uma combinação em que os usuários recebem recomendações.

Para configurar rótulos de sensibilidade, exiba [criar e gerenciar os rótulos de sensibilidade](https://support.office.com/en-us/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) vídeo.



### <a name="install-the-azure-information-protection-client-manually"></a>Instalar o cliente do Azure Information Protection manualmente

Para instalar manualmente o cliente AIP:

1. Baixar **AzinfoProtection_UL. exe** do [centro de download da Microsoft](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Você pode verificar se a instalação funcionou exibindo um documento do Word e certificando-se de que a opção de **sensibilidade** está disponível na guia **início** .
<br/>![Guia de proteção suspensa em um documento do Word.](media/word-sensitivity.png)

Para obter mais informações, consulte, [instalar o cliente](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
