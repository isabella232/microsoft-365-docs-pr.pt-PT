---
title: Utilizar o guia passo a passo para adicionar perfis e dispositivos Autopilot
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Saiba como utilizar o Windows AutoPilot para configurar novos dispositivos Windows 10 para o seu negócio para que estejam prontos para uso dos colaboradores.
ms.openlocfilehash: 75cc51b889f8673de8dba2357c777de47fd0d296
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913508"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="b2663-103">Utilizar o guia passo a passo para adicionar perfis e dispositivos Autopilot</span><span class="sxs-lookup"><span data-stu-id="b2663-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="b2663-104">Pode utilizar o Windows AutoPilot para configurar **novos** dispositivos Windows 10 para o seu negócio, para que estes estejam prontos a ser utilizados quando os entregar aos seus colaboradores.</span><span class="sxs-lookup"><span data-stu-id="b2663-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they're ready for use when you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="b2663-105">Requisitos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="b2663-105">Device requirements</span></span>

<span data-ttu-id="b2663-106">Os dispositivos devem satisfazer estes requisitos:</span><span class="sxs-lookup"><span data-stu-id="b2663-106">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="b2663-107">Windows 10, versão 1703 ou mais tarde</span><span class="sxs-lookup"><span data-stu-id="b2663-107">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="b2663-108">Novos dispositivos que não passaram pela experiência fora de caixa do Windows</span><span class="sxs-lookup"><span data-stu-id="b2663-108">New devices that haven't been through Windows out-of-box experience</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="b2663-109">Utilizar o guia de configuração para criar dispositivos e perfis</span><span class="sxs-lookup"><span data-stu-id="b2663-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="b2663-110">[![Etiqueta que informa que o centro de administração está a mudar e que pode encontrar mais detalhes em aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="b2663-110">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="b2663-111">Se ainda não criou grupos ou perfis de dispositivos, a melhor maneira de começar é usando o guia passo a passo.</span><span class="sxs-lookup"><span data-stu-id="b2663-111">If you haven't created device groups or profiles yet, the best way to get started is by using the step-by-step guide.</span></span> <span data-ttu-id="b2663-112">Também pode [adicionar dispositivos](create-and-edit-autopilot-devices.md) e [atribuir-lhes perfis](create-and-edit-autopilot-profiles.md) sem utilizar o guia.</span><span class="sxs-lookup"><span data-stu-id="b2663-112">You can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="b2663-113">Vá ao centro de administração em <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="b2663-113">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="b2663-114">No painel de navegação à esquerda, escolha **Dispositivos** \> **AutoPilot**.</span><span class="sxs-lookup"><span data-stu-id="b2663-114">On the left navigation pane, choose **Devices** \> **AutoPilot**.</span></span>

    ![No centro de administração, escolha dispositivos e, em seguida, AutoPilot.](../media/AutoPilot.png)
  
2. <span data-ttu-id="b2663-116">Na página **AutoPilot,** clique ou toque **no guia Iniciar .**</span><span class="sxs-lookup"><span data-stu-id="b2663-116">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="b2663-118">No **ficheiro upload .csv com a página da lista de dispositivos,** navegue para um local onde tenha o preparado . Ficheiro CSV e, em seguida, **Abrir** \> **Em Seguida**.</span><span class="sxs-lookup"><span data-stu-id="b2663-118">On the **Upload .csv file with list of devices** page, browse to a location where you have the prepared .CSV file, then **Open** \> **Next**.</span></span> <span data-ttu-id="b2663-119">O ficheiro deve ter três cabeçalhos:</span><span class="sxs-lookup"><span data-stu-id="b2663-119">The file must have three headers:</span></span>
    
    - <span data-ttu-id="b2663-120">Coluna A: Número de Série do Dispositivo</span><span class="sxs-lookup"><span data-stu-id="b2663-120">Column A: Device Serial Number</span></span>
    
    - <span data-ttu-id="b2663-121">Coluna B: ID do Produto Windows</span><span class="sxs-lookup"><span data-stu-id="b2663-121">Column B: Windows Product ID</span></span>
    
    - <span data-ttu-id="b2663-122">Coluna C: Hash do Hardware</span><span class="sxs-lookup"><span data-stu-id="b2663-122">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="b2663-123">Pode obter estas informações do seu fornecedor de hardware ou pode utilizar o [script Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) para gerar um ficheiro CSV.</span><span class="sxs-lookup"><span data-stu-id="b2663-123">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
    <span data-ttu-id="b2663-p103">Para obter mais informações, consulte [Ficheiro CSV da lista de dispositivos](../admin/misc/device-list.md). Também pode transferir um ficheiro de exemplo na página **Carregar um ficheiro .csv com a lista de dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="b2663-p103">For more information, see [Device list CSV-file](../admin/misc/device-list.md). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="b2663-126">Este script utiliza o WMI para recuperar propriedades necessárias para que um cliente registe um dispositivo com o Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="b2663-126">This script uses WMI to retrieve properties needed for a customer to register a device with Windows Autopilot.</span></span> <span data-ttu-id="b2663-127">Note que é normal que o ficheiro CSV resultante não recolha um valor de ID do Produto Do Windows (PKID), uma vez que este não é obrigado a registar um dispositivo e o PKID a ser NULO no CSV de saída é totalmente bom.</span><span class="sxs-lookup"><span data-stu-id="b2663-127">Note that it is normal for the resulting CSV file to not collect a Windows Product ID (PKID) value since this is not required to register a device and PKID being NULL in the output CSV is totally fine.</span></span> <span data-ttu-id="b2663-128">Apenas o número de série e o haxixe de hardware serão povoados.</span><span class="sxs-lookup"><span data-stu-id="b2663-128">Only the serial number and hardware hash will be populated.</span></span>
    
4. <span data-ttu-id="b2663-129">Na página **de perfil atribuir um perfil,** pode escolher um perfil existente ou criar um novo.</span><span class="sxs-lookup"><span data-stu-id="b2663-129">On the **Assign a profile** page, you can either pick an existing profile or create a new one.</span></span> <span data-ttu-id="b2663-130">Se ainda não tiver um, será solicitado a criar um.</span><span class="sxs-lookup"><span data-stu-id="b2663-130">If you don't have one yet, you'll be prompted to create one.</span></span> 
    
    <span data-ttu-id="b2663-131">Um perfil é uma coleção de definições que podem ser aplicadas a um único dispositivo ou a um grupo de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="b2663-131">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="b2663-132">As funcionalidades predefinidas são necessárias e são definidas automaticamente.</span><span class="sxs-lookup"><span data-stu-id="b2663-132">The default features are required and are set automatically.</span></span> <span data-ttu-id="b2663-133">As funcionalidades predefinidas são:</span><span class="sxs-lookup"><span data-stu-id="b2663-133">The default features are:</span></span>
    
    - <span data-ttu-id="b2663-134">Registos Skip Cortana, OneDrive e OEM.</span><span class="sxs-lookup"><span data-stu-id="b2663-134">Skip Cortana, OneDrive, and OEM registration.</span></span>
    
    - <span data-ttu-id="b2663-135">Crie uma experiência de início de sessão com a identidade corporativa da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="b2663-135">Create sign-in experience with your company brand.</span></span>
    
    - <span data-ttu-id="b2663-136">Ligue os seus dispositivos às contas do Azure Ative Directory e inscreva-os automaticamente para serem geridos pelo Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="b2663-136">Connect your devices to Azure Active Directory accounts, and automatically enroll them to be managed by Microsoft 365 Business Premium.</span></span>
    
    <span data-ttu-id="b2663-137">Para obter mais informações, consulte [as definições de Perfil de AutoPilot](autopilot-profile-settings.md).</span><span class="sxs-lookup"><span data-stu-id="b2663-137">For more information, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span> 
    
5. <span data-ttu-id="b2663-138">As outras definições são **Ignorar definições de privacidade** e **Não permitir que o utilizador se torne o administrador local**. Ambas estão configuradas como **Desativado** por predefinição.</span><span class="sxs-lookup"><span data-stu-id="b2663-138">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="b2663-139">Selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="b2663-139">Choose **Next**.</span></span>
    
6. <span data-ttu-id="b2663-140">**Está feito** indica que o perfil que criou (ou escolheu) será aplicado ao grupo de dispositivos que criou através do upload da lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="b2663-140">**You're done** indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices.</span></span> <span data-ttu-id="b2663-141">As definições estarão em vigor quando os utilizadores do dispositivo iniciarem a próxima sposição.</span><span class="sxs-lookup"><span data-stu-id="b2663-141">The settings will be in effect when the device users sign in next.</span></span> <span data-ttu-id="b2663-142">Selecione **Fechar**.</span><span class="sxs-lookup"><span data-stu-id="b2663-142">Choose **Close**.</span></span>
