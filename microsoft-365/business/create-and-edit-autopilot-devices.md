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
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="830d5-104">Criar e editar dispositivos AutoPilot</span><span class="sxs-lookup"><span data-stu-id="830d5-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="830d5-105">Carregar uma lista de dispositivos</span><span class="sxs-lookup"><span data-stu-id="830d5-105">Upload a list of devices</span></span>

<span data-ttu-id="830d5-106">Você pode usar o [guia passo a passo](add-autopilot-devices-and-profile.md) para carregar dispositivos, mas também pode carregar dispositivos na aba **dispositivos.**</span><span class="sxs-lookup"><span data-stu-id="830d5-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload devices in the **Devices** tab.</span></span> 
  
<span data-ttu-id="830d5-107">Os dispositivos devem atender a esses requisitos:</span><span class="sxs-lookup"><span data-stu-id="830d5-107">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="830d5-108">Windows 10, versão 1703 ou mais tarde</span><span class="sxs-lookup"><span data-stu-id="830d5-108">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="830d5-109">Novos dispositivos que não passaram pela experiência do Windows fora da caixa</span><span class="sxs-lookup"><span data-stu-id="830d5-109">New devices that haven't been through Windows out-of-box experience</span></span>

1. <span data-ttu-id="830d5-110">No centro de administração de negócios Microsoft 365, escolha **dispositivos** \> **AutoPilot**.</span><span class="sxs-lookup"><span data-stu-id="830d5-110">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="830d5-111">Na página **AutoPilot,** escolha a \> guia **dispositivos** **Adicionar dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="830d5-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="830d5-113">No painel **de adicionar dispositivos,** navegue em um arquivo [CSV da lista do dispositivo](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) que você preparou \> **Save** \> **Close.**</span><span class="sxs-lookup"><span data-stu-id="830d5-113">On the **Add devices** panel, browse to a [Device list CSV file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) that you prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="830d5-114">Você pode obter essas informações do fornecedor de hardware ou pode usar o [script Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) para gerar um arquivo CSV.</span><span class="sxs-lookup"><span data-stu-id="830d5-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="830d5-115">Atribuir um perfil a um dispositivo ou a um grupo de dispositivos</span><span class="sxs-lookup"><span data-stu-id="830d5-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="830d5-116">Na página **Prepare Windows,** escolha a guia **dispositivos** e selecione a caixa de seleção ao lado de um ou mais dispositivos.</span><span class="sxs-lookup"><span data-stu-id="830d5-116">On the **Prepare Windows** page, choose the **Devices** tab, and select the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="830d5-117">No painel **Dispositivo**, selecione um perfil a partir do menu pendente **Perfil atribuído**.</span><span class="sxs-lookup"><span data-stu-id="830d5-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="830d5-118">Se ainda não tiver perfis, consulte a secção [Criar e editar perfis AutoPilot](create-and-edit-autopilot-profiles.md) para obter instruções.</span><span class="sxs-lookup"><span data-stu-id="830d5-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
