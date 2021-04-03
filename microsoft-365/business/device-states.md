---
title: Estados do dispositivo
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: Conheça os vários estados de dispositivos na lista de ações do Dispositivo na casa do Administrador na Microsoft 365 para negócios.
ms.openlocfilehash: e6f1b428413d094e0a1ce3afb026528074038736
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578473"
---
# <a name="device-states"></a><span data-ttu-id="a7c3b-103">Estados do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a7c3b-103">Device states</span></span>

<span data-ttu-id="a7c3b-104">Este artigo aplica-se ao Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="a7c3b-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="a7c3b-105">Os dispositivos na lista **Ações de dispositivos** (Página principal de administração \> **Ações de dispositivos**) podem ter os seguintes estados.</span><span class="sxs-lookup"><span data-stu-id="a7c3b-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="a7c3b-107">**Estado**</span><span class="sxs-lookup"><span data-stu-id="a7c3b-107">**Status**</span></span>|<span data-ttu-id="a7c3b-108">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a7c3b-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a7c3b-109">Gerido pelo Intune</span><span class="sxs-lookup"><span data-stu-id="a7c3b-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="a7c3b-110">Gerido pela Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="a7c3b-110">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="a7c3b-111">Extinção pendente</span><span class="sxs-lookup"><span data-stu-id="a7c3b-111">Retire pending</span></span>  <br/> |<span data-ttu-id="a7c3b-112">O Microsoft 365 Business Premium está a preparar-se para remover os dados da empresa do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a7c3b-112">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="a7c3b-113">Extinção em curso</span><span class="sxs-lookup"><span data-stu-id="a7c3b-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="a7c3b-114">O Microsoft 365 Business Premium está atualmente a remover os dados da empresa do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a7c3b-114">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="a7c3b-115">Falha na extinção</span><span class="sxs-lookup"><span data-stu-id="a7c3b-115">Retire failed</span></span>  <br/> | <span data-ttu-id="a7c3b-116">A ação de remoção de dados empresariais falhou.</span><span class="sxs-lookup"><span data-stu-id="a7c3b-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="a7c3b-117">Aposentadoria cancelada</span><span class="sxs-lookup"><span data-stu-id="a7c3b-117">Retire canceled</span></span>  <br/> |<span data-ttu-id="a7c3b-118">A ação de reforma foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="a7c3b-118">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="a7c3b-119">Eliminação dos dados pendente</span><span class="sxs-lookup"><span data-stu-id="a7c3b-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="a7c3b-120">A aguardar o início da reposição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="a7c3b-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="a7c3b-121">Eliminação dos dados em curso</span><span class="sxs-lookup"><span data-stu-id="a7c3b-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="a7c3b-122">A reposição de fábrica foi emitida.</span><span class="sxs-lookup"><span data-stu-id="a7c3b-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="a7c3b-123">Falha ao limpar</span><span class="sxs-lookup"><span data-stu-id="a7c3b-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="a7c3b-124">Não podia fazer o reset da fábrica.</span><span class="sxs-lookup"><span data-stu-id="a7c3b-124">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="a7c3b-125">Limpeza cancelada</span><span class="sxs-lookup"><span data-stu-id="a7c3b-125">Wipe canceled</span></span>  <br/> |<span data-ttu-id="a7c3b-126">A limpeza da fábrica foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="a7c3b-126">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="a7c3b-127">Mau Estado de Funcionamento</span><span class="sxs-lookup"><span data-stu-id="a7c3b-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="a7c3b-128">Uma ação está pendente (ou em curso), mas o dispositivo não faz o check-in há mais de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="a7c3b-128">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="a7c3b-129">Eliminação pendente</span><span class="sxs-lookup"><span data-stu-id="a7c3b-129">Delete pending</span></span>  <br/> |<span data-ttu-id="a7c3b-130">A ação de eliminação está pendente.</span><span class="sxs-lookup"><span data-stu-id="a7c3b-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="a7c3b-131">Detetado</span><span class="sxs-lookup"><span data-stu-id="a7c3b-131">Discovered</span></span>  <br/> |<span data-ttu-id="a7c3b-132">O Microsoft 365 Business Premium detetou o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a7c3b-132">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   
