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
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="f529e-104">Criar e editar dispositivos AutoPilot</span><span class="sxs-lookup"><span data-stu-id="f529e-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="f529e-105">Carregar uma lista de dispositivos</span><span class="sxs-lookup"><span data-stu-id="f529e-105">Upload a list of devices</span></span>

<span data-ttu-id="f529e-106">Pode utilizar o [guia passo a passo](add-autopilot-devices-and-profile.md) para carregar dispositivos, mas também pode carregar no separador **Dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="f529e-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload the in the **Devices** tab.</span></span> 
  
<span data-ttu-id="f529e-107">Os dispositivos têm de cumprir os seguintes requisitos:</span><span class="sxs-lookup"><span data-stu-id="f529e-107">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="f529e-108">Windows 10, versão 1703 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="f529e-108">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="f529e-109">Novos dispositivos que não tenham tido a experiência de configuração inicial do Windows.</span><span class="sxs-lookup"><span data-stu-id="f529e-109">New devices that have not been through Windows out-of-box experience.</span></span>

1. <span data-ttu-id="f529e-110">No centro de administração de negócios do Microsoft 365, escolha **dispositivos** \> **piloto automático**.</span><span class="sxs-lookup"><span data-stu-id="f529e-110">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="f529e-111">Na página **AutoPilot** , escolha a \> guia **dispositivos** **Adicionar dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="f529e-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="f529e-113">No painel **Adicionar dispositivos** , navegue até um [arquivo CSV de lista de dispositivo](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) que você preparou \> **salvar** \> **fechar**.</span><span class="sxs-lookup"><span data-stu-id="f529e-113">On the **Add devices** panel, browse to a [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) that you have prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="f529e-114">Pode obter esta informação através do fabricante de hardware ou pode utilizar o [script do PowerShell Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) que irá gerar um ficheiro cvs.</span><span class="sxs-lookup"><span data-stu-id="f529e-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a csv file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="f529e-115">Atribuir um perfil a um dispositivo ou a um grupo de dispositivos</span><span class="sxs-lookup"><span data-stu-id="f529e-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="f529e-116">Na página **Preparar Windows**, selecione o separador **Dispositivos** e selecione a caixa de verificação junto a um ou mais dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f529e-116">On the **Prepare Windows** page, choose the **Devices** tab and check the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="f529e-117">No painel **Dispositivo**, selecione um perfil a partir do menu pendente **Perfil atribuído**.</span><span class="sxs-lookup"><span data-stu-id="f529e-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="f529e-118">Se ainda não tiver perfis, consulte a secção [Criar e editar perfis AutoPilot](create-and-edit-autopilot-profiles.md) para obter instruções.</span><span class="sxs-lookup"><span data-stu-id="f529e-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
