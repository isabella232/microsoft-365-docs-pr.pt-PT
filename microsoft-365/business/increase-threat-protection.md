---
title: Aumentar a proteção contra ameaças Microsoft 365 para Empresas
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: Configlige o Microsoft Defender Office 365 e proteja dados confidenciais contra phishing, software malicioso e outras ameaças.
ms.openlocfilehash: d5aad66642fc2b509ae40dc1277167deb53de6fbb0593a3dcd766062305fbd6a
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53831481"
---
# <a name="increase-threat-protection"></a>Aumentar a proteção contra ameaças

Este artigo ajuda-o a aumentar a proteção na sua subscrição Microsoft 365 proteção contra phishing, software malicial e outras ameaças. Estas recomendações são adequadas para organizações com uma necessidade crescente de segurança, como escritórios de advogados e médicos de saúde.

Antes de começar, verifique a sua Office 365 de Segurança. Office 365 A Pontuação de Segurança analisa a segurança da sua organização com base nas suas atividades regulares e definições de segurança e atribui uma pontuação. Comece por tomar nota da sua pontuação atual. Para aumentar o seu resultado, conclua as ações recomendadas neste artigo. O objetivo não é atingir o máximo de pontuações, mas estar a par das oportunidades para proteger o seu ambiente que não afetam negativamente a produtividade para os seus utilizadores.

Para obter mais informações, consulte [Pontuação de Segurança da Microsoft.](../security/defender/microsoft-secure-score.md)

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Elevar o nível de proteção contra software maliceiro no correio

O Office 365 ou Microsoft 365 seu ambiente inclui proteção contra software malictivo. Pode aumentar esta proteção ao bloquear anexos com tipos de ficheiro frequentemente utilizados para software malicioso. Para aumentar a proteção contra software malicónico no e-mail:

1. Vá para [https://protection.office.com](https://protection.office.com) e inscreva-se com as credenciais da sua conta de administrador.

2. No Centro de Conformidade de Segurança, no painel de navegação &amp; esquerdo, em Gestão de **ameaças,** selecionar  \> **Política Anti malware**.

3. Faça duplo clique na política predefinida para editar esta política para toda a empresa.

4. **Selecione Definições**.

5. Em Filtro **de Tipos de Anexo Comuns, selecione** **Ação**. Os tipos de ficheiro bloqueados são listados na janela diretamente abaixo deste controlo. Certifique-se de que adiciona estes tipos de ficheiro:

   `ade, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif`

   Se for necessário, pode adicionar ou eliminar tipos de ficheiro mais tarde.

6. **Selecione Guardar.**

Para obter mais informações, consulte [Proteção anti-software malware na EOP.](../security/office-365-security/anti-malware-protection.md)

## <a name="protect-against-ransomware"></a>Proteja-se contra ransomware

O ransomware restringe o acesso aos dados ao encriptar ficheiros ou bloquear ecrãs do computador. Em seguida, tenta extorquir dinheiro de uma moeda que lhe pede "resgate", normalmente sob a forma de criptocurrências como Bitcoin, em troca de acesso aos dados.

Para se proteger contra ransomware, crie uma ou mais regras de fluxo de correio para bloquear extensões de ficheiros frequentemente utilizadas para ransomware. (Adicionou estas regras ao aumentar [o nível de proteção contra software maliceiro no passo de](#raise-the-level-of-protection-against-malware-in-mail) correio.) Também pode avisar os utilizadores que recebem estes anexos por e-mail.

Além dos ficheiros que bloqueou no passo anterior, é uma boa prática criar uma regra para avisar os utilizadores antes de abrirem anexos de ficheiro Office que incluam macros. O ransomware pode ser ocultado dentro de macros, pelo que deve avisar os utilizadores para não abrirem estes ficheiros de pessoas que não conheçam.

Para criar uma regra de transporte de correio:

1. Vá para o centro de administração em <https://admin.microsoft.com> e **selecionar Centros de** administração \> **Exchange**.

2. Na categoria **de fluxo de** correio, selecione **regras**.

3. **+** Selecione e, em seguida, **selecione Criar uma nova regra**.

4. **Selecione Mais** opções na parte inferior da caixa de diálogo para ver o conjunto completo de opções.

5. Aplique as definições na seguinte tabela para a regra. Utilize os valores predefinido para as restantes definições, a menos que queira alterá-los.

6. Seleccione **Guardar**.

|Definição|Avisar os utilizadores antes de abrirem anexos de Office ficheiros|
|---|---|
|Name|Regra anti ransomware: avisar os utilizadores|
|Aplicar esta regra se . . .|Qualquer anexo . . . a extensão de ficheiro corresponde . . .|
|Especificar palavras ou expressões|Adicione estes tipos de ficheiro:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm|
|Faça o seguinte. . .|Notificar o destinatário com uma mensagem|
|Fornecer texto da mensagem|Não abra estes tipos de ficheiros de pessoas que não conhece porque podem conter macros com código malicioso.|

Para mais informações, consulte:

- [Ransomware: como reduzir os riscos](https://www.microsoft.com/security/blog/2020/04/28/ransomware-groups-continue-to-target-healthcare-critical-services-heres-how-to-reduce-risk/)

- [Restaurar os seus OneDrive](https://support.microsoft.com/office/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Parar o re encaminhamento automático para e-mail

Os hackers que têm acesso à caixa de correio de um utilizador podem roubar correio ao definir a caixa de correio para reencainhar e-mails automaticamente. Isto pode acontecer mesmo sem a consciência do utilizador. Para impedir que isto aconteça, configure uma regra de fluxo de correio.

Para criar uma regra de transporte de correio, veja [este breve vídeo](../business-video/stop-email-auto-forward.md) ou siga estes passos:

1. Na ação centro de administração do Microsoft 365, **selecione Centros de** \> **Exchange**.

2. Na categoria **de fluxo de** correio, selecione **regras**.

3. **+** Selecione e, em seguida, **selecione Criar uma nova regra**.

4. Para ver todas as opções, **selecione Mais opções** na parte inferior da caixa de diálogo.

5. Aplique as definições na seguinte tabela. Utilize os valores predefinido para as restantes definições, a menos que queira alterá-los.

6. Seleccione **Guardar**.

|Definição|Avisar os utilizadores antes de abrirem anexos de Office ficheiros|
|---|---|
|Name|Impedir o re encaminhamento automático de e-mail para domínios externos|
|Aplicar esta regra se...|O remetente . . . é externa/interna. . . Dentro da organização|
|Adicionar condição|As propriedades da mensagem . . . inclua o tipo de mensagem . . . Encaminhar automaticamente|
|Faça o seguinte...|Bloqueie a mensagem . . . rejeitar a mensagem e incluir uma explicação.|
|Fornecer texto da mensagem|O re encaminhamento automático de e-mail fora desta organização é impedido por motivos de segurança.|


## <a name="protect-your-email-from-phishing-attacks"></a>Proteger o seu e-mail contra ataques de phishing

Se tiver configurado um ou mais domínios personalizados para o seu ambiente Office 365 ou Microsoft 365, pode configurar a proteção anti-phishing direcizada. A proteção anti-phishing, parte do Microsoft Defender para Office 365, pode ajudar a proteger a sua organização de ataques de phishing baseados em representação maliciosa e outros ataques de phishing. Se ainda não tiver configurado um domínio personalizado, não precisa de o fazer.

Recomendamos que se inicie com esta proteção ao criar uma política para proteger os seus utilizadores mais importantes e o seu domínio personalizado.

Para criar uma política anti-phishing no Microsoft Defender [](../business-video/setup-anti-phishing.md)para Office 365, veja este breve vídeo de formação ou conclua os seguintes passos:

1. Aceda a [https://protection.office.com](https://protection.office.com).

2. No Centro de Conformidade &amp; de Segurança, no painel de navegação esquerdo, em Gestão **de ameaças,** escolha **Política**.

3. Na página **Política,** **selecionar Anti phishing**.

4. Na página **Anti phishing,** selecione **+ Criar.** Será iniciado um assistente que o ajuda a definir a sua política anti phishing.

5. Especifique o nome, a descrição e as definições da sua política conforme recomendado na seguinte tabela. Para obter mais detalhes, consulte Saber mais sobre a [política anti-phishing no Microsoft Defender Office 365 opções.](../security/office-365-security/set-up-anti-phishing-policies.md)

6. Após rever as suas definições, selecionar **Criar esta política ou** **Guardar,** conforme adequado.

|Definição ou opção|Definição recomendada|
|---|---|
|Name|Domínio e funcionários de campanhas mais valiosos|
|Descrição|Certifique-se de que a equipa mais importante e o nosso domínio não estão a ser representação.|
|Adicionar utilizadores para proteger|**Selecione + Adicionar uma condição, o destinatário é**. Escreva os nomes de utilizador ou introduza o endereço de e-mail do candidato, gestor de campanhas e de outros membros importantes da equipa. Pode adicionar até 20 endereços internos e externos que pretende proteger contra representação.|
|Adicionar domínios para proteger|**Selecione + Adicionar uma condição, o domínio do destinatário é**. Introduza o domínio personalizado associado à sua subscrição Microsoft 365, se tiver definido um. Pode introduzir mais do que um domínio.|
|Selecionar ações|Se o e-mail for enviado por um utilizador representação: Selecionar **Redirecionar** mensagem para outro endereço de e-mail e, em seguida, escreva o endereço de e-mail do administrador de segurança; Por exemplo, *Alice <span> <span> @contoso.com*. Se o e-mail for enviado por um domínio representação: Selecionar **Mensagem de quarentena**.|
|Informações sobre caixas de correio|Por predefinição, a inteligência da caixa de correio é selecionada quando cria uma nova política anti-phishing. Deixe esta definição **Ativos para** melhores resultados.|
|Adicionar domínios e recetores de confiança|Aqui pode adicionar o seu próprio domínio ou outros domínios de confiança.|
|Aplicado a|**Selecione O domínio do destinatário é**. Em **Qualquer uma destas , selecione** **Escolher**. **Selecione + Adicionar**. Selecione a caixa de verificação junto ao nome do domínio, por *exemplo, contoso. <span> <span> com,* na lista e, em seguida, **selecione Adicionar**. **Selecione Feito**.|

## <a name="protect-against-malicious-attachments-and-files-with-safe-attachments"></a>Proteja-se contra anexos e ficheiros maliciosos Cofre Anexos

As pessoas enviam, recebem e partilham anexos regularmente, como documentos, apresentações, páginas de livro e muito mais. Nem sempre é fácil saber se um anexo é seguro ou malicioso ao ver uma mensagem de e-mail. O Microsoft Defender para Office 365 inclui Cofre Proteção de anexos, mas esta proteção não está adada por predefinição. Recomendamos que crie uma nova regra para começar a utilizar esta proteção. Esta proteção abrange ficheiros no SharePoint, OneDrive e Microsoft Teams.

Para criar uma Cofre Anexo, veja [este breve vídeo ou](../business-video/safe-attachments.md)conclua os seguintes passos:

1. Vá para [https://protection.office.com](https://protection.office.com) e inscreva-se com a sua conta de administrador.

2. No Centro de Conformidade &amp; de Segurança, no painel de navegação esquerdo, em Gestão **de ameaças,** escolha **Política**.

3. Na página Política, selecionar **Cofre Anexos.**

4. Na página Cofre anexos, aplique esta proteção de forma abrangente ao selecionar a caixa de verificação Ativar a ATP para **o SharePoint, OneDrive** e Microsoft Teams proteção.

5. **+** Selecione para criar uma nova política.

6. Aplique as definições na seguinte tabela.

7. Depois de ter revisto as suas definições, **selecionar Criar esta política** ou **Guardar**, conforme adequado.

|Definição ou opção|Definição recomendada|
|---|---|
|Name|Bloquear e-mails atuais e futuros com software malictado detetado.|
|Descrição|Bloqueie e-mails e anexos atuais e futuros com software malicioso detetado.|
|Guardar anexos de resposta malitária desconhecida|**Selecione Bloquear – bloquear os e-mails e anexos atuais e futuros com software malicioso detetado**.|
|Redirecionar anexos ao detetar|Ativar o redirecionamento (selecione esta caixa) Introduza a conta de administrador ou a configuração da caixa de correio para quarentena.          Aplicar a seleção acima se ocorrer o tempo de ocorrência de falhas ou erros de análise de software malicioso (selecione esta caixa).|
|Aplicado a|O domínio do destinatário é . . . selecione o seu domínio.|

Para obter mais informações, consulte [Configurar políticas anti phishing no Microsoft Defender para Office 365](../security/office-365-security/set-up-anti-phishing-policies.md).

## <a name="protect-against-phishing-attacks-with-safe-links"></a>Proteger contra ataques de phishing com Cofre Ligações

Por vezes, os hackers ocultam sites maliciosos em ligações no e-mail ou noutros ficheiros. Cofre As ligações, que fazem parte do Microsoft Defender para Office 365, podem ajudar a proteger a sua organização ao fornecer uma verificação de tempo do clique dos endereços Web (URLs) em mensagens de e-mail e Office documentos. A proteção é definida através Cofre políticas de Ligações.

Recomendamos que faça o seguinte:

- Modifique a política predefinida para aumentar a proteção.

- Adicione uma nova política direcçada a todos os destinatários no seu domínio.

Para configurar o Cofre Links, veja este breve vídeo [de formação](../business-video/safe-links.md)ou conclua os seguintes passos:

1. Vá para [https://protection.office.com](https://protection.office.com) e inscreva-se com a sua conta de administrador.

2. No Centro de Conformidade &amp; de Segurança, no painel de navegação esquerdo, em Gestão **de ameaças,** escolha **Política**.

3. Na página Política, selecionar **Cofre Ligações**.

Para modificar a política predefinida:

1. Na página de Cofre, em Políticas que se aplicam a toda **a** organização , selecione a Política **predefinida.**

2. Em Definições **aplicam-se a** conteúdo exceto ao e-mail **, selecione Microsoft 365 Apps para Grandes Empresas, Office para iOS e Android**.

3. Seleccione **Guardar**.

Para criar uma nova política direcçada para todos os destinatários no seu domínio:

1. Na página Cofre, em Políticas que se aplicam a toda a organização **,** selecione para criar uma **+** nova política.

2. Aplique as definições listadas na seguinte tabela.

3. Seleccione **Guardar**.

|Definição ou opção|Definição recomendada|
|---|---|
|Name|Cofre a política de ligações para todos os destinatários no domínio|
|Selecione a ação para URLs potencialmente maliciosos desconhecidos em mensagens|Selecione Ativos – os URLs serão reescritos e verificados com uma lista de ligações **maliciosas conhecidas** quando o utilizador clicar na ligação .|
|Utilizar Cofre anexos para analisar conteúdo transferível|Selecione esta caixa.|
|Aplicado a|O domínio do destinatário é . . . selecione o seu domínio.|

Para obter mais informações, [consulte Cofre Ligações .](../security/office-365-security/safe-links.md)

## <a name="go-to-intune-admin-center"></a>Ir para o centro de administração do Intune

1. Inscreva-se [no portal do Azure.](https://portal.azure.com/)

2. **Selecione Todos** os serviços e escreva *Intune* na **Caixa de Pesquisa**.

3. Assim que os resultados aparecerem, selecione o início **junto a Microsoft Intune** para torná-lo favorito e fácil de encontrar mais tarde.

Além do centro de administração, pode utilizar o Intune para inscrever e gerir os dispositivos da sua organização. Para obter mais informações, consulte Recursos por método de inscrição para dispositivos [Windows](/intune/enrollment/enrollment-method-capab) e Opções de inscrição para [dispositivos geridos pelo Intune.](/intune/enrollment-options)
