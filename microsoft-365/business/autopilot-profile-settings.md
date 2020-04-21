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
ms.openlocfilehash: 5c2ec3f4c3e0ebc4ea545d11f819c897f414ad52
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/21/2020
ms.locfileid: "43627420"
---
# <a name="about-autopilot-profile-settings"></a>Sobre as definições do Perfil AutoPilot

## <a name="autopilot-profile-settings"></a>Definições de perfil AutoPilot

Pode utilizar perfis AutoPilot para controlar a forma como o Windows é instalado nos dispositivos do utilizador. Os perfis contêm as seguintes definições.
  
 **As funções de predefinição autoPilot (necessárias) que são definidas automaticamente:**
  
|**Definição**|**Descrição**|
|:-----|:-----|
|Registo skip Cortana, OneDrive e OEM  <br/> |Ignora a instalação de aplicações de consumo como cortana e oneDrive pessoal. O utilizador do dispositivo pode instalá-los mais tarde, desde que o utilizador seja um administrador local no dispositivo. O registo original do fabricante é ignorado porque o dispositivo será gerido pelo Microsoft 365 Business Premium.  <br/> |
|Inscreva-se em experiência com a marca da sua empresa  <br/> |Se a sua empresa tiver um [Add a sua marca de empresa na página Microsoft 365 Sign In](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), o utilizador do dispositivo terá essa experiência ao iniciar sessão.  <br/> |
|Mdm auto-inscrição com contas AAD configuradas.  <br/> |A identidade do utilizador será gerida pelo Azure Ative Directory, e os utilizadores irão iniciar sessão no Windows e Microsoft 365 com as suas credenciais Microsoft 365 Business Premium.  <br/> |
   
 **Configurações opcionais:**
  
|**Definição**|**Descrição**|
|:-----|:-----|
|Ignore as definições de privacidade (desligada por defeito)  <br/> |Se esta opção estiver definida para **O Início**, o utilizador do dispositivo não verá o contrato de licença para o dispositivo e Windows quando ele ou ela fizer a primeira inmissão.  <br/> |
|Não permita que o utilizador se torne o administrador local  <br/> |Se esta opção estiver definida para **O On,** o utilizador do dispositivo não poderá instalar quaisquer aplicações pessoais, como cortana.<br/> |
   
