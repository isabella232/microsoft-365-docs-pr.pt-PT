---
title: Criar e editar dispositivos AutoPilot
f1.keywords:
- NOCSH
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
description: Saiba como carregar dispositivos usando o AutoPilot no Microsoft 365 Business Premium. Pode atribuir um perfil a um dispositivo ou a um grupo de dispositivos.
ms.openlocfilehash: f2a7f801ae471352595a36b355a874b2de653326
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/21/2020
ms.locfileid: "43627400"
---
# <a name="create-and-edit-autopilot-devices"></a>Criar e editar dispositivos AutoPilot

## <a name="upload-a-list-of-devices"></a>Carregar uma lista de dispositivos

Pode utilizar o [guia Passo a passo](add-autopilot-devices-and-profile.md) para carregar dispositivos, mas também pode carregar dispositivos no separador **Dispositivos.** 
  
Os dispositivos devem satisfazer estes requisitos:
  
- Windows 10, versão 1703 ou mais tarde
    
- Novos dispositivos que não passaram pela experiência do Windows fora da caixa

1. No centro de administração da Microsoft 365, escolha **Dispositivos** \> **AutoPilot**.
  
2. Na página **AutoPilot,** escolha o \> separador **Dispositivos** **Adicionar dispositivos**.
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. No painel **adicionar dispositivos,** navegue para um [ficheiro CSV da lista de dispositivos](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) que preparou \> **Save** \> **Close**.
    
    Pode obter esta informação do seu fornecedor de hardware, ou pode utilizar o [script Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) para gerar um ficheiro CSV. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Atribuir um perfil a um dispositivo ou a um grupo de dispositivos

1. Na página **Prepare o Windows,** escolha o separador **Dispositivos** e selecione a caixa de verificação ao lado de um ou mais dispositivos. 
    
2. No painel **Dispositivo**, selecione um perfil a partir do menu pendente **Perfil atribuído**. 
    
    Se ainda não tiver perfis, consulte a secção [Criar e editar perfis AutoPilot](create-and-edit-autopilot-profiles.md) para obter instruções. 
    
