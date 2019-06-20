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
ms.openlocfilehash: b6e9941eee9de4f295b0f8056c1c91b7076e530c
ms.sourcegitcommit: 7ac06563c6ff034358e8fd3f9298fc426187ade2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/31/2019
ms.locfileid: "35086385"
---
# <a name="increase-threat-protection"></a>Aumentar a protecção contra ameaças

Este artigo ajuda-o a aumentar a protecção na sua subscrição do Microsoft 365 para protecção contra phishing, malware e outras ameaças. Estas recomendações são adequadas para organizações com uma necessidade crescente de segurança, tal como a lei, consultórios e clínicas médicas cuidados de saúde.

Antes de começar, verifique a sua pontuação de seguro do Office 365. Office 365 Secure pontuação analisa a segurança da organização do Office 365 com base nas actividades normais e as definições de segurança e atribui uma classificação. Comece por tomar nota do seu resultado actual. Executar acções recomendadas neste artigo aumenta a sua pontuação. O objectivo é não atingir a pontuação máxima, mas tenha em atenção de oportunidades para proteger o seu ambiente que não afectar negativamente a produtividade dos utilizadores. 

Para mais informações, consulte a [Pontuação de seguro da Microsoft](https://docs.microsoft.com/en-us/office365/securitycompliance/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Aumentar o nível de protecção contra malware no correio do

O ambiente do Office 365 ou Microsoft 365 inclui protecção contra malware, mas pode aumentar esta protecção, bloqueio de anexos com tipos de ficheiro que são normalmente utilizados para software malicioso. Para aumentar a protecção contra malware no correio electrónico:
  
1. Vá para [https://protection.office.com](https://protection.office.com) e inicie sessão com as credenciais de conta de administrador. 
    
2. No Office 365 título &amp; o Centro de conformidade, no painel de navegação do lado esquerdo, em **Gestão de ameaça**, escolher **política** \> **Anti-Malware**.
    
3. Faça duplo clique sobre a política predefinida para editar esta política ao nível da empresa.
    
4. Clique em **Definições**.
    
5. **Em **Comum anexo tipos de filtro**, seleccione.** Os tipos de ficheiro que são bloqueados são listados na janela directamente abaixo deste controlo.  Certifique-se de que adicionar estes tipos de ficheiros:
   - ade, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, tarefa, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, RCS, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif  <br/> Pode adicionar ou eliminar tipos de ficheiro mais tarde, se necessário.
    
6. Clique em **Guardar.**
    
Para mais informações, consulte [protecção anti-software malicioso](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409).
  
## <a name="protect-against-ransomware"></a>Proteger contra o ransomware

Ransomware restringe o acesso a dados por encriptação de ficheiros ou bloquear ecrãs de computador. Em seguida, tenta extort money a partir das vítimas, pedindo para "ransom", normalmente, sob forma de cryptocurrencies como Bitcoin, em troca de acesso a dados. 
  
Pode proteger-se ransomware, criando correio de um ou mais regras de fluxo para bloquear extensões de ficheiros que são normalmente utilizadas para ransomware (estes foram adicionados no passo [aumentar o nível de protecção contra malware no correio](#raise-the-level-of-protection-against-malware-in-mail) ), ou para avisar os utilizadores que recebem estas anexos de correio electrónico.

Para além dos ficheiros bloqueados no passo anterior, também é boa prática para criar uma regra para avisar os utilizadores antes de abrir anexos de ficheiros do Office que incluem macros. Ransomware pode ser escondido dentro de macros, pelo que iremos irá avisar os utilizadores para não abrir estes ficheiros de pessoas que não conhece.

Para criar uma regra de transporte de correio:
  
1. Vá para o Centro de administração no <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> e escolha a **centros de Admin** \> **Exchange**.
    
2. Na categoria de **fluxo de correio** , clique em **regras**.
    
3. Clique em **+** e, em seguida, clique em **criar uma nova regra**.
    
4. Clique em **mais opções** na parte inferior da caixa de diálogo para ver o conjunto completo de opções. 
    
5. Aplica as definições na seguinte tabela para a regra. Deixe o resto das definições a predefinição, a menos que pretenda alterá-las.
    
6. Clique em **Guardar**.
    
|**Definição**|**Avisar os utilizadores antes de abrir anexos de ficheiros do Office**||
|:-----|:-----|:-----|
|Name  <br/> |Regra de anti-ransomware: avisar os utilizadores  <br/>  |
|Se esta regra. . .  <br/> |Qualquer anexo. . . corresponde a extensão de ficheiro. . .  <br/> |
|Especifique palavras ou expressões  <br/> |Adicione estes tipos de ficheiro:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm  <br/>|
|Efectue o seguinte. . .  <br/> |Notificar o destinatário com uma mensagem  <br/> |
|Fornecer texto da mensagem  <br/> |Não abra este tipo de ficheiros de pessoas que não conhece porque podem conter macros com código malicioso.  <br/> |
   
Para obter mais informações, consulte:
  
- [Como lidar com ransomware](https://go.microsoft.com/fwlink/?linkid=2016501&amp;clcid=0x409)
    
- [Restaurar o OneDrive](https://support.office.com/article/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)
    


## <a name="stop-auto-forwarding-for-email"></a>Parar o reencaminhamento automático de correio electrónico

Os hackers que acederem à caixa de correio de um utilizador podem roubar o correio através da definição da caixa de correio para reencaminhar automaticamente correio electrónico. Isto pode acontecer mesmo sem a detecção do utilizador. Pode impedir que isto aconteça, configurando uma regra de fluxo de correio. 
  
Para criar uma regra de transporte de correio, assista a [Este vídeo curto](https://support.office.com/article/f9d693ba-5c78-47c0-b156-8e461e062aa7) ou siga estes passos:
  
1. No Centro de administração Microsoft 365, clique em **centros de Admin** \> **Exchange**.
    
2. Na categoria de **fluxo de correio** , clique em **regras**.
    
3. Clique em **+** e, em seguida, clique em **criar uma nova regra**.
    
4. Clique em **mais opções** na parte inferior da caixa de diálogo para ver o conjunto completo de opções. 
    
5. Aplica as definições na seguinte tabela. Deixe o resto das definições a predefinição, a menos que pretenda alterá-las.
    
6. Clique em **Guardar**.
    
|**Definição**|**Avisar os utilizadores antes de abrir anexos de ficheiros do Office**|
|:-----|:-----|
|Name  <br/> |Impedir o reencaminhamento automático de correio electrónico para domínios externos  <br/> |
|Aplica esta regra se...  <br/> |O remetente. . . é externo/interno. . . Dentro da organização  <br/> |
|Adicionar condição  <br/> |As propriedades da mensagem. . . inclua o tipo de mensagem. . . Reencaminhamento automático  <br/> |
|Efectue o seguinte procedimento...  <br/> |Bloquear a mensagem. . . rejeitar a mensagem e incluir uma explicação.  <br/> |
|Fornecer texto da mensagem  <br/> |Correio electrónico de reencaminhamento automático fora esta organização é impedido por razões de segurança.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Proteger o correio electrónico contra ataques de phishing

Se tiver configurado um ou mais domínios personalizados para o ambiente do Office 365 ou Microsoft 365, pode configurar a protecção de anti-phishing alvo. Protecção anti-phishing de ATP, parte do Office 365 avançada protecção contra ameaças, pode ajudar a proteger a sua organização contra ataques de phishing mal intencionado baseado na representação e outros ataques de phishing. Se ainda não configurou um domínio personalizado, não é necessário efectuar este procedimento.
  
Recomendamos que começar com esta protecção, criando uma política para proteger os utilizadores mais importantes e o domínio personalizado. 

  
Para criar uma política de anti-phishing ATP, assista a [Esta formação curta vídeo](https://support.office.com/article/86c425e1-1686-430a-9151-f7176cce4f2c)ou efectue os seguintes passos:
  
1. Aceda a [https://protection.office.com](https://protection.office.com). 
    
2. No Office 365 título &amp; o Centro de conformidade, no painel de navegação do lado esquerdo, em **Gestão de ameaça**, escolher **política**.
    
3. Na página de **política** , seleccione **ATP anti-phishing**.
    
4. Na página **Anti-phishing** , seleccione **+ Criar**. É iniciado um assistente que orienta-o por definir a política anti-phishing.
    
5. Especifique o nome, descrição e as definições da política, tal como recomendado no gráfico abaixo. Consulte para [aprender sobre as opções de política anti-phishing ATP](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409) para obter mais detalhes. 
    
6. Depois de rever as definições, escolha **criar esta política** ou **Guardar**, conforme adequado.
    

|**Definição ou opção**<br/>|**Definição recomendada** <br/>|
|:-----|:-----|
|Name  <br/> |Domínio e o pessoal de campanha mais importantes  <br/> |
|Descrição  <br/> |Certifique-se mais importantes, pessoal e o nosso domínio não estão a ser representadas.  <br/> |
|Adicionar utilizadores ao proteger  <br/> |Seleccione **+ Adicionar é uma condição, o destinatário**. Introduza nomes de utilizador ou o endereço de correio electrónico do candidato, Gestor de campanha e outros membros do pessoal importantes. Pode adicionar até 20 endereços internos e externos que pretende proteger de representação.  <br/> |
|Adicionar domínios para proteger  <br/> |Seleccione **+ Adicionar é uma condição, o domínio do destinatário**. Introduza o domínio personalizado associado a subscrição do Microsoft 365, se definiu um. Pode introduzir mais de um domínio.  <br/> |
|Escolher acções  <br/> |Se a mensagem de correio electrónico é enviada por um utilizador representado: Escolha a **redireccionar mensagens para outro endereço de correio electrónico**e, em seguida, escreva o endereço de correio electrónico do administrador de segurança; Por exemplo, *Alice<span><span>@contoso.com*.          Se a mensagem de correio electrónico é enviada por um domínio representado: Escolha a **mensagem de quarentena**.  <br/> |
|Análise da caixa de correio  <br/> |Por predefinição, a análise da caixa de correio está seleccionado quando cria uma nova política anti-phishing. Deixe **Esta definição para obter melhores resultados** .  <br/> |
|Adicionar remetentes e domínios  <br/> |Aqui pode adicionar o seu próprio domínio ou quaisquer outros domínios fidedignos.  <br/> |
|Aplicado a  <br/> |Seleccione **o domínio de destinatário é**. Em **qualquer um destes**, seleccione **Escolher**. Seleccione **+ Adicionar**. Seleccione a caixa de verificação junto ao nome do domínio, por exemplo, contoso de *.<span> <span>com*, na lista e, em seguida, seleccione **Adicionar**. Seleccione **Concluir**.  <br/> |
   
Para mais informações, consulte [configurar as políticas anti-phishing do ATP do Office 365](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409).
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Proteger contra anexos com conteúdo nocivo e de ficheiros com anexos seguros ATP

Pessoas regularmente enviam, receber e partilhar anexos, tal como documentos, apresentações, folhas de cálculo e mais. Nem sempre é fácil saber se um anexo é seguro ou maliciosos apenas por olhar para uma mensagem de correio electrónico. Protecção de ameaças avançada Office 365 inclui protecção de ATP anexo seguro, mas esta protecção não está activada por predefinição. Recomendamos que crie uma nova regra para começar a utilizar esta protecção. Esta protecção é extensível a ficheiros no SharePoint, OneDrive e Teams da Microsoft.
  
Para criar uma política de segurança de anexos de ATP, assista a [Este vídeo curto](https://support.office.com/article/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)ou efectue os seguintes passos:
  
1. Vá para [https://protection.office.com](https://protection.office.com) e inicie sessão com a conta de administrador. 
    
2. No Office 365 título &amp; o Centro de conformidade, no painel de navegação do lado esquerdo, em **Gestão de ameaça**, escolher **política**.
    
3. Na página de política, seleccione **anexos seguros ATP**.
    
4. Na página de anexos seguros, aplica esta protecção amplamente seleccionando a caixa de verificação **Activar ATP para SharePoint, OneDrive e equipas da Microsoft** . 
    
5. Seleccione **+** para criar uma nova política. 
    
6. Aplica as definições na seguinte tabela. 
    
7. Depois de rever as definições, escolha **criar esta política** ou **Guardar**, conforme adequado.
    

|**Definição ou opção**|**Definição recomendada** <br/>|
|:-----|:-----|
|Name  <br/> |Bloquear actuais e futuras mensagens de correio electrónico com software malicioso detectado.  <br/> |
|Descrição  <br/> |Bloquear actuais e futuras mensagens de correio electrónico e anexos com software malicioso detectado.  <br/> |
|Guardar anexos desconhecidos malware resposta  <br/> |Seleccione **bloco - bloquear os actuais e futuras mensagens de correio electrónico e anexos com software malicioso detectado**.  <br/> |
|Anexo a detecção de redireccionamento  <br/> |Activar o redireccionamento (seleccione esta caixa) introduza a conta de administrador ou um programa de configuração de caixa de correio de quarentena.          Se a selecção acima malware analisar anexos de tempo limite ou erro ocorre (seleccione esta caixa).  <br/> |
|Aplicado a  <br/> |É o domínio do destinatário. . . Seleccione o domínio.  <br/> |
   
Para mais informações, consulte [configurar as políticas anti-phishing do ATP do Office 365](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409).
  


## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Proteger contra ataques de phishing com ligações seguras de ATP

Os hackers, por vezes, ocultar os Web sites maliciosos hiperligações na mensagem de correio electrónico ou outros ficheiros. 365 ATP seguro ligações do Office (ligações seguras de ATP), parte do Office 365 avançada protecção contra ameaças, pode ajudar a proteger a sua organização, fornecendo tempo de clique verificação de endereços web (URLs) em mensagens de correio electrónico e documentos do Office. Protecção é definida através das políticas de ligações seguras de ATP.
  
Recomendamos que fizer o seguinte:
  
- Modificar a política predefinida para aumentar a protecção.
    
- Adicione uma nova política destinada a todos os destinatários do seu domínio.
    
Para configurar ligações seguras de ATP, assista a [Esta formação curta vídeo](https://support.office.com/article/61492713-53c2-47da-a6e7-fa97479e97fa)ou efectue os seguintes passos:
  
1. Vá para [https://protection.office.com](https://protection.office.com) e inicie sessão com a conta de administrador. 
    
2. No Office 365 título &amp; o Centro de conformidade, no painel de navegação do lado esquerdo, em **Gestão de ameaça**, escolher **política**.
    
3. Na página de política, seleccione **Ligações seguras de ATP**.
    
Para modificar a política predefinida:
  
1. Na página ligações seguras, no âmbito de **políticas que se aplicam a toda a organização**, seleccione a política **predefinida** . 
    
2. Em **definições que se aplicam ao conteúdo excepto correio electrónico**, seleccione **ProPlus do Office 365, Office para iOS e Android**.
    
3. Clique em **Guardar**. 
    
Para criar uma nova política destinada a todos os destinatários no domínio:
  
1. Na página ligações seguras, em **que se aplicam a toda a organização de políticas**, clique em **+** para criar uma nova política. 
    
2. Aplica as definições listadas na seguinte tabela.
    
3. Clique em **Guardar**. 

|**Definição ou opção**|**Definição recomendada** <br/>|
|:-----|:-----|
|Name  <br/> |Política de segurança de ligações para todos os destinatários no domínio  <br/> |
|Seleccione a acção para URLs potencialmente maliciosos desconhecidos em mensagens  <br/> |Seleccione **On - URLs serão escritas de novo e verificados numa lista de hiperligações maliciosas conhecidas quando utilizador clica na hiperligação**.  <br/> |
|Utilizar anexos seguros para pesquisar conteúdo transferível  <br/> |Seleccione esta caixa.  <br/> |
|Aplicado a  <br/> |É o domínio do destinatário. . . Seleccione o domínio.  <br/> |
   
Para mais informações, consulte [ligações de seguras do Office 365 ATP](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409).

## <a name="go-to-intune-admin-center"></a>Ir para Centro de administração de Intune

1. Iniciar sessão no [Azure portal](https://portal.azure.com/).

2. Seleccione **todos os serviços** e digite *Intune* na **Caixa de procura**.

3. Depois de visualizar os resultados, clique em Iniciar seguinte para **Microsoft Intune** para o tornar um favorito e fácil de localizar mais tarde.

Para além do Centro de administração, pode utilizar Intune para inscrição e gerir dispositivos da sua organização. Para mais informações, consulte [Opções de inscrição de dispositivos geridos por Intune](https://docs.microsoft.com/intune/enrollment-options)e as [capacidades pelo método de inscrição de dispositivos do Windows](https://docs.microsoft.com/intune/enrollment-method-capabs) .
