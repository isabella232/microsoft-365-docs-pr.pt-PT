---
title: Criar e editar dispositivos AutoPilot
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Obter informações sobre como carregar dispositivos a utilizar o piloto automático no Microsoft 365 Business. Pode atribuir um perfil para um dispositivo ou um grupo de dispositivos.
ms.openlocfilehash: 6492f1469a1ac9ea67750e9ffa071d19c88c743f
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660445"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="1ef75-104">Criar e editar dispositivos AutoPilot</span><span class="sxs-lookup"><span data-stu-id="1ef75-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="1ef75-105">Carregar uma lista de dispositivos</span><span class="sxs-lookup"><span data-stu-id="1ef75-105">Upload a list of devices</span></span>

<span data-ttu-id="1ef75-106">Pode utilizar o [guia passo a passo](add-autopilot-devices-and-profile.md) para carregar dispositivos, mas também pode carregar no separador **Dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="1ef75-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload the in the **Devices** tab.</span></span> 
  
<span data-ttu-id="1ef75-107">Os dispositivos têm de cumprir os seguintes requisitos:</span><span class="sxs-lookup"><span data-stu-id="1ef75-107">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="1ef75-108">Windows 10, versão 1703 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="1ef75-108">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="1ef75-109">Novos dispositivos que não tenham tido a experiência de configuração inicial do Windows.</span><span class="sxs-lookup"><span data-stu-id="1ef75-109">New devices that have not been through Windows out-of-box experience.</span></span>

1. <span data-ttu-id="1ef75-110">No Centro de Admin de negócio do Microsoft 365, escolher **dispositivos** \> **piloto automático**.</span><span class="sxs-lookup"><span data-stu-id="1ef75-110">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="1ef75-111">Na página **piloto automático** , seleccione o separador **dispositivos** \> **Adicionar dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="1ef75-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="1ef75-113">No painel **Adicionar dispositivos** , navegue para uma [lista de dispositivos ficheiro CSV](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) que tenha preparado \> **Guardar** \> **Fechar**.</span><span class="sxs-lookup"><span data-stu-id="1ef75-113">On the **Add devices** panel, browse to a [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) that you have prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="1ef75-114">Pode obter esta informação através do fabricante de hardware ou pode utilizar o [script do PowerShell Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) que irá gerar um ficheiro cvs.</span><span class="sxs-lookup"><span data-stu-id="1ef75-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a csv file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="1ef75-115">Atribuir um perfil a um dispositivo ou a um grupo de dispositivos</span><span class="sxs-lookup"><span data-stu-id="1ef75-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="1ef75-116">Na página **Preparar Windows**, selecione o separador **Dispositivos** e selecione a caixa de verificação junto a um ou mais dispositivos.</span><span class="sxs-lookup"><span data-stu-id="1ef75-116">On the **Prepare Windows** page, choose the **Devices** tab and check the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="1ef75-117">No painel **Dispositivo**, selecione um perfil a partir do menu pendente **Perfil atribuído**.</span><span class="sxs-lookup"><span data-stu-id="1ef75-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="1ef75-118">Se ainda não tiver perfis, consulte a secção [Criar e editar perfis AutoPilot](create-and-edit-autopilot-profiles.md) para obter instruções.</span><span class="sxs-lookup"><span data-stu-id="1ef75-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
