---
title: Resolver problemas de dispositivos AutoPilot
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- ZTDTroubleshootDeviceErrors
- O365E_ZTDTroubleshootDeviceErrors
- BCS365_ZTDTroubleshootDeviceErrors
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Saiba como resolver os erros que poderá ver enquanto trabalha com ficheiros de dispositivos AutoPilot no Microsoft 365 Business Premium.
ms.openlocfilehash: 1078ab74b07952e4bb565555a081b98ecce9db5c
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578093"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="0afe5-103">Resolver problemas de dispositivos AutoPilot</span><span class="sxs-lookup"><span data-stu-id="0afe5-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="0afe5-104">Mensagens de erro de ficheiro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="0afe5-104">Device file error messages</span></span>

<span data-ttu-id="0afe5-105">Aqui estão as informações sobre alguns dos erros que pode ver enquanto trabalha com ficheiros de dispositivos AutoPilot no Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="0afe5-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business Premium.</span></span> 
  
|<span data-ttu-id="0afe5-106">**Código de erro**</span><span class="sxs-lookup"><span data-stu-id="0afe5-106">**Error code**</span></span>|<span data-ttu-id="0afe5-107">**Corrigir para tentar**</span><span class="sxs-lookup"><span data-stu-id="0afe5-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0afe5-108">Corpo de pedido inválido</span><span class="sxs-lookup"><span data-stu-id="0afe5-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="0afe5-109">Este erro raramente deve acontecer, se vir este erro, tente novamente a operação.</span><span class="sxs-lookup"><span data-stu-id="0afe5-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="0afe5-110">O valor de hash de hardware para um dispositivo não está correto.</span><span class="sxs-lookup"><span data-stu-id="0afe5-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="0afe5-111">Se vir este erro, significa que o valor que forneceu no seu ficheiro CSV para o hash de hardware de um dispositivo não está correto.</span><span class="sxs-lookup"><span data-stu-id="0afe5-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="0afe5-112">Primeiro, verifique se o valor foi corretamente digitado.</span><span class="sxs-lookup"><span data-stu-id="0afe5-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="0afe5-113">Se acha que o valor está correto, mas este erro ainda está a acontecer, peça ajuda ao seu fornecedor de hardware.</span><span class="sxs-lookup"><span data-stu-id="0afe5-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="0afe5-114">Dispositivo atribuído a outro inquilino</span><span class="sxs-lookup"><span data-stu-id="0afe5-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="0afe5-115">Se vir este erro, significa que o valor que forneceu no seu ficheiro CSV para o número de série ou a chave de produto de um ou mais dispositivos não está correto.</span><span class="sxs-lookup"><span data-stu-id="0afe5-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="0afe5-116">Primeiro, verifique se o valor foi corretamente digitado.</span><span class="sxs-lookup"><span data-stu-id="0afe5-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="0afe5-117">Se acha que o valor está correto, mas este erro ainda está a acontecer, peça ajuda ao seu fornecedor de hardware.</span><span class="sxs-lookup"><span data-stu-id="0afe5-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="0afe5-118">O ficheiro CSV contém um número de série inválido ou chave de produto</span><span class="sxs-lookup"><span data-stu-id="0afe5-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="0afe5-119">Se vir este erro, significa que o dispositivo que está a tentar registar já está registado por outra organização.</span><span class="sxs-lookup"><span data-stu-id="0afe5-119">If you see this error, it means that the device you are trying to register is already registered by another organization.</span></span> <span data-ttu-id="0afe5-120">Para corrigir este erro, peça ajuda ao seu fornecedor de hardware.</span><span class="sxs-lookup"><span data-stu-id="0afe5-120">To fix this error, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="0afe5-121">Este dispositivo não é suportado para configuração utilizando o AutoPilot</span><span class="sxs-lookup"><span data-stu-id="0afe5-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="0afe5-122">Este erro significa que o dispositivo não satisfaz os requisitos de implementação do AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="0afe5-122">This error means the device doesn't meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="0afe5-123">Os dispositivos têm de cumprir os seguintes requisitos:</span><span class="sxs-lookup"><span data-stu-id="0afe5-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="0afe5-124">Windows 10, versão 1703 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="0afe5-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="0afe5-125">Novos dispositivos que não passaram pela experiência fora de caixa do Windows.</span><span class="sxs-lookup"><span data-stu-id="0afe5-125">New devices that haven't been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="0afe5-126">Dispositivo não encontrado</span><span class="sxs-lookup"><span data-stu-id="0afe5-126">Device not found</span></span>  <br/> |<span data-ttu-id="0afe5-127">Este erro significa que um ou mais dispositivos no seu ficheiro CSV não estão registados na sua organização.</span><span class="sxs-lookup"><span data-stu-id="0afe5-127">This error means that one or more devices in your CSV file isn't registered to your organization.</span></span> <span data-ttu-id="0afe5-128">Para corrigir isto, peça ajuda ao seu fornecedor de hardware.</span><span class="sxs-lookup"><span data-stu-id="0afe5-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
