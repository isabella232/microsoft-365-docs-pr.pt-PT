---
title: Resolver problemas de dispositivos AutoPilot
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Saiba como solucionar erros de arquivo de dispositivos AutoPilot.
ms.openlocfilehash: 1b5358bd6686c2548e82ec5297ac0ad675835718
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/19/2019
ms.locfileid: "38718705"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Resolver problemas de dispositivos AutoPilot

## <a name="device-file-error-messages"></a>Mensagens de erro de arquivo do dispositivo

Aqui estão as informações sobre alguns dos erros que você pode ver enquanto trabalha com arquivos de dispositivos AutoPilot no Microsoft 365 Business. 
  
|**Código de erro**|**Corrigir para tentar**|
|:-----|:-----|
|Órgão de solicitação inválido  <br/> |Este erro deve acontecer raramente, se você ver este erro, tente a operação outra vez.  <br/> |
|O valor do hash de hardware para um dispositivo não está correto.  <br/> |Se você ver esse erro, isso significa que o valor que você forneceu em seu arquivo CSV para o hash de hardware de um dispositivo não está correto. Primeiro, verifique se o valor foi digitado corretamente. Se você acha que o valor está correto, mas esse erro ainda está acontecendo, peça ajuda ao fornecedor de hardware.  <br/> |
|Dispositivo atribuído a outro inquilino  <br/> |Se você ver esse erro, isso significa que o valor que você forneceu em seu arquivo CSV para o número de série ou a chave do produto de um ou mais dispositivos não está correto. Primeiro, verifique se o valor foi digitado corretamente. Se você acha que o valor está correto, mas esse erro ainda está acontecendo, peça ajuda ao fornecedor de hardware.  <br/> |
|O arquivo CSV contém um número de série inválido ou chave do produto  <br/> |Se você ver esse erro, isso significa que o dispositivo que você está tentando registrar já está registrado por outra organização. Para corrigir esse erro, peça ajuda ao fornecedor de hardware.  <br/> |
|Este dispositivo não é suportado para configuração usando AutoPilot  <br/> | Esse erro significa que o dispositivo não atende aos requisitos de implantação do AutoPilot. Os dispositivos têm de cumprir os seguintes requisitos:  <br/>  Windows 10, versão 1703 ou posterior.  <br/>  Novos dispositivos que não passaram pela experiência do Windows fora da caixa.  <br/> |
|Dispositivo não encontrado  <br/> |Esse erro significa que um ou mais dispositivos em seu arquivo CSV não estão registrados em sua organização. Para corrigir isso, peça ajuda ao fornecedor de hardware.  <br/> |
