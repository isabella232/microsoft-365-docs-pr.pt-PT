---
title: Sobre as definições do Perfil AutoPilot
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: Os perfis AutoPilot ajudam-no a controlar a Windows é instalada em dispositivos de utilizador. Os perfis contêm predefinições e opcionais, como ignorar Cortana instalação.
ms.openlocfilehash: 67ad6e92583d71207e2807657a7ad00261e1249291e2e6a7546f544ea924b394
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53896329"
---
# <a name="about-autopilot-profile-settings"></a>Sobre as definições do Perfil AutoPilot

## <a name="autopilot-profile-settings"></a>Definições de perfil AutoPilot

Pode utilizar os perfis AutoPilot para controlar a Windows é instalada em dispositivos de utilizador. Os perfis contêm as seguintes definições.
  
 **Funcionalidades predefinidas autoPilot (obrigatório) que são definidas automaticamente:**
  
|**Definição**|**Descrição**|
|:-----|:-----|
|Ignorar Cortana, OneDrive e registo do OEM  <br/> |Ignora a instalação de aplicações de consumidor, como a Cortana e as aplicações OneDrive. O utilizador do dispositivo pode instalá-los mais tarde, desde que seja um administrador local no dispositivo. O registo do fabricante original é ignorado porque o dispositivo será gerido pela Microsoft 365 Empresas Premium.  <br/> |
|Experiência de inscrever-se com a marca da sua empresa  <br/> |Se a sua empresa tiver uma página Adicionar a imagem pessoal da sua [empresa Microsoft 365](../admin/setup/customize-sign-in-page.md)Página de Inscrever-se, o utilizador do dispositivo terá essa experiência ao começar a trabalhar.  <br/> |
|Inscrição automática da MDM com contas AAD configuradas.  <br/> |A identidade do utilizador será gerida pelo Azure Active Directory e os utilizadores irão inscrever-se no Windows e Microsoft 365 com as respetivos Microsoft 365 Empresas Premium utilizadores.  <br/> |
   
 **Definições opcionais:**
  
|**Definição**|**Descrição**|
|:-----|:-----|
|Ignorar as definições de privacidade (Desarmado por predefinição)  <br/> |Se esta opção estiver definida para Ativado, o utilizador do dispositivo não verá o contrato de licença do dispositivo e Windows quando este entrar pela primeira vez.  <br/> |
|Não permitir que o utilizador se torne o administrador local  <br/> |Se esta opção estiver definida **para** Ativo, o utilizador do dispositivo não poderá instalar aplicações pessoais, como a aplicação Cortana.<br/> |
