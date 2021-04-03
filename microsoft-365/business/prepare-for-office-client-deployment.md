---
title: Prepare-se para implementação de clientes do Office pela Microsoft 365 para negócios
f1.keywords:
- CSH
ms.author: efrene
author: efrene
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Saiba como instalar automaticamente as aplicações do Office de 32 bits nos computadores Windows 10 e mantê-las atualizadas.
ms.openlocfilehash: 868d06fadfef0f55b41131b7fdfbb368b9128405
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580060"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a><span data-ttu-id="d15e3-103">Prepare-se para implementação de clientes do Office pela Microsoft 365 para negócios</span><span class="sxs-lookup"><span data-stu-id="d15e3-103">Prepare for Office client deployment by Microsoft 365 for business</span></span>

<span data-ttu-id="d15e3-104">Este artigo aplica-se ao Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="d15e3-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="d15e3-105">Preparar a instalação automática das aplicações do Office em computadores cliente</span><span class="sxs-lookup"><span data-stu-id="d15e3-105">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="d15e3-106">Pode utilizar o Microsoft 365 Business Premium para instalar automaticamente as aplicações do Office de 32 bits nos computadores Windows 10 e mantê-las atualizadas com atualizações.</span><span class="sxs-lookup"><span data-stu-id="d15e3-106">You can use Microsoft 365 Business Premium to automatically install the 32-bit Office apps on Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="d15e3-107">A instalação automática funciona melhor se o computador do utilizador final estiver no Windows 10 Business e:</span><span class="sxs-lookup"><span data-stu-id="d15e3-107">Automatic installation works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="d15e3-108">Não tiver aplicações de ambiente de trabalho do Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access e OneDrive).</span><span class="sxs-lookup"><span data-stu-id="d15e3-108">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="d15e3-109">ou</span><span class="sxs-lookup"><span data-stu-id="d15e3-109">or</span></span>
    
- <span data-ttu-id="d15e3-110">Tiver uma versão do Office Clique-e-Use instalada.</span><span class="sxs-lookup"><span data-stu-id="d15e3-110">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="d15e3-111">Para determinar se tem a versão Clique-e-Use do Office, em qualquer aplicação do Office, aceda a **Ficheiro** \> **Conta** ( **Conta do Office** no Outlook).</span><span class="sxs-lookup"><span data-stu-id="d15e3-111">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook).</span></span> <span data-ttu-id="d15e3-112">Se vir **atualizações do Office** como mostrado na figura seguinte, a instalação foi feita utilizando o Click-to-Run.</span><span class="sxs-lookup"><span data-stu-id="d15e3-112">If you see **Office Updates** as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="d15e3-114">**Quem beneficia de ter esta funcionalidade**</span><span class="sxs-lookup"><span data-stu-id="d15e3-114">**Who benefits from having this feature**</span></span>
  
<span data-ttu-id="d15e3-115">O utilizador final cujo PC:</span><span class="sxs-lookup"><span data-stu-id="d15e3-115">The end user whose PC:</span></span>
  
- <span data-ttu-id="d15e3-116">**Possui**  uma licença de utilizador do Windows 10 Business, um Microsoft 365 ativo para licença de negócio, Windows 10 Creators Update, e junta-se ao Azure Ative Directory.</span><span class="sxs-lookup"><span data-stu-id="d15e3-116">**Has**  a Windows 10 Business user license, an active Microsoft 365 for business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="d15e3-117">**Não tem** aplicações de Escritório de 64 bits (exemplo: Word, Excel, PowerPoint).</span><span class="sxs-lookup"><span data-stu-id="d15e3-117">**Doesn't have** 64-bit Office apps (example: Word, Excel, PowerPoint).</span></span> <span data-ttu-id="d15e3-118">Se forem necessárias aplicações do Office de 64 bits, então esta funcionalidade não é um bom ajuste porque não há suporte para desencadear uma versão click-to-run de 64 bits do Office a partir da Microsoft 365 para a consola de administração de negócios.</span><span class="sxs-lookup"><span data-stu-id="d15e3-118">If 64-bit Office apps are required, then this feature isn't a good fit because there's no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 for business admin console.</span></span> 
    
- <span data-ttu-id="d15e3-119">**Não tem** quaisquer aplicações autónomas do Windows Installer (MSI) 2016 (por exemplo, o Visio ou Project).</span><span class="sxs-lookup"><span data-stu-id="d15e3-119">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project).</span></span> <span data-ttu-id="d15e3-120">Microsoft 365 para atualizações de negócios Office para a versão Click-to-Run do Office 2016 e que não funciona com aplicações autónomas do Office 2016 MSI.</span><span class="sxs-lookup"><span data-stu-id="d15e3-120">Microsoft 365 for business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="d15e3-121">A tabela que se segue mostra que ação os utilizadores/administradores finais podem ter de tomar, dependendo do seu estado inicial, para terem uma versão clic-to-run de 32 bits bem sucedida da implementação do Microsoft 365 para a consola de administração de negócios.</span><span class="sxs-lookup"><span data-stu-id="d15e3-121">The following table shows what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 for business admin console.</span></span>
  
|<span data-ttu-id="d15e3-122">**Estado inicial da instalação do Office**</span><span class="sxs-lookup"><span data-stu-id="d15e3-122">**Starting Office install status**</span></span>|<span data-ttu-id="d15e3-123">**Medidas a tomar antes da instalação do Microsoft 365 para o Business Office**</span><span class="sxs-lookup"><span data-stu-id="d15e3-123">**Action to take before Microsoft 365 for business Office install**</span></span>|<span data-ttu-id="d15e3-124">**Estado final**</span><span class="sxs-lookup"><span data-stu-id="d15e3-124">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d15e3-125">Nenhum conjunto de aplicações do Office instalado</span><span class="sxs-lookup"><span data-stu-id="d15e3-125">No Office suite installed</span></span>  <br/> |<span data-ttu-id="d15e3-126">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d15e3-126">None</span></span>  <br/> |<span data-ttu-id="d15e3-127">Office 2016 32-bit é instalado usando Click-to-Run</span><span class="sxs-lookup"><span data-stu-id="d15e3-127">Office 2016 32-bit is installed by using Click-to-Run</span></span>  <br/> |
|<span data-ttu-id="d15e3-128">Versão Clique-e-Use de 32 bits do Office (2016 ou anterior) sem aplicações autónomas</span><span class="sxs-lookup"><span data-stu-id="d15e3-128">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="d15e3-129">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d15e3-129">None</span></span>  <br/> |<span data-ttu-id="d15e3-130">Atualizada para a versão Clique-e-Use de 32 bits mais recente do Office 2016, conforme necessário **\***</span><span class="sxs-lookup"><span data-stu-id="d15e3-130">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="d15e3-131">Versão de 32 bits do Office e click-to-run de 32 bits ou 64 bits de escritório autónomo (por exemplo, Visio, Projeto)</span><span class="sxs-lookup"><span data-stu-id="d15e3-131">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32-bit or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="d15e3-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d15e3-132">None</span></span>  <br/> |<span data-ttu-id="d15e3-133">Aplicativos autónomos não são afetados.</span><span class="sxs-lookup"><span data-stu-id="d15e3-133">Standalone apps aren't affected.</span></span> <span data-ttu-id="d15e3-134">O conjunto de aplicações é atualizado para a versão Clique-e-Use de 32 bits do Office 2016</span><span class="sxs-lookup"><span data-stu-id="d15e3-134">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="d15e3-135">Versão Clique-e-Use de 32 bits do Office e quaisquer aplicações autónomas do Office MSI de 32 ou 64 bits (exceto o 2016)</span><span class="sxs-lookup"><span data-stu-id="d15e3-135">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="d15e3-136">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d15e3-136">None</span></span>  <br/> |<span data-ttu-id="d15e3-137">Aplicativos autónomos não são afetados.</span><span class="sxs-lookup"><span data-stu-id="d15e3-137">Standalone apps aren't affected.</span></span> <span data-ttu-id="d15e3-138">O conjunto de aplicações é atualizado para a versão Clique-e-Use de 32 bits do Office 2016</span><span class="sxs-lookup"><span data-stu-id="d15e3-138">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="d15e3-139">Qualquer versão Clique-e-Use de 64 bits do Office</span><span class="sxs-lookup"><span data-stu-id="d15e3-139">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="d15e3-140">Desinstale as aplicações do Office de 64 bits, se não houver problema em substituí-las por aplicações de 32 bits do Office</span><span class="sxs-lookup"><span data-stu-id="d15e3-140">Uninstall the 64-bit Office apps, if it's OK to replace them with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="d15e3-141">Se as aplicações do Office de 64 bits forem removidas, a versão Clique-e-Use de 32 bits do Office 2016 é instalada</span><span class="sxs-lookup"><span data-stu-id="d15e3-141">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="d15e3-142">Uma instalação MSI do Office 2016 com ou sem aplicações autónomas</span><span class="sxs-lookup"><span data-stu-id="d15e3-142">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="d15e3-143">Desinstale o Office 2016 MSI.</span><span class="sxs-lookup"><span data-stu-id="d15e3-143">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="d15e3-p106">A versão Clique-e-Use de 32 bits do Office 2016 é instalada. As aplicações autónomas não são alteradas</span><span class="sxs-lookup"><span data-stu-id="d15e3-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="d15e3-146">Instalação do Office 2013 MSI (ou anterior) e/ou aplicações autónomas do Office</span><span class="sxs-lookup"><span data-stu-id="d15e3-146">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="d15e3-147">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d15e3-147">None</span></span>  <br/> |<span data-ttu-id="d15e3-148">A versão Clique-e-Use de 32 bits do Office 2016 e a instalação do Office MSI já existente (e aplicações autónomas) existem em simultâneo</span><span class="sxs-lookup"><span data-stu-id="d15e3-148">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="d15e3-149">**(\*) Nota:** não é atualizada para a versão Clique-e-Use de 32 bits do Office 2016 devido a um erro desconhecido.</span><span class="sxs-lookup"><span data-stu-id="d15e3-149">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug.</span></span> <span data-ttu-id="d15e3-150">Está em curso uma correção.</span><span class="sxs-lookup"><span data-stu-id="d15e3-150">A fix is in progress.</span></span> 
  
