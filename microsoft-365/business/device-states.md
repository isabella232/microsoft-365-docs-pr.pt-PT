---
title: Estados do dispositivo
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Obter informações sobre Estados de dispositivo no Microsoft 365 Business.
ms.openlocfilehash: 06e5c800e6a104785c1fd0724223e05d7729722e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/15/2019
ms.locfileid: "34072726"
---
# <a name="device-states"></a>Estados do dispositivo

## <a name="device-states"></a>Estados do dispositivo

Os dispositivos na lista **Ações de dispositivos** (Página principal de administração \> **Ações de dispositivos**) podem ter os seguintes estados.
  
![In the Device actions list, you can see the Devices states.](media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|**Estado**|**Descrição**|
|:-----|:-----|
|Gerido pelo Intune  <br/> |Gerido pelo Microsoft 365 Business.  <br/> |
|Extinção pendente  <br/> |O Microsoft 365 Business está a preparar-se para remover dados empresariais do dispositivo.  <br/> |
|Extinção em curso  <br/> |O Microsoft 365 Business está a remover dados empresariais do dispositivo.  <br/> |
|Falha na extinção  <br/> | A ação de remoção de dados empresariais falhou.  <br/> |
|Extinção cancelada  <br/> |A ação de extinção foi cancelada.  <br/> |
|Eliminação dos dados pendente  <br/> |A aguardar o início da reposição de fábrica.  <br/> |
|Eliminação dos dados em curso  <br/> |A reposição de fábrica foi emitida.  <br/> |
|Falha ao limpar  <br/> |Não foi possível efetuar a reposição de fábrica.  <br/> |
|Eliminação dos dados cancelada  <br/> |A reposição de fábrica foi cancelada.  <br/> |
|Mau Estado de Funcionamento  <br/> |Isto significa que uma ação está pendente (ou em curso), mas o dispositivo não deu entrada durante 30 dias ou mais.  <br/> |
|Eliminação pendente  <br/> |A ação de eliminação está pendente.  <br/> |
|Detetado  <br/> |O Microsoft 365 Business detetou o dispositivo.  <br/> |
   
