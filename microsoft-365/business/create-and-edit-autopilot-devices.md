---
title: Criar e editar dispositivos AutoPilot
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: article
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
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Saiba como carregar dispositivos com o AutoPilot no Microsoft 365 Empresas Premium. Pode atribuir um perfil a um dispositivo ou grupo de dispositivos.
ms.openlocfilehash: ae3a760db4b94aac50301685a0c4f468e46ec8e9aa907a1b6fb35e03a9e541f0
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53867033"
---
# <a name="create-and-edit-autopilot-devices"></a>Criar e editar dispositivos AutoPilot

## <a name="upload-a-list-of-devices"></a>Carregar uma lista de dispositivos

Pode utilizar o guia [passo a](add-autopilot-devices-and-profile.md) passo para carregar dispositivos, mas também pode carregar dispositivos no separador **Dispositivos.** 
  
Os dispositivos têm de cumprir estes requisitos:
  
- Windows 10, versão 1703 ou posterior
    
- Novos dispositivos que não passaram por Windows experiência prática

1. Na seta centro de administração do Microsoft 365, **selecionar Dispositivos** \> **AutoPilot**.
  
2. Na página **AutoPilot,** selecionar o **separador Dispositivos** \> **Adicionar dispositivos.**
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. No painel **Adicionar dispositivos,** navegue para um ficheiro [CSV](../admin/misc/device-list.md) de lista de dispositivos que tenha preparado \> **Guardar** \> **Fechar.**
    
    Pode obter estas informações com o fornecedor de hardware ou pode utilizar o script do [PowerShell Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) para gerar um ficheiro CSV. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Atribuir um perfil a um dispositivo ou a um grupo de dispositivos

1. Na página **Preparar Windows, selecione** o **separador** Dispositivos e selecione a caixa de verificação junto a um ou mais dispositivos. 
    
2. No painel **Dispositivo**, selecione um perfil a partir do menu pendente **Perfil atribuído**. 
    
    Se ainda não tiver perfis, consulte a secção [Criar e editar perfis AutoPilot](create-and-edit-autopilot-profiles.md) para obter instruções. 
