---
title: Criar e editar perfis AutoPilot
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: 'Aprenda a criar, editar, eliminar ou remover perfis de piloto automático. '
ms.openlocfilehash: 7987cafb3ea234d81be72c79aee8e584a3770875
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/15/2019
ms.locfileid: "34073496"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="c894b-103">Criar e editar perfis AutoPilot</span><span class="sxs-lookup"><span data-stu-id="c894b-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="c894b-104">Criar um perfil</span><span class="sxs-lookup"><span data-stu-id="c894b-104">Create a profile</span></span>

<span data-ttu-id="c894b-105">Um perfil aplica-se a um dispositivo ou grupo de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="c894b-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="c894b-106">No Centro de Admin de negócio do Microsoft 365, escolher **dispositivos** \> **piloto automático**.</span><span class="sxs-lookup"><span data-stu-id="c894b-106">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="c894b-107">Na página do **piloto automático** , escolha o separador **perfis de** \> **Criar perfil**.</span><span class="sxs-lookup"><span data-stu-id="c894b-107">On the **AutoPilot** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="c894b-108">Na página **Criar perfil**, introduza um nome para o perfil que o ajude a identificá-lo, por exemplo Marketing, ative a definição que pretende (para obter mais informações, consulte [Sobre as definições do Perfil AutoPilot](autopilot-profile-settings.md)) e selecione **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="c894b-108">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing, turn on the setting you want (see [About AutoPilot Profile settings](autopilot-profile-settings.md) for more information), and choose **Save**.</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="c894b-110">Aplicar o perfil a um dispositivo</span><span class="sxs-lookup"><span data-stu-id="c894b-110">Apply profile to a device</span></span>

<span data-ttu-id="c894b-p101">Depois de criar um perfil, pode aplicá-lo a um dispositivo ou grupo de dispositivos. Pode escolher um perfil existente no [guia passo a passo](add-autopilot-devices-and-profile.md), aplicá-lo a novos dispositivos ou substituir um perfil existente por um dispositivo ou grupo de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="c894b-p101">After you create a profile you can apply it to a device or a group of devices. You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md), you can apply it to new devices, or you can replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="c894b-113">Na página **Preparar Windows**, selecione o separador **Dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="c894b-113">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="c894b-114">Clique na caixa de verificação junto ao nome do dispositivo e, em seguida, no painel **Dispositivo**, selecione um perfil a partir da lista pendente **Perfil atribuído** \> **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="c894b-114">Click the check-box next to a device name and in the **Device** panel, choose a profile from the **Assigned profile** drop-down \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="c894b-116">Editar, eliminar ou remover um perfil</span><span class="sxs-lookup"><span data-stu-id="c894b-116">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="c894b-p102">Depois de atribuir um perfil a um dispositivo, pode atualizá-lo, mesmo se já tiver atribuído o dispositivo a um utilizador. Quando o dispositivo for ligado à Internet, irá transferir a versão mais recente do seu perfil durante o processo de configuração. Se o utilizador restaurar o respetivo dispositivo para as predefinições de fábrica, o dispositivo irá transferir novamente as atualizações mais recentes para o seu perfil.</span><span class="sxs-lookup"><span data-stu-id="c894b-p102">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="c894b-120">Editar um perfil</span><span class="sxs-lookup"><span data-stu-id="c894b-120">Edit a profile</span></span>

1. <span data-ttu-id="c894b-121">Na página **Preparar Windows**, selecione o separador **Perfis**.</span><span class="sxs-lookup"><span data-stu-id="c894b-121">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="c894b-122">Clique na caixa de verificação junto ao nome de um dispositivo e, em seguida, no painel **Perfil**, atualize as definições disponíveis \> **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="c894b-122">Click the check-box next to a device name and in the **Profile** panel update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="c894b-123">Se o fizer antes de um utilizador ligar o dispositivo à Internet, o perfil será aplicado no processo de configuração.</span><span class="sxs-lookup"><span data-stu-id="c894b-123">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="c894b-124">Eliminar um perfil</span><span class="sxs-lookup"><span data-stu-id="c894b-124">Delete a profile</span></span>

1. <span data-ttu-id="c894b-125">Na página **Preparar Windows**, selecione o separador **Perfis**.</span><span class="sxs-lookup"><span data-stu-id="c894b-125">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="c894b-126">Clique na caixa de verificação junto ao nome de um dispositivo e, em seguida, no painel **Perfil**, clique em **Eliminar perfil** \> **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="c894b-126">Click the check-box next to a device name and in the **Profile** panel click **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="c894b-127">Quando eliminar um perfil, o mesmo será removido do dispositivo ou grupo de dispositivos ao qual estava atribuído.</span><span class="sxs-lookup"><span data-stu-id="c894b-127">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="c894b-128">Remover um perfil</span><span class="sxs-lookup"><span data-stu-id="c894b-128">Remove a profile</span></span>

1. <span data-ttu-id="c894b-129">Na página **Preparar Windows**, selecione o separador **Dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="c894b-129">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="c894b-130">Clique na caixa de verificação junto ao nome do dispositivo e, em seguida, no painel **Dispositivo**, selecione **Nenhum** na lista pendente **Perfil atribuído** \> **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="c894b-130">Click the check-box next to a device name and in the **Device** panel, choose a **None** from the **Assigned profile** drop-down \> **Save**.</span></span>
    
