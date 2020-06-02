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
ms.openlocfilehash: 03ae86861ddb0cb83cd39b7834f19e01bf3e99e2
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/01/2020
ms.locfileid: "44470633"
---
# <a name="secure-windows-10-devices"></a><span data-ttu-id="6d46a-103">Proteger dispositivos Windows 10</span><span class="sxs-lookup"><span data-stu-id="6d46a-103">Secure Windows 10 devices</span></span>

<span data-ttu-id="6d46a-104">Este artigo aplica-se ao Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="6d46a-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="6d46a-105">As definições que configurar aqui fazem parte da política de dispositivos predefinida para o Windows 10.</span><span class="sxs-lookup"><span data-stu-id="6d46a-105">The settings that you configure here are part of the default device policy for Windows 10.</span></span> <span data-ttu-id="6d46a-106">Todos os utilizadores que liguem um dispositivo Windows 10, incluindo dispositivos móveis e Computadores, ao iniciar sessão com a sua conta de trabalho receberão automaticamente estas definições.</span><span class="sxs-lookup"><span data-stu-id="6d46a-106">All users who connect a Windows 10 device, including mobile devices and PCs, by signing in with their work account will automatically receive these settings.</span></span> <span data-ttu-id="6d46a-107">Recomendamos que aceite a política predefinida durante a configuração e que adicione políticas destinadas a grupos de utilizadores específicos mais tarde.</span><span class="sxs-lookup"><span data-stu-id="6d46a-107">We recommend that you accept the default policy during setup and add policies later that target specific groups of users.</span></span>
  
## <a name="settings-to-secure-windows-10-devices"></a><span data-ttu-id="6d46a-108">Definições para proteger dispositivos Windows 10</span><span class="sxs-lookup"><span data-stu-id="6d46a-108">Settings to secure Windows 10 devices</span></span>

<span data-ttu-id="6d46a-p102">Por predefinição, todas as definições estão **Ativadas**. As seguintes definições estão disponíveis:</span><span class="sxs-lookup"><span data-stu-id="6d46a-p102">By default all settings are **On**. The following settings are available:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="6d46a-111">Definição</span><span class="sxs-lookup"><span data-stu-id="6d46a-111">Setting</span></span>  <br/> |<span data-ttu-id="6d46a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d46a-112">Description</span></span>  <br/> |
|<span data-ttu-id="6d46a-113">Ajudar a proteger os PCs contra vírus e outras ameaças com o Antivírus do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="6d46a-113">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="6d46a-114">Exige que o Antivírus do Windows Defender esteja ativado para proteger os PCs contra os perigos que uma ligação à Internet envolve.</span><span class="sxs-lookup"><span data-stu-id="6d46a-114">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="6d46a-115">Ajudar a proteger os PCs contra ameaças baseadas na Web no Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="6d46a-115">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="6d46a-116">Ativa as definições no Microsoft Edge que ajudam a proteger os utilizadores contra transferências e sites maliciosos.</span><span class="sxs-lookup"><span data-stu-id="6d46a-116">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="6d46a-117">Desligar o ecrã do dispositivo quando estiver inativo durante este período de tempo</span><span class="sxs-lookup"><span data-stu-id="6d46a-117">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="6d46a-p103">Garante que os dados da empresa são protegidos se um utilizador estiver inativo. É possível que um utilizador esteja a trabalhar num local público, como um café e se afaste ou distraia por um momento, deixando o dispositivo vulnerável a olhares alheios. Esta definição permite-lhe controlar quanto tempo um utilizador pode estar inativo antes de o ecrã se desligar.</span><span class="sxs-lookup"><span data-stu-id="6d46a-p103">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
|<span data-ttu-id="6d46a-121">Permitir que os utilizadores transfiram aplicações da Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="6d46a-121">Allow users to download apps from Microsoft Store</span></span>  <br/> |<span data-ttu-id="6d46a-p104">Permite que os utilizadores transfiram e instalem aplicações da Microsoft Store. As aplicações incluem tudo, desde jogos a ferramentas de produtividade, pelo que deixamos esta definição **Ativada**, embora a possa desativar para garantir uma segurança adicional.  </span><span class="sxs-lookup"><span data-stu-id="6d46a-p104">Lets users download and install apps from the Microsoft Store. Apps include everything from games to productivity tools, so we leave this setting **On**, but you can turn it off for extra security.  </span></span><br/> |
|<span data-ttu-id="6d46a-124">Permitir que os utilizadores acedam à Cortana</span><span class="sxs-lookup"><span data-stu-id="6d46a-124">Allow users to access Cortana</span></span>  <br/> |<span data-ttu-id="6d46a-125">A Cortana pode ser bastante útil!</span><span class="sxs-lookup"><span data-stu-id="6d46a-125">Cortana can be very helpful!</span></span> <span data-ttu-id="6d46a-126">Cortana pode ligar ou desligar as definições para si, dar instruções e certificar-se de que está a tempo para marcações, por isso mantemos esta definição **por** predefinição.</span><span class="sxs-lookup"><span data-stu-id="6d46a-126">Cortana can turn settings on or off for you, give directions, and make sure you're on time for appointments, so we keep this setting **On** by default.</span></span>  <br/> |
|<span data-ttu-id="6d46a-127">Permitir que os utilizadores recebam sugestões e anúncios da Microsoft acerca do Windows</span><span class="sxs-lookup"><span data-stu-id="6d46a-127">Allow users to receive Windows tips and advertisements from Microsoft</span></span>  <br/> |<span data-ttu-id="6d46a-128">As sugestões do Windows podem ser úteis e ajudar a orientar os utilizadores quando são lançadas novas versões.</span><span class="sxs-lookup"><span data-stu-id="6d46a-128">Windows tips can be handy and help orient users when new features are released.</span></span>  <br/> |
|<span data-ttu-id="6d46a-129">Manter os dispositivos Windows 10 atualizados automaticamente</span><span class="sxs-lookup"><span data-stu-id="6d46a-129">Keep Windows 10 devices up to date automatically</span></span>  <br/> |<span data-ttu-id="6d46a-130">Garante que os dispositivos Windows 10 recebem automaticamente as atualizações mais recentes.</span><span class="sxs-lookup"><span data-stu-id="6d46a-130">Makes sure that Windows 10 devices automatically receive the latest updates.</span></span>  <br/> |
   

