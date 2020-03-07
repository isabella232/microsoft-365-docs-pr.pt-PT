---
title: Resolver problemas de dispositivos AutoPilot
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: troubleshooting
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Saiba como resolver erros que poderá ver enquanto trabalha com ficheiros de dispositivos AutoPilot no Microsoft 365 Business.
ms.openlocfilehash: dc1abd508156c8525859f6ca7e291ab38fc8859c
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/07/2020
ms.locfileid: "42560706"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Resolver problemas de dispositivos AutoPilot

## <a name="device-file-error-messages"></a>Mensagens de erro de ficheiro do dispositivo

Aqui está a informação sobre alguns dos erros que poderá ver enquanto trabalha com ficheiros de dispositivos AutoPilot no Microsoft 365 Business. 
  
|**Código de erro**|**Corrigir para tentar**|
|:-----|:-----|
|Organismo de pedido inválido  <br/> |Este erro raramente deverá acontecer, se vir este erro, tente novamente a operação.  <br/> |
|O valor do hash de hardware para um dispositivo não está correto.  <br/> |Se vir este erro, significa que o valor que forneceu no seu ficheiro CSV para o hash de hardware de um dispositivo não está correto. Primeiro, verifique se o valor foi dactilografado corretamente. Se acha que o valor está correto, mas este erro ainda está a acontecer, peça ajuda ao seu fornecedor de hardware.  <br/> |
|Dispositivo atribuído a outro inquilino  <br/> |Se vir este erro, significa que o valor que forneceu no seu ficheiro CSV para o número de série ou a chave do produto de um ou mais dispositivos não está correto. Primeiro, verifique se o valor foi dactilografado corretamente. Se acha que o valor está correto, mas este erro ainda está a acontecer, peça ajuda ao seu fornecedor de hardware.  <br/> |
|O ficheiro CSV contém um número de série inválido ou chave do produto  <br/> |Se vir este erro, significa que o dispositivo que está a tentar registar já está registado por outra organização. Para corrigir este erro, peça ajuda ao seu fornecedor de hardware.  <br/> |
|Este dispositivo não é suportado para configuração utilizando o AutoPilot  <br/> | Este erro significa que o dispositivo não satisfaz os requisitos de implementação do AutoPilot. Os dispositivos têm de cumprir os seguintes requisitos:  <br/>  Windows 10, versão 1703 ou posterior.  <br/>  Novos dispositivos que não passaram pela experiência do Windows fora da caixa.  <br/> |
|Dispositivo não encontrado  <br/> |Este erro significa que um ou mais dispositivos no seu ficheiro CSV não estão registados na sua organização. Para corrigir isto, peça ajuda ao seu fornecedor de hardware.  <br/> |
