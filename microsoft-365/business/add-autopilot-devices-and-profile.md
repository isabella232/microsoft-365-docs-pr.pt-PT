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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Saiba como utilizar o Windows AutoPilot para configurar novos dispositivos Windows 10 para o seu negócio, para que estejam prontos para uso dos colaboradores.
ms.openlocfilehash: de14012ebf9e7cdd22e41505f316ab665773c670
ms.sourcegitcommit: 46644f9778bc70ab6d62783e0a1e60ba2eccc27f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/08/2020
ms.locfileid: "44165887"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="17b7b-103">Utilizar o guia passo a passo para adicionar perfis e dispositivos Autopilot</span><span class="sxs-lookup"><span data-stu-id="17b7b-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="17b7b-104">Pode utilizar o Windows AutoPilot para configurar **novos** dispositivos Windows 10 para o seu negócio, para que estejam prontos a ser utilizados quando os entregar aos seus colaboradores.</span><span class="sxs-lookup"><span data-stu-id="17b7b-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they're ready for use when you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="17b7b-105">Requisitos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="17b7b-105">Device requirements</span></span>

<span data-ttu-id="17b7b-106">Os dispositivos devem satisfazer estes requisitos:</span><span class="sxs-lookup"><span data-stu-id="17b7b-106">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="17b7b-107">Windows 10, versão 1703 ou mais tarde</span><span class="sxs-lookup"><span data-stu-id="17b7b-107">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="17b7b-108">Novos dispositivos que não passaram pela experiência do Windows fora da caixa</span><span class="sxs-lookup"><span data-stu-id="17b7b-108">New devices that haven't been through Windows out-of-box experience</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="17b7b-109">Utilizar o guia de configuração para criar dispositivos e perfis</span><span class="sxs-lookup"><span data-stu-id="17b7b-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="17b7b-110">[![Etiqueta que informa que o centro de administração está a mudar e que pode encontrar mais detalhes em aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="17b7b-110">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="17b7b-111">Se ainda não criou grupos de dispositivos ou perfis, a melhor maneira de começar é utilizando o guia passo a passo.</span><span class="sxs-lookup"><span data-stu-id="17b7b-111">If you haven't created device groups or profiles yet, the best way to get started is by using the step-by-step guide.</span></span> <span data-ttu-id="17b7b-112">Também pode [adicionar dispositivos](create-and-edit-autopilot-devices.md) e [atribuir-lhes perfis](create-and-edit-autopilot-profiles.md) sem utilizar o guia.</span><span class="sxs-lookup"><span data-stu-id="17b7b-112">You can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="17b7b-113">Vá ao centro de <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>administração em .</span><span class="sxs-lookup"><span data-stu-id="17b7b-113">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="17b7b-114">No painel de navegação à esquerda, escolha **Dispositivos** \> **AutoPilot**.</span><span class="sxs-lookup"><span data-stu-id="17b7b-114">On the left navigation pane, choose **Devices** \> **AutoPilot**.</span></span>

    ![No centro de administração, escolha os dispositivos e, em seguida, o AutoPilot.](../media/AutoPilot.png)
  
2. <span data-ttu-id="17b7b-116">Na página **AutoPilot,** clique ou toque no **guia Iniciar**.</span><span class="sxs-lookup"><span data-stu-id="17b7b-116">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="17b7b-118">No **ficheiro Upload .csv com página de dispositivos,** navegue para um local onde tenha o preparado . Ficheiro CSV, em **seguida, Abrir** \> **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="17b7b-118">On the **Upload .csv file with list of devices** page, browse to a location where you have the prepared .CSV file, then **Open** \> **Next**.</span></span> <span data-ttu-id="17b7b-119">O ficheiro deve ter três cabeçalhos:</span><span class="sxs-lookup"><span data-stu-id="17b7b-119">The file must have three headers:</span></span>
    
    - <span data-ttu-id="17b7b-120">Coluna A: Número de Série do Dispositivo</span><span class="sxs-lookup"><span data-stu-id="17b7b-120">Column A: Device Serial Number</span></span>
    
    - <span data-ttu-id="17b7b-121">Coluna B: ID do Produto Windows</span><span class="sxs-lookup"><span data-stu-id="17b7b-121">Column B: Windows Product ID</span></span>
    
    - <span data-ttu-id="17b7b-122">Coluna C: Hash do Hardware</span><span class="sxs-lookup"><span data-stu-id="17b7b-122">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="17b7b-123">Pode obter esta informação do seu fornecedor de hardware, ou pode utilizar o [script Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) para gerar um ficheiro CSV.</span><span class="sxs-lookup"><span data-stu-id="17b7b-123">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
    <span data-ttu-id="17b7b-p103">Para obter mais informações, consulte [Ficheiro CSV da lista de dispositivos](https://docs.microsoft.com/microsoft-365/admin/misc/device-list). Também pode transferir um ficheiro de exemplo na página **Carregar um ficheiro .csv com a lista de dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="17b7b-p103">For more information, see [Device list CSV-file](https://docs.microsoft.com/microsoft-365/admin/misc/device-list). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
4. <span data-ttu-id="17b7b-126">Na página de atribuir uma página de **perfil,** pode escolher um perfil existente ou criar um novo.</span><span class="sxs-lookup"><span data-stu-id="17b7b-126">On the **Assign a profile** page, you can either pick an existing profile or create a new one.</span></span> <span data-ttu-id="17b7b-127">Se ainda não tiver um, será solicitado a criar um.</span><span class="sxs-lookup"><span data-stu-id="17b7b-127">If you don't have one yet, you'll be prompted to create one.</span></span> 
    
    <span data-ttu-id="17b7b-128">Um perfil é uma coleção de definições que podem ser aplicadas a um único dispositivo ou a um grupo de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="17b7b-128">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="17b7b-129">As funcionalidades predefinidas são necessárias e são definidas automaticamente.</span><span class="sxs-lookup"><span data-stu-id="17b7b-129">The default features are required and are set automatically.</span></span> <span data-ttu-id="17b7b-130">As funcionalidades predefinidas são:</span><span class="sxs-lookup"><span data-stu-id="17b7b-130">The default features are:</span></span>
    
    - <span data-ttu-id="17b7b-131">Skip Cortana, OneDrive e registo OEM.</span><span class="sxs-lookup"><span data-stu-id="17b7b-131">Skip Cortana, OneDrive, and OEM registration.</span></span>
    
    - <span data-ttu-id="17b7b-132">Crie uma experiência de início de sessão com a identidade corporativa da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="17b7b-132">Create sign-in experience with your company brand.</span></span>
    
    - <span data-ttu-id="17b7b-133">Ligue os seus dispositivos às contas do Diretório Ativo Do Azure e inscreva-os automaticamente para serem geridos pelo Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="17b7b-133">Connect your devices to Azure Active Directory accounts, and automatically enroll them to be managed by Microsoft 365 Business Premium.</span></span>
    
    <span data-ttu-id="17b7b-134">Para mais informações, consulte as definições de [Perfil AutoPilot](autopilot-profile-settings.md).</span><span class="sxs-lookup"><span data-stu-id="17b7b-134">For more information, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span> 
    
5. <span data-ttu-id="17b7b-135">As outras definições são **Ignorar definições de privacidade** e **Não permitir que o utilizador se torne o administrador local**. Ambas estão configuradas como **Desativado** por predefinição.</span><span class="sxs-lookup"><span data-stu-id="17b7b-135">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="17b7b-136">Selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="17b7b-136">Choose **Next**.</span></span>
    
6. <span data-ttu-id="17b7b-137">**Está feito** indica que o perfil que criou (ou escolheu) será aplicado ao grupo de dispositivos que criou através do upload da lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="17b7b-137">**You're done** indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices.</span></span> <span data-ttu-id="17b7b-138">As definições estarão em vigor quando os utilizadores do dispositivo iniciarem o seu inicio.</span><span class="sxs-lookup"><span data-stu-id="17b7b-138">The settings will be in effect when the device users sign in next.</span></span> <span data-ttu-id="17b7b-139">Selecione **Fechar**.</span><span class="sxs-lookup"><span data-stu-id="17b7b-139">Choose **Close**.</span></span>
    
