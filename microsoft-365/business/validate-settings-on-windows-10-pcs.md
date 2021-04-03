---
title: Verificar definições de proteção de aplicações em PCs Windows 10
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
description: Saiba como verificar se o Microsoft 365 para as definições de proteção de aplicações empresariais entrou em vigor nos dispositivos windows 10 dos seus utilizadores.
ms.openlocfilehash: fcb463fd98f692f7d4802689e0c03fe4e3e648a1
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579848"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>Validar as definições de proteção do dispositivo nos PCs do Windows 10

## <a name="verify-that-windows-10-device-policies-are-set"></a>Verifique se as políticas de dispositivos do Windows 10 estão definidas

Depois de [configurar as políticas dos dispositivos,](protection-settings-for-windows-10-pcs.md)pode demorar até algumas horas para que a política produza efeitos nos dispositivos dos utilizadores. Pode confirmar que as políticas produziram efeito através da localização de vários ecrãs do Windows Settings nos dispositivos dos utilizadores. Uma vez que os utilizadores não poderão modificar as definições de Antivírus do Windows Update e Do Windows Defender nos seus dispositivos Windows 10, muitas opções serão acinzentadas.
  
1. Vá a **Definições** \> **Atualizar opções &amp; de** \> **arranque do Windows Update** e \>  confirme que todas as definições estão acinzentadas. 
    
    ![Todas as opções restart estão acinzentadas.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Vá a **Definições** \> **Atualizar &amp; opções** avançadas do \> **Windows Update** e \>  confirme que todas as definições estão acinzentadas. 
    
    ![As opções de atualizações avançadas do Windows estão todas acinzentadas.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Ir a **Definições** \> **Atualizar &amp; Opções** \> avançadas **de atualização do Windows Update** Escolha a forma como as \>  \> **atualizações são entregues**.
    
    Confirme que pode ver a mensagem (a vermelho) de que algumas definições são ocultadas ou geridas pela sua organização, e todas as opções estão acinzentadas.
    
    ![Escolha como as atualizações são entregues página indica que as definições são ocultadas ou geridas pela sua organização.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. Para abrir o Centro de Segurança do Windows Defender, vá a **Definições** \> **Atualizar &amp; Segurança** \> **Windows Defender** clique em Abrir as \> definições de proteção contra vírus **do sistema** de \> **&amp; proteção contra vírus** do Windows Defender \> **&amp;**. 
    
5. Verifique se todas as opções estão acinzentadas. 
    
    ![As definições de proteção contra vírus e ameaças estão acinzentadas.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Tópicos Relacionados

[Microsoft 365 para documentação e recursos de negócios](./index.yml)
  
[Começa com a Microsoft 365 para negócios](microsoft-365-business-overview.md)
  
[Gerir a Microsoft 365 para negócios](manage.md)
  
[Definir as configurações de dispositivos para PCs Windows 10](protection-settings-for-windows-10-pcs.md)
