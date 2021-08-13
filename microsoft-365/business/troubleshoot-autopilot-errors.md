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
description: Saiba como resolver problemas que poderá ver ao trabalhar com ficheiros de dispositivo AutoPilot no Microsoft 365 Empresas Premium.
ms.openlocfilehash: b74c57acbaa5682f6db97e7d8a090e6e28a40dcc3246f00cacc7984cb52cc758
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53809186"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Resolver problemas de dispositivos AutoPilot

## <a name="device-file-error-messages"></a>Mensagens de erro de ficheiro de dispositivo

Eis algumas informações sobre alguns dos erros que poderá ver ao trabalhar com ficheiros de dispositivos AutoPilot no Microsoft 365 Empresas Premium. 
  
|**Código de erro**|**Corrigir para experimentar**|
|:-----|:-----|
|Corpo do pedido inválido  <br/> |Este erro raramente deverá ocorrer. Se vir este erro, tente novamente a operação.  <br/> |
|O valor hash de hardware para um dispositivo não está correto.  <br/> |Se vir este erro, significa que o valor fornecido no seu ficheiro CSV para o hash de hardware de um dispositivo não está correto. Primeiro, verifique se o valor foi digitado corretamente. Se achar que o valor está correto, mas este erro continuar a ocorrer, peça ajuda ao fornecedor de hardware.  <br/> |
|Dispositivo atribuído a outro inquilino  <br/> |Se vir este erro, significa que o valor que forneceu no seu ficheiro CSV para o número de série ou para a chave de produto de um ou mais dispositivos não está correto. Primeiro, verifique se o valor foi digitado corretamente. Se achar que o valor está correto, mas este erro continuar a ocorrer, peça ajuda ao fornecedor de hardware.  <br/> |
|O ficheiro CSV contém um número de série ou chave de produto inválida  <br/> |Se vir este erro, significa que o dispositivo que está a tentar registar já está registado por outra organização. Para corrigir este erro, peça ajuda ao fornecedor de hardware.  <br/> |
|Este dispositivo não é suportado para a configuração através do AutoPilot  <br/> | Este erro significa que o dispositivo não cumpre os requisitos da implementação AutoPilot. Os dispositivos têm de cumprir os seguintes requisitos:  <br/>  Windows 10, versão 1703 ou posterior.  <br/>  Novos dispositivos que não passaram por Windows experiência prática.  <br/> |
|Dispositivo não encontrado  <br/> |Este erro significa que um ou mais dispositivos no seu ficheiro CSV não estão registados na sua organização. Para corrigir este problema, peça ajuda ao fornecedor de hardware.  <br/> |
