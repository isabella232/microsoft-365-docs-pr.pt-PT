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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Conheça os estados do dispositivo no Microsoft 365 Business.
ms.openlocfilehash: 26b218cb7b6a14f17e33d34a2e712b06ac814c0c
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/15/2020
ms.locfileid: "42065778"
---
# <a name="device-states"></a><span data-ttu-id="27c60-103">Estados do dispositivo</span><span class="sxs-lookup"><span data-stu-id="27c60-103">Device states</span></span>

<span data-ttu-id="27c60-104">Os dispositivos na lista **Ações de dispositivos** (Página principal de administração \> **Ações de dispositivos**) podem ter os seguintes estados.</span><span class="sxs-lookup"><span data-stu-id="27c60-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="27c60-106">**Estado**</span><span class="sxs-lookup"><span data-stu-id="27c60-106">**Status**</span></span>|<span data-ttu-id="27c60-107">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="27c60-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="27c60-108">Gerido pelo Intune</span><span class="sxs-lookup"><span data-stu-id="27c60-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="27c60-109">Gerido pelo Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="27c60-109">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="27c60-110">Extinção pendente</span><span class="sxs-lookup"><span data-stu-id="27c60-110">Retire pending</span></span>  <br/> |<span data-ttu-id="27c60-111">O Microsoft 365 Business está a preparar-se para remover dados empresariais do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27c60-111">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="27c60-112">Extinção em curso</span><span class="sxs-lookup"><span data-stu-id="27c60-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="27c60-113">O Microsoft 365 Business está a remover dados empresariais do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27c60-113">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="27c60-114">Falha na extinção</span><span class="sxs-lookup"><span data-stu-id="27c60-114">Retire failed</span></span>  <br/> | <span data-ttu-id="27c60-115">A ação de remoção de dados empresariais falhou.</span><span class="sxs-lookup"><span data-stu-id="27c60-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="27c60-116">Aposentadoria cancelada</span><span class="sxs-lookup"><span data-stu-id="27c60-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="27c60-117">A ação de reforma foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="27c60-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="27c60-118">Eliminação dos dados pendente</span><span class="sxs-lookup"><span data-stu-id="27c60-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="27c60-119">A aguardar o início da reposição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="27c60-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="27c60-120">Eliminação dos dados em curso</span><span class="sxs-lookup"><span data-stu-id="27c60-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="27c60-121">A reposição de fábrica foi emitida.</span><span class="sxs-lookup"><span data-stu-id="27c60-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="27c60-122">Falha ao limpar</span><span class="sxs-lookup"><span data-stu-id="27c60-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="27c60-123">Não podia fazer o reset da fábrica.</span><span class="sxs-lookup"><span data-stu-id="27c60-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="27c60-124">Limpeza cancelada</span><span class="sxs-lookup"><span data-stu-id="27c60-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="27c60-125">A limpeza da fábrica foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="27c60-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="27c60-126">Mau Estado de Funcionamento</span><span class="sxs-lookup"><span data-stu-id="27c60-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="27c60-127">Está pendente uma ação (ou em curso), mas o dispositivo não faz o check-in há mais de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="27c60-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="27c60-128">Eliminação pendente</span><span class="sxs-lookup"><span data-stu-id="27c60-128">Delete pending</span></span>  <br/> |<span data-ttu-id="27c60-129">A ação de eliminação está pendente.</span><span class="sxs-lookup"><span data-stu-id="27c60-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="27c60-130">Detetado</span><span class="sxs-lookup"><span data-stu-id="27c60-130">Discovered</span></span>  <br/> |<span data-ttu-id="27c60-131">O Microsoft 365 Business detetou o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27c60-131">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
