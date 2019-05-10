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
ms.openlocfilehash: 8c4a14b4b9dcbf7a30c1e6e0bdd53418a1ab8a03
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660691"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="6b092-103">Utilizar o guia passo a passo para adicionar perfis e dispositivos Autopilot</span><span class="sxs-lookup"><span data-stu-id="6b092-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="6b092-104">Pode utilizar o piloto automático do Windows para configurar **novos** dispositivos Windows 10 para a sua empresa para que estejam prontos para utilização produtiva, logo que lhes atribua aos seus empregados.</span><span class="sxs-lookup"><span data-stu-id="6b092-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they are ready for productive use as soon as you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="6b092-105">Requisitos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="6b092-105">Device requirements</span></span>

<span data-ttu-id="6b092-106">Os dispositivos têm de cumprir os seguintes requisitos:</span><span class="sxs-lookup"><span data-stu-id="6b092-106">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="6b092-107">Windows 10, versão 1703 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="6b092-107">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="6b092-108">Novos dispositivos que não tenham tido a experiência de configuração inicial do Windows.</span><span class="sxs-lookup"><span data-stu-id="6b092-108">New devices that have not been through Windows out-of-box experience.</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="6b092-109">Utilizar o guia de configuração para criar dispositivos e perfis</span><span class="sxs-lookup"><span data-stu-id="6b092-109">Use the setup guide to create devices and profiles</span></span>

![Faixa que apontam para https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

<span data-ttu-id="6b092-111">Se ainda não tiver criado perfis e grupos de dispositivos, a melhor forma de começar é com o guia passo a passo, mas também pode [adicionar dispositivos](create-and-edit-autopilot-devices.md) e [atribuir perfis](create-and-edit-autopilot-profiles.md) aos mesmos sem utilizar o guia.</span><span class="sxs-lookup"><span data-stu-id="6b092-111">If you have no device groups or profiles created yet, the best way to get started is by using the step-by-step guide, but you can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="6b092-112">Vá para o Centro de administração no <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span><span class="sxs-lookup"><span data-stu-id="6b092-112">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="6b092-113">Nav esquerda do escolher **dispositivos** \> **piloto automático**.</span><span class="sxs-lookup"><span data-stu-id="6b092-113">On the left nav choose **Devices** \> **AutoPilot**.</span></span>

    ![No Centro de administração seleccione os dispositivos e, em seguida, o piloto automático.](media/AutoPilot.png)
  
2. <span data-ttu-id="6b092-115">Na página **piloto automático** , clique ou toque em **Iniciar guia**.</span><span class="sxs-lookup"><span data-stu-id="6b092-115">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="6b092-p101">Na página **Carregar um ficheiro .csv com a lista de dispositivos**, procure uma localização com o ficheiro .CSV preparado e, em seguida, selecione **Abrir** \> **Seguinte**. O ficheiro deverá ter três cabeçalhos:</span><span class="sxs-lookup"><span data-stu-id="6b092-p101">On the **Upload .csv file with list of devices** page, browse to a locations where you have the prepared .CSV file, then **Open** \> **Next**. The file should have three headers:</span></span>
    
  - <span data-ttu-id="6b092-119">Coluna A: Número de Série do Dispositivo</span><span class="sxs-lookup"><span data-stu-id="6b092-119">Column A: Device Serial Number</span></span>
    
  - <span data-ttu-id="6b092-120">Coluna B: ID do Produto Windows</span><span class="sxs-lookup"><span data-stu-id="6b092-120">Column B: Windows Product ID</span></span>
    
  - <span data-ttu-id="6b092-121">Coluna C: Hash do Hardware</span><span class="sxs-lookup"><span data-stu-id="6b092-121">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="6b092-122">Pode obter esta informação através do fabricante de hardware ou pode utilizar o [script do PowerShell Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) que irá gerar um ficheiro CSV.</span><span class="sxs-lookup"><span data-stu-id="6b092-122">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a CSV file.</span></span> 
    
    <span data-ttu-id="6b092-p102">Para obter mais informações, consulte [Ficheiro CSV da lista de dispositivos](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Também pode transferir um ficheiro de exemplo na página **Carregar um ficheiro .csv com a lista de dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="6b092-p102">For more information, see [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
4. <span data-ttu-id="6b092-p103">Na página **Atribuir um perfil**, pode selecionar um perfil existente ou criar um novo. Se ainda não tiver um, ser-lhe-á pedido que crie um novo.</span><span class="sxs-lookup"><span data-stu-id="6b092-p103">On the **Assign a profile** page, you can either pick an existing profile, or create a new one. If you don't have one yet, you will be prompted to create a new one.</span></span> 
    
    <span data-ttu-id="6b092-127">Um perfil é uma coleção de definições que podem ser aplicadas a um único dispositivo ou a um grupo de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="6b092-127">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="6b092-p104">As funcionalidades predefinidas são necessárias e serão configuradas automaticamente. As funcionalidades predefinidas são:</span><span class="sxs-lookup"><span data-stu-id="6b092-p104">The default features are required and will be set automatically. The default features are:</span></span>
    
  - <span data-ttu-id="6b092-130">O registo da Cortana, do OneDrive e do OEM é ignorado.</span><span class="sxs-lookup"><span data-stu-id="6b092-130">Cortana, OneDrive and OEM registration is skipped.</span></span>
    
  - <span data-ttu-id="6b092-131">Crie uma experiência de início de sessão com a identidade corporativa da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="6b092-131">Create sign-in experience with your company brand.</span></span>
    
  - <span data-ttu-id="6b092-132">Os seus dispositivos serão ligados às contas do Azure Active Directory e automaticamente inscritos para serem geridos pelo Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="6b092-132">Your devices are going to be connected to Azure Active Directory accounts and automatically enrolled to be managed by Microsoft 365 Business.</span></span>
    
    <span data-ttu-id="6b092-133">Para obter mais informações, consulte</span><span class="sxs-lookup"><span data-stu-id="6b092-133">For more information, see</span></span>
    
    <span data-ttu-id="6b092-134">[Sobre as definições do Perfil AutoPilot](autopilot-profile-settings.md) .</span><span class="sxs-lookup"><span data-stu-id="6b092-134">[About AutoPilot Profile settings](autopilot-profile-settings.md) .</span></span> 
    
5. <span data-ttu-id="6b092-135">As outras definições são **Ignorar definições de privacidade** e **Não permitir que o utilizador se torne o administrador local**. Ambas estão configuradas como **Desativado** por predefinição.</span><span class="sxs-lookup"><span data-stu-id="6b092-135">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="6b092-136">Selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="6b092-136">Choose **Next**.</span></span>
    
6. <span data-ttu-id="6b092-p105">A página **Concluído** indica que o perfil criado (ou selecionado) será aplicado ao grupo de dispositivos criado ao atualizar a lista de dispositivos. Estas definições entrarão em vigor assim que os utilizadores dos dispositivos iniciarem sessão. Selecione **Fechar**.</span><span class="sxs-lookup"><span data-stu-id="6b092-p105">**You're done** page indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices. These settings will be in effect when the device users sign in next. Choose **Close**.</span></span>
    