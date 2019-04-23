---
title: Resolver problemas de dispositivos AutoPilot
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: troubleshooting
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Obter informações sobre como resolver erros de ficheiro do dispositivo de piloto automático.
ms.openlocfilehash: 9d4a47f78c38d8c076f5b3876a36b6bf46eaaaf3
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32279844"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="d252b-103">Resolver problemas de dispositivos AutoPilot</span><span class="sxs-lookup"><span data-stu-id="d252b-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="d252b-104">Mensagens de erro do ficheiro de dispositivo</span><span class="sxs-lookup"><span data-stu-id="d252b-104">Device file error messages</span></span>

<span data-ttu-id="d252b-105">Info de aqui em alguns dos erros poderá ver enquanto estiver a trabalhar com ficheiros de dispositivo de piloto automático no Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="d252b-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business.</span></span> 
  
|<span data-ttu-id="d252b-106">**Código de erro**</span><span class="sxs-lookup"><span data-stu-id="d252b-106">**Error code**</span></span>|<span data-ttu-id="d252b-107">**Corrigir a tentar**</span><span class="sxs-lookup"><span data-stu-id="d252b-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d252b-108">Corpo de pedido inválido</span><span class="sxs-lookup"><span data-stu-id="d252b-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="d252b-109">Este erro deve ocorrer raramente, se vir este erro, tente novamente a operação.</span><span class="sxs-lookup"><span data-stu-id="d252b-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="d252b-110">Valor de hash de hardware para um dispositivo não está correcto.</span><span class="sxs-lookup"><span data-stu-id="d252b-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="d252b-111">Se vir este erro, isso significa que o valor fornecido no ficheiro CSV para o hash de hardware de um dispositivo não está correcto.</span><span class="sxs-lookup"><span data-stu-id="d252b-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="d252b-112">Em primeiro lugar, certifique-se de que o valor foi escrito correctamente.</span><span class="sxs-lookup"><span data-stu-id="d252b-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="d252b-113">Se pensa que o valor está correcto, mas este erro ainda está a acontecer, peça ao seu fornecedor de hardware para obter ajuda.</span><span class="sxs-lookup"><span data-stu-id="d252b-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="d252b-114">Dispositivo atribuído ao outro tenant</span><span class="sxs-lookup"><span data-stu-id="d252b-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="d252b-115">Se vir este erro, isso significa que o valor fornecido no ficheiro CSV para o número de série ou a chave de produto de um ou mais dispositivos não é correcto.</span><span class="sxs-lookup"><span data-stu-id="d252b-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="d252b-116">Em primeiro lugar, certifique-se de que o valor foi escrito correctamente.</span><span class="sxs-lookup"><span data-stu-id="d252b-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="d252b-117">Se pensa que o valor está correcto, mas este erro ainda está a acontecer, peça ao seu fornecedor de hardware para obter ajuda.</span><span class="sxs-lookup"><span data-stu-id="d252b-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="d252b-118">O ficheiro CSV contém uma chave de produto ou número de série inválido</span><span class="sxs-lookup"><span data-stu-id="d252b-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="d252b-119">Se vir este erro significa que o dispositivo que está a tentar registar já está registado por uma outra organização.</span><span class="sxs-lookup"><span data-stu-id="d252b-119">If you see this error it means that the device you are tyring to register is already registered by an other organization.</span></span> <span data-ttu-id="d252b-120">Para corrigir este problema, peça ao seu fornecedor de hardware para obter ajuda.</span><span class="sxs-lookup"><span data-stu-id="d252b-120">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="d252b-121">Este dispositivo não é suportado para o programa de configuração utilizando o piloto automático</span><span class="sxs-lookup"><span data-stu-id="d252b-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="d252b-122">Este erro significa que o dispositivo não cumpre requisitos de implementação piloto automático.</span><span class="sxs-lookup"><span data-stu-id="d252b-122">This error means the device does not meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="d252b-123">Os dispositivos têm de cumprir os seguintes requisitos:</span><span class="sxs-lookup"><span data-stu-id="d252b-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="d252b-124">Windows 10, versão 1703 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="d252b-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="d252b-125">Novos dispositivos que não tenham tido a experiência de configuração inicial do Windows.</span><span class="sxs-lookup"><span data-stu-id="d252b-125">New devices that have not been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="d252b-126">Não foi encontrado nenhum dispositivo</span><span class="sxs-lookup"><span data-stu-id="d252b-126">Device not found</span></span>  <br/> |<span data-ttu-id="d252b-127">Este erro significa que um ou mais dispositivos no ficheiro CSV não está registado para a sua organização.</span><span class="sxs-lookup"><span data-stu-id="d252b-127">This error means that one or more devices in your CSV file is not registered to your organization.</span></span> <span data-ttu-id="d252b-128">Para corrigir este problema, peça ao seu fornecedor de hardware para obter ajuda.</span><span class="sxs-lookup"><span data-stu-id="d252b-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
   
