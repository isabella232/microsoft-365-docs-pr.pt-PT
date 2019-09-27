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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Saiba como carregar dispositivos usando o AutoPilot no Microsoft 365 Business. Você pode atribuir um perfil a um dispositivo ou a um grupo de dispositivos.
ms.openlocfilehash: 9ae94266f5a41d8d115fc92f0f080a6fdbdc9f15
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288021"
---
# <a name="create-and-edit-autopilot-devices"></a>Criar e editar dispositivos AutoPilot

## <a name="upload-a-list-of-devices"></a>Carregar uma lista de dispositivos

Pode utilizar o [guia passo a passo](add-autopilot-devices-and-profile.md) para carregar dispositivos, mas também pode carregar no separador **Dispositivos**. 
  
Os dispositivos têm de cumprir os seguintes requisitos:
  
- Windows 10, versão 1703 ou posterior.
    
- Novos dispositivos que não tenham tido a experiência de configuração inicial do Windows.

1. No centro de administração de negócios do Microsoft 365, escolha **dispositivos** \> **piloto automático**.
  
2. Na página **AutoPilot** , escolha a \> guia **dispositivos** **Adicionar dispositivos**.
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. No painel **Adicionar dispositivos** , navegue até um [arquivo CSV de lista de dispositivo](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) que você preparou \> **salvar** \> **fechar**.
    
    Pode obter esta informação através do fabricante de hardware ou pode utilizar o [script do PowerShell Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) que irá gerar um ficheiro cvs. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Atribuir um perfil a um dispositivo ou a um grupo de dispositivos

1. Na página **Preparar Windows**, selecione o separador **Dispositivos** e selecione a caixa de verificação junto a um ou mais dispositivos. 
    
2. No painel **Dispositivo**, selecione um perfil a partir do menu pendente **Perfil atribuído**. 
    
    Se ainda não tiver perfis, consulte a secção [Criar e editar perfis AutoPilot](create-and-edit-autopilot-profiles.md) para obter instruções. 
    
