---
title: Funcionalidades de segurança do Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-security-compliance
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Obter informações sobre as funcionalidades de segurança fornecidas com o Microsoft 365 Business.
ms.openlocfilehash: 24d4c4e79e7d8737beb82336796956774f127209
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32286902"
---
# <a name="microsoft-365-business-security-features"></a>Funcionalidades de segurança do Microsoft 365 Business

Microsoft 365 Business oferece funcionalidades de segurança simplificada para ajudar a salvaguardar os dados em PCs, telefones e mesas de dados.
    
## <a name="microsoft-365-business-admin-center-security-features"></a>Funcionalidades de segurança do Microsoft 365 Business admin Centro

Pode gerir muitas das funcionalidades de segurança do Microsoft 365 Business no Centro de administração, dá-lhe uma forma simplificada para activar ou desactivar estas funcionalidades. No Centro de administração pode fazer o seguinte:
  
![Screenshot of the Devices card in the admin center](media/9982e784-dbf9-4a76-a159-bb3e2e5aa23f.png)
  
- [Definir definições de gestão de aplicações para dispositivos Android ou iOS](app-protection-settings-for-android-and-ios.md) . 
    
    Estas definições incluem eliminar ficheiros a partir de um dispositivo inactivo após um período definido, a encriptação dos ficheiros de trabalho, que exijam que os utilizadores definem um PIN, etc.
    
- [Definir definições de protecção da aplicação para Windows 10 dispositivos](protection-settings-for-windows-10-devices.md) . 
    
    Estas definições podem ser aplicadas para dispositivos de propriedade pessoalmente ou dados da empresa em ambos pertencentes à empresa.
    
- [Definir definições de protecção do dispositivo para o Windows 10 dispositivos](protection-settings-for-windows-10-pcs.md) . 
    
    Pode activar a encriptação [BitLocker](https://go.microsoft.com/fwlink/p/?linkid=871405) ajudar a proteger os dados no caso de um dispositivo for perdido ou roubado e activar a [Protecção de tirar partido do Windows](https://go.microsoft.com/fwlink/p/?linkid=871404) fornecer protecção avançada contra ransomware. 
    
- [Remover dados empresariais de dispositivos](remove-company-data.md)
    
    Pode limpar dados da empresa remotamente se um dispositivo for perdido, roubado, ou um empregado deixa a empresa.
    
- [Dispositivos Windows 10 repor as definições de fábrica](reset-devices-to-factory-settings.md) . 
    
    Pode repor todos os dispositivos Windows 10 que têm definições de protecção de dispositivo aplicadas.
    
## <a name="additional-security-features"></a>Funcionalidades de segurança adicionais 

Funcionalidades avançadas no Microsoft 365 Business estão disponíveis para ajudar a proteger a sua empresa contra ciber-ameaças e proteger informações confidenciais.
  
- **[Protecção do Office 365 ameaça avançadas](https://support.office.com/article/e100fe7c-f2a1-4b7d-9e08-622330b83653)**
    
    Avançada protecção de ameaças (ATP) ajuda a proteger a sua empresa contra phishing sofisticada e ataques de ransomware, concebidos para comprometer empregado ou informações de cliente. As funcionalidades incluem:
    
  - Análise de anexos sofisticados e alimentados AI análise para detectar e eliminar mensagens perigosas.
    
  - Automático verifica-se de hiperligações da web por correio electrónico para avaliar se são parte de um esquema de phishing. Mantém a segurança de aceder a Web sites inseguros.
    
- **[Descrição geral das políticas de prevenção de perda de dados](https://support.office.com/article/1966b2a7-d1e2-4d92-ab61-42efbb137f5e)** (DLP). 
    
    Pode configurar DLP para detectar automaticamente informações sensíveis, tais como números de cartão de crédito, números de segurança social, etc. para impedir a sua inadvertida partilha fora da empresa.
    
- **[Arquivo do Exchange Online](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Licença Online arquivo do Exchange permite mensagens facilmente ser arquivada com cópia de segurança de dados contínua. Armazena todas as mensagens de correio electrónico do utilizador, incluindo itens eliminados, no caso de forem necessários mais tarde para detecção ou de restauro. Além disso, pode utilizar políticas de retenção diferente para manter os dados de correio electrónico para porões de litígio, detecção de dados electrónicos, ou para satisfazer requisitos de conformidade.
    
- **[Protecção de informações Azure](https://go.microsoft.com/fwlink/p/?linkid=871406)**
    
    Informações protecção ajuda-o a que controlar o acesso a informações confidenciais no correio electrónico e documentos com controlos como "Não reencaminhar" e "Não copia". Também pode classificar as informações confidenciais como "Confidencial" e especificar como as informações classificadas podem ser partilhadas fora e dentro de negócio. Encriptação de escala da empresa é fácil aplicar a mensagem de correio electrónico e documentos para manter as suas informações privadas. Microsoft 365 Business inclui todas as funcionalidades do [Azure informações protecção planear 1](https://go.microsoft.com/fwlink/p/?linkid=871407). Também pode instalar o protecção de informações de Azure cliente suplemento para aplicações do Office. Para obter mais detalhes, consulte o [Guia do administrador de cliente de protecção de informações de Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide).
    
- **[Todas as capacidades de Intune no Azure portal](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Aceder a Intune Centro de administração no Azure portal permite-lhe configurar funcionalidades de segurança adicionais, tais como a gestão de dispositivos MacOS, iPhone e dispositivos Android juntamente com a gestão de dispositivos avançado para Windows, que não estão disponíveis através da Microsoft Centro de administração de negócio 365.
    
As secções seguintes descrevem como pode gerir estas funcionalidades na segurança &amp; Centro de conformidade e o Centro de administração Intune. Ao longo do tempo serão adicionados os controlos simplificados para o Centro admin do Microsoft 365 Business.
  
## <a name="set-up-advanced-threat-protection-features"></a>Configurar funcionalidades de protecção contra ameaças avançadas

- **Proteger contra anexos não seguros:** ATP identifica conteúdo malicioso através da abertura de anexos de correio electrónico num ambiente virtual e efectuar uma análise do comportamento resultante. O conteúdo é avaliado para determinar a sua intenção de (se normal ou malicioso), e ATP bloqueia entrega de anexos inseguros, ajudando a proteger o computador contra infecções de ransomware e esquemas de phishing. Para activar a protecção do anexo, consulte [Configurar políticas de anexos seguros do Office 365 ATP](https://support.office.com/article/078eb946-819a-4e13-8673-fe0c0ad3a775).
    
- Proteger o seu ambiente quando os utilizadores clicam em hiperligações maliciosas: ATP também examina hiperligações na mensagem de correio electrónico quando um utilizador clica-los. Se uma hiperligação não é segura, o utilizador é avisado não a visitar o site ou informado que o site foi bloqueado. Isto ajuda a proteger contra esquemas de phishing. Pode [Configurar políticas de segurança ligações do Office 365 ATP](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#reveddefaultscc) ou [configurar as políticas de segurança ligações do Office 365 ATP](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#addemailpolscc).
    
## <a name="set-up-dlp-features"></a>Configurar funcionalidades do DLP

Consulte [criar uma política DLP a partir de um modelo](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) para obter um exemplo sobre como configurar uma política para proteger informações de identificação pessoal (PII). 
  
DLP é fornecido com modelos de política de prontos a utilizar muitos para muitos idiomas diferentes. Por exemplo, dados financeiros da Austrália, Canadá lei de informações pessoais, dados financeiros dos e.u.a., etc. Para obter uma lista completa, consulte a [incluem modelos de política que do DLP](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) . Todos estes modelos podem ser activados semelhante ao exemplo de modelo do PII. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Configurar a retenção de correio electrónico com o arquivo Online do Exchange

 Funcionalidades de licença **Online arquivo do Exchange** -lhe a capacidade de ajudar a manter a conformidade e normas reguladoras mantiver o correio electrónico conteúdo para fins de detecção de dados electrónicos. Também ajuda a reduzir os riscos em caso de litígio e fornece uma forma de recuperar os dados após uma falha de segurança ou quando necessitar de recuperar itens eliminados. Para activar estas capacidades, pode utilizar o litígio suspenso para manter todo o conteúdo de um utilizador, ou utilizar políticas de retenção para maior personalização do. 
  
**Espera litígio:** Pode preservar todo o conteúdo da caixa de correio reter itens eliminados incluindo colocando a caixa de correio de todo um utilizador no litígio. 
    
Para colocar uma caixa de correio em espera de litígio, no Centro de administração:
    
1. No nav esquerda, vá para **os utilizadores** \> **os utilizadores activos**.
    
2. Seleccione um utilizador cuja caixa de correio que pretende colocar no litígio mantenha e no painel do utilizador expanda **definições de correio** e junto de **definições mais** escolha **Exchange editar propriedades**.
    
3. Na página da caixa de correio do utilizador, seleccione * * funcionalidades de correio * * no nav esquerda e, em seguida, seleccione a hiperligação **Activar** em **litígio mantenha**.
    
4. Em **litígios mantenha** a caixa de diálogo pode especificar os litígios Mantenha duração no campo **litígio Mantenha duração** , deixe o campo vazio se pretende colocar uma espera infinita. Também pode adicionar notas e direccionar o proprietário de caixa de correio para um Web site poderá ter de explicar mais informações sobre os litígios mantém \> **Guardar**.
    
**Retenção:** Pode activar políticas de retenção personalizado como, por exemplo, a preservar de um determinado período de tempo ou eliminar permanentemente o conteúdo no final do período de retenção. Para obter mais informações, consulte [Descrição geral de políticas de retenção](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).
## <a name="set-up-azure-information-protection-features"></a>Configurar funcionalidades de protecção de informações de Azure

Protecção de informações Azure (AIP) é uma solução baseada na nuvem que ajuda a uma organização para classificar e opcionalmente, proteger o seus documentos e mensagens de correio electrónico através da aplicação de etiquetas. Rótulos podem ser aplicados automaticamente pelos administradores que definem as regras e condições, manualmente por utilizadores, ou uma combinação de onde os utilizadores tiverem recomendações.

A capacidade de aplicar as seguintes restrições ao enviar mensagens de correio electrónico no Outlook na web é activada automaticamente para todos os utilizadores:
  
- **Não reencaminhar**: os destinatários podem ler a mensagem, mas não é possível reencaminhar, imprimir ou copiar conteúdo
    
- **Encriptar**: toda a mensagem está encriptada. Os destinatários devem tomar medidas adicionais para confirmar a respectiva identidade antes de aceder a conteúdo encriptado e não é possível remover a encriptação.
    
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

Para mais informações, consulte [instalar o cliente](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3)

## <a name="go-to-intune-admin-center"></a>Ir para Centro de administração de Intune

1. Iniciar sessão no [Azure portal](https://portal.azure.com/).

2. Seleccione **todos os serviços** e digite *Intune* na **Caixa de procura**.

3. Depois de visualizar os resultados, clique em Iniciar seguinte para **Microsoft Intune** para o tornar um favorito e fácil de localizar mais tarde.
 
Pode utilizar Intune para inscrição e gerir dispositivos da sua organização. Para mais informações, consulte [Opções de inscrição de dispositivos geridos por Intune](https://docs.microsoft.com/intune/enrollment-options)e as [capacidades pelo método de inscrição de dispositivos do Windows](https://docs.microsoft.com/intune/enrollment-method-capabs) .
    
## <a name="faq"></a>FAQ

 ### <a name="are-these-security-features-available-in-all-markets"></a>Estas funcionalidades de segurança estão disponíveis em todos os mercados?
  
Sim, estas funcionalidades estão disponíveis em todos os mercados em que o Microsoft 365 Business é vendido.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Como encontrar a segurança &amp; center conformidade?
  
1. [Iniciar sessão no Microsoft 365 Business](https://portal.microsoft.com/) utilizando as credenciais de administrador. 
    
2. No nav esquerdo, localize a **centros de administração** e expandi-lo. 
    
    ![Nav esquerda no Centro de administração de Microsoft 365, escolha os centros de Admin.](media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Escolher **segurança &amp; conformidade** para ir para a segurança &amp; Centro de conformidade.