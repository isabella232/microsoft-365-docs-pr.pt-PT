---
title: Criar e editar dispositivos AutoPilot
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
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Obter informações sobre como carregar dispositivos a utilizar o piloto automático no Microsoft 365 Business. Pode atribuir um perfil para um dispositivo ou um grupo de dispositivos.
ms.openlocfilehash: cc1f81e9efd9b16e27b8abfbb0927d241535077e
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982938"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="54f7d-104">Criar e editar dispositivos AutoPilot</span><span class="sxs-lookup"><span data-stu-id="54f7d-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="54f7d-105">Carregar uma lista de dispositivos</span><span class="sxs-lookup"><span data-stu-id="54f7d-105">Upload a list of devices</span></span>

<span data-ttu-id="54f7d-106">Pode utilizar o [guia passo a passo](add-autopilot-devices-and-profile.md) para carregar dispositivos, mas também pode carregar no separador **Dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="54f7d-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload the in the **Devices** tab.</span></span> 
  
<span data-ttu-id="54f7d-107">Os dispositivos têm de cumprir os seguintes requisitos:</span><span class="sxs-lookup"><span data-stu-id="54f7d-107">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="54f7d-108">Windows 10, versão 1703 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="54f7d-108">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="54f7d-109">Novos dispositivos que não tenham tido a experiência de configuração inicial do Windows.</span><span class="sxs-lookup"><span data-stu-id="54f7d-109">New devices that have not been through Windows out-of-box experience.</span></span>
    
1. <span data-ttu-id="54f7d-110">No centro de administração do Microsoft 365 Business, selecione **Implementar o Windows com o Autopilot** no cartão **Ações do dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="54f7d-110">In the Microsoft 365 Business Admin center, choose **Deploy Windows with AutoPilot** on the **Device actions** card.</span></span> 
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. <span data-ttu-id="54f7d-112">Na página **Preparar Windows**, selecione o separador **Dispositivos** \> **Adicionar dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="54f7d-112">On the **Prepare Windows** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="54f7d-114">No painel **Adicionar dispositivos** , navegue para uma [lista de dispositivos ficheiro CSV](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) que tenha preparado \> **Guardar** \> **Fechar**.</span><span class="sxs-lookup"><span data-stu-id="54f7d-114">On the **Add devices** panel, browse to a [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) that you have prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="54f7d-115">Pode obter esta informação através do fabricante de hardware ou pode utilizar o [script do PowerShell Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) que irá gerar um ficheiro cvs.</span><span class="sxs-lookup"><span data-stu-id="54f7d-115">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a csv file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="54f7d-116">Atribuir um perfil a um dispositivo ou a um grupo de dispositivos</span><span class="sxs-lookup"><span data-stu-id="54f7d-116">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="54f7d-117">Na página **Preparar Windows**, selecione o separador **Dispositivos** e selecione a caixa de verificação junto a um ou mais dispositivos.</span><span class="sxs-lookup"><span data-stu-id="54f7d-117">On the **Prepare Windows** page, choose the **Devices** tab and check the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="54f7d-118">No painel **Dispositivo**, selecione um perfil a partir do menu pendente **Perfil atribuído**.</span><span class="sxs-lookup"><span data-stu-id="54f7d-118">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="54f7d-119">Se ainda não tiver perfis, consulte a secção [Criar e editar perfis AutoPilot](create-and-edit-autopilot-profiles.md) para obter instruções.</span><span class="sxs-lookup"><span data-stu-id="54f7d-119">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
