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
description: Saiba como carregar dispositivos utilizando o AutoPilot no Microsoft 365 Business Premium. Pode atribuir um perfil a um dispositivo ou a um grupo de dispositivos.
ms.openlocfilehash: 910abb98b94b749177b04cd12c766f82d348e379
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913404"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="609b8-104">Criar e editar dispositivos AutoPilot</span><span class="sxs-lookup"><span data-stu-id="609b8-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="609b8-105">Carregar uma lista de dispositivos</span><span class="sxs-lookup"><span data-stu-id="609b8-105">Upload a list of devices</span></span>

<span data-ttu-id="609b8-106">Pode utilizar o [guia passo a passo](add-autopilot-devices-and-profile.md) para carregar dispositivos, mas também pode carregar dispositivos no separador **Dispositivos.**</span><span class="sxs-lookup"><span data-stu-id="609b8-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload devices in the **Devices** tab.</span></span> 
  
<span data-ttu-id="609b8-107">Os dispositivos devem satisfazer estes requisitos:</span><span class="sxs-lookup"><span data-stu-id="609b8-107">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="609b8-108">Windows 10, versão 1703 ou mais tarde</span><span class="sxs-lookup"><span data-stu-id="609b8-108">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="609b8-109">Novos dispositivos que não passaram pela experiência fora de caixa do Windows</span><span class="sxs-lookup"><span data-stu-id="609b8-109">New devices that haven't been through Windows out-of-box experience</span></span>

1. <span data-ttu-id="609b8-110">No centro de administração Microsoft 365, escolha **Dispositivos** \> **AutoPilot**.</span><span class="sxs-lookup"><span data-stu-id="609b8-110">In the Microsoft 365 admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="609b8-111">Na página **AutoPilot,** escolha o separador **Dispositivos** \> **Adicionar dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="609b8-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="609b8-113">No painel **de dispositivos Adicionar,** navegue num [ficheiro CSV da lista de dispositivos](../admin/misc/device-list.md) que preparou \> **Save** \> **Close**.</span><span class="sxs-lookup"><span data-stu-id="609b8-113">On the **Add devices** panel, browse to a [Device list CSV file](../admin/misc/device-list.md) that you prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="609b8-114">Pode obter estas informações do seu fornecedor de hardware ou pode utilizar o [script Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) para gerar um ficheiro CSV.</span><span class="sxs-lookup"><span data-stu-id="609b8-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="609b8-115">Atribuir um perfil a um dispositivo ou a um grupo de dispositivos</span><span class="sxs-lookup"><span data-stu-id="609b8-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="609b8-116">Na página Preparar o **Windows,** escolha o separador **Dispositivos** e selecione a caixa de verificação ao lado de um ou mais dispositivos.</span><span class="sxs-lookup"><span data-stu-id="609b8-116">On the **Prepare Windows** page, choose the **Devices** tab, and select the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="609b8-117">No painel **Dispositivo**, selecione um perfil a partir do menu pendente **Perfil atribuído**.</span><span class="sxs-lookup"><span data-stu-id="609b8-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="609b8-118">Se ainda não tiver perfis, consulte a secção [Criar e editar perfis AutoPilot](create-and-edit-autopilot-profiles.md) para obter instruções.</span><span class="sxs-lookup"><span data-stu-id="609b8-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
