---
title: Criar e editar dispositivos AutoPilot
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Saiba como carregar dispositivos usando o AutoPilot no Microsoft 365 Business. Você pode atribuir um perfil a um dispositivo ou a um grupo de dispositivos.
ms.openlocfilehash: 1dd6b1a574166379e29465bf3699e47e3b155e0b
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/14/2019
ms.locfileid: "38320264"
---
# <a name="create-and-edit-autopilot-devices"></a>Criar e editar dispositivos AutoPilot

## <a name="upload-a-list-of-devices"></a>Carregar uma lista de dispositivos

Você pode usar o [guia passo a passo](add-autopilot-devices-and-profile.md) para carregar dispositivos, mas também pode carregar dispositivos na aba **dispositivos.** 
  
Os dispositivos devem atender a esses requisitos:
  
- Windows 10, versão 1703 ou mais tarde
    
- Novos dispositivos que não passaram pela experiência do Windows fora da caixa

1. No centro de administração de negócios Microsoft 365, escolha **dispositivos** \> **AutoPilot**.
  
2. Na página **AutoPilot,** escolha a \> guia **dispositivos** **Adicionar dispositivos**.
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. No painel **de adicionar dispositivos,** navegue em um arquivo [CSV da lista do dispositivo](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) que você preparou \> **Save** \> **Close.**
    
    Você pode obter essas informações do fornecedor de hardware ou pode usar o [script Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) para gerar um arquivo CSV. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Atribuir um perfil a um dispositivo ou a um grupo de dispositivos

1. Na página **Prepare Windows,** escolha a guia **dispositivos** e selecione a caixa de seleção ao lado de um ou mais dispositivos. 
    
2. No painel **Dispositivo**, selecione um perfil a partir do menu pendente **Perfil atribuído**. 
    
    Se ainda não tiver perfis, consulte a secção [Criar e editar perfis AutoPilot](create-and-edit-autopilot-profiles.md) para obter instruções. 
    
