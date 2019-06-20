---
title: Aumentar a protecção contra ameaças para a Microsoft 365 empresa
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
search.appverid:
- BCS160
- MET150
description: Configurar a protecção de ameaças avançado do Office 365 e proteger dados sensíveis.
ms.openlocfilehash: 53741a7726222bb32329a401953be72257df95cc
ms.sourcegitcommit: 7ac06563c6ff034358e8fd3f9298fc426187ade2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/31/2019
ms.locfileid: "35086384"
---
# <a name="set-up-compliance-features"></a>Configurar funcionalidades de conformidade

A Microsoft 365 Business é fornecido com funcionalidades para proteger os dados e dispositivos e ajudar a proteger o seu e informações confidenciais dos clientes.

## <a name="set-up-dlp-features"></a>Configurar funcionalidades do DLP

Consulte [criar uma política DLP a partir de um modelo](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) para obter um exemplo sobre como configurar uma política para proteger informações de identificação pessoal (PII). 
  
DLP é fornecido com modelos de política de prontos a utilizar muitos para muitos idiomas diferentes. Por exemplo, dados financeiros da Austrália, Canadá lei de informações pessoais, dados financeiros dos e.u.a., etc. Para obter uma lista completa, consulte a [incluem modelos de política que do DLP](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) . Todos estes modelos podem ser activados semelhante ao exemplo de modelo do PII. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Configurar a retenção de correio electrónico com o arquivo Online do Exchange

 Funcionalidades de licença **Online arquivo do Exchange** ajudam a manter a conformidade e normas reguladoras mantiver o correio electrónico conteúdo para detecção de dados electrónicos. Também ajuda a reduzir os riscos em caso de uma acção judicial e fornece uma forma de recuperar os dados após uma falha de segurança, ou quando necessitar de recuperar itens eliminados. Pode utilizar o litígio suspenso para manter todo o conteúdo de um utilizador, ou utilizar políticas de retenção para personalizar o que pretende preservar.
  
**Espera litígio:** Pode preservar todo o conteúdo da caixa de correio reter itens eliminados incluindo colocando a caixa de correio de todo um utilizador no litígio. 
    
Para colocar uma caixa de correio em espera de litígio, no Centro de administração:
    
1. No nav esquerda, vá para **os utilizadores** \> **os utilizadores activos**.
    
2. Seleccione um utilizador cuja caixa de correio que pretende colocar no litígio mantenha e no painel do utilizador expanda **definições de correio** e junto de **definições mais** escolha **Exchange editar propriedades**.
    
3. Na página da caixa de correio do utilizador, seleccione * * funcionalidades de correio * * no nav esquerda e, em seguida, seleccione a hiperligação **Activar** em **litígio mantenha**.
    
4. Em **litígios mantenha** a caixa de diálogo pode especificar os litígios Mantenha duração no campo **litígio Mantenha duração** , deixe o campo vazio se pretende colocar uma espera infinita. Também pode adicionar notas e direccionar o proprietário de caixa de correio para um Web site poderá ter de explicar mais informações sobre os litígios mantém \> **Guardar**.
    
**Retenção:** Pode activar políticas de retenção personalizado como, por exemplo, a preservar de um determinado período de tempo ou eliminar permanentemente o conteúdo no final do período de retenção. Para obter mais informações, consulte [Descrição geral de políticas de retenção](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).

## <a name="set-up-azure-information-protection-features"></a>Configurar funcionalidades de protecção de informações de Azure

Protecção de informações Azure (AIP) ajuda a classificar e opcionalmente, proteger os seus documentos e mensagens de correio electrónico, através da aplicação de etiquetas. Podem ser aplicados automaticamente rótulos por administradores que definem as regras e condições, manualmente por utilizadores ou utilizando uma combinação de onde os utilizadores tiverem recomendações.

No Outlook na web pode aplicar as restrições e os seguintes rótulos incorporados para mensagens de correio electrónico:
  
- **Não reencaminhar**: os destinatários podem ler a mensagem, mas não é possível reencaminhar, imprimir ou copiar conteúdo
    
- **Encriptar**: toda a mensagem está encriptada. Os destinatários têm de confirmar sua identidade antes de aceder a conteúdo encriptado e não é possível remover a encriptação.
    
- **Confidencial**: dá os empregados da organização todas as permissões para o conteúdo de correio electrónico e anexos, mas não para pessoas fora da organização. Proprietários de dados podem controlar e revogar o conteúdo em qualquer altura.
    
- **Altamente confidenciais**: esta restrição pode ser aplicada aos dados altamente confidenciais, permitindo que os empregados ver, editar e responder, mas não reencaminhar, imprimir ou copiar os dados. Proprietários de dados podem controlar e revogar o conteúdo em qualquer altura.

### <a name="make-sure-azure-information-protection-is-activated"></a>Garantir a protecção de informações Azure está activada

Para verificar que AIP está activado:

1. Iniciar sessão no [Azure portal](https://portal.azure.com/).

2. Seleccione **todos os serviços** e escreva *Azure a protecção de informações* na **Caixa de procura**.

3. Depois de visualizar os resultados, clique em Iniciar seguinte para **A protecção de informações Azure** para o tornar um favorito e fácil de localizar mais tarde.

4. Seleccione **A protecção de informações Azure** \> **a activação de protecção** e certifique-se de que o estado estiver definido para activada. 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a>Visualizar as etiquetas de política e a predefinição de protecção de informações de Azure 

Para ver e modificar, os existentes etiquetas:

1. No dashboard Azure a protecção de informações, seleccione as **classificações de** \> **etiquetas**. <br/>![Etiquetas padrão para a protecção de informações Azure.](media/AIPLabels.png)

2. Pode escolher qualquer etiqueta para ver opções, pode alterar o nome a apresentar, cores, etc.
 
3. Consulte [modificar e criar novos rótulos](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) se pretender criar os seus próprios. 

### <a name="install-the-azure-information-protection-client-manually"></a>Instalar manualmente o cliente de protecção de informações de Azure

Para instalar manualmente o cliente AIP:

1. Transferir o **AzInfoProtection.exe** do [Centro de transferências da Microsoft](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Pode verificar que a instalação trabalhou visualizando um documento do Word e certificando-se de que a opção de **protecção** está disponível no separador **base** . <br/>![Separador protecção pendente num documento do Word.](media/Word_Protect.png)

Para mais informações, consulte [instalar o cliente](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
