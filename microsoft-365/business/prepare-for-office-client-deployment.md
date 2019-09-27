---
title: Preparar a implementação do cliente do Office pelo Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 10/31/2017
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Saiba como instalar automaticamente os aplicativos do Office de 32 bits em computadores com Windows 10 e mantê-los atualizados.
ms.openlocfilehash: fe1f946e4a216050e533604afa7c6e74e7b5980f
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288401"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a><span data-ttu-id="3b047-103">Preparar a implementação do cliente do Office pelo Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="3b047-103">Prepare for Office client deployment by Microsoft 365 Business</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="3b047-104">Preparar a instalação automática das aplicações do Office em computadores cliente</span><span class="sxs-lookup"><span data-stu-id="3b047-104">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="3b047-105">Pode utilizar o Microsoft 365 Business para instalar automaticamente as aplicações do Office de 32 bits em computadores com Windows 10 e mantê-las atualizadas.</span><span class="sxs-lookup"><span data-stu-id="3b047-105">You can use Microsoft 365 Business to automatically install the 32-bit Office apps to Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="3b047-106">Isto funciona melhor se o computador do utilizador final tiver o Windows 10 Business e:</span><span class="sxs-lookup"><span data-stu-id="3b047-106">This works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="3b047-107">Não tiver aplicações de ambiente de trabalho do Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access e OneDrive).</span><span class="sxs-lookup"><span data-stu-id="3b047-107">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="3b047-108">ou</span><span class="sxs-lookup"><span data-stu-id="3b047-108">or</span></span>
    
- <span data-ttu-id="3b047-109">Tiver uma versão do Office Clique-e-Use instalada.</span><span class="sxs-lookup"><span data-stu-id="3b047-109">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="3b047-p101">Para determinar se tem a versão Clique-e-Use do Office, em qualquer aplicação do Office, aceda a **Ficheiro** \> **Conta** ( **Conta do Office** no Outlook). Se vir as Atualizações do Office conforme apresentado na seguinte imagem, a instalação foi efetuada com a tecnologia Clique-e-Use.</span><span class="sxs-lookup"><span data-stu-id="3b047-p101">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook). If you see Office Updates as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="3b047-113">**Quem irá beneficiar desta funcionalidade**</span><span class="sxs-lookup"><span data-stu-id="3b047-113">**Who will benefit from having this feature**</span></span>
  
<span data-ttu-id="3b047-114">O utilizador final cujo PC:</span><span class="sxs-lookup"><span data-stu-id="3b047-114">The end user whose PC:</span></span>
  
- <span data-ttu-id="3b047-115">**Tem** uma licença de utilizador do Windows 10 Business, uma licença ativa do Microsoft 365 Business, a Atualização para Criativos do Windows 10 e está ligado ao Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3b047-115">**Has**  a Windows 10 Business user license, an active Microsoft 365 Business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="3b047-p102">**Não tem** aplicações do Office de 64 bits (por exemplo: Word, Excel, Powerpoint). Se for necessário ter aplicações do Office de 64 bits, esta funcionalidade não é uma boa opção pois não existe suporte para acionar uma versão Clique-e-Use de 64 bits do Office 2016 a partir da consola do administrador do Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="3b047-p102">**Doesn't have** 64-bit Office apps (example: Word, Excel, Powerpoint). If 64-bit Office apps are required, then this feature is not a good fit because there is no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 Business admin console.</span></span> 
    
- <span data-ttu-id="3b047-p103">**Não tem** quaisquer aplicações autónomas do Windows Installer (MSI) 2016 (por exemplo, o Visio ou Project). O Microsoft 365 Business atualiza o Office para a versão Clique-e-Use do Office 2016 e a mesma não funciona com as aplicações autónomas do Office 2016 MSI.</span><span class="sxs-lookup"><span data-stu-id="3b047-p103">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project). Microsoft 365 Business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="3b047-120">A seguinte tabela indica detalhadamente que ação os utilizadores/administradores poderão ter de efetuar, dependendo do respetivo estado inicial, para realizar uma implementação com êxito da versão Clique-e-Use de 32 bits do Office a partir da consola do administrador do Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="3b047-120">The following table details what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 Business admin console.</span></span>
  
|<span data-ttu-id="3b047-121">**Estado inicial da instalação do Office**</span><span class="sxs-lookup"><span data-stu-id="3b047-121">**Starting Office install status**</span></span>|<span data-ttu-id="3b047-122">**Ação a tomar antes da instalação do Office do Microsoft 365 Business**</span><span class="sxs-lookup"><span data-stu-id="3b047-122">**Action to take before Microsoft 365 Business Office install**</span></span>|<span data-ttu-id="3b047-123">**Estado final**</span><span class="sxs-lookup"><span data-stu-id="3b047-123">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3b047-124">Nenhum conjunto de aplicações do Office instalado</span><span class="sxs-lookup"><span data-stu-id="3b047-124">No Office suite installed</span></span>  <br/> |<span data-ttu-id="3b047-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="3b047-125">None</span></span>  <br/> |<span data-ttu-id="3b047-126">Office 2016 de 32 bits instalado com a tecnologia Clique-e-Use</span><span class="sxs-lookup"><span data-stu-id="3b047-126">Office 2016 32-bit is installed by using click-to-run</span></span>  <br/> |
|<span data-ttu-id="3b047-127">Versão Clique-e-Use de 32 bits do Office (2016 ou anterior) sem aplicações autónomas</span><span class="sxs-lookup"><span data-stu-id="3b047-127">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="3b047-128">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="3b047-128">None</span></span>  <br/> |<span data-ttu-id="3b047-129">Atualizada para a versão Clique-e-Use de 32 bits mais recente do Office 2016, conforme necessário **\***</span><span class="sxs-lookup"><span data-stu-id="3b047-129">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="3b047-130">Versão Clique-e-Use de 32 bits do Office e aplicações autónomas do Office Clique-e-Use de 32 ou 64 bits (por exemplo, o Visio ou Project)</span><span class="sxs-lookup"><span data-stu-id="3b047-130">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32- or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="3b047-131">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="3b047-131">None</span></span>  <br/> |<span data-ttu-id="3b047-p104">As aplicações autónomas não são afetadas. O conjunto de aplicações é atualizado para a versão Clique-e-Use de 32 bits do Office 2016</span><span class="sxs-lookup"><span data-stu-id="3b047-p104">Standalone apps are not affected. Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="3b047-134">Versão Clique-e-Use de 32 bits do Office e quaisquer aplicações autónomas do Office MSI de 32 ou 64 bits (exceto o 2016)</span><span class="sxs-lookup"><span data-stu-id="3b047-134">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="3b047-135">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="3b047-135">None</span></span>  <br/> |<span data-ttu-id="3b047-p105">As aplicações autónomas não são afetadas. O conjunto de aplicações é atualizado para a versão Clique-e-Use de 32 bits do Office 2016</span><span class="sxs-lookup"><span data-stu-id="3b047-p105">Standalone apps are not affected. Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="3b047-138">Qualquer versão Clique-e-Use de 64 bits do Office</span><span class="sxs-lookup"><span data-stu-id="3b047-138">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="3b047-139">Desinstale as aplicações do Office de 64 bits se não houver problema em substitui-las pelas aplicações do Office de 32 bits</span><span class="sxs-lookup"><span data-stu-id="3b047-139">Uninstall the 64-bit Office apps, if it is OK to replace it with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="3b047-140">Se as aplicações do Office de 64 bits forem removidas, a versão Clique-e-Use de 32 bits do Office 2016 é instalada</span><span class="sxs-lookup"><span data-stu-id="3b047-140">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="3b047-141">Uma instalação MSI do Office 2016 com ou sem aplicações autónomas</span><span class="sxs-lookup"><span data-stu-id="3b047-141">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="3b047-142">Desinstale o Office 2016 MSI.</span><span class="sxs-lookup"><span data-stu-id="3b047-142">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="3b047-p106">A versão Clique-e-Use de 32 bits do Office 2016 é instalada. As aplicações autónomas não são alteradas</span><span class="sxs-lookup"><span data-stu-id="3b047-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="3b047-145">Instalação do Office 2013 MSI (ou anterior) e/ou aplicações autónomas do Office</span><span class="sxs-lookup"><span data-stu-id="3b047-145">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="3b047-146">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="3b047-146">None</span></span>  <br/> |<span data-ttu-id="3b047-147">A versão Clique-e-Use de 32 bits do Office 2016 e a instalação do Office MSI já existente (e aplicações autónomas) existem em simultâneo</span><span class="sxs-lookup"><span data-stu-id="3b047-147">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="3b047-p107">**(\*) Nota:** não é atualizada para a versão Clique-e-Use de 32 bits do Office 2016 devido a um erro desconhecido. A correção está em curso.</span><span class="sxs-lookup"><span data-stu-id="3b047-p107">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug. Fix is in progress.</span></span> 
  


