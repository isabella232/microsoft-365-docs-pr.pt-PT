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
description: Configure o Office 365 Advanced Threat Protection e proteja dados confidenciais.
ms.openlocfilehash: 1827b70f1e4d78a072753390c1a99d7cb4bd5cfd
ms.sourcegitcommit: 70e920f76526f47fc849df615de4569e0ac2f4be
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/07/2019
ms.locfileid: "38030770"
---
# <a name="increase-threat-protection"></a>Aumentar a proteção contra ameaças

Este artigo ajuda você a aumentar a proteção em sua assinatura Microsoft 365 para proteger contra phishing, malware e outras ameaças. Essas recomendações são apropriadas para organizações com maior necessidade de segurança, como escritórios de advocacia e clínicas de saúde.

Antes de começar, verifique sua Pontuação Segura do Office 365. O Office 365 Secure Score analisa a segurança da organização do Office 365 com base em suas atividades e configurações regulares de segurança e atribui uma pontuação. Comece tomando nota de sua pontuação atual. Tomar as ações recomendadas neste artigo aumenta sua pontuação. O objetivo não é alcançar a pontuação máxima, mas estar ciente das oportunidades de proteger seu ambiente que não afetam negativamente a produtividade de seus usuários. 

Para mais informações, consulte o [Microsoft Secure Score](https://docs.microsoft.com/office365/securitycompliance/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Aumentar o nível de proteção contra malware no correio

Seu ambiente Office 365 ou Microsoft 365 inclui proteção contra malware, mas você pode aumentar essa proteção bloqueando anexos com tipos de arquivos que são comumente usados para malware. Para aumentar a proteção contra malware no e-mail:
  
1. Acesse [https://protection.office.com](https://protection.office.com) e entre com as credenciais da conta de administração. 
    
2. No Office 365 &amp; Security Compliance Center, no painel de navegação à esquerda, gerenciamento de **ameaças,** escolha **Política** \> **Antimalware.**
    
3. Clique duas vezes na política padrão para eitar essa política em toda a empresa.
    
4. Clique **em configurações.**
    
5. **o filtro comum**dos tipos do acessório, selecione **sobre.** Os tipos de arquivo que estão bloqueados estão listados na janela diretamente abaixo desse controle.  Certifique-se de adicionar esses filetypes:
   - ade, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, vbs, wsc, wsf, wsh, exe, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, pif, vbs, wsc, wsf, wsh, exe, pif, pif, p  <br/> Você pode adicionar ou excluir os tipos de arquivos mais tarde, se necessário.
    
6. Clique **em Salvar.**
    
Para mais informações, consulte a [proteção antimalware.](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409)
  
## <a name="protect-against-ransomware"></a>Proteger contra ransomware

Ransomware restringe o acesso aos dados criptografando arquivos ou bloqueando telas de computador. Em seguida, ele tenta extorquir dinheiro das vítimas, pedindo "resgate", geralmente em forma de criptomoedas como bitcoin, em troca de acesso aos dados. 
  
Você pode proteger contra ransomware criando uma ou mais regras de fluxo de correio para bloquear extensões de arquivos que são comumente usadas para ransomware (estas foram adicionadas no aumento do nível de proteção contra malware na etapa do [e-mail),](#raise-the-level-of-protection-against-malware-in-mail) ou para avisar os usuários que recebem estes anexos no e-mail.

Além dos arquivos que você bloqueou na etapa anterior, também é uma boa prática criar uma regra para avisar os usuários antes de abrir anexos de arquivos do Office que incluem macros. Ransomware pode ser escondido dentro macros, por isso vamos avisar os usuários para não abrir esses arquivos de pessoas que não conhecem.

Criar uma regra de transporte por correspondência:
  
1. Vá para o centro <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> de administração e escolha **Centros Admin** \> **Exchange**.
    
2. Na categoria de fluxo de **correio,** clique **em regras.**
    
3. Clique **+** e, em seguida, clique **criar uma nova regra**.
    
4. Clique em **mais opções** na parte inferior da caixa de diálogo para ver o conjunto completo de opções. 
    
5. Aplique as configurações na tabela a seguir para a regra. Deixe o resto das configurações no padrão, a menos que você queira alterá-los.
    
6. Clique em **Guardar**.
    
|**Definição**|**Avisar os usuários antes de abrir anexos de arquivos do Office**||
|:-----|:-----|:-----|
|Name  <br/> |Regra anti-ransomware: avise os usuários  <br/>  |
|Aplique esta regra se . . .  <br/> |Qualquer anexo . . . correspondências de extensão de arquivo . . .  <br/> |
|Especifique palavras ou frases  <br/> |Adicione esses tipos de arquivos:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm  <br/>|
|Faça o seguinte . . .  <br/> |Notifique o destinatário com uma mensagem  <br/> |
|Fornecer texto de mensagem  <br/> |Não abra esse tipo de arquivos de pessoas que você não conhece porque eles podem conter macros com código malicioso.  <br/> |
   
Para obter mais informações, consulte:
  
- [Como lidar com ransomware](https://go.microsoft.com/fwlink/?linkid=2016501&amp;clcid=0x409)
    
- [Restaure o OneDrive](https://support.office.com/article/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)
    


## <a name="stop-auto-forwarding-for-email"></a>Pare de avançar automaticamente para e-mail

Hackers que têm acesso à caixa de correio de um usuário podem roubar seu e-mail, definindo a caixa de correio para encaminhar automaticamente o e-mail. Isso pode acontecer mesmo sem a consciência do usuário. Você pode evitar que isso aconteça configurando uma regra de fluxo de correio. 
  
Para criar uma regra de transporte por correspondência, assista a [este vídeo curto](https://support.office.com/article/f9d693ba-5c78-47c0-b156-8e461e062aa7) ou siga essas etapas:
  
1. No centro de administração microsoft 365, clique em **centros** \> de administração **Exchange.**
    
2. Na categoria de fluxo de **correio,** clique **em regras.**
    
3. Clique **+** e, em seguida, clique **criar uma nova regra**.
    
4. Clique em **mais opções** na parte inferior da caixa de diálogo para ver o conjunto completo de opções. 
    
5. Aplique as configurações na tabela a seguir. Deixe o resto das configurações no padrão, a menos que você queira alterá-los.
    
6. Clique em **Guardar**.
    
|**Definição**|**Avisar os usuários antes de abrir anexos de arquivos do Office**|
|:-----|:-----|
|Name  <br/> |Impedir o encaminhar automaticamente de e-mail para domínios externos  <br/> |
|Aplique esta regra se ...  <br/> |O remetente . . . é externo/interno. . . Dentro da organização  <br/> |
|Adicionar condição  <br/> |A mensagem é propriedade. . . incluir o tipo de mensagem . . . Auto-forward  <br/> |
|Faça o seguinte ...  <br/> |Bloqueie a mensagem. . . rejeitar a mensagem e incluir uma explicação.  <br/> |
|Fornecer texto de mensagem  <br/> |O e-mail de auto-encaminhar fora desta organização é evitado por razões de segurança.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Proteger seu e-mail contra ataques de phishing

Se você configurou um ou mais domínios personalizados para o seu ambiente Office 365 ou Microsoft 365, poderá configurar a proteção antiphishing direcionada. A proteção antiphishing atp, parte do Office 365 Advanced Threat Protection, pode ajudar a proteger sua organização de ataques de phishing baseados em identidade maliciosa e outros ataques de phishing. Se você ainda não configurou um domínio personalizado, não precisa fazer isso.
  
Recomendamos que você comece com essa proteção criando uma política para proteger seus usuários mais importantes e seu domínio personalizado. 

  
Para criar uma política anti-phishing atp, assista [a este vídeo de treinamento curto](https://support.office.com/article/86c425e1-1686-430a-9151-f7176cce4f2c)ou complete as seguintes etapas:
  
1. Aceda a [https://protection.office.com](https://protection.office.com). 
    
2. No Office 365 &amp; Security Compliance Center, no painel de navegação à esquerda, gestão de **ameaças,** escolha **Política.**
    
3. Na página **política,** escolha **atp anti-phishing**.
    
4. Na página **anti-phishing,** selecione **+ Crie**. Um assistente lança que o incomode através da definição de sua política anti-phishing.
    
5. Especifique o nome, a descrição e as configurações para sua política, conforme recomendado no gráfico abaixo. [Veja as opções](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies#learn-about-atp-anti-phishing-policy-options) de política antiphishing da ATP para obter mais detalhes. 
    
6. Depois de revisar suas configurações, escolha **criar essa política** ou **economizar,** conforme apropriado.
    

|**Configuração ou opção**<br/>|**Configuração recomendada** <br/>|
|:-----|:-----|
|Name  <br/> |Domínio e pessoal de campanha mais valioso  <br/> |
|Descrição  <br/> |Certifique-se de que a equipe mais importante e nosso domínio não estão sendo personificados.  <br/> |
|Adicionar usuários para proteger  <br/> |Selecione **+ Adicione uma condição, o destinatário é.** Digite nomes de usuário ou digite o endereço de e-mail do candidato, gerente de campanha e outros membros importantes da equipe. Você pode adicionar até 20 endereços internos e externos que você deseja proteger da representação.  <br/> |
|Adicionar domínios para proteger  <br/> |Selecione **+ Adicione uma condição, o domínio do destinatário é.** Insira o domínio personalizado associado à assinatura Microsoft 365, se você definiu um. Você pode inserir mais de um domínio.  <br/> |
|Escolha ações  <br/> |Se o e-mail for enviado por um usuário imitado: escolha **a mensagem de redirecionamento para outro endereço de e-mail**e, em seguida, digite o endereço de e-mail do administrador de segurança; por exemplo, *<span><span>Alice @contoso.com*.          Se o e-mail for enviado por um domínio imitado: escolha **a mensagem de quarentena.**  <br/> |
|Inteligência da caixa de correio  <br/> |Por padrão, a inteligência da caixa de correio é selecionada quando você cria uma nova política antiphishing. Deixe esta configuração **para** obter melhores resultados.  <br/> |
|Adicionar remetentes e domínios confiáveis  <br/> |Aqui você pode adicionar seu próprio domínio, ou quaisquer outros domínios confiáveis.  <br/> |
|Aplicado a  <br/> |Selecione **o domínio destinatário é**. **qualquer um destes,** **selecione Escolha**. Selecione **+ Adicionar**. Selecione a caixa de seleção ao lado do nome do domínio, por exemplo, *contoso.<span> <span>com,* na lista, e, em seguida, **selecione Adicionar**. Selecione **Feito**.  <br/> |
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Proteger contra anexos e arquivos maliciosos com anexos seguros ATP

As pessoas enviam, recebem e compartilham anexos regularmente, como documentos, apresentações, planilhas e muito mais. Nem sempre é fácil dizer se um anexo é seguro ou malicioso apenas olhando para uma mensagem de e-mail. O Office 365 Advanced Threat Protection inclui proteção de anexo seguro ATP, mas essa proteção não é ativada por padrão. Recomendamos que você crie uma nova regra para começar a usar essa proteção. Essa proteção se estende aos arquivos do SharePoint, OneDrive e Microsoft Teams.
  
Para criar uma política de anexo seguro ATP, assista a [este vídeo curto](https://support.office.com/article/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)ou complete as seguintes etapas:
  
1. Vá [https://protection.office.com](https://protection.office.com) e entre com sua conta administrativa. 
    
2. No Office 365 &amp; Security Compliance Center, no painel de navegação à esquerda, gestão de **ameaças,** escolha **Política.**
    
3. Na página política, escolha **anexos seguros ATP**.
    
4. Na página de anexos Safe, aplique essa proteção amplamente selecionando a caixa de seleção **do Turn on ATP para SharePoint, OneDrive e Microsoft Teams.** 
    
5. Selecione **+** criar uma nova política. 
    
6. Aplique as configurações na tabela a seguir. 
    
7. Depois de revisar suas configurações, escolha **criar essa política** ou **economizar,** conforme apropriado.
    

|**Configuração ou opção**|**Configuração recomendada** <br/>|
|:-----|:-----|
|Name  <br/> |Bloqueie e-mails atuais e futuros com malware detectado.  <br/> |
|Descrição  <br/> |Bloqueie e-mails e anexos atuais e futuros com malware detectado.  <br/> |
|Salvar anexos resposta de malware desconhecida  <br/> |Selecione **Bloco - Bloqueie os e-mails e anexos atuais e futuros com malware detectado.**  <br/> |
|Redirecionar o anexo na detecção  <br/> |Ativar o redirecionamento (selecione esta caixa) Digite a conta de administração ou uma configuração de caixa de correio para quarentena.          Aplique a seleção acima se a digitalização de malware para anexos ocorrer vezes ou ocorrer erro (selecione esta caixa).  <br/> |
|Aplicado a  <br/> |O domínio destinatário é . . . selecione seu domínio.  <br/> |
   
Para mais informações, consulte as [políticas antiphishing do Office 365 ATP](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409).
  


## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Proteger contra ataques de phishing com links seguros atp

Hackers às vezes escondem sites maliciosos em links em e-mail ou outros arquivos. O Office 365 ATP Safe Links (ATP Safe Links), parte do Office 365 Advanced Threat Protection, pode ajudar a proteger sua organização fornecendo verificação de tempo de clique de endereços da web (URLs) em mensagens de e-mail e documentos do Office. A proteção é definida por meio de políticas de Links Seguros da ATP.
  
Recomendamos que você faça o seguinte:
  
- Modifique a política de inadimplência para aumentar a proteção.
    
- Adicione uma nova política direcionada a todos os destinatários em seu domínio.
    
Para configurar o ATP Safe Links, assista [a este vídeo](https://support.office.com/article/61492713-53c2-47da-a6e7-fa97479e97fa)de treinamento curto ou complete as seguintes etapas:
  
1. Vá [https://protection.office.com](https://protection.office.com) e entre com sua conta administrativa. 
    
2. No Office 365 &amp; Security Compliance Center, no painel de navegação à esquerda, gestão de **ameaças,** escolha **Política.**
    
3. Na página política, escolha **ATP Safe Links**.
    
Para modificar a política padrão:
  
1. Na página de links Seguros, **políticas que se aplicam a toda a organização,** selecione a política **padrão.** 
    
2. Em **configurações que se aplicam ao conteúdo, exceto e-mail,** selecione **Office 365 ProPlus, Office para iOS e Android**.
    
3. Clique em **Guardar**. 
    
Para criar uma nova política direcionada a todos os destinatários em seu domínio:
  
1. Na página de links Seguros, **políticas que se aplicam a toda a organização,** clique **+** para criar uma nova política. 
    
2. Aplique as configurações listadas na tabela a seguir.
    
3. Clique em **Guardar**. 

|**Configuração ou opção**|**Configuração recomendada** <br/>|
|:-----|:-----|
|Name  <br/> |Política de links seguros para todos os destinatários no domínio  <br/> |
|Selecione a ação para URLs potencialmente maliciosos desconhecidos em mensagens  <br/> |Selecione **On - URLs serão reescritos e verificados em uma lista de links maliciosos conhecidos quando o usuário clicar no link**.  <br/> |
|Use anexos seguros para digitalizar conteúdo para download  <br/> |Selecione esta caixa.  <br/> |
|Aplicado a  <br/> |O domínio destinatário é . . . selecione seu domínio.  <br/> |
   
Para mais informações, consulte [os links seguros do Office 365 ATP.](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409)

## <a name="go-to-intune-admin-center"></a>Vá para o centro de administração Intune

1. Entre no [portal Azure.](https://portal.azure.com/)

2. Selecione **todos os serviços** e digite *Intune* na Caixa de **Pesquisa**.

3. Depois que os resultados exibirem, clique no início ao lado do **Microsoft Intune** para torná-lo um favorito e fácil de encontrar mais tarde.

Além do centro de administração, você pode usar o Intune para se inscrever e gerenciar os dispositivos da sua organização. Para obter mais informações, consulte os Recursos por método de [inscrição para dispositivos Windows](https://docs.microsoft.com/intune/enrollment-method-capabs) e opções de inscrição para [dispositivos gerenciados pela Intune](https://docs.microsoft.com/intune/enrollment-options).
