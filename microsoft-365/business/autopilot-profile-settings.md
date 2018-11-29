---
title: Sobre as definições do Perfil AutoPilot
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: overview
f1_keywords:
- ZTDProfileSettings
- O365E_ZTDProfileSettings
- BCS365_ZTDProfileSettings
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
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
ms.openlocfilehash: 5440286f1363780c87ab60514584c4addfeea0b2
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982248"
---
# <a name="about-autopilot-profile-settings"></a>Sobre as definições do Perfil AutoPilot

## <a name="autopilot-profile-settings"></a>Definições do perfil de piloto automático

Pode controlar como o Windows é instalado em dispositivos de utilizador, utilizando os perfis de piloto automático. Os perfis de contenham as seguintes definições.
  
 **Piloto automático funcionalidades predefinidas (obrigatórias) que são definidas automaticamente:**
  
|**Definição**|**Descrição**|
|:-----|:-----|
|Ignorar o registo de Cortana, OneDrive e OEM  <br/> |Ignora a instalação de aplicações do consumidor tal como Cortana e OneDrive pessoal. O dispositivo de utilizador pode instalar estes posterior, desde que ele ou ela é um administrador local no dispositivo. O registo de fabricante original é ignorado porque o dispositivo será gerido pelo Microsoft 365 Business.  <br/> |
|Iniciar sessão na experiência adquirida com a marca de empresa  <br/> |Se a empresa tiver uma [imagem corporativa adicionar empresa Office 365 Iniciar sessão na página](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), o utilizador do dispositivo irá obter essa experiência ao iniciar sessão no.  <br/> |
|MDM-inscrição automática com contas AAD configuradas.  <br/> |A identidade do utilizador será gerida pelo Azure Active directory e os utilizadores vão iniciar sessão no Windows e Office 365 com as respectivas credenciais de Microsoft 365 Business.  <br/> |
   
 **Definições opcionais:**
  
|**Definição**|**Descrição**|
|:-----|:-----|
|Ignorar definições de privacidade (desactivado por predefinição)  <br/> |Se esta opção é definida como **no**, o utilizador do dispositivo não verá o contrato de licença para o dispositivo e o Windows quando ele ou ela primeiro inicia sessão.  <br/> |
|Não permitir que o utilizador tornar-se o administrador local  <br/> |Se esta opção estiver definida para **activado**, o dispositivo de utilizador não poderá instalar quaisquer aplicações pessoais, tais como Cortana.  <br/> |
   
