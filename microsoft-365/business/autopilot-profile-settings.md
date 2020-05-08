---
title: Sobre as definições do Perfil AutoPilot
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: Os perfis AutoPilot ajudam-no a controlar a forma como o Windows é instalado nos dispositivos do utilizador. Os perfis contêm definições predefinidas e opcionais, como saltar a instalação cortana.
ms.openlocfilehash: 0c706d12ba262856ff40ea3bee57c64234fd77f7
ms.sourcegitcommit: 46644f9778bc70ab6d62783e0a1e60ba2eccc27f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/08/2020
ms.locfileid: "44165847"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="6b4fa-104">Sobre as definições do Perfil AutoPilot</span><span class="sxs-lookup"><span data-stu-id="6b4fa-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="6b4fa-105">Definições de perfil AutoPilot</span><span class="sxs-lookup"><span data-stu-id="6b4fa-105">AutoPilot profile settings</span></span>

<span data-ttu-id="6b4fa-106">Pode utilizar perfis AutoPilot para controlar a forma como o Windows é instalado nos dispositivos do utilizador.</span><span class="sxs-lookup"><span data-stu-id="6b4fa-106">You can use AutoPilot profiles to control how Windows is installed on user devices.</span></span> <span data-ttu-id="6b4fa-107">Os perfis contêm as seguintes definições.</span><span class="sxs-lookup"><span data-stu-id="6b4fa-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="6b4fa-108">**As funções de predefinição autoPilot (necessárias) que são definidas automaticamente:**</span><span class="sxs-lookup"><span data-stu-id="6b4fa-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="6b4fa-109">**Definição**</span><span class="sxs-lookup"><span data-stu-id="6b4fa-109">**Setting**</span></span>|<span data-ttu-id="6b4fa-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6b4fa-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6b4fa-111">Registo skip Cortana, OneDrive e OEM</span><span class="sxs-lookup"><span data-stu-id="6b4fa-111">Skip Cortana, OneDrive, and OEM registration</span></span>  <br/> |<span data-ttu-id="6b4fa-112">Ignora a instalação de aplicações de consumo como cortana e oneDrive pessoal.</span><span class="sxs-lookup"><span data-stu-id="6b4fa-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="6b4fa-113">O utilizador do dispositivo pode instalá-los mais tarde, desde que o utilizador seja um administrador local no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6b4fa-113">The device user can install these later as long as the user is a local admin on the device.</span></span> <span data-ttu-id="6b4fa-114">O registo original do fabricante é ignorado porque o dispositivo será gerido pelo Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="6b4fa-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="6b4fa-115">Inscreva-se em experiência com a marca da sua empresa</span><span class="sxs-lookup"><span data-stu-id="6b4fa-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="6b4fa-116">Se a sua empresa tiver um [Add a sua marca de empresa na página Microsoft 365 Sign In](https://docs.microsoft.com/microsoft-365/admin/setup/customize-sign-in-page), o utilizador do dispositivo terá essa experiência ao iniciar sessão.</span><span class="sxs-lookup"><span data-stu-id="6b4fa-116">If your company has a [Add your company branding to Microsoft 365 Sign In page](https://docs.microsoft.com/microsoft-365/admin/setup/customize-sign-in-page), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="6b4fa-117">Mdm auto-inscrição com contas AAD configuradas.</span><span class="sxs-lookup"><span data-stu-id="6b4fa-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="6b4fa-118">A identidade do utilizador será gerida pelo Azure Ative Directory, e os utilizadores irão iniciar sessão no Windows e Microsoft 365 com as suas credenciais Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="6b4fa-118">The user identity will be managed by Azure Active Directory, and users will sign in to Windows and Microsoft 365 with their Microsoft 365 Business Premium credentials.</span></span>  <br/> |
   
 <span data-ttu-id="6b4fa-119">**Configurações opcionais:**</span><span class="sxs-lookup"><span data-stu-id="6b4fa-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="6b4fa-120">**Definição**</span><span class="sxs-lookup"><span data-stu-id="6b4fa-120">**Setting**</span></span>|<span data-ttu-id="6b4fa-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6b4fa-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6b4fa-122">Ignore as definições de privacidade (desligada por defeito)</span><span class="sxs-lookup"><span data-stu-id="6b4fa-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="6b4fa-123">Se esta opção estiver definida para **O Início**, o utilizador do dispositivo não verá o contrato de licença para o dispositivo e Windows quando ele ou ela fizer a primeira inmissão.</span><span class="sxs-lookup"><span data-stu-id="6b4fa-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="6b4fa-124">Não permita que o utilizador se torne o administrador local</span><span class="sxs-lookup"><span data-stu-id="6b4fa-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="6b4fa-125">Se esta opção estiver definida para **O On,** o utilizador do dispositivo não poderá instalar quaisquer aplicações pessoais, como cortana.</span><span class="sxs-lookup"><span data-stu-id="6b4fa-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span><br/> |
   
