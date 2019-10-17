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
description: Os perfis do AutoPilot ajudam você a controlar como o Windows é instalado em dispositivos de usuário. Os perfis contêm configurações padrão e opcionais, como ignorar a instalação da Cortana.
ms.openlocfilehash: eb0d9a95c796909d024db1d061aaeace7d07ed1b
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/17/2019
ms.locfileid: "37574584"
---
# <a name="about-autopilot-profile-settings"></a>Sobre as definições do Perfil AutoPilot

## <a name="autopilot-profile-settings"></a>Configurações do perfil do AutoPilot

Você pode controlar como o Windows é instalado em dispositivos de usuário usando os perfis do AutoPilot. Os perfis contêm as seguintes configurações.
  
 **Recursos padrão do AutoPilot (obrigatório) que são definidos automaticamente:**
  
|**Definição**|**Descrição**|
|:-----|:-----|
|Ignorar Cortana, OneDrive e registro de OEM  <br/> |Ignora a instalação de aplicativos de consumidor como Cortana e OneDrive pessoal. O usuário do dispositivo pode instalá-los mais tarde, desde que ele ou ela é um administrador local no dispositivo. O registro original do fabricante é ignorado porque o dispositivo será gerenciado pelo Microsoft 365 Business.  <br/> |
|Entre em experiência com a sua marca da empresa  <br/> |Se a sua empresa tiver uma [Adicionar a marca da sua empresa à página de início de sessão do Office 365](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), o utilizador do dispositivo receberá essa experiência quando iniciar sessão.  <br/> |
|Registro automático do MDM com contas AAD configuradas.  <br/> |A identidade do usuário será gerenciada pelo Active Directory do Azure e os usuários farão logon no Windows e no Office 365 com suas credenciais do Microsoft 365 Business.  <br/> |
   
 **Configurações opcionais:**
  
|**Definição**|**Descrição**|
|:-----|:-----|
|Ignorar configurações de privacidade (desativado por padrão)  <br/> |Se essa opção estiver definida como **ativado**, o usuário do dispositivo não verá o contrato de licença para o dispositivo e o Windows quando ele ou ela entrar pela primeira vez.  <br/> |
|Não permita que o usuário se torne o administrador local  <br/> |Se essa opção estiver definida como **ativado**, o usuário do dispositivo não poderá instalar nenhum aplicativo pessoal, como a Cortana.  <br/> |
   
