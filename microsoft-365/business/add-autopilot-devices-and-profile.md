---
title: Utilizar o guia passo a passo para adicionar perfis e dispositivos Autopilot
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Obter informações sobre como utilizar o piloto automático do Windows para configurar novos dispositivos Windows 10 para a sua empresa.
ms.openlocfilehash: e0802ddcc0964d0b8d102f7dbdb9116b33cdcf58
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32277153"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="b0d7c-103">Utilizar o guia passo a passo para adicionar perfis e dispositivos Autopilot</span><span class="sxs-lookup"><span data-stu-id="b0d7c-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="b0d7c-104">Pode utilizar o Windows AutoPilot para configurar novos dispositivos com Windows 10 da sua empresa, para que estejam prontos para uma utilização produtiva assim que os der aos seus funcionários.</span><span class="sxs-lookup"><span data-stu-id="b0d7c-104">You can use Windows AutoPilot to set up new Windows 10 devices for your business so they are ready for productive use as soon as you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="b0d7c-105">Requisitos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="b0d7c-105">Device requirements</span></span>

<span data-ttu-id="b0d7c-106">Os dispositivos têm de cumprir os seguintes requisitos:</span><span class="sxs-lookup"><span data-stu-id="b0d7c-106">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="b0d7c-107">Windows 10, versão 1703 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="b0d7c-107">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="b0d7c-108">Novos dispositivos que não tenham tido a experiência de configuração inicial do Windows.</span><span class="sxs-lookup"><span data-stu-id="b0d7c-108">New devices that have not been through Windows out-of-box experience.</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="b0d7c-109">Utilizar o guia de configuração para criar dispositivos e perfis</span><span class="sxs-lookup"><span data-stu-id="b0d7c-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="b0d7c-110">Se ainda não tiver criado perfis e grupos de dispositivos, a melhor forma de começar é com o guia passo a passo, mas também pode [adicionar dispositivos](create-and-edit-autopilot-devices.md) e [atribuir perfis](create-and-edit-autopilot-profiles.md) aos mesmos sem utilizar o guia.</span><span class="sxs-lookup"><span data-stu-id="b0d7c-110">If you have no device groups or profiles created yet, the best way to get started is by using the step-by-step guide, but you can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="b0d7c-111">No centro de administração do Microsoft 365 Business, localize o cartão **Ações do dispositivo** e selecione **Implementar o Windows com o AutoPilot**.</span><span class="sxs-lookup"><span data-stu-id="b0d7c-111">In the Microsoft 365 Business admin center, locate the **Device actions** card, and choose **Deploy Windows with Autopilot**.</span></span>
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. <span data-ttu-id="b0d7c-113">Na página **Preparar Windows**, clique ou toque em **Guia de introdução**.</span><span class="sxs-lookup"><span data-stu-id="b0d7c-113">On the **Prepare Windows** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="b0d7c-p101">Na página **Carregar um ficheiro .csv com a lista de dispositivos**, procure uma localização com o ficheiro .CSV preparado e, em seguida, selecione **Abrir** \> **Seguinte**. O ficheiro deverá ter três cabeçalhos:</span><span class="sxs-lookup"><span data-stu-id="b0d7c-p101">On the **Upload .csv file with list of devices** page, browse to a locations where you have the prepared .CSV file, then **Open** \> **Next**. The file should have three headers:</span></span>
    
  - <span data-ttu-id="b0d7c-117">Coluna A: Número de Série do Dispositivo</span><span class="sxs-lookup"><span data-stu-id="b0d7c-117">Column A: Device Serial Number</span></span>
    
  - <span data-ttu-id="b0d7c-118">Coluna B: ID do Produto Windows</span><span class="sxs-lookup"><span data-stu-id="b0d7c-118">Column B: Windows Product ID</span></span>
    
  - <span data-ttu-id="b0d7c-119">Coluna C: Hash do Hardware</span><span class="sxs-lookup"><span data-stu-id="b0d7c-119">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="b0d7c-120">Pode obter esta informação através do fabricante de hardware ou pode utilizar o [script do PowerShell Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) que irá gerar um ficheiro CSV.</span><span class="sxs-lookup"><span data-stu-id="b0d7c-120">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a CSV file.</span></span> 
    
    <span data-ttu-id="b0d7c-p102">Para obter mais informações, consulte [Ficheiro CSV da lista de dispositivos](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Também pode transferir um ficheiro de exemplo na página **Carregar um ficheiro .csv com a lista de dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="b0d7c-p102">For more information, see [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
4. <span data-ttu-id="b0d7c-p103">Na página **Atribuir um perfil**, pode selecionar um perfil existente ou criar um novo. Se ainda não tiver um, ser-lhe-á pedido que crie um novo.</span><span class="sxs-lookup"><span data-stu-id="b0d7c-p103">On the **Assign a profile** page, you can either pick an existing profile, or create a new one. If you don't have one yet, you will be prompted to create a new one.</span></span> 
    
    <span data-ttu-id="b0d7c-125">Um perfil é uma coleção de definições que podem ser aplicadas a um único dispositivo ou a um grupo de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="b0d7c-125">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="b0d7c-p104">As funcionalidades predefinidas são necessárias e serão configuradas automaticamente. As funcionalidades predefinidas são:</span><span class="sxs-lookup"><span data-stu-id="b0d7c-p104">The default features are required and will be set automatically. The default features are:</span></span>
    
  - <span data-ttu-id="b0d7c-128">O registo da Cortana, do OneDrive e do OEM é ignorado.</span><span class="sxs-lookup"><span data-stu-id="b0d7c-128">Cortana, OneDrive and OEM registration is skipped.</span></span>
    
  - <span data-ttu-id="b0d7c-129">Crie uma experiência de início de sessão com a identidade corporativa da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="b0d7c-129">Create sign-in experience with your company brand.</span></span>
    
  - <span data-ttu-id="b0d7c-130">Os seus dispositivos serão ligados às contas do Azure Active Directory e automaticamente inscritos para serem geridos pelo Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="b0d7c-130">Your devices are going to be connected to Azure Active Directory accounts and automatically enrolled to be managed by Microsoft 365 Business.</span></span>
    
    <span data-ttu-id="b0d7c-131">Para obter mais informações, consulte</span><span class="sxs-lookup"><span data-stu-id="b0d7c-131">For more information, see</span></span>
    
    <span data-ttu-id="b0d7c-132">[Sobre as definições do Perfil AutoPilot](autopilot-profile-settings.md) .</span><span class="sxs-lookup"><span data-stu-id="b0d7c-132">[About AutoPilot Profile settings](autopilot-profile-settings.md) .</span></span> 
    
5. <span data-ttu-id="b0d7c-133">As outras definições são **Ignorar definições de privacidade** e **Não permitir que o utilizador se torne o administrador local**. Ambas estão configuradas como **Desativado** por predefinição.</span><span class="sxs-lookup"><span data-stu-id="b0d7c-133">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="b0d7c-134">Selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="b0d7c-134">Choose **Next**.</span></span>
    
6. <span data-ttu-id="b0d7c-p105">A página **Concluído** indica que o perfil criado (ou selecionado) será aplicado ao grupo de dispositivos criado ao atualizar a lista de dispositivos. Estas definições entrarão em vigor assim que os utilizadores dos dispositivos iniciarem sessão. Selecione **Fechar**.</span><span class="sxs-lookup"><span data-stu-id="b0d7c-p105">**You're done** page indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices. These settings will be in effect when the device users sign in next. Choose **Close**.</span></span>
    