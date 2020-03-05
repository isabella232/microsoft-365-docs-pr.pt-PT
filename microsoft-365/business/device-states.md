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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Conheça os vários estados do dispositivo na lista de ações do Dispositivo em casa da Admin no Microsoft 365 Business.
ms.openlocfilehash: cb1e5172a6e2d0bfc5748fe982024ead26e8cd62
ms.sourcegitcommit: d6c871bf3f94d9299d22695f5dbaf25dc1bd6ff9
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/05/2020
ms.locfileid: "42417322"
---
# <a name="device-states"></a><span data-ttu-id="39491-103">Estados do dispositivo</span><span class="sxs-lookup"><span data-stu-id="39491-103">Device states</span></span>

<span data-ttu-id="39491-104">Os dispositivos na lista **Ações de dispositivos** (Página principal de administração \> **Ações de dispositivos**) podem ter os seguintes estados.</span><span class="sxs-lookup"><span data-stu-id="39491-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="39491-106">**Estado**</span><span class="sxs-lookup"><span data-stu-id="39491-106">**Status**</span></span>|<span data-ttu-id="39491-107">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="39491-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="39491-108">Gerido pelo Intune</span><span class="sxs-lookup"><span data-stu-id="39491-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="39491-109">Gerido pelo Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="39491-109">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="39491-110">Extinção pendente</span><span class="sxs-lookup"><span data-stu-id="39491-110">Retire pending</span></span>  <br/> |<span data-ttu-id="39491-111">O Microsoft 365 Business está a preparar-se para remover dados empresariais do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="39491-111">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="39491-112">Extinção em curso</span><span class="sxs-lookup"><span data-stu-id="39491-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="39491-113">O Microsoft 365 Business está a remover dados empresariais do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="39491-113">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="39491-114">Falha na extinção</span><span class="sxs-lookup"><span data-stu-id="39491-114">Retire failed</span></span>  <br/> | <span data-ttu-id="39491-115">A ação de remoção de dados empresariais falhou.</span><span class="sxs-lookup"><span data-stu-id="39491-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="39491-116">Aposentadoria cancelada</span><span class="sxs-lookup"><span data-stu-id="39491-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="39491-117">A ação de reforma foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="39491-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="39491-118">Eliminação dos dados pendente</span><span class="sxs-lookup"><span data-stu-id="39491-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="39491-119">A aguardar o início da reposição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="39491-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="39491-120">Eliminação dos dados em curso</span><span class="sxs-lookup"><span data-stu-id="39491-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="39491-121">A reposição de fábrica foi emitida.</span><span class="sxs-lookup"><span data-stu-id="39491-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="39491-122">Falha ao limpar</span><span class="sxs-lookup"><span data-stu-id="39491-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="39491-123">Não podia fazer o reset da fábrica.</span><span class="sxs-lookup"><span data-stu-id="39491-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="39491-124">Limpeza cancelada</span><span class="sxs-lookup"><span data-stu-id="39491-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="39491-125">A limpeza da fábrica foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="39491-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="39491-126">Mau Estado de Funcionamento</span><span class="sxs-lookup"><span data-stu-id="39491-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="39491-127">Está pendente uma ação (ou em curso), mas o dispositivo não faz o check-in há mais de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="39491-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="39491-128">Eliminação pendente</span><span class="sxs-lookup"><span data-stu-id="39491-128">Delete pending</span></span>  <br/> |<span data-ttu-id="39491-129">A ação de eliminação está pendente.</span><span class="sxs-lookup"><span data-stu-id="39491-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="39491-130">Detetado</span><span class="sxs-lookup"><span data-stu-id="39491-130">Discovered</span></span>  <br/> |<span data-ttu-id="39491-131">O Microsoft 365 Business detetou o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="39491-131">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
