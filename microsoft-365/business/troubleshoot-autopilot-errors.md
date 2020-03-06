---
title: Resolver problemas de dispositivos AutoPilot
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Saiba como resolver erros que poderá ver enquanto trabalha com ficheiros de dispositivos AutoPilot no Microsoft 365 Business.
ms.openlocfilehash: 7569f18097a1f5959b3dd491958c78886e1e05d6
ms.sourcegitcommit: 41c0bc5cf50f4ca63b4286d1ea0f58ab82984b7a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/05/2020
ms.locfileid: "42547477"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="ea59a-103">Resolver problemas de dispositivos AutoPilot</span><span class="sxs-lookup"><span data-stu-id="ea59a-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="ea59a-104">Mensagens de erro de ficheiro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ea59a-104">Device file error messages</span></span>

<span data-ttu-id="ea59a-105">Aqui está a informação sobre alguns dos erros que poderá ver enquanto trabalha com ficheiros de dispositivos AutoPilot no Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="ea59a-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business.</span></span> 
  
|<span data-ttu-id="ea59a-106">**Código de erro**</span><span class="sxs-lookup"><span data-stu-id="ea59a-106">**Error code**</span></span>|<span data-ttu-id="ea59a-107">**Corrigir para tentar**</span><span class="sxs-lookup"><span data-stu-id="ea59a-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ea59a-108">Organismo de pedido inválido</span><span class="sxs-lookup"><span data-stu-id="ea59a-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="ea59a-109">Este erro raramente deverá acontecer, se vir este erro, tente novamente a operação.</span><span class="sxs-lookup"><span data-stu-id="ea59a-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="ea59a-110">O valor do hash de hardware para um dispositivo não está correto.</span><span class="sxs-lookup"><span data-stu-id="ea59a-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="ea59a-111">Se vir este erro, significa que o valor que forneceu no seu ficheiro CSV para o hash de hardware de um dispositivo não está correto.</span><span class="sxs-lookup"><span data-stu-id="ea59a-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="ea59a-112">Primeiro, verifique se o valor foi dactilografado corretamente.</span><span class="sxs-lookup"><span data-stu-id="ea59a-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="ea59a-113">Se acha que o valor está correto, mas este erro ainda está a acontecer, peça ajuda ao seu fornecedor de hardware.</span><span class="sxs-lookup"><span data-stu-id="ea59a-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="ea59a-114">Dispositivo atribuído a outro inquilino</span><span class="sxs-lookup"><span data-stu-id="ea59a-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="ea59a-115">Se vir este erro, significa que o valor que forneceu no seu ficheiro CSV para o número de série ou a chave do produto de um ou mais dispositivos não está correto.</span><span class="sxs-lookup"><span data-stu-id="ea59a-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="ea59a-116">Primeiro, verifique se o valor foi dactilografado corretamente.</span><span class="sxs-lookup"><span data-stu-id="ea59a-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="ea59a-117">Se acha que o valor está correto, mas este erro ainda está a acontecer, peça ajuda ao seu fornecedor de hardware.</span><span class="sxs-lookup"><span data-stu-id="ea59a-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="ea59a-118">O ficheiro CSV contém um número de série inválido ou chave do produto</span><span class="sxs-lookup"><span data-stu-id="ea59a-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="ea59a-119">Se vir este erro, significa que o dispositivo que está a tentar registar já está registado por outra organização.</span><span class="sxs-lookup"><span data-stu-id="ea59a-119">If you see this error, it means that the device you are trying to register is already registered by another organization.</span></span> <span data-ttu-id="ea59a-120">Para corrigir este erro, peça ajuda ao seu fornecedor de hardware.</span><span class="sxs-lookup"><span data-stu-id="ea59a-120">To fix this error, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="ea59a-121">Este dispositivo não é suportado para configuração utilizando o AutoPilot</span><span class="sxs-lookup"><span data-stu-id="ea59a-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="ea59a-122">Este erro significa que o dispositivo não satisfaz os requisitos de implementação do AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="ea59a-122">This error means the device doesn't meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="ea59a-123">Os dispositivos têm de cumprir os seguintes requisitos:</span><span class="sxs-lookup"><span data-stu-id="ea59a-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="ea59a-124">Windows 10, versão 1703 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="ea59a-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="ea59a-125">Novos dispositivos que não passaram pela experiência do Windows fora da caixa.</span><span class="sxs-lookup"><span data-stu-id="ea59a-125">New devices that haven't been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="ea59a-126">Dispositivo não encontrado</span><span class="sxs-lookup"><span data-stu-id="ea59a-126">Device not found</span></span>  <br/> |<span data-ttu-id="ea59a-127">Este erro significa que um ou mais dispositivos no seu ficheiro CSV não estão registados na sua organização.</span><span class="sxs-lookup"><span data-stu-id="ea59a-127">This error means that one or more devices in your CSV file isn't registered to your organization.</span></span> <span data-ttu-id="ea59a-128">Para corrigir isto, peça ajuda ao seu fornecedor de hardware.</span><span class="sxs-lookup"><span data-stu-id="ea59a-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
