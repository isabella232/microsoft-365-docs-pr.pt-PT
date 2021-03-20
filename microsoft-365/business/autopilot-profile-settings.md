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
# <a name="about-autopilot-profile-settings"></a>Sobre as definições do Perfil AutoPilot

## <a name="autopilot-profile-settings"></a>Definições de perfil autoPilot

Pode utilizar perfis AutoPilot para controlar a instalação do Windows nos dispositivos do utilizador. Os perfis contêm as seguintes definições.
  
 **Funcionalidades predefinidas do Predefinido AutoPilot (necessárias) que são definidas automaticamente:**
  
|**Definição**|**Descrição**|
|:-----|:-----|
|Registos Skip Cortana, OneDrive e OEM  <br/> |Ignora a instalação de aplicativos de consumo como cortana e onedrive pessoal. O utilizador do dispositivo pode instalá-los mais tarde, desde que o utilizador seja um administrador local no dispositivo. O registo original do fabricante é ignorado porque o dispositivo será gerido pelo Microsoft 365 Business Premium.  <br/> |
|Assine experiência com a marca da sua empresa  <br/> |Se a sua empresa tiver uma [marca De adicionar a sua empresa à página Microsoft 365 Sign In,](../admin/setup/customize-sign-in-page.md)o utilizador do dispositivo terá essa experiência ao iniciar sessão.  <br/> |
|Inscrição automática do MDM com contas AAD configuradas.  <br/> |A identidade do utilizador será gerida pelo Azure Ative Directory, e os utilizadores iniciarão seducas no Windows e Microsoft 365 com as suas credenciais Microsoft 365 Business Premium.  <br/> |
   
 **Definições opcionais:**
  
|**Definição**|**Descrição**|
|:-----|:-----|
|Saltar as definições de privacidade (desligado por padrão)  <br/> |Se esta opção for definida para **On**, o utilizador do dispositivo não verá o contrato de licença do dispositivo e do Windows quando ele ou ela entrar pela primeira vez.  <br/> |
|Não permita que o utilizador se torne o administrador local  <br/> |Se esta opção for definida para **On**, o utilizador do dispositivo não poderá instalar nenhuma aplicação pessoal, como é o caso do Cortana.<br/> |
