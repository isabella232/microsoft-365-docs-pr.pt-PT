---
title: Criar e editar perfis AutoPilot
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
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: Aprenda a criar, editar, excluir ou remover perfis AutoPilot.
ms.openlocfilehash: 28f5b679d58711d11d9af26dffb7022024b72c79
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/15/2020
ms.locfileid: "42065913"
---
# <a name="create-and-edit-autopilot-profiles"></a>Criar e editar perfis AutoPilot

## <a name="create-a-profile"></a>Criar um perfil

Um perfil aplica-se a um dispositivo ou grupo de dispositivos.
  
1. No centro de Administração de Negócios Microsoft 365, escolha **Dispositivos** \> **AutoPilot**.
  
2. Na página **AutoPilot,** **** escolha o \> separador Perfis **Criar perfil**.
    
3. Na página de **perfil Criar,** introduza um nome para o perfil que o ajude a identificá-lo, por exemplo, marketing. Ligue a definição que deseja e, em seguida, escolha **Guardar**. Para obter mais informações sobre as definições de perfil autoPilot, consulte as definições de [perfil autopilot](autopilot-profile-settings.md).
    
    ![Enter name and turn on settings in the Create profile panel.](../media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a>Aplicar o perfil a um dispositivo

Depois de criar um perfil, pode aplicá-lo a um dispositivo ou a um grupo de dispositivos. Pode escolher um perfil existente no [guia passo a passo](add-autopilot-devices-and-profile.md) e aplicá-lo a novos dispositivos ou substituir um perfil existente para um dispositivo ou grupo de dispositivos. 
  
1. Na página **Preparar Windows**, selecione o separador **Dispositivos**. 
    
2. Selecione a caixa de verificação ao lado de um nome de dispositivo e, no painel **dispositivo,** escolha um perfil da lista \> de abandono do **perfil atribuído** **Save**.
    
    ![In the Device panel, select an Assigned profile to apply it.](../media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a>Editar, eliminar ou remover um perfil

Depois de atribuir um perfil a um dispositivo, pode atualizá-lo, mesmo se já tiver atribuído o dispositivo a um utilizador. Quando o dispositivo for ligado à Internet, irá transferir a versão mais recente do seu perfil durante o processo de configuração. Se o utilizador restaurar o respetivo dispositivo para as predefinições de fábrica, o dispositivo irá transferir novamente as atualizações mais recentes para o seu perfil. 
  
### <a name="edit-a-profile"></a>Editar um perfil

1. Na página **Preparar Windows**, selecione o separador **Perfis**. 
    
2. Selecione a caixa de verificação ao lado de um nome \> de dispositivo e, no painel **Profile,** atualize qualquer uma das definições disponíveis **Guardar**.
    
    Se o fizer antes de um utilizador ligar o dispositivo à Internet, o perfil será aplicado no processo de configuração.
    
### <a name="delete-a-profile"></a>Eliminar um perfil

1. Na página **Preparar Windows**, selecione o separador **Perfis**. 
    
2. Selecione a caixa de verificação ao lado de um nome de dispositivo e, no painel **profile,** selecione Eliminar o **perfil** \> **Save**.
    
    Quando eliminar um perfil, o mesmo será removido do dispositivo ou grupo de dispositivos ao qual estava atribuído.
    
### <a name="remove-a-profile"></a>Remover um perfil

1. Na página **Preparar Windows**, selecione o separador **Dispositivos**. 
    
2. Selecione a caixa de verificação ao lado de um nome de dispositivo \> e, no painel **dispositivo,** escolha **nenhuma** da lista de abandono do **perfil atribuído** **Save**.
    
