---
title: Prepare-se para implementação de clientes do Office pela Microsoft 365 para negócios
f1.keywords:
- CSH
ms.author: efrene
author: efrene
manager: scotv
ms.date: 10/31/2017
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Saiba como instalar automaticamente as aplicações do Office de 32 bits nos computadores Windows 10 e mantê-las atualizadas.
ms.openlocfilehash: 868d06fadfef0f55b41131b7fdfbb368b9128405
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580060"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a>Prepare-se para implementação de clientes do Office pela Microsoft 365 para negócios

Este artigo aplica-se ao Microsoft 365 Business Premium.

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Preparar a instalação automática das aplicações do Office em computadores cliente

Pode utilizar o Microsoft 365 Business Premium para instalar automaticamente as aplicações do Office de 32 bits nos computadores Windows 10 e mantê-las atualizadas com atualizações.
  
A instalação automática funciona melhor se o computador do utilizador final estiver no Windows 10 Business e:
  
- Não tiver aplicações de ambiente de trabalho do Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access e OneDrive).
    
    ou
    
- Tiver uma versão do Office Clique-e-Use instalada.
    
Para determinar se tem a versão Clique-e-Use do Office, em qualquer aplicação do Office, aceda a **Ficheiro** \> **Conta** ( **Conta do Office** no Outlook). Se vir **atualizações do Office** como mostrado na figura seguinte, a instalação foi feita utilizando o Click-to-Run. 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Quem beneficia de ter esta funcionalidade**
  
O utilizador final cujo PC:
  
- **Possui**  uma licença de utilizador do Windows 10 Business, um Microsoft 365 ativo para licença de negócio, Windows 10 Creators Update, e junta-se ao Azure Ative Directory. 
    
- **Não tem** aplicações de Escritório de 64 bits (exemplo: Word, Excel, PowerPoint). Se forem necessárias aplicações do Office de 64 bits, então esta funcionalidade não é um bom ajuste porque não há suporte para desencadear uma versão click-to-run de 64 bits do Office a partir da Microsoft 365 para a consola de administração de negócios. 
    
- **Não tem** quaisquer aplicações autónomas do Windows Installer (MSI) 2016 (por exemplo, o Visio ou Project). Microsoft 365 para atualizações de negócios Office para a versão Click-to-Run do Office 2016 e que não funciona com aplicações autónomas do Office 2016 MSI. 
    
A tabela que se segue mostra que ação os utilizadores/administradores finais podem ter de tomar, dependendo do seu estado inicial, para terem uma versão clic-to-run de 32 bits bem sucedida da implementação do Microsoft 365 para a consola de administração de negócios.
  
|**Estado inicial da instalação do Office**|**Medidas a tomar antes da instalação do Microsoft 365 para o Business Office**|**Estado final**|
|:-----|:-----|:-----|
|Nenhum conjunto de aplicações do Office instalado  <br/> |Nenhuma  <br/> |Office 2016 32-bit é instalado usando Click-to-Run  <br/> |
|Versão Clique-e-Use de 32 bits do Office (2016 ou anterior) sem aplicações autónomas  <br/> |Nenhuma  <br/> |Atualizada para a versão Clique-e-Use de 32 bits mais recente do Office 2016, conforme necessário **\*** <br/> |
|Versão de 32 bits do Office e click-to-run de 32 bits ou 64 bits de escritório autónomo (por exemplo, Visio, Projeto)  <br/> |Nenhum  <br/> |Aplicativos autónomos não são afetados. O conjunto de aplicações é atualizado para a versão Clique-e-Use de 32 bits do Office 2016  <br/> |
|Versão Clique-e-Use de 32 bits do Office e quaisquer aplicações autónomas do Office MSI de 32 ou 64 bits (exceto o 2016)  <br/> |Nenhuma  <br/> |Aplicativos autónomos não são afetados. O conjunto de aplicações é atualizado para a versão Clique-e-Use de 32 bits do Office 2016  <br/> ||||
|Qualquer versão Clique-e-Use de 64 bits do Office  <br/> |Desinstale as aplicações do Office de 64 bits, se não houver problema em substituí-las por aplicações de 32 bits do Office  <br/> |Se as aplicações do Office de 64 bits forem removidas, a versão Clique-e-Use de 32 bits do Office 2016 é instalada  <br/> |
|Uma instalação MSI do Office 2016 com ou sem aplicações autónomas  <br/> |Desinstale o Office 2016 MSI.  <br/> |A versão Clique-e-Use de 32 bits do Office 2016 é instalada. As aplicações autónomas não são alteradas  <br/> |
|Instalação do Office 2013 MSI (ou anterior) e/ou aplicações autónomas do Office  <br/> |Nenhuma  <br/> |A versão Clique-e-Use de 32 bits do Office 2016 e a instalação do Office MSI já existente (e aplicações autónomas) existem em simultâneo  <br/> |
||||
   
 **(\*) Nota:** não é atualizada para a versão Clique-e-Use de 32 bits do Office 2016 devido a um erro desconhecido. Está em curso uma correção. 
  
