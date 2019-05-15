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
description: Obter informações sobre Estados de dispositivo no Microsoft 365 Business.
ms.openlocfilehash: 06e5c800e6a104785c1fd0724223e05d7729722e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/15/2019
ms.locfileid: "34072726"
---
# <a name="device-states"></a><span data-ttu-id="cbe91-103">Estados do dispositivo</span><span class="sxs-lookup"><span data-stu-id="cbe91-103">Device states</span></span>

## <a name="device-states"></a><span data-ttu-id="cbe91-104">Estados do dispositivo</span><span class="sxs-lookup"><span data-stu-id="cbe91-104">Device states</span></span>

<span data-ttu-id="cbe91-105">Os dispositivos na lista **Ações de dispositivos** (Página principal de administração \> **Ações de dispositivos**) podem ter os seguintes estados.</span><span class="sxs-lookup"><span data-stu-id="cbe91-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="cbe91-107">**Estado**</span><span class="sxs-lookup"><span data-stu-id="cbe91-107">**Status**</span></span>|<span data-ttu-id="cbe91-108">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cbe91-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cbe91-109">Gerido pelo Intune</span><span class="sxs-lookup"><span data-stu-id="cbe91-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="cbe91-110">Gerido pelo Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="cbe91-110">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="cbe91-111">Extinção pendente</span><span class="sxs-lookup"><span data-stu-id="cbe91-111">Retire pending</span></span>  <br/> |<span data-ttu-id="cbe91-112">O Microsoft 365 Business está a preparar-se para remover dados empresariais do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cbe91-112">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="cbe91-113">Extinção em curso</span><span class="sxs-lookup"><span data-stu-id="cbe91-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="cbe91-114">O Microsoft 365 Business está a remover dados empresariais do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cbe91-114">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="cbe91-115">Falha na extinção</span><span class="sxs-lookup"><span data-stu-id="cbe91-115">Retire failed</span></span>  <br/> | <span data-ttu-id="cbe91-116">A ação de remoção de dados empresariais falhou.</span><span class="sxs-lookup"><span data-stu-id="cbe91-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="cbe91-117">Extinção cancelada</span><span class="sxs-lookup"><span data-stu-id="cbe91-117">Retire cancelled</span></span>  <br/> |<span data-ttu-id="cbe91-118">A ação de extinção foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="cbe91-118">Retire action was cancelled.</span></span>  <br/> |
|<span data-ttu-id="cbe91-119">Eliminação dos dados pendente</span><span class="sxs-lookup"><span data-stu-id="cbe91-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="cbe91-120">A aguardar o início da reposição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="cbe91-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="cbe91-121">Eliminação dos dados em curso</span><span class="sxs-lookup"><span data-stu-id="cbe91-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="cbe91-122">A reposição de fábrica foi emitida.</span><span class="sxs-lookup"><span data-stu-id="cbe91-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="cbe91-123">Falha ao limpar</span><span class="sxs-lookup"><span data-stu-id="cbe91-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="cbe91-124">Não foi possível efetuar a reposição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="cbe91-124">Couldn't perform factory reset.</span></span>  <br/> |
|<span data-ttu-id="cbe91-125">Eliminação dos dados cancelada</span><span class="sxs-lookup"><span data-stu-id="cbe91-125">Wipe cancelled</span></span>  <br/> |<span data-ttu-id="cbe91-126">A reposição de fábrica foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="cbe91-126">Factory wipe was cancelled.</span></span>  <br/> |
|<span data-ttu-id="cbe91-127">Mau Estado de Funcionamento</span><span class="sxs-lookup"><span data-stu-id="cbe91-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="cbe91-128">Isto significa que uma ação está pendente (ou em curso), mas o dispositivo não deu entrada durante 30 dias ou mais.</span><span class="sxs-lookup"><span data-stu-id="cbe91-128">This means that an action is pending (or in progress) but the device has not checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="cbe91-129">Eliminação pendente</span><span class="sxs-lookup"><span data-stu-id="cbe91-129">Delete pending</span></span>  <br/> |<span data-ttu-id="cbe91-130">A ação de eliminação está pendente.</span><span class="sxs-lookup"><span data-stu-id="cbe91-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="cbe91-131">Detetado</span><span class="sxs-lookup"><span data-stu-id="cbe91-131">Discovered</span></span>  <br/> |<span data-ttu-id="cbe91-132">O Microsoft 365 Business detetou o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cbe91-132">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
