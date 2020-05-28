---
title: Verificar definições de proteção de aplicações em PCs Windows 10
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
description: Saiba como verificar se o Microsoft 365 para definições de proteção de aplicações empresariais entrou em vigor nos dispositivos Windows 10 dos seus utilizadores.
ms.openlocfilehash: 39aee3bc811cb0090d58f9a282de7a8162c097b3
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403596"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>Valide as definições de proteção do dispositivo em PCs do Windows 10

## <a name="verify-that-windows-10-device-policies-are-set"></a>Verifique se as políticas do dispositivo Windows 10 estão definidas

Depois de configurar as políticas dos [dispositivos,](protection-settings-for-windows-10-pcs.md)pode demorar até algumas horas para que a política entre em vigor nos dispositivos dos utilizadores. Pode confirmar que as políticas produziram efeito ao analisar vários ecrãs de Definições do Windows nos dispositivos dos utilizadores. Uma vez que os utilizadores não conseguirão modificar as definições de Windows Update e Windows Defender Antivirus nos seus dispositivos Windows 10, muitas opções serão acinzentadas.
  
1. Vá às **opções** de reinício do Windows Update \> ** &amp; e** \> **Windows Update** \> **Restart options** confirme que todas as definições estão acinzentadas. 
    
    ![Todas as opções de Reinício estão cinzentas.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Vá a **Definições** \> **De &amp; segurança** \> As opções avançadas **do Windows Update** e \> **Advanced options** confirme que todas as definições estão acinzentadas. 
    
    ![As opções de atualizações do Windows Advanced estão todas cinzentas.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Vá a **Definições** De atualização De \> ** &amp; atualização** \> **As** \> **opções avançadas** do Windows \> **Escolha como as atualizações são entregues**.
    
    Confirme que pode ver a mensagem (em vermelho) de que algumas configurações são ocultadas ou geridas pela sua organização, e todas as opções estão cinzentas.
    
    ![Escolha como as atualizações são entregues a página indica que as definições são ocultadas ou geridas pela sua organização.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. Para abrir o Centro de Segurança do Windows Defender, vá a **Definições** \> **de &amp; segurança O** Windows \> **Defender** clique \> em **definições de** \> ** &amp; ** \> ** &amp; proteção**contra vírus do Centro de Segurança do Windows Defender . 
    
5. Verifique se todas as opções estão cinzentas. 
    
    ![As definições de proteção contra vírus e ameaças estão acinzentadas.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Tópicos Relacionados

[Microsoft 365 para documentação e recursos empresariais](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Começar com a Microsoft 365 para negócios](microsoft-365-business-overview.md)
  
[Gerir o Microsoft 365 para negócios](manage.md)
  
[Definir as configurações de dispositivos para PCs Windows 10](protection-settings-for-windows-10-pcs.md)
  

