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
ms.custom:
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
description: Configure a proteção avançada contra ameaças do Office 365 e proteja os dados confidenciais.
ms.openlocfilehash: fb63ca7e3cf38ecf31aab98e425b02e8b9983bf8
ms.sourcegitcommit: 4d5e4cb3fa3ab45ad15f103c720c77277b22fc23
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/22/2019
ms.locfileid: "37636758"
---
# <a name="increase-threat-protection"></a>Aumente a proteção contra ameaças

Este artigo ajuda você a aumentar a proteção em sua assinatura do Microsoft 365 para proteger contra phishing, malware e outras ameaças. Essas recomendações são apropriadas para organizações com maior necessidade de segurança, como escritórios de advocacia e clínicas de saúde.

Antes de começar, verifique sua pontuação segura do Office 365. A pontuação segura do Office 365 analisa a segurança da organização do Office 365 com base nas suas atividades regulares e nas configurações de segurança e atribui uma pontuação. Comece tomando nota da sua pontuação atual. Tomar as ações recomendadas neste artigo aumenta sua pontuação. O objetivo não é alcançar a pontuação máxima, mas estar ciente das oportunidades para proteger seu ambiente que não afetam negativamente a produtividade de seus usuários. 

Para obter mais informações, consulte [Microsoft Secure Score](https://docs.microsoft.com/en-us/office365/securitycompliance/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Aumente o nível de proteção contra malware no mail

Seu ambiente do Office 365 ou Microsoft 365 inclui proteção contra malware, mas você pode aumentar essa proteção bloqueando anexos com tipos de arquivo que são comumente usados para malware. Para aumentar a proteção contra malware no e-mail:
  
1. Aceda a [https://protection.office.com](https://protection.office.com) e inicie sessão com as credenciais da sua conta de administrador. 
    
2. No centro de conformidade de &amp; segurança do Office 365, no painel de navegação esquerdo, em **Gerenciamento de ameaças**, escolha **Antimalware** **de política** \> .
    
3. Clique duas vezes na política padrão para editar essa política de toda a empresa.
    
4. Clique em **configurações**.
    
5. Em **filtro de tipos de anexos comuns**, selecione **ativado**. Os tipos de arquivo que estão bloqueados são listados na janela diretamente abaixo desse controle.  Certifique-se de adicionar estes tipos de arquivos:
   - Ade, ADP, Ani, Bas, bat, CHM, cmd, com, CPL, CRT, HLP, HT, HTA, inf, ins, ISP, Job, js, jse, lnk, MDA, mdb, MDE, MDZ, MSc, MSI, MSP, MST, PCD, Reg, SCR, SCT, SHS, URL, VB, vbe, vbs, WSC, wsf, WSH, exe, PIF  <br/> Você pode adicionar ou excluir tipos de arquivo posteriormente, se necessário.
    
6. Clique em **salvar.**
    
Para obter mais informações, consulte [proteção contra malware](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409).
  
## <a name="protect-against-ransomware"></a>Proteja-se contra ransomware

O ransomware restringe o acesso aos dados criptografando arquivos ou bloqueando telas de computador. Em seguida, ele tenta extorc dinheiro das vítimas, pedindo "resgate", geralmente em forma de criptomoedas como Bitcoin, em troca de acesso aos dados. 
  
Você pode proteger contra ransomware criando uma ou mais regras de fluxo de email para bloquear extensões de arquivo que são comumente usadas para ransomware (elas foram adicionadas no [aumento do nível de proteção contra malware na etapa de email](#raise-the-level-of-protection-against-malware-in-mail) ) ou para avisar os usuários que recebem esses anexos no e-mail.

Além dos arquivos que você bloqueou na etapa anterior, também é uma boa prática criar uma regra para avisar os usuários antes de abrir anexos de arquivo do Office que incluem macros. Ransomware pode ser escondido dentro de macros, por isso vamos avisar os usuários para não abrir esses arquivos de pessoas que não conhecem.

Para criar uma regra de transporte de email:
  
1. Vá para o <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> centro de administração e escolha **admin centers** \> **Exchange**.
    
2. Na categoria de **fluxo de email** , clique em **regras**.
    
3. Clique **+** em e, em seguida, clique em **criar uma nova regra**.
    
4. Clique em **mais opções** na parte inferior da caixa de diálogo para ver o conjunto completo de opções. 
    
5. Aplique as configurações na tabela a seguir para a regra. Deixe o restante das configurações no padrão, a menos que você queira alterá-los.
    
6. Clique em **Guardar**.
    
|**Definição**|**Avisar os usuários antes de abrir anexos de arquivos do Office**||
|:-----|:-----|:-----|
|Name  <br/> |Regra anti-ransomware: avisar os usuários  <br/>  |
|Aplique esta regra se. . .  <br/> |Qualquer apego. . . extensão de ficheiro corresponde. . .  <br/> |
|Especificar palavras ou frases  <br/> |Adicione esses tipos de arquivo:  <br/> dotm, docm, xlsm, sltm, xla, xlam, XLL, pptm, potm, ppam, ppsm, sldm  <br/>|
|Faça o seguinte. . .  <br/> |Notificar o destinatário com uma mensagem  <br/> |
|Forneça o texto da mensagem  <br/> |Não abra esses tipos de arquivos de pessoas que você não conhece porque eles podem conter macros com código mal-intencionado.  <br/> |
   
Para obter mais informações, consulte:
  
- [Como lidar com ransomware](https://go.microsoft.com/fwlink/?linkid=2016501&amp;clcid=0x409)
    
- [Restaurar o OneDrive](https://support.office.com/article/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)
    


## <a name="stop-auto-forwarding-for-email"></a>Interromper o encaminhamento automático para e-mail

Os hackers que obtêm acesso à caixa de correio de um usuário podem roubar seu email definindo a caixa de correio para encaminhar emails automaticamente. Isso pode acontecer mesmo sem a consciência do usuário. Você pode impedir que isso aconteça Configurando uma regra de fluxo de email. 
  
Para criar uma regra de transporte de email, Assista a [este vídeo curto](https://support.office.com/article/f9d693ba-5c78-47c0-b156-8e461e062aa7) ou siga estas etapas:
  
1. No centro de administração do Microsoft 365, clique em **troca de** **centros** \> de administração.
    
2. Na categoria de **fluxo de email** , clique em **regras**.
    
3. Clique **+** em e, em seguida, clique em **criar uma nova regra**.
    
4. Clique em **mais opções** na parte inferior da caixa de diálogo para ver o conjunto completo de opções. 
    
5. Aplique as configurações na tabela a seguir. Deixe o restante das configurações no padrão, a menos que você queira alterá-los.
    
6. Clique em **Guardar**.
    
|**Definição**|**Avisar os usuários antes de abrir anexos de arquivos do Office**|
|:-----|:-----|
|Name  <br/> |Impedir o encaminhamento automático de e-mail para domínios externos  <br/> |
|Aplique esta regra se...  <br/> |O remetente. . . é externo/interno. . . Dentro da organização  <br/> |
|Adicionar condição  <br/> |As propriedades de mensagem. . . incluir o tipo de mensagem. . . Avanço automático  <br/> |
|Faça o seguinte...  <br/> |Bloqueie a mensagem. . . rejeitar a mensagem e incluir uma explicação.  <br/> |
|Forneça o texto da mensagem  <br/> |O envio automático de emails fora dessa organização é impedido por motivos de segurança.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Proteja seu e-mail contra ataques de phishing

Se você configurou um ou mais domínios personalizados para seu ambiente do Office 365 ou Microsoft 365, poderá configurar a proteção antiphishing direcionada. A proteção antiphishing do ATP, parte da proteção avançada contra ameaças do Office 365, pode ajudar a proteger sua organização contra ataques de phishing baseados em representação maliciosas e outros ataques de phishing. Se você não configurou um domínio personalizado, não precisará fazer isso.
  
Recomendamos que você comece a usar essa proteção criando uma política para proteger seus usuários mais importantes e seu domínio personalizado. 

  
Para criar uma política de antiphishing do ATP, Assista a [este vídeo de treinamento curto](https://support.office.com/article/86c425e1-1686-430a-9151-f7176cce4f2c)ou conclua as seguintes etapas:
  
1. Aceda a [https://protection.office.com](https://protection.office.com). 
    
2. No centro de conformidade de &amp; segurança do Office 365, no painel de navegação esquerdo, em **Gerenciamento de ameaças**, escolha **política**.
    
3. Na página **política** , escolha **ATP anti-phishing**.
    
4. Na página **anti-phishing** , selecione **+ criar**. Um assistente é iniciado que orienta você na definição de sua política de antiphishing.
    
5. Especifique o nome, a descrição e as configurações da sua política, conforme recomendado no gráfico abaixo. Consulte [saiba mais sobre as opções de política de antiphishing do ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies#learn-about-atp-anti-phishing-policy-options) para obter mais detalhes. 
    
6. Depois de ter revisto as definições, escolha **criar esta política** ou **guardar**, conforme apropriado.
    

|**Configuração ou opção**<br/>|**Configuração recomendada** <br/>|
|:-----|:-----|
|Name  <br/> |Domínio e pessoal de campanha mais valioso  <br/> |
|Descrição  <br/> |Certifique-se de que a equipe mais importante e nosso domínio não estão sendo representados.  <br/> |
|Adicionar usuários para proteger  <br/> |Selecione **+ Adicionar uma condição, o destinatário é**. Digite os nomes de usuário ou digite o endereço de e-mail do candidato, gerente de campanha e outros membros importantes da equipe. Você pode adicionar até 20 endereços internos e externos que você deseja proteger da representação.  <br/> |
|Adicionar domínios para proteger  <br/> |Selecione **+ Adicionar uma condição, o domínio do destinatário é**. Insira o domínio personalizado associado à sua assinatura do Microsoft 365, se você definiu um. Você pode inserir mais de um domínio.  <br/> |
|Escolha ações  <br/> |Se o email for enviado por um usuário representado: escolha **redirecionar mensagem para outro endereço de email**e digite o endereço de email do administrador de segurança; por exemplo, *Alice<span><span>@contoso. com*.          Se o email for enviado por um domínio representado: escolha **mensagem de quarentena**.  <br/> |
|Inteligência de caixa de correio  <br/> |Por padrão, a inteligência de caixa de correio é selecionada quando você cria uma nova política de antiphishing. Deixe esta definição **em** para obter melhores resultados.  <br/> |
|Adicionar domínios e remetentes confiáveis  <br/> |Aqui você pode adicionar seu próprio domínio, ou quaisquer outros domínios confiáveis.  <br/> |
|Aplicado a  <br/> |Selecione **o domínio do destinatário**. Em **qualquer um desses**, selecione **escolher**. Selecione **+ Adicionar**. Marque a caixa de seleção ao lado do nome do domínio, por exemplo, *contoso.<span> com <span>*, na lista e, em seguida, selecione **Adicionar**. Selecione **concluído**.  <br/> |
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Proteja-se contra anexos e arquivos maliciosos com anexos seguros ATP

As pessoas enviam, recebem e compartilham anexos regularmente, como documentos, apresentações, planilhas e muito mais. Nem sempre é fácil dizer se um anexo é seguro ou malicioso apenas olhando para uma mensagem de e-mail. A proteção avançada contra ameaças do Office 365 inclui a proteção de anexos seguros de ATP, mas essa proteção não é ativada por padrão. Recomendamos que você crie uma nova regra para começar a usar essa proteção. Essa proteção se estende aos arquivos no SharePoint, no OneDrive e no Microsoft Teams.
  
Para criar uma política de anexo seguro de ATP, Assista a [este vídeo curto](https://support.office.com/article/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)ou conclua as seguintes etapas:
  
1. Aceda a [https://protection.office.com](https://protection.office.com) e inicie sessão com a sua conta de administrador. 
    
2. No centro de conformidade de &amp; segurança do Office 365, no painel de navegação esquerdo, em **Gerenciamento de ameaças**, escolha **política**.
    
3. Na página política, escolha **anexos seguros de ATP**.
    
4. Na página anexos seguros, aplique essa proteção amplamente selecionando a caixa de seleção **Ativar ATP para SharePoint, onedrive e Microsoft Teams** . 
    
5. Selecione **+** para criar uma nova política. 
    
6. Aplique as configurações na tabela a seguir. 
    
7. Depois de ter revisto as definições, escolha **criar esta política** ou **guardar**, conforme apropriado.
    

|**Configuração ou opção**|**Configuração recomendada** <br/>|
|:-----|:-----|
|Name  <br/> |Bloqueie e-mails atuais e futuros com malware detectado.  <br/> |
|Descrição  <br/> |Bloqueie e-mails e anexos atuais e futuros com malware detectado.  <br/> |
|Salvar anexos resposta de malware desconhecido  <br/> |Selecione **bloco-bloqueie os emails e anexos atuais e futuros com malware detectado**.  <br/> |
|Redirecionar anexo na detecção  <br/> |Habilitar redirecionamento (Selecione esta caixa) Insira a conta de administrador ou uma configuração de caixa de correio para quarentena.          Aplique a seleção acima se a verificação de malware para o tempo limite de anexos ou erro ocorrer (Selecione esta caixa).  <br/> |
|Aplicado a  <br/> |O domínio do destinatário é. . . Selecione seu domínio.  <br/> |
   
Para obter mais informações, consulte [Configurar políticas de antiphishing do Office 365 ATP](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409).
  


## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Proteja contra ataques de phishing com o ATP Safe links

Hackers, por vezes, esconder sites maliciosos em links em e-mail ou outros arquivos. O Office 365 ATP Safe links (links seguros de ATP), parte da proteção avançada contra ameaças do Office 365, pode ajudar a proteger sua organização, fornecendo verificação de tempo de clique de endereços da Web (URLs) em mensagens de email e documentos do Office. A proteção é definida por meio das políticas do ATP Safe links.
  
Recomendamos que você faça o seguinte:
  
- Modifique a política padrão para aumentar a proteção.
    
- Adicione uma nova política direcionada a todos os destinatários em seu domínio.
    
Para configurar o ATP Safe links, Assista a [este vídeo de treinamento curto](https://support.office.com/article/61492713-53c2-47da-a6e7-fa97479e97fa)ou conclua as seguintes etapas:
  
1. Aceda a [https://protection.office.com](https://protection.office.com) e inicie sessão com a sua conta de administrador. 
    
2. No centro de conformidade de &amp; segurança do Office 365, no painel de navegação esquerdo, em **Gerenciamento de ameaças**, escolha **política**.
    
3. Na página política, escolha **links seguros de ATP**.
    
Para modificar a política padrão:
  
1. Na página links seguros, em **diretivas que se aplicam a toda a organização**, selecione a política **padrão** . 
    
2. Em **configurações que se aplicam ao conteúdo, exceto e-mail**, selecione **Office 365 ProPlus, Office para IOS e Android**.
    
3. Clique em **Guardar**. 
    
Para criar uma nova política direcionada a todos os destinatários no seu domínio:
  
1. Na página links seguros, em **diretivas que se aplicam a toda a organização**, clique **+** em para criar uma nova política. 
    
2. Aplique as configurações listadas na tabela a seguir.
    
3. Clique em **Guardar**. 

|**Configuração ou opção**|**Configuração recomendada** <br/>|
|:-----|:-----|
|Name  <br/> |Política de links seguros para todos os destinatários no domínio  <br/> |
|Selecione a ação para URLs potencialmente maliciosas desconhecidas em mensagens  <br/> |Selecione **on-URLs será reescrito e verificado em relação a uma lista de links maliciosos conhecidos quando o usuário clica no link**.  <br/> |
|Usar anexos seguros para digitalizar Conteúdo transferível  <br/> |Selecione esta caixa.  <br/> |
|Aplicado a  <br/> |O domínio do destinatário é. . . Selecione seu domínio.  <br/> |
   
Para obter mais informações, consulte [links seguros do Office 365 ATP](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409).

## <a name="go-to-intune-admin-center"></a>Ir para o centro de administração do Intune

1. Entre no [portal do Azure](https://portal.azure.com/).

2. Selecione **todos os serviços** e digite no *Intune* na **caixa de pesquisa**.

3. Depois que os resultados forem exibidos, clique no início ao lado do **Microsoft Intune** para torná-lo um favorito e fácil de encontrar mais tarde.

Além do centro de administração, você pode usar o Intune para registrar e gerenciar os dispositivos da sua organização. Para obter mais informações, consulte [recursos por método de registro para dispositivos Windows](https://docs.microsoft.com/intune/enrollment-method-capabs) e [Opções de registro para dispositivos gerenciados pelo Intune](https://docs.microsoft.com/intune/enrollment-options).
