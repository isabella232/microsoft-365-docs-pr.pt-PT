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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: Os perfis de ComputadorEs Automáticos ajudam-no a controlar a instalação do Windows nos dispositivos do utilizador. Os perfis contêm definições predefinidos e opcionais como saltar a instalação cortana.
ms.openlocfilehash: be10e0e1c8c96ce05aab8526d2010313662ed5f2
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913384"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="53d73-104">Sobre as definições do Perfil AutoPilot</span><span class="sxs-lookup"><span data-stu-id="53d73-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="53d73-105">Definições de perfil autoPilot</span><span class="sxs-lookup"><span data-stu-id="53d73-105">AutoPilot profile settings</span></span>

<span data-ttu-id="53d73-106">Pode utilizar perfis AutoPilot para controlar a instalação do Windows nos dispositivos do utilizador.</span><span class="sxs-lookup"><span data-stu-id="53d73-106">You can use AutoPilot profiles to control how Windows is installed on user devices.</span></span> <span data-ttu-id="53d73-107">Os perfis contêm as seguintes definições.</span><span class="sxs-lookup"><span data-stu-id="53d73-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="53d73-108">**Funcionalidades predefinidas do Predefinido AutoPilot (necessárias) que são definidas automaticamente:**</span><span class="sxs-lookup"><span data-stu-id="53d73-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="53d73-109">**Definição**</span><span class="sxs-lookup"><span data-stu-id="53d73-109">**Setting**</span></span>|<span data-ttu-id="53d73-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="53d73-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="53d73-111">Registos Skip Cortana, OneDrive e OEM</span><span class="sxs-lookup"><span data-stu-id="53d73-111">Skip Cortana, OneDrive, and OEM registration</span></span>  <br/> |<span data-ttu-id="53d73-112">Ignora a instalação de aplicativos de consumo como cortana e onedrive pessoal.</span><span class="sxs-lookup"><span data-stu-id="53d73-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="53d73-113">O utilizador do dispositivo pode instalá-los mais tarde, desde que o utilizador seja um administrador local no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="53d73-113">The device user can install these later as long as the user is a local admin on the device.</span></span> <span data-ttu-id="53d73-114">O registo original do fabricante é ignorado porque o dispositivo será gerido pelo Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="53d73-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="53d73-115">Assine experiência com a marca da sua empresa</span><span class="sxs-lookup"><span data-stu-id="53d73-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="53d73-116">Se a sua empresa tiver uma [marca De adicionar a sua empresa à página Microsoft 365 Sign In,](../admin/setup/customize-sign-in-page.md)o utilizador do dispositivo terá essa experiência ao iniciar sessão.</span><span class="sxs-lookup"><span data-stu-id="53d73-116">If your company has a [Add your company branding to Microsoft 365 Sign In page](../admin/setup/customize-sign-in-page.md), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="53d73-117">Inscrição automática do MDM com contas AAD configuradas.</span><span class="sxs-lookup"><span data-stu-id="53d73-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="53d73-118">A identidade do utilizador será gerida pelo Azure Ative Directory, e os utilizadores iniciarão seducas no Windows e Microsoft 365 com as suas credenciais Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="53d73-118">The user identity will be managed by Azure Active Directory, and users will sign in to Windows and Microsoft 365 with their Microsoft 365 Business Premium credentials.</span></span>  <br/> |
   
 <span data-ttu-id="53d73-119">**Definições opcionais:**</span><span class="sxs-lookup"><span data-stu-id="53d73-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="53d73-120">**Definição**</span><span class="sxs-lookup"><span data-stu-id="53d73-120">**Setting**</span></span>|<span data-ttu-id="53d73-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="53d73-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="53d73-122">Saltar as definições de privacidade (desligado por padrão)</span><span class="sxs-lookup"><span data-stu-id="53d73-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="53d73-123">Se esta opção for definida para **On**, o utilizador do dispositivo não verá o contrato de licença do dispositivo e do Windows quando ele ou ela entrar pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="53d73-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="53d73-124">Não permita que o utilizador se torne o administrador local</span><span class="sxs-lookup"><span data-stu-id="53d73-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="53d73-125">Se esta opção for definida para **On**, o utilizador do dispositivo não poderá instalar nenhuma aplicação pessoal, como é o caso do Cortana.</span><span class="sxs-lookup"><span data-stu-id="53d73-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span><br/> |
