---
title: Resolver problemas de dispositivos AutoPilot
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Saiba como solucionar erros de arquivo de dispositivos AutoPilot.
ms.openlocfilehash: 1b5358bd6686c2548e82ec5297ac0ad675835718
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/19/2019
ms.locfileid: "38718705"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="c9aa0-103">Resolver problemas de dispositivos AutoPilot</span><span class="sxs-lookup"><span data-stu-id="c9aa0-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="c9aa0-104">Mensagens de erro de arquivo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="c9aa0-104">Device file error messages</span></span>

<span data-ttu-id="c9aa0-105">Aqui estão as informações sobre alguns dos erros que você pode ver enquanto trabalha com arquivos de dispositivos AutoPilot no Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="c9aa0-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business.</span></span> 
  
|<span data-ttu-id="c9aa0-106">**Código de erro**</span><span class="sxs-lookup"><span data-stu-id="c9aa0-106">**Error code**</span></span>|<span data-ttu-id="c9aa0-107">**Corrigir para tentar**</span><span class="sxs-lookup"><span data-stu-id="c9aa0-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c9aa0-108">Órgão de solicitação inválido</span><span class="sxs-lookup"><span data-stu-id="c9aa0-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="c9aa0-109">Este erro deve acontecer raramente, se você ver este erro, tente a operação outra vez.</span><span class="sxs-lookup"><span data-stu-id="c9aa0-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="c9aa0-110">O valor do hash de hardware para um dispositivo não está correto.</span><span class="sxs-lookup"><span data-stu-id="c9aa0-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="c9aa0-111">Se você ver esse erro, isso significa que o valor que você forneceu em seu arquivo CSV para o hash de hardware de um dispositivo não está correto.</span><span class="sxs-lookup"><span data-stu-id="c9aa0-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="c9aa0-112">Primeiro, verifique se o valor foi digitado corretamente.</span><span class="sxs-lookup"><span data-stu-id="c9aa0-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="c9aa0-113">Se você acha que o valor está correto, mas esse erro ainda está acontecendo, peça ajuda ao fornecedor de hardware.</span><span class="sxs-lookup"><span data-stu-id="c9aa0-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="c9aa0-114">Dispositivo atribuído a outro inquilino</span><span class="sxs-lookup"><span data-stu-id="c9aa0-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="c9aa0-115">Se você ver esse erro, isso significa que o valor que você forneceu em seu arquivo CSV para o número de série ou a chave do produto de um ou mais dispositivos não está correto.</span><span class="sxs-lookup"><span data-stu-id="c9aa0-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="c9aa0-116">Primeiro, verifique se o valor foi digitado corretamente.</span><span class="sxs-lookup"><span data-stu-id="c9aa0-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="c9aa0-117">Se você acha que o valor está correto, mas esse erro ainda está acontecendo, peça ajuda ao fornecedor de hardware.</span><span class="sxs-lookup"><span data-stu-id="c9aa0-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="c9aa0-118">O arquivo CSV contém um número de série inválido ou chave do produto</span><span class="sxs-lookup"><span data-stu-id="c9aa0-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="c9aa0-119">Se você ver esse erro, isso significa que o dispositivo que você está tentando registrar já está registrado por outra organização.</span><span class="sxs-lookup"><span data-stu-id="c9aa0-119">If you see this error, it means that the device you are trying to register is already registered by another organization.</span></span> <span data-ttu-id="c9aa0-120">Para corrigir esse erro, peça ajuda ao fornecedor de hardware.</span><span class="sxs-lookup"><span data-stu-id="c9aa0-120">To fix this error, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="c9aa0-121">Este dispositivo não é suportado para configuração usando AutoPilot</span><span class="sxs-lookup"><span data-stu-id="c9aa0-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="c9aa0-122">Esse erro significa que o dispositivo não atende aos requisitos de implantação do AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="c9aa0-122">This error means the device doesn't meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="c9aa0-123">Os dispositivos têm de cumprir os seguintes requisitos:</span><span class="sxs-lookup"><span data-stu-id="c9aa0-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="c9aa0-124">Windows 10, versão 1703 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="c9aa0-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="c9aa0-125">Novos dispositivos que não passaram pela experiência do Windows fora da caixa.</span><span class="sxs-lookup"><span data-stu-id="c9aa0-125">New devices that haven't been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="c9aa0-126">Dispositivo não encontrado</span><span class="sxs-lookup"><span data-stu-id="c9aa0-126">Device not found</span></span>  <br/> |<span data-ttu-id="c9aa0-127">Esse erro significa que um ou mais dispositivos em seu arquivo CSV não estão registrados em sua organização.</span><span class="sxs-lookup"><span data-stu-id="c9aa0-127">This error means that one or more devices in your CSV file isn't registered to your organization.</span></span> <span data-ttu-id="c9aa0-128">Para corrigir isso, peça ajuda ao fornecedor de hardware.</span><span class="sxs-lookup"><span data-stu-id="c9aa0-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
