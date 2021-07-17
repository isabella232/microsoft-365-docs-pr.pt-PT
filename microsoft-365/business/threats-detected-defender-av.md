---
title: Ameaças detetadas por Antivírus do Microsoft Defender
f1.keywords: CSH
ms.author: sharik
author: SKjerland
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- Adm_O365
- Adm_TOC
ms.custom: AdminSurgePortfolio
search.appverid: MET150
description: Saiba como Antivírus do Microsoft Defender os seus dispositivos Windows contra ameaças de software, como vírus, software malicioso e spyware.
ms.openlocfilehash: 7c5d000e2a8c30e17d1f890cef69fe88beed75bb
ms.sourcegitcommit: dcb97fbfdae52960ae62b6faa707a05358193ed5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/25/2021
ms.locfileid: "53465439"
---
# <a name="threats-detected-by-microsoft-defender-antivirus"></a>Ameaças detetadas por Antivírus do Microsoft Defender

Antivírus do Microsoft Defender protege os seus dispositivos Windows contra ameaças de software, como vírus, software malicioso e spyware.

- Normalmente, os vírus espalham-se ao anexar o respetivo código a outros ficheiros no seu dispositivo ou rede e podem fazer com que os programas infetados funcionem incorretamente.
- O software malicioso inclui ficheiros, aplicações e código maliciosos que podem causar danos e interromper a utilização normal dos dispositivos. Além disso, o malware pode permitir acesso não autorizado, utilizar recursos de sistema, roubar palavras-passe e informações da conta, bloqueá-lo do computador e pedir resgates e muito mais.
- O spyware recolhe dados, como a atividade de navegação na Web, e envia os dados para servidores remotos.
 
Para fornecer proteção contra ameaças, Antivírus do Microsoft Defender utiliza vários métodos. Estes métodos incluem proteção em tempo real, proteção em tempo real e atualizações de proteção dedicadas.

- A proteção fornecida pela nuvem ajuda a proporcionar deteção e bloqueio de ameaças novas e emergentes perto de instantâneas.
- A análise sempre ativo utiliza a monitorização do comportamento do processo e de ficheiros e outras técnicas (também conhecidas como *proteção em tempo real).*
- As atualizações de proteção dedicadas baseiam-se na aprendizagem automática, análise de grandes dados humanas e automatizadas e pesquisa aprofundada de resistência a ameaças. 

Para saber mais sobre software malic Antivírus do Microsoft Defender, consulte os seguintes artigos: 

- [Noções sobre software malic & outras ameaças](/windows/security/threat-protection/intelligence/understanding-malware)
- [Como a Microsoft identifica malware e aplicações potencialmente indesejadas](/windows/security/threat-protection/intelligence/criteria)
- [Proteção de nova geração no Windows 10](/windows/security/threat-protection/microsoft-defender-antivirus/microsoft-defender-antivirus-in-windows-10)

## <a name="what-happens-when-a-non-microsoft-antivirus-solution-is-used"></a>O que acontece quando é utilizada uma solução antivírus que não seja da Microsoft? 

Antivírus do Microsoft Defender faz parte do sistema operativo e está ativado em dispositivos que estão a executar Windows 10. No entanto, se estiver a utilizar uma solução antivírus que não seja da Microsoft e não estiver a utilizar o Microsoft Defender para [Endpoint,](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-advanced-threat-protection)o Antivírus do Microsoft Defender entrará automaticamente no modo desativado.  

Quando estão no modo desativado, os utilizadores e clientes ainda podem utilizar Antivírus do Microsoft Defender para análises agendadas ou a pedido para identificar ameaças; no entanto, Antivírus do Microsoft Defender deixará de ser:

- ser utilizada como a aplicação antivírus predefinida.
- analisar ativamente ficheiros para deteção de ameaças.
- ameaças remediar ou resolver.

Se desinstalar a solução antivírus que não é da Microsoft, o Antivírus do Microsoft Defender entrará automaticamente no modo ativo para proteger os seus Windows dispositivos contra ameaças.

> [!TIP]
> - Se estiver a utilizar o Microsoft 365, considere utilizar o Antivírus do Microsoft Defender como a sua solução antivírus principal. A integração pode fornecer uma melhor proteção. Veja [Melhor em conjunto: Antivírus do Microsoft Defender e Office 365](/windows/security/threat-protection/microsoft-defender-antivirus/office-365-microsoft-defender-antivirus).
> - Certifique-se de que Antivírus do Microsoft Defender a par, mesmo que esteja a utilizar uma solução antivírus que não seja da Microsoft.

## <a name="what-to-expect-when-threats-are-detected"></a>O que esperar quando são detetadas ameaças

Quando são detetadas ameaças por Antivírus do Microsoft Defender, acontece o seguinte:

- Os utilizadores [recebem notificações no Windows](https://support.microsoft.com/windows/8942c744-6198-fe56-4639-34320cf9444e). 
- As deteções estão listadas na [Segurança do Windows de Dados](/windows/security/threat-protection/windows-defender-security-center/windows-defender-security-center) na página Histórico **de** proteção.  
- Se protegeu os seus dispositivos [Windows 10](secure-win-10-pcs.md) e inscreveu-os no [Intune](/mem/intune/enrollment/windows-enrollment-methods)e a sua organização tiver 800 ou menos dispositivos inscritos, verá deteções e insights sobre ameaças no <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">centro de administração do Microsoft 365</a> na página Ameaças e  **antivírus,** a que pode aceder a partir do cartão **Antivírus do Microsoft Defender** na Home **page** (ou a partir do painel de navegação, ao selecionar Ameaças de Saúde  >  **& antivírus).**

    Se a sua organização tiver mais de 800 dispositivos inscritos no Intune, ser-lhe-á pedido que veja deteções e informações sobre ameaças [do Microsoft Endpoint Manager](/mem/endpoint-manager-overview) em vez da página Ameaças e **antivírus.**
 
    > [!NOTE]
    > A **Antivírus do Microsoft Defender** e a página Ameaças e **Antivírus** do Antivírus do Microsoft Defender, pelo que poderá não ter acesso imediato às mesmas.

Na maioria dos casos, os utilizadores não precisam de tomar medidas. Assim que um ficheiro ou programa malicioso for detetado num dispositivo, o Antivírus do Microsoft Defender bloqueia-o e impede-o de ser executado. Além disso, são adicionadas novas ameaças ao motor antivírus e antimalware para que outros dispositivos e utilizadores também sejam protegidos.  

Se um utilizador precisar de fazer uma ação, como aprovar a remoção de um ficheiro malicioso, o utilizador verá isso na notificação que receber. Para saber mais sobre as ações que Antivírus do Microsoft Defender tomar em nome de um utilizador ou sobre as ações que os utilizadores podem ter de tomar, consulte Histórico [de Proteção.](https://support.microsoft.com/office/f1e5fd95-09b4-46d1-b8c7-1059a1e09708) Para saber como gerir deteções de ameaças como um profissional/administrador de TI, consulte Rever [ameaças detetadas e tomar medidas.](review-threats-take-action.md)

Para saber mais sobre diferentes ameaças, visite <a href="https://www.microsoft.com/wdsi/threats" target="_blank">o Informações de Segurança da Microsoft site Ameaças,</a>onde pode efetuar as seguintes ações: 

- Ver informações atuais sobre as principais ameaças.
- Veja as ameaças mais recentes de uma região específica.
- Procure detalhes sobre uma ameaça específica na encyclopedia ameaça.

## <a name="related-content"></a>Conteúdos relacionados

[Proteger Windows 10 dispositivos](secure-windows-10-devices.md) (artigo)\
[Avaliar Antivírus do Microsoft Defender](/windows/security/threat-protection/microsoft-defender-antivirus/evaluate-microsoft-defender-antivirus) (artigo)\
[Como a ligar a proteção antivírus](/mem/intune/user-help/turn-on-defender-windows#turn-on-real-time-and-cloud-delivered-protection) em tempo real e entregue na nuvem (artigo)\
[Como ativo e utilizar o Antivírus do Microsoft Defender a partir da aplicação Segurança do Windows](/windows/security/threat-protection/microsoft-defender-antivirus/microsoft-defender-security-center-antivirus) (artigo)\
[Como ativar o Antivírus do Microsoft Defender utilizando a Política de Grupo](/mem/intune/user-help/turn-on-defender-windows#turn-on-windows-defender) (artigo)\
[Como atualizar as definições de antivírus](/mem/intune/user-help/turn-on-defender-windows#update-your-antivirus-definitions) (artigo)\
[Como submeter software malictado e não malware para a Microsoft para análise](/microsoft-365/security/office-365-security/submitting-malware-and-non-malware-to-microsoft-for-analysis) (artigo)
