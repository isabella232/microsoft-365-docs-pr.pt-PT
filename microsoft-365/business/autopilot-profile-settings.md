---
title: Sobre as definições do Perfil AutoPilot
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
description: Os perfis AutoPilot ajudam a controlar como o Windows é instalado em dispositivos de usuário. Os perfis contêm configurações padrão e opcionais, como pular a instalação cortana.
ms.openlocfilehash: 912a24e3d458986a4bcf7dcf903f80211996aca2
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/14/2019
ms.locfileid: "38321791"
---
# <a name="about-autopilot-profile-settings"></a>Sobre as definições do Perfil AutoPilot

## <a name="autopilot-profile-settings"></a>Configurações de perfil do Piloto Automático

Você pode usar perfis AutoPilot para controlar como o Windows está instalado em dispositivos do usuário. Os perfis contêm as seguintes configurações.
  
 **Recursos padrão do Piloto Automático (necessários) que são definidos automaticamente:**
  
|**Definição**|**Descrição**|
|:-----|:-----|
|Pule o registro Cortana, OneDrive e OEM  <br/> |Ignora a instalação de aplicativos de consumo como cortana e onedrive pessoal. O usuário do dispositivo pode instalá-los mais tarde, desde que o usuário seja um administrador local no dispositivo. O registro original do fabricante é ignorado porque o dispositivo será gerenciado pela Microsoft 365 Business.  <br/> |
|Assine com experiência com a marca da empresa  <br/> |Se a sua empresa tiver uma [marca da empresa para a página de login do Office 365,](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a)o usuário do dispositivo terá essa experiência ao se inscrever.  <br/> |
|MDM auto-inscrição com contas AAD configuradas.  <br/> |A identidade do usuário será gerenciada pelo Diretório Ativo Do Azure, e os usuários entrarão no Windows e no Office 365 com suas credenciais de negócios microsoft 365.  <br/> |
   
 **Configurações opcionais:**
  
|**Definição**|**Descrição**|
|:-----|:-----|
|Evite as configurações de privacidade (desafinada por padrão)  <br/> |Se esta opção estiver definida para **on,** o usuário do dispositivo não verá o contrato de licença para o dispositivo e o Windows quando ele ou ela entrar pela primeira vez.  <br/> |
|Não permita que o usuário se torne o administrador local  <br/> |Se essa opção for definida para **on,** o usuário do dispositivo não será capaz de instalar aplicativos pessoais, como cortana.<br/> |
   
