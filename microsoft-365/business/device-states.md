---
title: Estados do dispositivo
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Conheça os vários estados do dispositivo na lista de ações do Dispositivo em casa da Admin na Microsoft 365 para negócios.
ms.openlocfilehash: 90c11caa03249408ba2916d303bcb4a59fbcca8c
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/27/2020
ms.locfileid: "44400960"
---
# <a name="device-states"></a><span data-ttu-id="ece54-103">Estados do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ece54-103">Device states</span></span>

<span data-ttu-id="ece54-104">Os dispositivos na lista **Ações de dispositivos** (Página principal de administração \> **Ações de dispositivos**) podem ter os seguintes estados.</span><span class="sxs-lookup"><span data-stu-id="ece54-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="ece54-106">**Estado**</span><span class="sxs-lookup"><span data-stu-id="ece54-106">**Status**</span></span>|<span data-ttu-id="ece54-107">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ece54-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ece54-108">Gerido pelo Intune</span><span class="sxs-lookup"><span data-stu-id="ece54-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="ece54-109">Gerido pelo Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="ece54-109">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="ece54-110">Extinção pendente</span><span class="sxs-lookup"><span data-stu-id="ece54-110">Retire pending</span></span>  <br/> |<span data-ttu-id="ece54-111">O Microsoft 365 Business Premium está a preparar-se para remover os dados da empresa do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ece54-111">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="ece54-112">Extinção em curso</span><span class="sxs-lookup"><span data-stu-id="ece54-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="ece54-113">O Microsoft 365 Business Premium está neste momento a remover os dados da empresa do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ece54-113">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="ece54-114">Falha na extinção</span><span class="sxs-lookup"><span data-stu-id="ece54-114">Retire failed</span></span>  <br/> | <span data-ttu-id="ece54-115">A ação de remoção de dados empresariais falhou.</span><span class="sxs-lookup"><span data-stu-id="ece54-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="ece54-116">Aposentadoria cancelada</span><span class="sxs-lookup"><span data-stu-id="ece54-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="ece54-117">A ação de reforma foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="ece54-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="ece54-118">Eliminação dos dados pendente</span><span class="sxs-lookup"><span data-stu-id="ece54-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="ece54-119">A aguardar o início da reposição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="ece54-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="ece54-120">Eliminação dos dados em curso</span><span class="sxs-lookup"><span data-stu-id="ece54-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="ece54-121">A reposição de fábrica foi emitida.</span><span class="sxs-lookup"><span data-stu-id="ece54-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="ece54-122">Falha ao limpar</span><span class="sxs-lookup"><span data-stu-id="ece54-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="ece54-123">Não podia fazer o reset da fábrica.</span><span class="sxs-lookup"><span data-stu-id="ece54-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="ece54-124">Limpeza cancelada</span><span class="sxs-lookup"><span data-stu-id="ece54-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="ece54-125">A limpeza da fábrica foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="ece54-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="ece54-126">Mau Estado de Funcionamento</span><span class="sxs-lookup"><span data-stu-id="ece54-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="ece54-127">Está pendente uma ação (ou em curso), mas o dispositivo não faz o check-in há mais de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="ece54-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="ece54-128">Eliminação pendente</span><span class="sxs-lookup"><span data-stu-id="ece54-128">Delete pending</span></span>  <br/> |<span data-ttu-id="ece54-129">A ação de eliminação está pendente.</span><span class="sxs-lookup"><span data-stu-id="ece54-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="ece54-130">Detetado</span><span class="sxs-lookup"><span data-stu-id="ece54-130">Discovered</span></span>  <br/> |<span data-ttu-id="ece54-131">O Microsoft 365 Business Premium detetou o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ece54-131">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   
