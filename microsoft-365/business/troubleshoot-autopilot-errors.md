---
title: Resolver problemas de dispositivos AutoPilot
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Obter informações sobre como resolver erros de ficheiro do dispositivo de piloto automático.
ms.openlocfilehash: 9d4a47f78c38d8c076f5b3876a36b6bf46eaaaf3
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32279844"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Resolver problemas de dispositivos AutoPilot

## <a name="device-file-error-messages"></a>Mensagens de erro do ficheiro de dispositivo

Info de aqui em alguns dos erros poderá ver enquanto estiver a trabalhar com ficheiros de dispositivo de piloto automático no Microsoft 365 Business. 
  
|**Código de erro**|**Corrigir a tentar**|
|:-----|:-----|
|Corpo de pedido inválido  <br/> |Este erro deve ocorrer raramente, se vir este erro, tente novamente a operação.  <br/> |
|Valor de hash de hardware para um dispositivo não está correcto.  <br/> |Se vir este erro, isso significa que o valor fornecido no ficheiro CSV para o hash de hardware de um dispositivo não está correcto. Em primeiro lugar, certifique-se de que o valor foi escrito correctamente. Se pensa que o valor está correcto, mas este erro ainda está a acontecer, peça ao seu fornecedor de hardware para obter ajuda.  <br/> |
|Dispositivo atribuído ao outro tenant  <br/> |Se vir este erro, isso significa que o valor fornecido no ficheiro CSV para o número de série ou a chave de produto de um ou mais dispositivos não é correcto. Em primeiro lugar, certifique-se de que o valor foi escrito correctamente. Se pensa que o valor está correcto, mas este erro ainda está a acontecer, peça ao seu fornecedor de hardware para obter ajuda.  <br/> |
|O ficheiro CSV contém uma chave de produto ou número de série inválido  <br/> |Se vir este erro significa que o dispositivo que está a tentar registar já está registado por uma outra organização. Para corrigir este problema, peça ao seu fornecedor de hardware para obter ajuda.  <br/> |
|Este dispositivo não é suportado para o programa de configuração utilizando o piloto automático  <br/> | Este erro significa que o dispositivo não cumpre requisitos de implementação piloto automático. Os dispositivos têm de cumprir os seguintes requisitos:  <br/>  Windows 10, versão 1703 ou posterior.  <br/>  Novos dispositivos que não tenham tido a experiência de configuração inicial do Windows.  <br/> |
|Não foi encontrado nenhum dispositivo  <br/> |Este erro significa que um ou mais dispositivos no ficheiro CSV não está registado para a sua organização. Para corrigir este problema, peça ao seu fornecedor de hardware para obter ajuda.  <br/> |
   
