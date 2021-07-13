---
title: Utilizar o guia passo a passo para adicionar perfis e dispositivos Autopilot
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection:
- M365-subscription-management
- M365-identity-device-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
- AdminTemplateSet
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Saiba como utilizar o Windows AutoPilot para configurar novos dispositivos Windows 10 para a sua empresa, de modo a ficarem prontos para utilização por funcionários.
ms.openlocfilehash: f160ddcd1e41bd44c908ecc8bbd30a9819f76902
ms.sourcegitcommit: 00f001019c653269d85718d410f970887d904304
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/12/2021
ms.locfileid: "53393445"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="0e996-103">Utilizar o guia passo a passo para adicionar perfis e dispositivos Autopilot</span><span class="sxs-lookup"><span data-stu-id="0e996-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="0e996-104">Pode utilizar o Windows AutoPilot para configurar novos **dispositivos** Windows 10 para a sua empresa, para que possam ser utilizados quando os der aos seus funcionários.</span><span class="sxs-lookup"><span data-stu-id="0e996-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they're ready for use when you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="0e996-105">Requisitos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="0e996-105">Device requirements</span></span>

<span data-ttu-id="0e996-106">Os dispositivos têm de cumprir estes requisitos:</span><span class="sxs-lookup"><span data-stu-id="0e996-106">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="0e996-107">Windows 10, versão 1703 ou posterior</span><span class="sxs-lookup"><span data-stu-id="0e996-107">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="0e996-108">Novos dispositivos que não passaram por Windows experiência prática</span><span class="sxs-lookup"><span data-stu-id="0e996-108">New devices that haven't been through Windows out-of-box experience</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="0e996-109">Utilizar o guia de configuração para criar dispositivos e perfis</span><span class="sxs-lookup"><span data-stu-id="0e996-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="0e996-110">Se ainda não criou grupos ou perfis de dispositivos, a melhor forma de começar é utilizar o guia passo a passo.</span><span class="sxs-lookup"><span data-stu-id="0e996-110">If you haven't created device groups or profiles yet, the best way to get started is by using the step-by-step guide.</span></span> <span data-ttu-id="0e996-111">Também pode adicionar [dispositivos e](create-and-edit-autopilot-devices.md) [atribuir perfis](create-and-edit-autopilot-profiles.md) aos utilizadores sem utilizar o guia.</span><span class="sxs-lookup"><span data-stu-id="0e996-111">You can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="0e996-112">Vá para o centro de administração em <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="0e996-112">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="0e996-113">No painel de navegação esquerdo, selecionar **Dispositivos** \> **AutoPilot**.</span><span class="sxs-lookup"><span data-stu-id="0e996-113">On the left navigation pane, choose **Devices** \> **AutoPilot**.</span></span>

    ![No centro de administração, selecionar dispositivos e, em seguida, AutoPilot.](../media/AutoPilot.png)
  
2. <span data-ttu-id="0e996-115">Na página **AutoPilot,** clique ou toque em **Guia de início**.</span><span class="sxs-lookup"><span data-stu-id="0e996-115">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="0e996-117">Na página **Carregar .csv** com a lista de dispositivos, navegue para uma localização onde tenha o ficheiro preparado para .CSV e, em seguida, **abrir** \> **Seguinte.**</span><span class="sxs-lookup"><span data-stu-id="0e996-117">On the **Upload .csv file with list of devices** page, browse to a location where you have the prepared .CSV file, then **Open** \> **Next**.</span></span> <span data-ttu-id="0e996-118">O ficheiro tem de ter três cabeçalhos:</span><span class="sxs-lookup"><span data-stu-id="0e996-118">The file must have three headers:</span></span>
    
    - <span data-ttu-id="0e996-119">Coluna A: Número de Série do Dispositivo</span><span class="sxs-lookup"><span data-stu-id="0e996-119">Column A: Device Serial Number</span></span>
    
    - <span data-ttu-id="0e996-120">Coluna B: ID do Produto Windows</span><span class="sxs-lookup"><span data-stu-id="0e996-120">Column B: Windows Product ID</span></span>
    
    - <span data-ttu-id="0e996-121">Coluna C: Hash do Hardware</span><span class="sxs-lookup"><span data-stu-id="0e996-121">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="0e996-122">Pode obter estas informações com o fornecedor de hardware ou pode utilizar o script do [PowerShell Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) para gerar um ficheiro CSV.</span><span class="sxs-lookup"><span data-stu-id="0e996-122">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
    <span data-ttu-id="0e996-p103">Para obter mais informações, consulte [Ficheiro CSV da lista de dispositivos](../admin/misc/device-list.md). Também pode transferir um ficheiro de exemplo na página **Carregar um ficheiro .csv com a lista de dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="0e996-p103">For more information, see [Device list CSV-file](../admin/misc/device-list.md). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="0e996-125">Este script utiliza WMI para obter as propriedades necessárias para um cliente registar um dispositivo com o Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="0e996-125">This script uses WMI to retrieve properties needed for a customer to register a device with Windows Autopilot.</span></span> <span data-ttu-id="0e996-126">Tenha em atenção que é normal que o ficheiro CSV resultante não recolha um valor de ID do Produto Windows (PKID), uma vez que este não é necessário para registar um dispositivo e que o valor PKID seja NULO no CSV de saída está totalmente bem.</span><span class="sxs-lookup"><span data-stu-id="0e996-126">Note that it is normal for the resulting CSV file to not collect a Windows Product ID (PKID) value since this is not required to register a device and PKID being NULL in the output CSV is totally fine.</span></span> <span data-ttu-id="0e996-127">Só será preenchido o número de série e a hash de hardware.</span><span class="sxs-lookup"><span data-stu-id="0e996-127">Only the serial number and hardware hash will be populated.</span></span>
    
4. <span data-ttu-id="0e996-128">Na página **Atribuir um perfil,** pode escolher um perfil existente ou criar um novo.</span><span class="sxs-lookup"><span data-stu-id="0e996-128">On the **Assign a profile** page, you can either pick an existing profile or create a new one.</span></span> <span data-ttu-id="0e996-129">Se ainda não tiver uma, ser-lhe-á pedido para criar uma.</span><span class="sxs-lookup"><span data-stu-id="0e996-129">If you don't have one yet, you'll be prompted to create one.</span></span> 
    
    <span data-ttu-id="0e996-130">Um perfil é uma coleção de definições que podem ser aplicadas a um único dispositivo ou a um grupo de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="0e996-130">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="0e996-131">As funcionalidades predefinidas são necessárias e são definidas automaticamente.</span><span class="sxs-lookup"><span data-stu-id="0e996-131">The default features are required and are set automatically.</span></span> <span data-ttu-id="0e996-132">As funcionalidades predefinidas são:</span><span class="sxs-lookup"><span data-stu-id="0e996-132">The default features are:</span></span>
    
    - <span data-ttu-id="0e996-133">Ignorar Cortana, OneDrive e registo OEM.</span><span class="sxs-lookup"><span data-stu-id="0e996-133">Skip Cortana, OneDrive, and OEM registration.</span></span>
    
    - <span data-ttu-id="0e996-134">Crie uma experiência de início de sessão com a identidade corporativa da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="0e996-134">Create sign-in experience with your company brand.</span></span>
    
    - <span data-ttu-id="0e996-135">Ligação seus dispositivos para Azure Active Directory contas e inscreva-os automaticamente para que sejam geridos pelos Microsoft 365 Empresas Premium.</span><span class="sxs-lookup"><span data-stu-id="0e996-135">Connect your devices to Azure Active Directory accounts, and automatically enroll them to be managed by Microsoft 365 Business Premium.</span></span>
    
    <span data-ttu-id="0e996-136">Para obter mais informações, consulte [Acerca das definições do Perfil AutoPilot.](autopilot-profile-settings.md)</span><span class="sxs-lookup"><span data-stu-id="0e996-136">For more information, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span> 
    
5. <span data-ttu-id="0e996-137">As outras definições são **Ignorar definições de privacidade** e **Não permitir que o utilizador se torne o administrador local**. Ambas estão configuradas como **Desativado** por predefinição.</span><span class="sxs-lookup"><span data-stu-id="0e996-137">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="0e996-138">Selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="0e996-138">Choose **Next**.</span></span>
    
6. <span data-ttu-id="0e996-139">**A ação terminar** indica que o perfil que criou (ou que escolheu) será aplicado ao grupo de dispositivos que criou ao carregar a lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="0e996-139">**You're done** indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices.</span></span> <span data-ttu-id="0e996-140">As definições entrarão em vigor assim que os utilizadores dos dispositivos entrarem em ação.</span><span class="sxs-lookup"><span data-stu-id="0e996-140">The settings will be in effect when the device users sign in next.</span></span> <span data-ttu-id="0e996-141">Selecione **Fechar**.</span><span class="sxs-lookup"><span data-stu-id="0e996-141">Choose **Close**.</span></span>

## <a name="related-content"></a><span data-ttu-id="0e996-142">Conteúdos relacionados</span><span class="sxs-lookup"><span data-stu-id="0e996-142">Related content</span></span>

<span data-ttu-id="0e996-143">[Acerca das definições do Perfil AutoPilot](autopilot-profile-settings.md) (artigo)</span><span class="sxs-lookup"><span data-stu-id="0e996-143">[About AutoPilot Profile settings](autopilot-profile-settings.md) (article)</span></span>\
<span data-ttu-id="0e996-144">[Opções para proteger os seus dispositivos e dados da aplicação](../admin/devices/choose-device-security.md) (artigo)</span><span class="sxs-lookup"><span data-stu-id="0e996-144">[Options for protecting your devices and app data](../admin/devices/choose-device-security.md) (article)</span></span>
