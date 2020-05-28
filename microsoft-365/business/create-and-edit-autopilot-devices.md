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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Saiba como carregar dispositivos usando o AutoPilot no Microsoft 365 Business Premium. Pode atribuir um perfil a um dispositivo ou a um grupo de dispositivos.
ms.openlocfilehash: 8c3d029d682ae30444bdc7d30a4790a8f982e0e0
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/27/2020
ms.locfileid: "44401000"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="db0f4-104">Criar e editar dispositivos AutoPilot</span><span class="sxs-lookup"><span data-stu-id="db0f4-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="db0f4-105">Carregar uma lista de dispositivos</span><span class="sxs-lookup"><span data-stu-id="db0f4-105">Upload a list of devices</span></span>

<span data-ttu-id="db0f4-106">Pode utilizar o [guia Passo a passo](add-autopilot-devices-and-profile.md) para carregar dispositivos, mas também pode carregar dispositivos no separador **Dispositivos.**</span><span class="sxs-lookup"><span data-stu-id="db0f4-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload devices in the **Devices** tab.</span></span> 
  
<span data-ttu-id="db0f4-107">Os dispositivos devem satisfazer estes requisitos:</span><span class="sxs-lookup"><span data-stu-id="db0f4-107">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="db0f4-108">Windows 10, versão 1703 ou mais tarde</span><span class="sxs-lookup"><span data-stu-id="db0f4-108">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="db0f4-109">Novos dispositivos que não passaram pela experiência do Windows fora da caixa</span><span class="sxs-lookup"><span data-stu-id="db0f4-109">New devices that haven't been through Windows out-of-box experience</span></span>

1. <span data-ttu-id="db0f4-110">No centro de administração da Microsoft 365, escolha **Dispositivos** \> **AutoPilot**.</span><span class="sxs-lookup"><span data-stu-id="db0f4-110">In the Microsoft 365 admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="db0f4-111">Na página **AutoPilot,** escolha o separador **Devices** \> **Dispositivos Adicionar dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="db0f4-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="db0f4-113">No painel **adicionar dispositivos,** navegue para um [ficheiro CSV da lista de dispositivos](https://docs.microsoft.com/microsoft-365/admin/misc/device-list) que preparou \> **Save** \> **Close**.</span><span class="sxs-lookup"><span data-stu-id="db0f4-113">On the **Add devices** panel, browse to a [Device list CSV file](https://docs.microsoft.com/microsoft-365/admin/misc/device-list) that you prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="db0f4-114">Pode obter esta informação do seu fornecedor de hardware, ou pode utilizar o [script Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) para gerar um ficheiro CSV.</span><span class="sxs-lookup"><span data-stu-id="db0f4-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="db0f4-115">Atribuir um perfil a um dispositivo ou a um grupo de dispositivos</span><span class="sxs-lookup"><span data-stu-id="db0f4-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="db0f4-116">Na página **Prepare o Windows,** escolha o separador **Dispositivos** e selecione a caixa de verificação ao lado de um ou mais dispositivos.</span><span class="sxs-lookup"><span data-stu-id="db0f4-116">On the **Prepare Windows** page, choose the **Devices** tab, and select the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="db0f4-117">No painel **Dispositivo**, selecione um perfil a partir do menu pendente **Perfil atribuído**.</span><span class="sxs-lookup"><span data-stu-id="db0f4-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="db0f4-118">Se ainda não tiver perfis, consulte a secção [Criar e editar perfis AutoPilot](create-and-edit-autopilot-profiles.md) para obter instruções.</span><span class="sxs-lookup"><span data-stu-id="db0f4-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
