---
title: Verificar definições de proteção de aplicações em PCs Windows 10
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
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Saiba como validar as configurações de proteção de aplicativos do Microsoft 365 Business em dispositivos Windows 10.
ms.openlocfilehash: b8793ab7f77bbc7f608f237e2455f6fd12c3bb26
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/19/2019
ms.locfileid: "38721806"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>Validar as configurações de proteção do dispositivo em PCs do Windows 10

## <a name="verify-that-windows-10-device-policies-are-set"></a>Verifique se as políticas do dispositivo Windows 10 estão definidas

Depois de configurar as políticas de [dispositivos,](protection-settings-for-windows-10-pcs.md)pode levar até algumas horas para que a política entre em vigor nos dispositivos dos usuários. Você pode confirmar que as políticas efeitoram olhando várias telas de configurações do Windows nos dispositivos dos usuários. Como os usuários não poderão modificar as configurações do Windows Update e do Windows Defender Antivirus em seus dispositivos Windows 10, muitas opções serão acinzentadas.
  
1. Acesse **as opções** \> de \> **reinício** de atualização de segurança do **Windows de** \> ** &amp; atualização** de configurações e confirme que todas as configurações estão acinzentadas. 
    
    ![Todas as opções de reinício são acinzentadas.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Acesse **configurações** \> ** &amp; atualizaas** de **opções avançadas** de \> **atualização** \> do Windows e confirme que todas as configurações estão acinzentadas. 
    
    ![As opções de atualizações do Windows Advanced estão todas acinzentadas.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Acesse **configurações** \> ** &amp; atualizando** **opções** \> avançadas de **atualização** \> de windows \> **atualização escolha como as atualizações são entregues.**
    
    Confirme que você pode ver a mensagem (em vermelho) que algumas configurações são ocultas ou gerenciadas por sua organização, e todas as opções são acinzentadas.
    
    ![Escolha como as atualizações são entregues, a página indica que as configurações estão ocultas ou gerenciadas por sua organização.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. Para abrir o Windows Defender Security Center, acesse **Configurações** \> **atualizações de &amp; segurança** \> **do Windows Defender** \> clique em **configurações &amp; **de proteção contra \> **vírus &amp; ** do Open Defender Security **Center** \> Virus. 
    
5. Verifique se todas as opções estão acinzentadas. 
    
    ![As configurações de proteção contra vírus e ameaças são acinzentadas.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Tópicos relacionados

[Recursos e documentação do Microsoft 365 Business](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Introdução ao Microsoft 365 Business](microsoft-365-business-overview.md)
  
[Gerir o Microsoft 365 Business](manage.md)
  
[Definir as configurações de dispositivos para PCs Windows 10](protection-settings-for-windows-10-pcs.md)
  

