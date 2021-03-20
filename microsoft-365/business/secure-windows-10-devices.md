---
title: Proteger dispositivos Windows 10
f1.keywords:
- CSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4WindowsConfig
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 21e5551f-fa35-4f13-9418-f80d668b6a2b
description: Saiba como configurar as definições da política do dispositivo predefinido que qualquer dispositivo Do Windows 10 receberá ao iniciar sessão na sua conta de trabalho ou escola.
ms.openlocfilehash: 85383b1e1d2f2af3fd49d4a0c56c5d99586d607d
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912616"
---
# <a name="secure-windows-10-devices"></a>Proteger dispositivos Windows 10

Este artigo aplica-se ao Microsoft 365 Business Premium.

As definições que configurar aqui fazem parte da política de dispositivos predefinida para o Windows 10. Todos os utilizadores que liguem um dispositivo Windows 10, incluindo dispositivos móveis e Computadores, ao iniciar sessão com a sua conta de trabalho receberão automaticamente estas definições. Recomendamos que aceite a política predefinida durante a configuração e que adicione políticas destinadas a grupos de utilizadores específicos mais tarde.
  
## <a name="settings-to-secure-windows-10-devices"></a>Definições para proteger dispositivos Windows 10

Por predefinição, todas as definições estão **Ativadas**. As seguintes definições estão disponíveis:
  
|||
|:-----|:-----|
|Definição  <br/> |Descrição  <br/> |
|Ajudar a proteger os PCs contra vírus e outras ameaças com o Antivírus do Windows Defender  <br/> |Exige que o Antivírus do Windows Defender esteja ativado para proteger os PCs contra os perigos que uma ligação à Internet envolve.  <br/> |
|Ajudar a proteger os PCs contra ameaças baseadas na Web no Microsoft Edge  <br/> |Ativa as definições no Microsoft Edge que ajudam a proteger os utilizadores contra transferências e sites maliciosos.  <br/> |
|Ajudar a proteger ficheiros e pastas nos PCs contra acesso não autorizado com o BitLocker  <br/> |O Bitlocker protege os dados ao encriptar os discos rígidos do computador e proteger contra exposição de dados em caso de roubo ou perda do computador. Para mais informações, consulte [bitlocker FAQ](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions).  <br/> |
|Desligar o ecrã do dispositivo quando estiver inativo durante este período de tempo  <br/> |Garante que os dados da empresa são protegidos se um utilizador estiver inativo. É possível que um utilizador esteja a trabalhar num local público, como um café, e se afaste ou distraia por um momento, deixando o dispositivo vulnerável a olhares alheios. Esta definição permite-lhe controlar quanto tempo um utilizador pode estar inativo antes de o ecrã se desligar.  <br/> |
|