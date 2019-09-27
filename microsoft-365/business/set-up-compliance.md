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
description: Configure a proteção avançada contra ameaças do Office 365 e proteja os dados confidenciais.
ms.openlocfilehash: 8144bcebe8a0cdf28a5e092f592362922ccbdd48
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288751"
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

## <a name="set-up-azure-information-protection-features"></a>Configurar os recursos do Azure Information Protection

O AIP (proteção de informações do Azure) ajuda você a classificar e, opcionalmente, proteger seus documentos e emails, aplicando rótulos. Os rótulos podem ser aplicados automaticamente por administradores que definem regras e condições, manualmente por usuários, ou usando uma combinação em que os usuários recebem recomendações.

No Outlook na Web, você pode aplicar os seguintes rótulos e restrições incorporados aos seus emails:
  
- **Não encaminhar**: os destinatários podem ler a mensagem, mas não conseguem encaminhar, imprimir ou copiar conteúdo
    
- **Criptografar**: a mensagem inteira é criptografada. Os destinatários devem confirmar sua identidade antes de acessar o conteúdo criptografado e não podem remover a criptografia.
    
- **Confidencial**: concede aos funcionários da sua organização permissões completas para o conteúdo e os anexos de e-mail, mas não para pessoas fora da sua organização. Os proprietários de dados podem rastrear e revogar conteúdo em qualquer ponto.
    
- **Altamente confidencial**: essa restrição pode ser aplicada a dados altamente confidenciais, permitindo que os funcionários visualizem, editem e respondam, mas não reencaminhar, imprimir ou copiar os dados. Os proprietários de dados podem rastrear e revogar conteúdo em qualquer ponto.

### <a name="make-sure-azure-information-protection-is-activated"></a>Certifique-se de que a proteção de informações do Azure está ativada

Para verificar se o AIP está ativado:

1. Entre no [portal do Azure](https://portal.azure.com/).

2. Selecione **todos os serviços** e digite a *proteção de informações do Azure* na **caixa de pesquisa**.

3. Depois que os resultados forem exibidos, clique no início ao lado da **proteção de informações do Azure** para torná-lo um favorito e fácil de encontrar mais tarde.

4. Selecione \> **ativação da proteção** de **proteção de informações do Azure** e certifique-se de que o status esteja definido como ativado. 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a>Exibir a política de proteção de informações do Azure e rótulos padrão 

Para exibir e modificar os rótulos existentes:

1. No painel de proteção de informações do Azure, selecione **Rótulos**de **classificações** \> . <br/>![Rótulos padrão para a proteção de informações do Azure.](media/AIPLabels.png)

2. Você pode escolher qualquer etiqueta para ver as opções, você pode alterar o nome de exibição, cores, etc.
 
3. Consulte [modificar e criar novos rótulos](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) se você quiser criar o seu próprio. 

### <a name="install-the-azure-information-protection-client-manually"></a>Instalar o cliente do Azure Information Protection manualmente

Para instalar manualmente o cliente AIP:

1. Baixar **Azinfoprotection. exe** do [centro de download da Microsoft](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Você pode verificar se a instalação funcionou exibindo um documento do Word e certificando-se de que a opção **Protect** está disponível na guia **início** . <br/>![Guia de proteção suspensa em um documento do Word.](media/Word_Protect.png)

Para obter mais informações, consulte, [instalar o cliente](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
