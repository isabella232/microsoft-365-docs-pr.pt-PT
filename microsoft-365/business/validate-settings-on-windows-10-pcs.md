---
title: Validar as definições de proteção de aplicações Windows 10 PCs
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
manager: scotv
audience: Admin
ms.topic: article
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Saiba como verificar se as Microsoft 365 de proteção de aplicações empresariais tomaram efeito nos dispositivos Windows 10 utilizadores.
ms.openlocfilehash: 0b896ae21139adcc425295f31de9232f65380d692a46bd1ef9f81d4516e0e9ec
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53861681"
---
# <a name="validate-device-protection-settings-for-windows-10-pcs"></a>Validar as definições de proteção de dispositivos Windows 10 PCs

## <a name="verify-that-windows-10-device-policies-are-set"></a>Verificar se as Windows 10 dispositivos estão definidas

Após [configurar as políticas de dispositivos,](protection-settings-for-windows-10-pcs.md)poderá demorar até algumas horas para que a política entre em vigor nos dispositivos dos utilizadores. Pode confirmar que as políticas foram em vigor ao ver vários ecrãs Windows Definições ecrãs nos dispositivos dos utilizadores. Uma vez que os utilizadores não poderão modificar as definições Windows Atualização Antivírus do Windows Defender dos respetivos dispositivos de Windows 10, muitas opções estarão a cinzento.
  
1. Vá para a **Definições** Opções de \> **&amp; Windows** Atualizar \>  \> **Reinício** e confirme que todas as definições estão a cinzento. 
    
    ![Todas as opções de Reinício estão a cinzento.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Vá para o **Definições** \> **&amp; Atualizar segurança** Windows Atualizar opções Avançadas e confirme que todas as \>  \>  definições estão a cinzento. 
    
    ![Windows As opções de atualizações avançadas estão todas a cinzento.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Vá para o **Definições** \> **Atualizar &amp; segurança Windows** Opções \> **de** \> **Atualização Avançadas** \> **Selecionar a forma como as atualizações são entregues**.
    
    Confirme que consegue ver a mensagem (a vermelho) de que algumas definições estão ocultas ou geridas pela sua organização e de que todas as opções estão desa cinzento.
    
    ![Selecionar a forma como as atualizações são entregues indica que as definições estão ocultas ou geridas pela sua organização.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. Para abrir o Centro de Windows Defender  de Segurança do Definições atualizar a segurança Windows Defender clique em Abrir Windows Defender definições de proteção contra vírus contra \> **&amp;** \>  \>  \> **&amp;** \> **&amp; ameaças** por thread do Centro de Segurança do Windows Defender . 
    
5. Verifique se todas as opções estão a cinzento. 
    
    ![As definições de proteção contra vírus e ameaças estão desa cinzento.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Tópicos Relacionados

[Microsoft 365 para recursos e documentação empresarial](./index.yml)
  
[Começar a trabalhar com o Microsoft 365 para empresas](microsoft-365-business-overview.md)
  
[Gerir Microsoft 365 para empresas](manage.md)
  
[Definir as configurações de dispositivos para PCs Windows 10](protection-settings-for-windows-10-pcs.md)
