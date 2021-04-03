---
title: Resolver problemas de dispositivos AutoPilot
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- ZTDTroubleshootDeviceErrors
- O365E_ZTDTroubleshootDeviceErrors
- BCS365_ZTDTroubleshootDeviceErrors
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Saiba como resolver os erros que poderá ver enquanto trabalha com ficheiros de dispositivos AutoPilot no Microsoft 365 Business Premium.
ms.openlocfilehash: 1078ab74b07952e4bb565555a081b98ecce9db5c
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578093"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Resolver problemas de dispositivos AutoPilot

## <a name="device-file-error-messages"></a>Mensagens de erro de ficheiro do dispositivo

Aqui estão as informações sobre alguns dos erros que pode ver enquanto trabalha com ficheiros de dispositivos AutoPilot no Microsoft 365 Business Premium. 
  
|**Código de erro**|**Corrigir para tentar**|
|:-----|:-----|
|Corpo de pedido inválido  <br/> |Este erro raramente deve acontecer, se vir este erro, tente novamente a operação.  <br/> |
|O valor de hash de hardware para um dispositivo não está correto.  <br/> |Se vir este erro, significa que o valor que forneceu no seu ficheiro CSV para o hash de hardware de um dispositivo não está correto. Primeiro, verifique se o valor foi corretamente digitado. Se acha que o valor está correto, mas este erro ainda está a acontecer, peça ajuda ao seu fornecedor de hardware.  <br/> |
|Dispositivo atribuído a outro inquilino  <br/> |Se vir este erro, significa que o valor que forneceu no seu ficheiro CSV para o número de série ou a chave de produto de um ou mais dispositivos não está correto. Primeiro, verifique se o valor foi corretamente digitado. Se acha que o valor está correto, mas este erro ainda está a acontecer, peça ajuda ao seu fornecedor de hardware.  <br/> |
|O ficheiro CSV contém um número de série inválido ou chave de produto  <br/> |Se vir este erro, significa que o dispositivo que está a tentar registar já está registado por outra organização. Para corrigir este erro, peça ajuda ao seu fornecedor de hardware.  <br/> |
|Este dispositivo não é suportado para configuração utilizando o AutoPilot  <br/> | Este erro significa que o dispositivo não satisfaz os requisitos de implementação do AutoPilot. Os dispositivos têm de cumprir os seguintes requisitos:  <br/>  Windows 10, versão 1703 ou posterior.  <br/>  Novos dispositivos que não passaram pela experiência fora de caixa do Windows.  <br/> |
|Dispositivo não encontrado  <br/> |Este erro significa que um ou mais dispositivos no seu ficheiro CSV não estão registados na sua organização. Para corrigir isto, peça ajuda ao seu fornecedor de hardware.  <br/> |
