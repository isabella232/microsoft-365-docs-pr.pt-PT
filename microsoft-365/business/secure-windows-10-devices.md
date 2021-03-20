---
title: Proteger dispositivos Windows 10
f1.keywords:
- CSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4WindowsConfig
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 21e5551f-fa35-4f13-9418-f80d668b6a2b
description: Saiba como configurar as definições da política do dispositivo predefinido que qualquer dispositivo Do Windows 10 receberá ao iniciar sessão na sua conta de trabalho ou escola.
ms.openlocfilehash: 85383b1e1d2f2af3fd49d4a0c56c5d99586d607d
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912616"
---
# <a name="secure-windows-10-devices"></a><span data-ttu-id="60948-103">Proteger dispositivos Windows 10</span><span class="sxs-lookup"><span data-stu-id="60948-103">Secure Windows 10 devices</span></span>

<span data-ttu-id="60948-104">Este artigo aplica-se ao Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="60948-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="60948-105">As definições que configurar aqui fazem parte da política de dispositivos predefinida para o Windows 10.</span><span class="sxs-lookup"><span data-stu-id="60948-105">The settings that you configure here are part of the default device policy for Windows 10.</span></span> <span data-ttu-id="60948-106">Todos os utilizadores que liguem um dispositivo Windows 10, incluindo dispositivos móveis e Computadores, ao iniciar sessão com a sua conta de trabalho receberão automaticamente estas definições.</span><span class="sxs-lookup"><span data-stu-id="60948-106">All users who connect a Windows 10 device, including mobile devices and PCs, by signing in with their work account will automatically receive these settings.</span></span> <span data-ttu-id="60948-107">Recomendamos que aceite a política predefinida durante a configuração e que adicione políticas destinadas a grupos de utilizadores específicos mais tarde.</span><span class="sxs-lookup"><span data-stu-id="60948-107">We recommend that you accept the default policy during setup and add policies later that target specific groups of users.</span></span>
  
## <a name="settings-to-secure-windows-10-devices"></a><span data-ttu-id="60948-108">Definições para proteger dispositivos Windows 10</span><span class="sxs-lookup"><span data-stu-id="60948-108">Settings to secure Windows 10 devices</span></span>

<span data-ttu-id="60948-p102">Por predefinição, todas as definições estão **Ativadas**. As seguintes definições estão disponíveis:</span><span class="sxs-lookup"><span data-stu-id="60948-p102">By default all settings are **On**. The following settings are available:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="60948-111">Definição</span><span class="sxs-lookup"><span data-stu-id="60948-111">Setting</span></span>  <br/> |<span data-ttu-id="60948-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="60948-112">Description</span></span>  <br/> |
|<span data-ttu-id="60948-113">Ajudar a proteger os PCs contra vírus e outras ameaças com o Antivírus do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="60948-113">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="60948-114">Exige que o Antivírus do Windows Defender esteja ativado para proteger os PCs contra os perigos que uma ligação à Internet envolve.</span><span class="sxs-lookup"><span data-stu-id="60948-114">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="60948-115">Ajudar a proteger os PCs contra ameaças baseadas na Web no Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="60948-115">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="60948-116">Ativa as definições no Microsoft Edge que ajudam a proteger os utilizadores contra transferências e sites maliciosos.</span><span class="sxs-lookup"><span data-stu-id="60948-116">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="60948-117">Ajudar a proteger ficheiros e pastas nos PCs contra acesso não autorizado com o BitLocker</span><span class="sxs-lookup"><span data-stu-id="60948-117">Help protect files and folders on PCs from unauthorized access with BitLocker</span></span>  <br/> |<span data-ttu-id="60948-118">O Bitlocker protege os dados ao encriptar os discos rígidos do computador e proteger contra exposição de dados em caso de roubo ou perda do computador.</span><span class="sxs-lookup"><span data-stu-id="60948-118">Bitlocker protects data by encrypting the computer hard drives and protect against data exposure if a computer is lost or stolen.</span></span> <span data-ttu-id="60948-119">Para mais informações, consulte [bitlocker FAQ](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions).</span><span class="sxs-lookup"><span data-stu-id="60948-119">For more information, see [Bitlocker FAQ](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions).</span></span>  <br/> |
|<span data-ttu-id="60948-120">Desligar o ecrã do dispositivo quando estiver inativo durante este período de tempo</span><span class="sxs-lookup"><span data-stu-id="60948-120">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="60948-p104">Garante que os dados da empresa são protegidos se um utilizador estiver inativo. É possível que um utilizador esteja a trabalhar num local público, como um café, e se afaste ou distraia por um momento, deixando o dispositivo vulnerável a olhares alheios. Esta definição permite-lhe controlar quanto tempo um utilizador pode estar inativo antes de o ecrã se desligar.</span><span class="sxs-lookup"><span data-stu-id="60948-p104">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
|