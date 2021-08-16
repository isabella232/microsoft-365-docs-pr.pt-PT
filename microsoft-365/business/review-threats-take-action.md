---
title: Rever ameaças detetadas e tomar medidas
f1.keywords: NOCSH
ms.author: sharik
author: SKjerland
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- Adm_O365
- Adm_TOC
ms.custom: AdminSurgePortfolio
search.appverid: MET150
description: Saiba como rever e gerir ameaças detetadas por Antivírus do Microsoft Defender nos seus Windows 10 dispositivos.
ms.openlocfilehash: f2edd27c527cc2b9fd8c986191a0bad5c0844da68880f8d8d775491e3480babd
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53882099"
---
# <a name="review-detected-threats-and-take-action"></a>Rever ameaças detetadas e tomar medidas

Assim que um ficheiro ou software malicioso for detetado, o Antivírus do Microsoft Defender bloqueia-o e impede-o de ser executado. Com a proteção fornecida na nuvem ativada, são adicionadas novas ameaças ao antivírus e ao motor de antimalware para que os seus outros dispositivos e utilizadores também sejam protegidos.

Antivírus do Microsoft Defender deteta e protege contra os seguintes tipos de ameaças:

- Vírus, software malicático e ameaças baseadas na Web em dispositivos
- Tentativas de phishing
- Tentativas de roubo de dados

Enquanto profissional/administrador de TI, pode ver informações sobre deteções de ameaças em diferentes Windows 10 que estão inscritos no [Intune](/mem/intune/enrollment/device-enrollment) na centro de administração do Microsoft 365. Verá informações de resumo, tais como:

- Quantos dispositivos precisam de proteção antivírus
- Quantos dispositivos não estão em conformidade com as políticas de segurança
- Quantas ameaças estão atualmente ativas, atenuadas ou resolvidas

Tem várias opções para ver informações específicas sobre deteções de ameaças e dispositivos:

- A **página Dispositivos** ativos na <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">centro de administração do Microsoft 365</a>. Consulte [Gerir deteções de ameaças na página Dispositivos ativos](#manage-threat-detections-on-the-active-devices-page) neste artigo.
- A **página Ameaças** ativas na <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">centro de administração do Microsoft 365</a>. Consulte [Gerir deteções de ameaças na página Ameaças ativas](#manage-threat-detections-on-the-active-threats-page) neste artigo.
- A **página do Antivírus** na <a href="https://go.microsoft.com/fwlink/p/?linkid=2150463" target="_blank">Microsoft Endpoint Manager</a>. Consulte [Gerir deteções de ameaças Microsoft Endpoint Manager](#manage-threat-detections-in-microsoft-endpoint-manager) neste artigo.

Para saber mais, consulte [Ameaças detetadas por Antivírus do Microsoft Defender](threats-detected-defender-av.md).

## <a name="manage-threat-detections-on-the-active-devices-page"></a>Gerir deteções de ameaças na página **Dispositivos ativos**

O seguinte procedimento aplica-se a clientes que Microsoft 365 Empresas Premium.

1. Vá para o centro de administração do Microsoft 365 em <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> e inscreva-se.

2. Na página de navegação, selecione **Dispositivos**  >  **Ativos**. Verá uma lista de dispositivos e detalhes ativos, como o estado de proteção, o estado de proteção do antivírus (AV) e o número de ameaças ativas detetadas.

3. Selecione um dispositivo para ver mais detalhes sobre esse dispositivo e as ações disponíveis. É aberta uma lista de opções com recomendações e ações disponíveis, tais como Atualizar **política,** Atualizar **antivírus,** Executar análise **rápida,** Executar **análise** completa e muito mais.

## <a name="manage-threat-detections-on-the-active-threats-page"></a>Gerir deteções de ameaças na **página Ameaças ativas**

O seguinte procedimento aplica-se a clientes que Microsoft 365 Empresas Premium. [Windows 10 dispositivos têm de estar protegidos](./secure-win-10-pcs.md) [e inscritos no Intune.](/mem/intune/enrollment/windows-enrollment-methods)

> [!NOTE]
> A **Antivírus do Microsoft Defender** e a página **Ameaças** ativas estão a ser faseadas, pelo que poderá não ter acesso imediato às mesmas.

1. Vá para o centro de administração do Microsoft 365 em <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> e inscreva-se.

2. No cartão **Antivírus do Microsoft Defender,** selecione **Ver ameaças ativas.** (Em alternativa, no painel de navegação, selecione Estado de **Trabalho**  >  **Ameaças & antivírus**.)

3. Na página **Ameaças ativas,** selecione uma ameaça detetada para saber mais sobre a mesma. É aberta uma panfleto com detalhes sobre essa ameaça, incluindo os dispositivos afetados.

4. Na lista de opções, selecione um dispositivo para ver **as** ações disponíveis, como Atualizar política , Atualizar **antivírus**, **Executar** análise rápida e muito mais.

## <a name="actions-you-can-take"></a>Ações que pode tomar

Quando vir detalhes sobre ameaças ou dispositivos específicos, verá recomendações e uma ou mais ações que pode tomar. A seguinte tabela descreve as ações que poderá ver.<br><br>

| Ação | Descrição |
|--|--|
| Configurar proteção | As suas políticas de proteção contra ameaças têm de ser configuradas. Selecione a ligação para ir para a página de configuração da sua política.<br><br>Precisa de ajuda? Consulte [Gerir a segurança dos dispositivos com as políticas de segurança de pontos finais Microsoft Intune](/mem/intune/protect/endpoint-security-policy). |
| Atualizar política | O seu antivírus e políticas de proteção em tempo real têm de ser atualizados ou configurados. Selecione a ligação para ir para a página de configuração da política.<br><br>Precisa de ajuda? Consulte [Gerir a segurança dos dispositivos com as políticas de segurança de pontos finais Microsoft Intune](/mem/intune/protect/endpoint-security-policy). |
| Executar a análise rápida | Inicia uma análise rápida de antivírus no dispositivo, focando-se em localizações comuns onde o malware poderá estar registado, como chaves de registo e pastas de arranque conhecidas Windows arranque. |
| Executar a análise completa | Inicia uma análise antivírus completa no dispositivo, focando-se em localizações comuns onde o malware poderá estar registado e incluindo todos os ficheiros e pastas no dispositivo. Os resultados são enviados [para o Microsoft Endpoint Manager](/mem/intune/fundamentals/tutorial-walkthrough-endpoint-manager). |
| Atualizar o antivírus | Necessita do dispositivo para obter [atualizações de informações de segurança para](https://go.microsoft.com/fwlink/?linkid=2149926) antivírus e proteção antimalware. |
| Reiniciar dispositivo | Força um dispositivo Windows 10 dispositivo a reiniciar dentro de cinco minutos.<br><br>**IMPORTANTE:** O proprietário ou utilizador do dispositivo não é notificado automaticamente do reinício e poderá perder trabalho não guardado. |

## <a name="manage-threat-detections-in-microsoft-endpoint-manager"></a>Gerir deteções de ameaças no Microsoft Endpoint Manager

Pode utilizar o Microsoft Endpoint Manager gerir deteções de ameaças. Windows 10 dispositivos têm [de estar inscritos no Intune](/mem/intune/enrollment/windows-enrollment-methods) (parte da Microsoft Endpoint Manager).

1. Vá para o Microsoft Endpoint Manager de administração em e <a href="https://go.microsoft.com/fwlink/p/?linkid=2150463" target="_blank">https://endpoint.microsoft.com</a> inscreva-se.

2. No painel de navegação, selecione **Segurança do ponto final**.

3. Em **Gerir**, selecione **Antivírus**. Verá vários separadores, como **Resumo,** pontos **finais Windows 10** desaloados e software **malic Windows 10 detetado**.

4. Reveja as informações nos separadores disponíveis e, em seguida, tome as ações necessárias.

Por exemplo, suponha que os dispositivos estão listados no **separador software malic Windows 10 detetado.** Ao selecionar um dispositivo, terá algumas ações disponíveis, tais como Reiniciar, Análise Rápida **,** Análise Completa **,** **Sincronização** ou Atualizar **assinaturas**. Selecione uma ação para esse dispositivo.

A seguinte tabela descreve as ações que poderá ver Microsoft Endpoint Manager.<br><br>

| Ação | Descrição |
|--|--|
| Reiniciar | Força um dispositivo Windows 10 dispositivo a reiniciar dentro de cinco minutos.<br><br>**IMPORTANTE:** O proprietário ou utilizador do dispositivo não é notificado automaticamente do reinício e poderá perder trabalho não guardado. |
| Análise Rápida | Inicia uma análise rápida de antivírus no dispositivo, focando-se em localizações comuns onde o malware poderá estar registado, como chaves de registo e pastas de arranque conhecidas Windows arranque. Os resultados são enviados [para o Microsoft Endpoint Manager](/mem/intune/fundamentals/tutorial-walkthrough-endpoint-manager). |
| Análise Completa | Inicia uma análise antivírus completa no dispositivo, focando-se em localizações comuns onde o malware poderá estar registado e incluindo todos os ficheiros e pastas no dispositivo. Os resultados são enviados [para o Microsoft Endpoint Manager](/mem/intune/fundamentals/tutorial-walkthrough-endpoint-manager). |
| Sincronização | Necessita de um dispositivo para consultar com o Intune (parte da Microsoft Endpoint Manager). Quando o dispositivo é verificado, o dispositivo recebe todas as políticas ou ações pendentes atribuídas ao dispositivo. |
| Atualizar assinaturas | Necessita do dispositivo para obter [atualizações de informações de segurança para](https://go.microsoft.com/fwlink/?linkid=2149926) antivírus e proteção antimalware. |

> [!TIP]
> Para obter mais informações, consulte [Ações remotas para dispositivos.](/mem/intune/protect/endpoint-security-manage-devices#remote-actions-for-devices)

## <a name="how-to-submit-a-file-for-malware-analysis"></a>Como submeter um ficheiro para análise de software malicial

Se tiver um ficheiro que acha que foi perdido ou que foi classificado injustamente como malware, pode submeter esse ficheiro à Microsoft para análise de software malicial. Os utilizadores e administradores de TI podem submeter um ficheiro para análise. Visite [https://www.microsoft.com/wdsi/filesubmission](https://www.microsoft.com/wdsi/filesubmission) .