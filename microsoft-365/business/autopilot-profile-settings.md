---
title: Sobre as definições do Perfil AutoPilot
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: conceptual
f1_keywords:
- ZTDProfileSettings
- O365E_ZTDProfileSettings
- BCS365_ZTDProfileSettings
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
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: Perfis de piloto automático ajudam-na controlar como o Windows é instalado em dispositivos de utilizador. Os perfis contêm predefinido e definições opcionais como ignorar a instalação de Cortana.
ms.openlocfilehash: d43a15e5f3dc83596b5c23dd0ceb416b24810298
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32276947"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="83e84-104">Sobre as definições do Perfil AutoPilot</span><span class="sxs-lookup"><span data-stu-id="83e84-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="83e84-105">Definições do perfil de piloto automático</span><span class="sxs-lookup"><span data-stu-id="83e84-105">AutoPilot profile settings</span></span>

<span data-ttu-id="83e84-106">Pode controlar como o Windows é instalado em dispositivos de utilizador, utilizando os perfis de piloto automático.</span><span class="sxs-lookup"><span data-stu-id="83e84-106">You can control how Windows gets installed on user devices by using the AutoPilot profiles.</span></span> <span data-ttu-id="83e84-107">Os perfis de contenham as seguintes definições.</span><span class="sxs-lookup"><span data-stu-id="83e84-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="83e84-108">**Piloto automático funcionalidades predefinidas (obrigatórias) que são definidas automaticamente:**</span><span class="sxs-lookup"><span data-stu-id="83e84-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="83e84-109">**Definição**</span><span class="sxs-lookup"><span data-stu-id="83e84-109">**Setting**</span></span>|<span data-ttu-id="83e84-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="83e84-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="83e84-111">Ignorar o registo de Cortana, OneDrive e OEM</span><span class="sxs-lookup"><span data-stu-id="83e84-111">Skip Cortana, OneDrive and OEM registration</span></span>  <br/> |<span data-ttu-id="83e84-112">Ignora a instalação de aplicações do consumidor tal como Cortana e OneDrive pessoal.</span><span class="sxs-lookup"><span data-stu-id="83e84-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="83e84-113">O dispositivo de utilizador pode instalar estes posterior, desde que ele ou ela é um administrador local no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="83e84-113">The device user can install these later as long as he or she is a local admin on the device.</span></span> <span data-ttu-id="83e84-114">O registo de fabricante original é ignorado porque o dispositivo será gerido pelo Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="83e84-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="83e84-115">Iniciar sessão na experiência adquirida com a marca de empresa</span><span class="sxs-lookup"><span data-stu-id="83e84-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="83e84-116">Se a empresa tiver uma [imagem corporativa adicionar empresa Office 365 Iniciar sessão na página](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), o utilizador do dispositivo irá obter essa experiência ao iniciar sessão no.</span><span class="sxs-lookup"><span data-stu-id="83e84-116">If your company has a [Add your company branding to Office 365 Sign In page](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="83e84-117">MDM-inscrição automática com contas AAD configuradas.</span><span class="sxs-lookup"><span data-stu-id="83e84-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="83e84-118">A identidade do utilizador será gerida pelo Azure Active directory e os utilizadores vão iniciar sessão no Windows e Office 365 com as respectivas credenciais de Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="83e84-118">The user identity will be managed by Azure Active directory, and the users will sign into Windows and Office 365 with their Microsoft 365 Business credentials.</span></span>  <br/> |
   
 <span data-ttu-id="83e84-119">**Definições opcionais:**</span><span class="sxs-lookup"><span data-stu-id="83e84-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="83e84-120">**Definição**</span><span class="sxs-lookup"><span data-stu-id="83e84-120">**Setting**</span></span>|<span data-ttu-id="83e84-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="83e84-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="83e84-122">Ignorar definições de privacidade (desactivado por predefinição)</span><span class="sxs-lookup"><span data-stu-id="83e84-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="83e84-123">Se esta opção é definida como **no**, o utilizador do dispositivo não verá o contrato de licença para o dispositivo e o Windows quando ele ou ela primeiro inicia sessão.</span><span class="sxs-lookup"><span data-stu-id="83e84-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="83e84-124">Não permitir que o utilizador tornar-se o administrador local</span><span class="sxs-lookup"><span data-stu-id="83e84-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="83e84-125">Se esta opção estiver definida para **activado**, o dispositivo de utilizador não poderá instalar quaisquer aplicações pessoais, tais como Cortana.</span><span class="sxs-lookup"><span data-stu-id="83e84-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span>  <br/> |
   
