---
title: Criar e editar perfis AutoPilot
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
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
ms.openlocfilehash: 4658a27e5f2c64a52f8a7d08b3fc13df5e239dc3
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983138"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="9ae2b-103">Criar e editar perfis AutoPilot</span><span class="sxs-lookup"><span data-stu-id="9ae2b-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="9ae2b-104">Criar um perfil</span><span class="sxs-lookup"><span data-stu-id="9ae2b-104">Create a profile</span></span>

<span data-ttu-id="9ae2b-105">Um perfil aplica-se a um dispositivo ou grupo de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="9ae2b-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="9ae2b-106">No centro de administração do Microsoft 365 Business, selecione **Implementar o Windows com o Autopilot** no cartão **Ações do dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="9ae2b-106">In the Microsoft 365 Business Admin center, choose **Deploy Windows with AutoPilot** on the **Device actions** card.</span></span> 
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. <span data-ttu-id="9ae2b-108">Na página **Preparar Windows**, selecione o separador **Perfis** \> **Criar perfil**.</span><span class="sxs-lookup"><span data-stu-id="9ae2b-108">On the **Prepare Windows** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="9ae2b-109">Na página **Criar perfil**, introduza um nome para o perfil que o ajude a identificá-lo, por exemplo Marketing, ative a definição que pretende (para obter mais informações, consulte [Sobre as definições do Perfil AutoPilot](autopilot-profile-settings.md)) e selecione **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="9ae2b-109">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing, turn on the setting you want (see [About AutoPilot Profile settings](autopilot-profile-settings.md) for more information), and choose **Save**.</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="9ae2b-111">Aplicar o perfil a um dispositivo</span><span class="sxs-lookup"><span data-stu-id="9ae2b-111">Apply profile to a device</span></span>

<span data-ttu-id="9ae2b-p101">Depois de criar um perfil, pode aplicá-lo a um dispositivo ou grupo de dispositivos. Pode escolher um perfil existente no [guia passo a passo](add-autopilot-devices-and-profile.md), aplicá-lo a novos dispositivos ou substituir um perfil existente por um dispositivo ou grupo de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="9ae2b-p101">After you create a profile you can apply it to a device or a group of devices. You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md), you can apply it to new devices, or you can replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="9ae2b-114">Na página **Preparar Windows**, selecione o separador **Dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="9ae2b-114">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="9ae2b-115">Clique na caixa de verificação junto ao nome do dispositivo e, em seguida, no painel **Dispositivo**, selecione um perfil a partir da lista pendente **Perfil atribuído** \> **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="9ae2b-115">Click the check-box next to a device name and in the **Device** panel, choose a profile from the **Assigned profile** drop-down \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="9ae2b-117">Editar, eliminar ou remover um perfil</span><span class="sxs-lookup"><span data-stu-id="9ae2b-117">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="9ae2b-p102">Depois de atribuir um perfil a um dispositivo, pode atualizá-lo, mesmo se já tiver atribuído o dispositivo a um utilizador. Quando o dispositivo for ligado à Internet, irá transferir a versão mais recente do seu perfil durante o processo de configuração. Se o utilizador restaurar o respetivo dispositivo para as predefinições de fábrica, o dispositivo irá transferir novamente as atualizações mais recentes para o seu perfil.</span><span class="sxs-lookup"><span data-stu-id="9ae2b-p102">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="9ae2b-121">Editar um perfil</span><span class="sxs-lookup"><span data-stu-id="9ae2b-121">Edit a profile</span></span>

1. <span data-ttu-id="9ae2b-122">Na página **Preparar Windows**, selecione o separador **Perfis**.</span><span class="sxs-lookup"><span data-stu-id="9ae2b-122">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="9ae2b-123">Clique na caixa de verificação junto ao nome de um dispositivo e, em seguida, no painel **Perfil**, atualize as definições disponíveis \> **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="9ae2b-123">Click the check-box next to a device name and in the **Profile** panel update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="9ae2b-124">Se o fizer antes de um utilizador ligar o dispositivo à Internet, o perfil será aplicado no processo de configuração.</span><span class="sxs-lookup"><span data-stu-id="9ae2b-124">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="9ae2b-125">Eliminar um perfil</span><span class="sxs-lookup"><span data-stu-id="9ae2b-125">Delete a profile</span></span>

1. <span data-ttu-id="9ae2b-126">Na página **Preparar Windows**, selecione o separador **Perfis**.</span><span class="sxs-lookup"><span data-stu-id="9ae2b-126">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="9ae2b-127">Clique na caixa de verificação junto ao nome de um dispositivo e, em seguida, no painel **Perfil**, clique em **Eliminar perfil** \> **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="9ae2b-127">Click the check-box next to a device name and in the **Profile** panel click **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="9ae2b-128">Quando eliminar um perfil, o mesmo será removido do dispositivo ou grupo de dispositivos ao qual estava atribuído.</span><span class="sxs-lookup"><span data-stu-id="9ae2b-128">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="9ae2b-129">Remover um perfil</span><span class="sxs-lookup"><span data-stu-id="9ae2b-129">Remove a profile</span></span>

1. <span data-ttu-id="9ae2b-130">Na página **Preparar Windows**, selecione o separador **Dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="9ae2b-130">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="9ae2b-131">Clique na caixa de verificação junto ao nome do dispositivo e, em seguida, no painel **Dispositivo**, selecione **Nenhum** na lista pendente **Perfil atribuído** \> **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="9ae2b-131">Click the check-box next to a device name and in the **Device** panel, choose a **None** from the **Assigned profile** drop-down \> **Save**.</span></span>
    
