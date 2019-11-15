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
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Saiba como instalar automaticamente os aplicativos do Office de 32 bits nos computadores do Windows 10 e mantê-los atualizados.
ms.openlocfilehash: 09857ddeb28e953da07979045a65f6b91925aeaf
ms.sourcegitcommit: 2c2248b03f7753d64490f2f7e56ec644a235b65a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/15/2019
ms.locfileid: "38640775"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a><span data-ttu-id="aeae7-103">Preparar a implementação do cliente do Office pelo Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="aeae7-103">Prepare for Office client deployment by Microsoft 365 Business</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="aeae7-104">Preparar a instalação automática das aplicações do Office em computadores cliente</span><span class="sxs-lookup"><span data-stu-id="aeae7-104">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="aeae7-105">Você pode usar o Microsoft 365 Business para instalar automaticamente os aplicativos do Office de 32 bits em computadores Windows 10 e mantê-los atualizados com atualizações.</span><span class="sxs-lookup"><span data-stu-id="aeae7-105">You can use Microsoft 365 Business to automatically install the 32-bit Office apps on Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="aeae7-106">A instalação automática funciona melhor se o computador do usuário final estiver no Windows 10 Business e:</span><span class="sxs-lookup"><span data-stu-id="aeae7-106">Automatic installation works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="aeae7-107">Não tiver aplicações de ambiente de trabalho do Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access e OneDrive).</span><span class="sxs-lookup"><span data-stu-id="aeae7-107">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="aeae7-108">ou</span><span class="sxs-lookup"><span data-stu-id="aeae7-108">or</span></span>
    
- <span data-ttu-id="aeae7-109">Tiver uma versão do Office Clique-e-Use instalada.</span><span class="sxs-lookup"><span data-stu-id="aeae7-109">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="aeae7-110">Para determinar se tem a versão Clique-e-Use do Office, em qualquer aplicação do Office, aceda a **Ficheiro** \> **Conta** ( **Conta do Office** no Outlook).</span><span class="sxs-lookup"><span data-stu-id="aeae7-110">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook).</span></span> <span data-ttu-id="aeae7-111">Se você vir **atualizações do escritório** como mostrado na figura seguinte, então a instalação foi feita usando Clique para Executar.</span><span class="sxs-lookup"><span data-stu-id="aeae7-111">If you see **Office Updates** as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="aeae7-113">**Quem se beneficia de ter esse recurso**</span><span class="sxs-lookup"><span data-stu-id="aeae7-113">**Who benefits from having this feature**</span></span>
  
<span data-ttu-id="aeae7-114">O utilizador final cujo PC:</span><span class="sxs-lookup"><span data-stu-id="aeae7-114">The end user whose PC:</span></span>
  
- <span data-ttu-id="aeae7-115">**Tem** uma licença de utilizador do Windows 10 Business, uma licença ativa do Microsoft 365 Business, a Atualização para Criativos do Windows 10 e está ligado ao Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="aeae7-115">**Has**  a Windows 10 Business user license, an active Microsoft 365 Business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="aeae7-116">**Não tem** aplicativos do Office de 64 bits (exemplo: Word, Excel, PowerPoint).</span><span class="sxs-lookup"><span data-stu-id="aeae7-116">**Doesn't have** 64-bit Office apps (example: Word, Excel, PowerPoint).</span></span> <span data-ttu-id="aeae7-117">Se são necessários aplicativos do Office de 64 bits, esse recurso não é um bom ajuste porque não há suporte para acionar uma versão clique para execução de 64 bits 2016 do Office do console de administração Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="aeae7-117">If 64-bit Office apps are required, then this feature isn't a good fit because there's no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 Business admin console.</span></span> 
    
- <span data-ttu-id="aeae7-118">**Não tem** quaisquer aplicações autónomas do Windows Installer (MSI) 2016 (por exemplo, o Visio ou Project).</span><span class="sxs-lookup"><span data-stu-id="aeae7-118">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project).</span></span> <span data-ttu-id="aeae7-119">O Microsoft 365 Business atualiza o Office para a versão Click-to-Run do Office 2016 e isso não funciona com aplicativos autônomos do Office 2016 MSI.</span><span class="sxs-lookup"><span data-stu-id="aeae7-119">Microsoft 365 Business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="aeae7-120">A tabela a seguir mostra que ação os usuários/administradores finais podem precisar tomar, dependendo de seu estado de início, para ter uma versão clique-a-run bem-sucedida de 32 bits da implantação do Office do console de administração Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="aeae7-120">The following table shows what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 Business admin console.</span></span>
  
|<span data-ttu-id="aeae7-121">**Estado inicial da instalação do Office**</span><span class="sxs-lookup"><span data-stu-id="aeae7-121">**Starting Office install status**</span></span>|<span data-ttu-id="aeae7-122">**Ação a tomar antes da instalação do Office do Microsoft 365 Business**</span><span class="sxs-lookup"><span data-stu-id="aeae7-122">**Action to take before Microsoft 365 Business Office install**</span></span>|<span data-ttu-id="aeae7-123">**Estado final**</span><span class="sxs-lookup"><span data-stu-id="aeae7-123">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="aeae7-124">Nenhum conjunto de aplicações do Office instalado</span><span class="sxs-lookup"><span data-stu-id="aeae7-124">No Office suite installed</span></span>  <br/> |<span data-ttu-id="aeae7-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aeae7-125">None</span></span>  <br/> |<span data-ttu-id="aeae7-126">O Office 2016 de 32 bits é instalado usando clique para execução</span><span class="sxs-lookup"><span data-stu-id="aeae7-126">Office 2016 32-bit is installed by using Click-to-Run</span></span>  <br/> |
|<span data-ttu-id="aeae7-127">Versão Clique-e-Use de 32 bits do Office (2016 ou anterior) sem aplicações autónomas</span><span class="sxs-lookup"><span data-stu-id="aeae7-127">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="aeae7-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aeae7-128">None</span></span>  <br/> |<span data-ttu-id="aeae7-129">Atualizada para a versão Clique-e-Use de 32 bits mais recente do Office 2016, conforme necessário **\***</span><span class="sxs-lookup"><span data-stu-id="aeae7-129">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="aeae7-130">Versão existente de 32 bits do Office e aplicativos autônomos de 32 bits do Office e Click-to-Run de 32 bits ou 64 bits (por exemplo, Visio, Projeto)</span><span class="sxs-lookup"><span data-stu-id="aeae7-130">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32-bit or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="aeae7-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aeae7-131">None</span></span>  <br/> |<span data-ttu-id="aeae7-132">Aplicativos autônomos não são afetados.</span><span class="sxs-lookup"><span data-stu-id="aeae7-132">Standalone apps aren't affected.</span></span> <span data-ttu-id="aeae7-133">O conjunto de aplicações é atualizado para a versão Clique-e-Use de 32 bits do Office 2016</span><span class="sxs-lookup"><span data-stu-id="aeae7-133">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="aeae7-134">Versão Clique-e-Use de 32 bits do Office e quaisquer aplicações autónomas do Office MSI de 32 ou 64 bits (exceto o 2016)</span><span class="sxs-lookup"><span data-stu-id="aeae7-134">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="aeae7-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aeae7-135">None</span></span>  <br/> |<span data-ttu-id="aeae7-136">Aplicativos autônomos não são afetados.</span><span class="sxs-lookup"><span data-stu-id="aeae7-136">Standalone apps aren't affected.</span></span> <span data-ttu-id="aeae7-137">O conjunto de aplicações é atualizado para a versão Clique-e-Use de 32 bits do Office 2016</span><span class="sxs-lookup"><span data-stu-id="aeae7-137">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="aeae7-138">Qualquer versão Clique-e-Use de 64 bits do Office</span><span class="sxs-lookup"><span data-stu-id="aeae7-138">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="aeae7-139">Desinstale os aplicativos do Office de 64 bits, se não houver problema em substituí-los por aplicativos do Office de 32 bits</span><span class="sxs-lookup"><span data-stu-id="aeae7-139">Uninstall the 64-bit Office apps, if it's OK to replace them with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="aeae7-140">Se as aplicações do Office de 64 bits forem removidas, a versão Clique-e-Use de 32 bits do Office 2016 é instalada</span><span class="sxs-lookup"><span data-stu-id="aeae7-140">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="aeae7-141">Uma instalação MSI do Office 2016 com ou sem aplicações autónomas</span><span class="sxs-lookup"><span data-stu-id="aeae7-141">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="aeae7-142">Desinstale o Office 2016 MSI.</span><span class="sxs-lookup"><span data-stu-id="aeae7-142">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="aeae7-p106">A versão Clique-e-Use de 32 bits do Office 2016 é instalada. As aplicações autónomas não são alteradas</span><span class="sxs-lookup"><span data-stu-id="aeae7-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="aeae7-145">Instalação do Office 2013 MSI (ou anterior) e/ou aplicações autónomas do Office</span><span class="sxs-lookup"><span data-stu-id="aeae7-145">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="aeae7-146">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="aeae7-146">None</span></span>  <br/> |<span data-ttu-id="aeae7-147">A versão Clique-e-Use de 32 bits do Office 2016 e a instalação do Office MSI já existente (e aplicações autónomas) existem em simultâneo</span><span class="sxs-lookup"><span data-stu-id="aeae7-147">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="aeae7-148">**(\*) Nota:** não é atualizada para a versão Clique-e-Use de 32 bits do Office 2016 devido a um erro desconhecido.</span><span class="sxs-lookup"><span data-stu-id="aeae7-148">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug.</span></span> <span data-ttu-id="aeae7-149">Uma correção está em andamento.</span><span class="sxs-lookup"><span data-stu-id="aeae7-149">A fix is in progress.</span></span> 
  