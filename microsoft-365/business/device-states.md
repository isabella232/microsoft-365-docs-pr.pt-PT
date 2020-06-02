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
description: Conheça os vários estados de dispositivos na lista de ações do Dispositivo na casa do Administrador na Microsoft 365 para negócios.
ms.openlocfilehash: 64138e2b6ae73c067709cde1912a96615d08ebf1
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471185"
---
# <a name="device-states"></a><span data-ttu-id="0a242-103">Estados do dispositivo</span><span class="sxs-lookup"><span data-stu-id="0a242-103">Device states</span></span>

<span data-ttu-id="0a242-104">Este artigo aplica-se ao Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="0a242-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="0a242-105">Os dispositivos na lista **Ações de dispositivos** (Página principal de administração \> **Ações de dispositivos**) podem ter os seguintes estados.</span><span class="sxs-lookup"><span data-stu-id="0a242-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="0a242-107">**Estado**</span><span class="sxs-lookup"><span data-stu-id="0a242-107">**Status**</span></span>|<span data-ttu-id="0a242-108">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0a242-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0a242-109">Gerido pelo Intune</span><span class="sxs-lookup"><span data-stu-id="0a242-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="0a242-110">Gerido pela Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="0a242-110">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="0a242-111">Extinção pendente</span><span class="sxs-lookup"><span data-stu-id="0a242-111">Retire pending</span></span>  <br/> |<span data-ttu-id="0a242-112">O Microsoft 365 Business Premium está a preparar-se para remover os dados da empresa do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0a242-112">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="0a242-113">Extinção em curso</span><span class="sxs-lookup"><span data-stu-id="0a242-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="0a242-114">O Microsoft 365 Business Premium está atualmente a remover os dados da empresa do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0a242-114">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="0a242-115">Falha na extinção</span><span class="sxs-lookup"><span data-stu-id="0a242-115">Retire failed</span></span>  <br/> | <span data-ttu-id="0a242-116">A ação de remoção de dados empresariais falhou.</span><span class="sxs-lookup"><span data-stu-id="0a242-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="0a242-117">Aposentadoria cancelada</span><span class="sxs-lookup"><span data-stu-id="0a242-117">Retire canceled</span></span>  <br/> |<span data-ttu-id="0a242-118">A ação de reforma foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="0a242-118">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="0a242-119">Eliminação dos dados pendente</span><span class="sxs-lookup"><span data-stu-id="0a242-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="0a242-120">A aguardar o início da reposição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="0a242-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="0a242-121">Eliminação dos dados em curso</span><span class="sxs-lookup"><span data-stu-id="0a242-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="0a242-122">A reposição de fábrica foi emitida.</span><span class="sxs-lookup"><span data-stu-id="0a242-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="0a242-123">Falha ao limpar</span><span class="sxs-lookup"><span data-stu-id="0a242-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="0a242-124">Não podia fazer o reset da fábrica.</span><span class="sxs-lookup"><span data-stu-id="0a242-124">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="0a242-125">Limpeza cancelada</span><span class="sxs-lookup"><span data-stu-id="0a242-125">Wipe canceled</span></span>  <br/> |<span data-ttu-id="0a242-126">A limpeza da fábrica foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="0a242-126">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="0a242-127">Mau Estado de Funcionamento</span><span class="sxs-lookup"><span data-stu-id="0a242-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="0a242-128">Uma ação está pendente (ou em curso), mas o dispositivo não faz o check-in há mais de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="0a242-128">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="0a242-129">Eliminação pendente</span><span class="sxs-lookup"><span data-stu-id="0a242-129">Delete pending</span></span>  <br/> |<span data-ttu-id="0a242-130">A ação de eliminação está pendente.</span><span class="sxs-lookup"><span data-stu-id="0a242-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="0a242-131">Detetado</span><span class="sxs-lookup"><span data-stu-id="0a242-131">Discovered</span></span>  <br/> |<span data-ttu-id="0a242-132">O Microsoft 365 Business Premium detetou o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0a242-132">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   
