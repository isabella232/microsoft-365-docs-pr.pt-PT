---
title: Criar e editar perfis AutoPilot
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: Saiba como criar um perfil AutoPilot e aplicá-lo a um dispositivo, bem como editar ou eliminar um perfil ou remover um perfil de um dispositivo.
ms.openlocfilehash: d2a3038346b7879006dc2eb50ebe2e70cc6fae92c020a38465cec9d468c638b2
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53797232"
---
# <a name="create-and-edit-autopilot-profiles"></a>Criar e editar perfis AutoPilot

## <a name="create-a-profile"></a>Criar um perfil

Um perfil aplica-se a um dispositivo ou grupo de dispositivos.
  
1. Na seta centro de administração do Microsoft 365, **selecionar Dispositivos** \> **AutoPilot**.
  
2. Na página **AutoPilot,** selecionar o **separador Perfis** \> **Criar perfil.**
    
3. Na página **Criar perfil,** introduza um nome para o perfil que o ajude a identificá-lo, por exemplo Marketing. A turn on the setting you want, and then choose **Save**. Para obter mais informações sobre as definições de perfil AutoPilot, consulte [Acerca das definições do Perfil AutoPilot.](autopilot-profile-settings.md)
    
    ![Enter name and turn on settings in the Create profile panel.](../media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a>Aplicar o perfil a um dispositivo

Depois de criar um perfil, pode aplicá-lo a um dispositivo ou grupo de dispositivos. Pode escolher um perfil existente no guia passo a passo e [aplicá-lo](add-autopilot-devices-and-profile.md) a novos dispositivos ou substituir um perfil existente por um dispositivo ou grupo de dispositivos. 
  
1. Na página **Preparar Windows**, selecione o separador **Dispositivos**. 
    
2. Selecione a caixa de verificação junto  ao nome de um  dispositivo e, no painel Dispositivo, selecione um perfil a partir da lista de listas de perfil atribuído \> **Guardar.**
    
    ![In the Device panel, select an Assigned profile to apply it.](../media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a>Editar, eliminar ou remover um perfil

Depois de atribuir um perfil a um dispositivo, pode atualizá-lo, mesmo se já tiver atribuído o dispositivo a um utilizador. Quando o dispositivo for ligado à Internet, irá transferir a versão mais recente do seu perfil durante o processo de configuração. Se o utilizador restaurar o respetivo dispositivo para as predefinições de fábrica, o dispositivo irá transferir novamente as atualizações mais recentes para o seu perfil. 
  
### <a name="edit-a-profile"></a>Editar um perfil

1. Na página **Preparar Windows**, selecione o separador **Perfis**. 
    
2. Selecione a caixa de verificação junto ao nome do dispositivo e, no **painel Perfil,** atualize qualquer uma das definições \> **disponíveis Guardar.**
    
    Se o fizer antes de um utilizador ligar o dispositivo à Internet, o perfil será aplicado no processo de configuração.
    
### <a name="delete-a-profile"></a>Eliminar um perfil

1. Na página **Preparar Windows**, selecione o separador **Perfis**. 
    
2. Selecione a caixa de verificação junto ao nome de um dispositivo e, no **painel Perfil,** selecione **Eliminar perfil** \> **Guardar**.
    
    Quando eliminar um perfil, o mesmo será removido do dispositivo ou grupo de dispositivos ao qual estava atribuído.
    
### <a name="remove-a-profile"></a>Remover um perfil

1. Na página **Preparar Windows**, selecione o separador **Dispositivos**. 
    
2. Selecione a caixa de verificação ao  lado do nome de um dispositivo e, no painel Dispositivo, selecione **Nenhum** na lista de listas drop-down **perfil** atribuído \> **Guardar.**
    
