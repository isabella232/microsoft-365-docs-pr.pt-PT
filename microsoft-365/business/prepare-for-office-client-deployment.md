---
title: Preparar a implementação do cliente do Office pelo Microsoft 365 Business
f1.keywords:
- CSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 10/31/2017
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Aprenda a instalar automaticamente as aplicações de 32 bits do Office nos computadores do Windows 10 e mantê-las atualizadas.
ms.openlocfilehash: fa5b2ce1852ebdb1e76c1fa844793fee56af3d68
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593625"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a><span data-ttu-id="90b9b-103">Preparar a implementação do cliente do Office pelo Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="90b9b-103">Prepare for Office client deployment by Microsoft 365 Business</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="90b9b-104">Preparar a instalação automática das aplicações do Office em computadores cliente</span><span class="sxs-lookup"><span data-stu-id="90b9b-104">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="90b9b-105">Pode utilizar o Microsoft 365 Business para instalar automaticamente as aplicações de 32 bits do Office nos computadores do Windows 10 e mantê-las atualizadas com atualizações.</span><span class="sxs-lookup"><span data-stu-id="90b9b-105">You can use Microsoft 365 Business to automatically install the 32-bit Office apps on Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="90b9b-106">A instalação automática funciona melhor se o computador do utilizador final estiver no Windows 10 Business e:</span><span class="sxs-lookup"><span data-stu-id="90b9b-106">Automatic installation works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="90b9b-107">Não tiver aplicações de ambiente de trabalho do Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access e OneDrive).</span><span class="sxs-lookup"><span data-stu-id="90b9b-107">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="90b9b-108">ou</span><span class="sxs-lookup"><span data-stu-id="90b9b-108">or</span></span>
    
- <span data-ttu-id="90b9b-109">Tiver uma versão do Office Clique-e-Use instalada.</span><span class="sxs-lookup"><span data-stu-id="90b9b-109">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="90b9b-110">Para determinar se tem a versão Clique-e-Use do Office, em qualquer aplicação do Office, aceda a **Ficheiro** \> **Conta** ( **Conta do Office** no Outlook).</span><span class="sxs-lookup"><span data-stu-id="90b9b-110">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook).</span></span> <span data-ttu-id="90b9b-111">Se vir **as Atualizações do Office** como mostrado na figura seguinte, então a instalação foi feita utilizando o Click-to-Run.</span><span class="sxs-lookup"><span data-stu-id="90b9b-111">If you see **Office Updates** as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="90b9b-113">**Quem beneficia de ter esta funcionalidade**</span><span class="sxs-lookup"><span data-stu-id="90b9b-113">**Who benefits from having this feature**</span></span>
  
<span data-ttu-id="90b9b-114">O utilizador final cujo PC:</span><span class="sxs-lookup"><span data-stu-id="90b9b-114">The end user whose PC:</span></span>
  
- <span data-ttu-id="90b9b-115">**Tem** uma licença de utilizador do Windows 10 Business, uma licença ativa do Microsoft 365 Business, a Atualização para Criativos do Windows 10 e está ligado ao Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="90b9b-115">**Has**  a Windows 10 Business user license, an active Microsoft 365 Business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="90b9b-116">**Não tem** aplicações de 64 bits do Office (exemplo: Word, Excel, PowerPoint).</span><span class="sxs-lookup"><span data-stu-id="90b9b-116">**Doesn't have** 64-bit Office apps (example: Word, Excel, PowerPoint).</span></span> <span data-ttu-id="90b9b-117">Se forem necessárias aplicações de Office de 64 bits, então esta funcionalidade não é um bom ajuste porque não há suporte para desencadear uma versão click-to-Run de 64 bits de 2016 da consola de administração microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="90b9b-117">If 64-bit Office apps are required, then this feature isn't a good fit because there's no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 Business admin console.</span></span> 
    
- <span data-ttu-id="90b9b-118">**Não tem** quaisquer aplicações autónomas do Windows Installer (MSI) 2016 (por exemplo, o Visio ou Project).</span><span class="sxs-lookup"><span data-stu-id="90b9b-118">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project).</span></span> <span data-ttu-id="90b9b-119">O Microsoft 365 Business atualiza o Office para a versão Click-to-Run do Office 2016 e isso não funciona com aplicações autónomas do Office 2016 MSI.</span><span class="sxs-lookup"><span data-stu-id="90b9b-119">Microsoft 365 Business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="90b9b-120">A tabela que se segue mostra que medidas os utilizadores/administradores finais podem ter de tomar, dependendo do seu estado inicial, para ter uma versão bem sucedida de 32 bits click-to-Run da consola de administração do Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="90b9b-120">The following table shows what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 Business admin console.</span></span>
  
|<span data-ttu-id="90b9b-121">**Estado inicial da instalação do Office**</span><span class="sxs-lookup"><span data-stu-id="90b9b-121">**Starting Office install status**</span></span>|<span data-ttu-id="90b9b-122">**Ação a tomar antes da instalação do Office do Microsoft 365 Business**</span><span class="sxs-lookup"><span data-stu-id="90b9b-122">**Action to take before Microsoft 365 Business Office install**</span></span>|<span data-ttu-id="90b9b-123">**Estado final**</span><span class="sxs-lookup"><span data-stu-id="90b9b-123">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="90b9b-124">Nenhum conjunto de aplicações do Office instalado</span><span class="sxs-lookup"><span data-stu-id="90b9b-124">No Office suite installed</span></span>  <br/> |<span data-ttu-id="90b9b-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="90b9b-125">None</span></span>  <br/> |<span data-ttu-id="90b9b-126">Office 2016 32-bit é instalado usando Click-to-Run</span><span class="sxs-lookup"><span data-stu-id="90b9b-126">Office 2016 32-bit is installed by using Click-to-Run</span></span>  <br/> |
|<span data-ttu-id="90b9b-127">Versão Clique-e-Use de 32 bits do Office (2016 ou anterior) sem aplicações autónomas</span><span class="sxs-lookup"><span data-stu-id="90b9b-127">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="90b9b-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="90b9b-128">None</span></span>  <br/> |<span data-ttu-id="90b9b-129">Atualizada para a versão Clique-e-Use de 32 bits mais recente do Office 2016, conforme necessário **\***</span><span class="sxs-lookup"><span data-stu-id="90b9b-129">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="90b9b-130">Já existente, versão de 32 bits do Office e do Click-to-Run 32-bit ou 64 bits de aplicações autónomas do Office (por exemplo, Visio, Project)</span><span class="sxs-lookup"><span data-stu-id="90b9b-130">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32-bit or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="90b9b-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="90b9b-131">None</span></span>  <br/> |<span data-ttu-id="90b9b-132">As aplicações autónomas não são afetadas.</span><span class="sxs-lookup"><span data-stu-id="90b9b-132">Standalone apps aren't affected.</span></span> <span data-ttu-id="90b9b-133">O conjunto de aplicações é atualizado para a versão Clique-e-Use de 32 bits do Office 2016</span><span class="sxs-lookup"><span data-stu-id="90b9b-133">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="90b9b-134">Versão Clique-e-Use de 32 bits do Office e quaisquer aplicações autónomas do Office MSI de 32 ou 64 bits (exceto o 2016)</span><span class="sxs-lookup"><span data-stu-id="90b9b-134">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="90b9b-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="90b9b-135">None</span></span>  <br/> |<span data-ttu-id="90b9b-136">As aplicações autónomas não são afetadas.</span><span class="sxs-lookup"><span data-stu-id="90b9b-136">Standalone apps aren't affected.</span></span> <span data-ttu-id="90b9b-137">O conjunto de aplicações é atualizado para a versão Clique-e-Use de 32 bits do Office 2016</span><span class="sxs-lookup"><span data-stu-id="90b9b-137">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="90b9b-138">Qualquer versão Clique-e-Use de 64 bits do Office</span><span class="sxs-lookup"><span data-stu-id="90b9b-138">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="90b9b-139">Desinstale as aplicações do Office de 64 bits, se não houver problema em substituí-las por aplicações de 32 bits do Office</span><span class="sxs-lookup"><span data-stu-id="90b9b-139">Uninstall the 64-bit Office apps, if it's OK to replace them with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="90b9b-140">Se as aplicações do Office de 64 bits forem removidas, a versão Clique-e-Use de 32 bits do Office 2016 é instalada</span><span class="sxs-lookup"><span data-stu-id="90b9b-140">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="90b9b-141">Uma instalação MSI do Office 2016 com ou sem aplicações autónomas</span><span class="sxs-lookup"><span data-stu-id="90b9b-141">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="90b9b-142">Desinstale o Office 2016 MSI.</span><span class="sxs-lookup"><span data-stu-id="90b9b-142">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="90b9b-p106">A versão Clique-e-Use de 32 bits do Office 2016 é instalada. As aplicações autónomas não são alteradas</span><span class="sxs-lookup"><span data-stu-id="90b9b-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="90b9b-145">Instalação do Office 2013 MSI (ou anterior) e/ou aplicações autónomas do Office</span><span class="sxs-lookup"><span data-stu-id="90b9b-145">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="90b9b-146">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="90b9b-146">None</span></span>  <br/> |<span data-ttu-id="90b9b-147">A versão Clique-e-Use de 32 bits do Office 2016 e a instalação do Office MSI já existente (e aplicações autónomas) existem em simultâneo</span><span class="sxs-lookup"><span data-stu-id="90b9b-147">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="90b9b-148">**(\*) Nota:** não é atualizada para a versão Clique-e-Use de 32 bits do Office 2016 devido a um erro desconhecido.</span><span class="sxs-lookup"><span data-stu-id="90b9b-148">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug.</span></span> <span data-ttu-id="90b9b-149">Está em curso uma correção.</span><span class="sxs-lookup"><span data-stu-id="90b9b-149">A fix is in progress.</span></span> 
  