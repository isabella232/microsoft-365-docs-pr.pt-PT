---
title: Preparar a implementação do cliente do Office pelo Microsoft 365 para empresas
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
description: Saiba como instalar automaticamente as aplicações do Office de 32 bits em computadores com Windows 10 e mantê-las atualizadas.
ms.openlocfilehash: 843be426d817da1173769b3b66dc4c054179f0fd
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/14/2021
ms.locfileid: "52924233"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a><span data-ttu-id="066fe-103">Preparar a implementação do cliente do Office pelo Microsoft 365 para empresas</span><span class="sxs-lookup"><span data-stu-id="066fe-103">Prepare for Office client deployment by Microsoft 365 for business</span></span>

<span data-ttu-id="066fe-104">Este artigo aplica-se ao Microsoft 365 Empresas - Formatos Premium.</span><span class="sxs-lookup"><span data-stu-id="066fe-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="066fe-105">Preparar a instalação automática das aplicações do Office em computadores cliente</span><span class="sxs-lookup"><span data-stu-id="066fe-105">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="066fe-106">Pode utilizar o Microsoft 365 Empresas – Versão Premium para instalar automaticamente as aplicações do Office de 32 bits em computadores com Windows 10 e mantê-las atualizadas.</span><span class="sxs-lookup"><span data-stu-id="066fe-106">You can use Microsoft 365 Business Premium to automatically install the 32-bit Office apps on Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="066fe-107">A instalação automática funciona melhor se o computador do utilizador final tiver o Windows 10 Business e:</span><span class="sxs-lookup"><span data-stu-id="066fe-107">Automatic installation works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="066fe-108">Não tiver aplicações de ambiente de trabalho do Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access e OneDrive).</span><span class="sxs-lookup"><span data-stu-id="066fe-108">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="066fe-109">ou</span><span class="sxs-lookup"><span data-stu-id="066fe-109">or</span></span>
    
- <span data-ttu-id="066fe-110">Tiver uma versão do Office Clique-e-Use instalada.</span><span class="sxs-lookup"><span data-stu-id="066fe-110">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="066fe-111">Para determinar se tem a versão Clique-e-Use do Office, em qualquer aplicação do Office, aceda a **Ficheiro** \> **Conta** ( **Conta do Office** no Outlook).</span><span class="sxs-lookup"><span data-stu-id="066fe-111">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook).</span></span> <span data-ttu-id="066fe-112">Se vir as **Atualizações do Office** conforme apresentado na seguinte imagem, a instalação foi e feita com a versão Clique-e-Use.</span><span class="sxs-lookup"><span data-stu-id="066fe-112">If you see **Office Updates** as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="066fe-114">**Quem beneficia desta funcionalidade**</span><span class="sxs-lookup"><span data-stu-id="066fe-114">**Who benefits from having this feature**</span></span>
  
<span data-ttu-id="066fe-115">O utilizador final cujo PC:</span><span class="sxs-lookup"><span data-stu-id="066fe-115">The end user whose PC:</span></span>
  
- <span data-ttu-id="066fe-116">**Tem**  uma licença de utilizador do Windows 10 Business, uma licença ativa do Microsoft 365 para empresas, a Atualização para Criativos do Windows 10 e está associado ao Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="066fe-116">**Has**  a Windows 10 Business user license, an active Microsoft 365 for business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="066fe-117">**Não tem aplicações do** Office de 64 bits (por exemplo: Word, Excel, PowerPoint).</span><span class="sxs-lookup"><span data-stu-id="066fe-117">**Doesn't have** 64-bit Office apps (example: Word, Excel, PowerPoint).</span></span> <span data-ttu-id="066fe-118">Se for necessário ter aplicações do Office de 64 bits, esta funcionalidade não é uma boa forma de o fazer porque não existe suporte para ativar uma versão Clique-e-Run de 64 bits do Office 2016 a partir da consola do administrador do Microsoft 365 para empresas.</span><span class="sxs-lookup"><span data-stu-id="066fe-118">If 64-bit Office apps are required, then this feature isn't a good fit because there's no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 for business admin console.</span></span> 
    
- <span data-ttu-id="066fe-119">**Não tem** quaisquer aplicações autónomas do Windows Installer (MSI) 2016 (por exemplo, o Visio ou Project).</span><span class="sxs-lookup"><span data-stu-id="066fe-119">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project).</span></span> <span data-ttu-id="066fe-120">O Microsoft 365 para empresas atualiza o Office para a versão Clique-e-Run do Office 2016 e a mesma não funciona com as aplicações aplicações aleacionais do Office 2016 MSI.</span><span class="sxs-lookup"><span data-stu-id="066fe-120">Microsoft 365 for business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="066fe-121">A seguinte tabela mostra que ação os utilizadores/administradores finais poderão ter de tomar, dependendo do respetiva estado inicial, para que a implementação do Office na versão Clique-e-Run de 32 bits do Office seja bem-sucedida a partir da consola do administrador do Microsoft 365 para empresas.</span><span class="sxs-lookup"><span data-stu-id="066fe-121">The following table shows what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 for business admin console.</span></span><br/>


|<span data-ttu-id="066fe-122">Estado inicial da instalação do Office</span><span class="sxs-lookup"><span data-stu-id="066fe-122">Starting Office install status</span></span>|<span data-ttu-id="066fe-123">Ação a tomar antes da instalação do Office do Microsoft 365 para empresas</span><span class="sxs-lookup"><span data-stu-id="066fe-123">Action to take before Microsoft 365 for business Office install</span></span>|<span data-ttu-id="066fe-124">Estado final</span><span class="sxs-lookup"><span data-stu-id="066fe-124">End state</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="066fe-125">Nenhum conjunto de aplicações do Office instalado</span><span class="sxs-lookup"><span data-stu-id="066fe-125">No Office suite installed</span></span>  <br/> |<span data-ttu-id="066fe-126">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="066fe-126">None</span></span>  <br/> |<span data-ttu-id="066fe-127">O Office 2016 de 32 bits é instalado com a clique-e-Use</span><span class="sxs-lookup"><span data-stu-id="066fe-127">Office 2016 32-bit is installed by using Click-to-Run</span></span>  <br/> |
|<span data-ttu-id="066fe-128">Versão Clique-e-Use de 32 bits do Office (2016 ou anterior) sem aplicações autónomas</span><span class="sxs-lookup"><span data-stu-id="066fe-128">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="066fe-129">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="066fe-129">None</span></span>  <br/> |<span data-ttu-id="066fe-130">Atualizada para a versão Clique-e-Use de 32 bits mais recente do Office 2016, conforme necessário **\***</span><span class="sxs-lookup"><span data-stu-id="066fe-130">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="066fe-131">Versão Clique-e-Utilize de 32 bits do Office e aplicações a mesmas do Office Clique-e-Utilize 32 bits ou 64 bits (por exemplo, o Visio, Project)</span><span class="sxs-lookup"><span data-stu-id="066fe-131">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32-bit or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="066fe-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="066fe-132">None</span></span>  <br/> |<span data-ttu-id="066fe-133">As aplicações a standalone não são afetadas.</span><span class="sxs-lookup"><span data-stu-id="066fe-133">Standalone apps aren't affected.</span></span> <span data-ttu-id="066fe-134">O conjunto de aplicações é atualizado para a versão Clique-e-Use de 32 bits do Office 2016</span><span class="sxs-lookup"><span data-stu-id="066fe-134">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="066fe-135">Versão Clique-e-Use de 32 bits do Office e quaisquer aplicações autónomas do Office MSI de 32 ou 64 bits (exceto o 2016)</span><span class="sxs-lookup"><span data-stu-id="066fe-135">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="066fe-136">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="066fe-136">None</span></span>  <br/> |<span data-ttu-id="066fe-137">As aplicações a standalone não são afetadas.</span><span class="sxs-lookup"><span data-stu-id="066fe-137">Standalone apps aren't affected.</span></span> <span data-ttu-id="066fe-138">O conjunto de aplicações é atualizado para a versão Clique-e-Use de 32 bits do Office 2016</span><span class="sxs-lookup"><span data-stu-id="066fe-138">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="066fe-139">Qualquer versão Clique-e-Use de 64 bits do Office</span><span class="sxs-lookup"><span data-stu-id="066fe-139">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="066fe-140">Desinstale as aplicações do Office de 64 bits, se não se importar de substituí-las por aplicações do Office de 32 bits</span><span class="sxs-lookup"><span data-stu-id="066fe-140">Uninstall the 64-bit Office apps, if it's OK to replace them with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="066fe-141">Se as aplicações do Office de 64 bits forem removidas, a versão Clique-e-Use de 32 bits do Office 2016 é instalada</span><span class="sxs-lookup"><span data-stu-id="066fe-141">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="066fe-142">Uma instalação MSI do Office 2016 com ou sem aplicações autónomas</span><span class="sxs-lookup"><span data-stu-id="066fe-142">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="066fe-143">Desinstale o Office 2016 MSI.</span><span class="sxs-lookup"><span data-stu-id="066fe-143">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="066fe-p106">A versão Clique-e-Use de 32 bits do Office 2016 é instalada. As aplicações autónomas não são alteradas</span><span class="sxs-lookup"><span data-stu-id="066fe-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="066fe-146">Instalação do Office 2013 MSI (ou anterior) e/ou aplicações autónomas do Office</span><span class="sxs-lookup"><span data-stu-id="066fe-146">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="066fe-147">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="066fe-147">None</span></span>  <br/> |<span data-ttu-id="066fe-148">A versão Clique-e-Use de 32 bits do Office 2016 e a instalação do Office MSI já existente (e aplicações autónomas) existem em simultâneo</span><span class="sxs-lookup"><span data-stu-id="066fe-148">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="066fe-149">**(\*) Nota:** não é atualizada para a versão Clique-e-Use de 32 bits do Office 2016 devido a um erro desconhecido.</span><span class="sxs-lookup"><span data-stu-id="066fe-149">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug.</span></span> <span data-ttu-id="066fe-150">Está em curso uma correção.</span><span class="sxs-lookup"><span data-stu-id="066fe-150">A fix is in progress.</span></span> 
  
