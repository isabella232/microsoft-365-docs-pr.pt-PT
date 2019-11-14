---
title: Estados do dispositivo
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Saiba mais sobre os estados de dispositivos no Microsoft 365 Business.
ms.openlocfilehash: b55e6a5d538ec28d195225e93797cea27afd2e8b
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/14/2019
ms.locfileid: "38320214"
---
# <a name="device-states"></a><span data-ttu-id="45afa-103">Estados do dispositivo</span><span class="sxs-lookup"><span data-stu-id="45afa-103">Device states</span></span>

<span data-ttu-id="45afa-104">Os dispositivos na lista **Ações de dispositivos** (Página principal de administração \> **Ações de dispositivos**) podem ter os seguintes estados.</span><span class="sxs-lookup"><span data-stu-id="45afa-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="45afa-106">**Estado**</span><span class="sxs-lookup"><span data-stu-id="45afa-106">**Status**</span></span>|<span data-ttu-id="45afa-107">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="45afa-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="45afa-108">Gerido pelo Intune</span><span class="sxs-lookup"><span data-stu-id="45afa-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="45afa-109">Gerido pelo Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="45afa-109">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="45afa-110">Extinção pendente</span><span class="sxs-lookup"><span data-stu-id="45afa-110">Retire pending</span></span>  <br/> |<span data-ttu-id="45afa-111">O Microsoft 365 Business está a preparar-se para remover dados empresariais do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45afa-111">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="45afa-112">Extinção em curso</span><span class="sxs-lookup"><span data-stu-id="45afa-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="45afa-113">O Microsoft 365 Business está a remover dados empresariais do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45afa-113">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="45afa-114">Falha na extinção</span><span class="sxs-lookup"><span data-stu-id="45afa-114">Retire failed</span></span>  <br/> | <span data-ttu-id="45afa-115">A ação de remoção de dados empresariais falhou.</span><span class="sxs-lookup"><span data-stu-id="45afa-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="45afa-116">Aposentar-se cancelado</span><span class="sxs-lookup"><span data-stu-id="45afa-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="45afa-117">A ação de aposentadoria foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="45afa-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="45afa-118">Eliminação dos dados pendente</span><span class="sxs-lookup"><span data-stu-id="45afa-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="45afa-119">A aguardar o início da reposição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="45afa-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="45afa-120">Eliminação dos dados em curso</span><span class="sxs-lookup"><span data-stu-id="45afa-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="45afa-121">A reposição de fábrica foi emitida.</span><span class="sxs-lookup"><span data-stu-id="45afa-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="45afa-122">Falha ao limpar</span><span class="sxs-lookup"><span data-stu-id="45afa-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="45afa-123">Não poderia fazer reset fábrica.</span><span class="sxs-lookup"><span data-stu-id="45afa-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="45afa-124">Limpeza cancelada</span><span class="sxs-lookup"><span data-stu-id="45afa-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="45afa-125">A limpeza da fábrica foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="45afa-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="45afa-126">Mau Estado de Funcionamento</span><span class="sxs-lookup"><span data-stu-id="45afa-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="45afa-127">Uma ação está pendente (ou em andamento), mas o dispositivo não faz o check-in por mais de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="45afa-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="45afa-128">Eliminação pendente</span><span class="sxs-lookup"><span data-stu-id="45afa-128">Delete pending</span></span>  <br/> |<span data-ttu-id="45afa-129">A ação de eliminação está pendente.</span><span class="sxs-lookup"><span data-stu-id="45afa-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="45afa-130">Detetado</span><span class="sxs-lookup"><span data-stu-id="45afa-130">Discovered</span></span>  <br/> |<span data-ttu-id="45afa-131">O Microsoft 365 Business detetou o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45afa-131">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
