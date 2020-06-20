---
title: Aumentar a proteção contra ameaças para a Microsoft 365 para o Negócio
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
description: Crie o Office 365 Advanced Threat Protection e proteja dados sensíveis contra phishing, malware e outras ameaças.
ms.openlocfilehash: d5510cdc082781fd9a1776e86b1bab1d8a2723d6
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/18/2020
ms.locfileid: "44786212"
---
# <a name="increase-threat-protection"></a>Aumentar a proteção contra ameaças

Este artigo ajuda-o a aumentar a proteção na subscrição da Microsoft 365 para proteger contra phishing, malware e outras ameaças. Estas recomendações são adequadas para organizações com uma necessidade acrescida de segurança, como escritórios de advogados e clínicas de saúde.

Antes de começar, verifique o seu Office 365 Secure Score. O Office 365 Secure Score analisa a segurança da sua organização com base nas suas atividades regulares e definições de segurança e atribui uma pontuação. Comece por tomar nota da sua pontuação atual. Para aumentar a sua pontuação, complete as ações recomendadas neste artigo. O objetivo não é alcançar a pontuação máxima, mas estar atento a oportunidades para proteger o seu ambiente que não afetam negativamente a produtividade dos seus utilizadores. 

Para obter mais informações, consulte [o Microsoft Secure Score](https://docs.microsoft.com/microsoft-365/security/mtp/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Aumentar o nível de proteção contra malware no correio

O ambiente do Seu Office 365 ou Microsoft 365 inclui proteção contra malware. Pode aumentar esta proteção bloqueando anexos com tipos de ficheiros que são normalmente utilizados para malware. Para aumentar a proteção contra malware no e-mail:
  
1. Vá [https://protection.office.com](https://protection.office.com) e inscreva-se com as credenciais da sua conta de administração. 
    
2. No &amp; Centro de Conformidade de Segurança, no painel de navegação à esquerda, sob **gestão de ameaças,** escolha **Política** \> **Anti-Malware**.
    
3. Clique duas vezes na política padrão para editar esta política em toda a empresa.
    
4. Selecione **Definições**.
    
5. Sob **o filtro de tipos de acessórios comuns,** selecione **On**. Os tipos de ficheiros que estão bloqueados estão listados na janela diretamente por baixo deste controlo. Certifique-se de que adiciona estes tipos de ficheiros:
   - ade, adp, ani, bas, morcego, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif, pif, pif, pif,  <br/> 
   
   Se necessário, pode adicionar ou eliminar tipos de ficheiros mais tarde.
    
6. **Selecione Save.**
    
Para obter mais informações, consulte [a proteção anti-malware.](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409)
  
## <a name="protect-against-ransomware"></a>Proteja contra ransomware

O ransomware restringe o acesso aos dados encriptando ficheiros ou bloqueando ecrãs de computador. Em seguida, tenta extorquir dinheiro às vítimas pedindo "resgate", geralmente sob a forma de criptomoedas como o Bitcoin, em troca do acesso aos dados. 
  
Para proteger contra ransomware, crie uma ou mais regras de fluxo de correio para bloquear extensões de ficheiros que são normalmente usadas para ransomware. (Adicionou estas regras no [aumento do nível de proteção contra malware no passo do correio.)](#raise-the-level-of-protection-against-malware-in-mail) Também pode alertar os utilizadores que recebem estes anexos por e-mail.

Além dos ficheiros que bloqueou no passo anterior, é uma boa prática criar uma regra para alertar os utilizadores antes de abrir anexos de ficheiros do Office que incluem macros. O ransomware pode ser escondido dentro de macros, por isso avisa os utilizadores para não abrirem estes ficheiros a pessoas que não conhecem.

Para criar uma regra de transporte de correio:
  
1. Vá ao centro de administração em <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> , e escolha **Admin centers** \> **Exchange**.
    
2. Na categoria **de fluxo de correio,** selecione **regras**.
    
3. Selecione **+** e, em seguida, **selecione Criar uma nova regra**.
    
4. Selecione **Mais opções** na parte inferior da caixa de diálogo para ver o conjunto completo de opções. 
    
5. Aplique as definições na tabela seguinte para a regra. Utilize os valores predefinidos para o resto das definições, a não ser que pretenda alterá-los.
    
6. Selecione **Guardar**.
    
|**Definição**|**Avise os utilizadores antes de abrir anexos de ficheiros do Office**||
|:-----|:-----|:-----|
|Name  <br/> |Regra anti-ransomware: avise os utilizadores  <br/>  |
|Aplique esta regra se . . . .  <br/> |Qualquer anexo. . . correspondência de extensão de ficheiros . . .  <br/> |
|Especificar palavras ou frases  <br/> |Adicione estes tipos de ficheiros:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm  <br/>|
|Faça o seguinte. . .  <br/> |Notifique o destinatário com uma mensagem  <br/> |
|Fornecer texto de mensagem  <br/> |Não abra este tipo de ficheiros a pessoas que não conhece, pois podem conter macros com código malicioso.  <br/> |
   
Para obter mais informações, consulte:
  
- [Como lidar com ransomware](https://go.microsoft.com/fwlink/?linkid=2016501)
    
- [Restaurar o seu OneDrive](https://support.microsoft.com/office/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Pare de reencaminhar automaticamente para e-mail

Os hackers que tenham acesso à caixa de correio de um utilizador podem roubar correio, definindo a caixa de correio para enviar automaticamente o e-mail. Isto pode acontecer mesmo sem a consciência do utilizador. Para evitar que isto aconteça, configuure uma regra de fluxo de correio. 
  
Para criar uma regra de transporte de correio, veja [este pequeno vídeo](https://support.microsoft.com/office/f9d693ba-5c78-47c0-b156-8e461e062aa7) ou siga estes passos:
  
1. No centro de administração Microsoft 365, selecione **Admin centers** \> **Exchange**.
    
2. Na categoria **de fluxo de correio,** selecione **regras**.
    
3. Selecione **+** e, em seguida, **selecione Criar uma nova regra**.
    
4. Para ver todas as opções, selecione **Mais opções** na parte inferior da caixa de diálogo. 
    
5. Aplique as definições na tabela seguinte. Utilize os valores predefinidos para o resto das definições, a não ser que pretenda alterá-los.
    
6. Selecione **Guardar**.
    
|**Definição**|**Avise os utilizadores antes de abrir anexos de ficheiros do Office**|
|:-----|:-----|
|Name  <br/> |Impedir o encaminhamento automático de e-mail para domínios externos  <br/> |
|Aplique esta regra se...  <br/> |O remetente. . . é externo/interno. . . Dentro da organização  <br/> |
|Adicionar condição  <br/> |As propriedades da mensagem. . . incluir o tipo de mensagem . . . Auto-para-frente  <br/> |
|Faça o seguinte...  <br/> |Bloqueie a mensagem. . . rejeitar a mensagem e incluir uma explicação.  <br/> |
|Fornecer texto de mensagem  <br/> |O e-mail de reencaminhamento automático para fora desta organização é impedido por razões de segurança.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Proteja o seu e-mail de ataques de phishing

Se configurar um ou mais domínios personalizados para o ambiente Office 365 ou Microsoft 365, pode configurar uma proteção anti-phishing direcionada. A proteção anti-phishing DA ATP, parte do Office 365 Advanced Threat Protection, pode ajudar a proteger a sua organização de ataques de phishing baseados em imitação maliciosa e outros ataques de phishing. Se ainda não configuraste um domínio personalizado, não precisas de fazer isto.
  
Recomendamos que inicie com esta proteção criando uma política para proteger os seus utilizadores mais importantes e o seu domínio personalizado. 

Para criar uma política anti-phishing ATP, assista [a este vídeo de treino curto,](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)ou complete os seguintes passos:
  
1. Aceda a [https://protection.office.com](https://protection.office.com). 
    
2. No &amp; Centro de Conformidade de Segurança, no painel de navegação à esquerda, sob **gestão de ameaças,** escolha **a Política**.
    
3. Na página **Política,** escolha **anti-phishing ATP.**
    
4. Na página **Anti-phishing,** selecione **+ Criar**. Um assistente lança-o através da definição da sua política anti-phishing.
    
5. Especifique o nome, descrição e configurações da sua política como recomendado na tabela seguinte. Para mais detalhes, consulte [Saiba mais sobre as opções de política anti-phishing ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies#learn-about-atp-anti-phishing-policy-options). 
    
6. Depois de rever as suas definições, escolha **Criar esta política** ou **Guardar,** conforme apropriado.
    

|**Definição ou opção**<br/>|**Definição recomendada** <br/>|
|:-----|:-----|
|Name  <br/> |Domínio e pessoal de campanha mais valioso  <br/> |
|Descrição  <br/> |Certifique-se de que o pessoal mais importante e o nosso domínio não estão a ser personificados.  <br/> |
|Adicionar utilizadores para proteger  <br/> |**Selecione + Adicione uma condição, o destinatário é**. Digite os nomes de utilizador ou introduza o endereço de e-mail do candidato, gestor de campanha e outros membros importantes do pessoal. Pode adicionar até 20 endereços internos e externos que pretende proteger da personificação.  <br/> |
|Adicionar domínios para proteger  <br/> |**Selecione + Adicione uma condição, o domínio do destinatário é**. Introduza o domínio personalizado associado à subscrição microsoft 365, se tiver definido um. Pode introduzir mais do que um domínio.  <br/> |
|Escolha ações  <br/> |Se o e-mail for enviado por um utilizador personificado: Escolha **redirecionar a mensagem para outro endereço de e-mail**e, em seguida, digitar o endereço de e-mail do administrador de segurança; por exemplo, *Alice <span> <span> @contoso.com*. Se o e-mail for enviado por um domínio personificado: Escolha **a mensagem de quarentena**.  <br/> |
|Inteligência da caixa de correio  <br/> |Por predefinição, a inteligência da caixa de correio é selecionada quando cria uma nova política anti-phishing. Deixe esta definição **On** para obter os melhores resultados.  <br/> |
|Adicionar remetentes e domínios fidedignos  <br/> |Aqui pode adicionar o seu próprio domínio, ou quaisquer outros domínios fidedignos.  <br/> |
|Aplicado a  <br/> |Selecione **O domínio do destinatário é**. Em **qualquer um destes**, selecione **Escolha**. Selecione **+ Adicionar**. Selecione a caixa de verificação ao lado do nome do domínio, por exemplo, *contoso. <span> <span> com*, na lista e, em seguida, **selecione Add**. Selecione **Feito**.  <br/> |
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Proteger contra anexos e ficheiros maliciosos com anexos ATP Safe

As pessoas enviam, recebem e partilham anexos regularmente, tais como documentos, apresentações, folhas de cálculo e muito mais. Nem sempre é fácil dizer se um anexo é seguro ou malicioso apenas olhando para uma mensagem de e-mail. O Office 365 Advanced Threat Protection inclui a proteção do apSA Safe Attachment, mas esta proteção não é ligada por defeito. Recomendamos que crie uma nova regra para começar a utilizar esta proteção. Esta proteção estende-se a ficheiros em SharePoint, OneDrive e Microsoft Teams.
  
Para criar uma política de fixação segura ATP, veja [este pequeno vídeo](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)ou complete os seguintes passos:
  
1. Vá [https://protection.office.com](https://protection.office.com) para, e inscreva-se na sua conta de administração. 
    
2. No &amp; Centro de Conformidade de Segurança, no painel de navegação à esquerda, sob **gestão de ameaças,** escolha **a Política**.
    
3. Na página Política, escolha **anexos seguros ATP.**
    
4. Na página De anexos Safe, aplique esta proteção de forma geral selecionando a caixa de verificação **DE Turn on ATP para SharePoint, OneDrive e Microsoft Teams.** 
    
5. Selecione **+** para criar uma nova política. 
    
6. Aplique as definições na tabela seguinte. 
    
7. Depois de ter revisto as suas definições, escolha **Criar esta política** ou **Guardar,** conforme apropriado.
    

|**Definição ou opção**|**Definição recomendada** <br/>|
|:-----|:-----|
|Name  <br/> |Bloqueie e-mails atuais e futuros com malware detetado.  <br/> |
|Descrição  <br/> |Bloqueie e-mails e anexos atuais e futuros com malware detetado.  <br/> |
|Guardar anexos desconhecidos resposta de malware  <br/> |Selecione **Bloco - Bloqueie os e-mails e anexos atuais e futuros com malware detetado.**  <br/> |
|Redirecione o acessório na deteção  <br/> |Ativar a reorientação (selecione esta caixa) Introduza a conta de administração ou uma configuração da caixa de correio para quarentena.          Aplique a seleção acima se ocorrer uma verificação de malware para os anexos vezes fora ou se ocorrer erro (selecione esta caixa).  <br/> |
|Aplicado a  <br/> |O domínio do destinatário é . . . selecione o seu domínio.  <br/> |
   
Para obter mais informações, consulte [configurar as políticas anti-phishing DO Office 365 ATP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies)
  
## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Proteja contra ataques de phishing com LIGAções Seguras ATP

Os hackers às vezes escondem sites maliciosos em links em e-mails ou outros ficheiros. O Office 365 ATP Safe Links (ATP Safe Links), parte do Office 365 Advanced Threat Protection, pode ajudar a proteger a sua organização fornecendo a verificação de tempo de clique dos endereços web (URLs) em mensagens de correio eletrónico e documentos do Office. A proteção é definida através das políticas ATP Safe Links.
  
Recomendamos que faça o seguinte:
  
- Modifique a política de predefinição para aumentar a proteção.
    
- Adicione uma nova política direcionada a todos os destinatários do seu domínio.
    
Para configurar o ATP Safe Links, assista [a este vídeo de treino curto,](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)ou complete os seguintes passos:
  
1. Vá [https://protection.office.com](https://protection.office.com) para, e inscreva-se na sua conta de administração. 
    
2. No &amp; Centro de Conformidade de Segurança, no painel de navegação à esquerda, sob **gestão de ameaças,** escolha **a Política**.
    
3. Na página Política, escolha **LINKS SEGUROS ATP**.
    
Para modificar a política de incumprimento:
  
1. Na página 'Links Seguro', ao abrigo **de Políticas aplicáveis a toda a organização,** selecione a política **Padrão.** 
    
2. Em **Definições que se aplicam a conteúdos exceto e-mail**, selecione **Microsoft 365 Apps for enterprise, Office for iOS e Android**.
    
3. Selecione **Guardar**. 
    
Para criar uma nova política direcionada a todos os destinatários do seu domínio:
  
1. Na página 'Ligações Seguras', ao abrigo **de Políticas aplicáveis a toda a organização,** selecione **+** para criar uma nova política. 
    
2. Aplique as definições listadas na tabela seguinte.
    
3. Selecione **Guardar**. 

|**Definição ou opção**|**Definição recomendada** <br/>|
|:-----|:-----|
|Name  <br/> |Política de ligações seguras para todos os destinatários no domínio  <br/> |
|Selecione a ação para URLs potencialmente maliciosos desconhecidos em mensagens  <br/> |Selecione **On - URLs serão reescritos e verificados contra uma lista de links maliciosos conhecidos quando o utilizador clicar no link**.  <br/> |
|Utilize anexos seguros para digitalizar conteúdo transferível  <br/> |Selecione esta caixa.  <br/> |
|Aplicado a  <br/> |O domínio do destinatário é . . . selecione o seu domínio.  <br/> |
   
Para mais informações, consulte [as ligações seguras ATP do Office 365.](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409)

## <a name="go-to-intune-admin-center"></a>Vá ao Centro de Administração Intune

1. Inscreva-se no [portal Azure](https://portal.azure.com/).

2. Selecione **Todos os serviços** e *digite inTune* na **Caixa de Busca.**

3. Assim que os resultados aparecerem, selecione o início ao lado do **Microsoft Intune** para torná-lo um favorito e fácil de encontrar mais tarde.

Além do centro de administração, pode utilizar o Intune para se inscrever e gerir os dispositivos da sua organização. Para obter mais informações, consulte [Capabilities por método de inscrição para dispositivos Windows](https://docs.microsoft.com/intune/enrollment/enrollment-method-capab) e [opções de inscrição para dispositivos geridos pela Intune](https://docs.microsoft.com/intune/enrollment-options).
