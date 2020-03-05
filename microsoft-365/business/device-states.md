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
description: Conheça os vários estados do dispositivo na lista de ações do Dispositivo em casa da Admin no Microsoft 365 Business.
ms.openlocfilehash: 878050fbe11acca1d5d434a5d2ab0b5b48510e45
ms.sourcegitcommit: ab916c216053999c9c4ef4838217e82cd861f23f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2020
ms.locfileid: "42415671"
---
# <a name="device-states"></a><span data-ttu-id="43507-103">Estados do dispositivo</span><span class="sxs-lookup"><span data-stu-id="43507-103">Device states</span></span>

<span data-ttu-id="43507-104">Os dispositivos na lista **Ações de dispositivos** (Página principal de administração \> **Ações de dispositivos**) podem ter os seguintes estados.</span><span class="sxs-lookup"><span data-stu-id="43507-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="43507-106">**Estado**</span><span class="sxs-lookup"><span data-stu-id="43507-106">**Status**</span></span>|<span data-ttu-id="43507-107">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="43507-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="43507-108">Gerido pelo Intune</span><span class="sxs-lookup"><span data-stu-id="43507-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="43507-109">Gerido pelo Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="43507-109">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="43507-110">Extinção pendente</span><span class="sxs-lookup"><span data-stu-id="43507-110">Retire pending</span></span>  <br/> |<span data-ttu-id="43507-111">O Microsoft 365 Business está a preparar-se para remover dados empresariais do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="43507-111">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="43507-112">Extinção em curso</span><span class="sxs-lookup"><span data-stu-id="43507-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="43507-113">O Microsoft 365 Business está a remover dados empresariais do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="43507-113">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="43507-114">Falha na extinção</span><span class="sxs-lookup"><span data-stu-id="43507-114">Retire failed</span></span>  <br/> | <span data-ttu-id="43507-115">A ação de remoção de dados empresariais falhou.</span><span class="sxs-lookup"><span data-stu-id="43507-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="43507-116">Aposentadoria cancelada</span><span class="sxs-lookup"><span data-stu-id="43507-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="43507-117">A ação de reforma foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="43507-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="43507-118">Eliminação dos dados pendente</span><span class="sxs-lookup"><span data-stu-id="43507-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="43507-119">A aguardar o início da reposição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="43507-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="43507-120">Eliminação dos dados em curso</span><span class="sxs-lookup"><span data-stu-id="43507-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="43507-121">A reposição de fábrica foi emitida.</span><span class="sxs-lookup"><span data-stu-id="43507-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="43507-122">Falha ao limpar</span><span class="sxs-lookup"><span data-stu-id="43507-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="43507-123">Não podia fazer o reset da fábrica.</span><span class="sxs-lookup"><span data-stu-id="43507-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="43507-124">Limpeza cancelada</span><span class="sxs-lookup"><span data-stu-id="43507-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="43507-125">A limpeza da fábrica foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="43507-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="43507-126">Mau Estado de Funcionamento</span><span class="sxs-lookup"><span data-stu-id="43507-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="43507-127">Está pendente uma ação (ou em curso), mas o dispositivo não faz o check-in há mais de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="43507-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="43507-128">Eliminação pendente</span><span class="sxs-lookup"><span data-stu-id="43507-128">Delete pending</span></span>  <br/> |<span data-ttu-id="43507-129">A ação de eliminação está pendente.</span><span class="sxs-lookup"><span data-stu-id="43507-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="43507-130">Detetado</span><span class="sxs-lookup"><span data-stu-id="43507-130">Discovered</span></span>  <br/> |<span data-ttu-id="43507-131">O Microsoft 365 Business detetou o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="43507-131">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
