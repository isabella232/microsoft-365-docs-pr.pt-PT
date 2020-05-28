---
title: Prepare-se para a implementação de clientes do Office pela Microsoft 365 para negócios
f1.keywords:
- CSH
ms.author: sirkkuw
author: Sirkkuw
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
description: Aprenda a instalar automaticamente as aplicações de 32 bits do Office nos computadores do Windows 10 e mantê-las atualizadas.
ms.openlocfilehash: 6f3a80be9729a3818607c0f42e2cc7ece66a07ee
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/27/2020
ms.locfileid: "44401328"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a>Prepare-se para a implementação de clientes do Office pela Microsoft 365 para negócios

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Preparar a instalação automática das aplicações do Office em computadores cliente

Pode utilizar o Microsoft 365 para as empresas instalarem automaticamente as aplicações do Office de 32 bits nos computadores do Windows 10 e mantê-las atualizadas com atualizações.
  
A instalação automática funciona melhor se o computador do utilizador final estiver no Windows 10 Business e:
  
- Não tiver aplicações de ambiente de trabalho do Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access e OneDrive).
    
    ou
    
- Tiver uma versão do Office Clique-e-Use instalada.
    
Para determinar se tem a versão Clique-e-Use do Office, em qualquer aplicação do Office, aceda a **Ficheiro** \> **Conta** ( **Conta do Office** no Outlook). Se vir **as Atualizações do Office** como mostrado na figura seguinte, então a instalação foi feita utilizando o Click-to-Run. 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Quem beneficia de ter esta funcionalidade**
  
O utilizador final cujo PC:
  
- **Possui** uma licença de utilizador do Windows 10 Business, um Microsoft 365 ativo para licença de negócio, Atualização de Criadores do Windows 10, e está acompanhado pelo Azure Ative Directory. 
    
- **Não tem** aplicações de 64 bits do Office (exemplo: Word, Excel, PowerPoint). Se forem necessárias aplicações de Office de 64 bits, então esta funcionalidade não é um bom ajuste porque não há suporte para desencadear uma versão click-to-Run de 64 bits de 2016 do Office a partir da consola de administração de negócios. 
    
- **Não tem** quaisquer aplicações autónomas do Windows Installer (MSI) 2016 (por exemplo, o Visio ou Project). O Microsoft 365 para atualizações de negócios Office para a versão Click-to-Run do Office 2016 e que não funciona com aplicações autónomas do Office 2016 MSI. 
    
A tabela que se segue mostra que medidas os utilizadores/administradores finais podem ter de tomar, dependendo do seu estado inicial, para ter uma versão bem sucedida de 32 bits click-to-Run da implementação do Office a partir da Microsoft 365 para a consola de administração de empresas.
  
|**Estado inicial da instalação do Office**|**Medidas a tomar antes da Microsoft 365 para instalação de business Office**|**Estado final**|
|:-----|:-----|:-----|
|Nenhum conjunto de aplicações do Office instalado  <br/> |Nenhum  <br/> |Office 2016 32-bit é instalado usando Click-to-Run  <br/> |
|Versão Clique-e-Use de 32 bits do Office (2016 ou anterior) sem aplicações autónomas  <br/> |Nenhum  <br/> |Atualizada para a versão Clique-e-Use de 32 bits mais recente do Office 2016, conforme necessário **\*** <br/> |
|Já existente, versão de 32 bits do Office e do Click-to-Run 32-bit ou 64 bits de aplicações autónomas do Office (por exemplo, Visio, Project)  <br/> |Nenhum  <br/> |As aplicações autónomas não são afetadas. O conjunto de aplicações é atualizado para a versão Clique-e-Use de 32 bits do Office 2016  <br/> |
|Versão Clique-e-Use de 32 bits do Office e quaisquer aplicações autónomas do Office MSI de 32 ou 64 bits (exceto o 2016)  <br/> |Nenhum  <br/> |As aplicações autónomas não são afetadas. O conjunto de aplicações é atualizado para a versão Clique-e-Use de 32 bits do Office 2016  <br/> ||||
|Qualquer versão Clique-e-Use de 64 bits do Office  <br/> |Desinstale as aplicações do Office de 64 bits, se não houver problema em substituí-las por aplicações de 32 bits do Office  <br/> |Se as aplicações do Office de 64 bits forem removidas, a versão Clique-e-Use de 32 bits do Office 2016 é instalada  <br/> |
|Uma instalação MSI do Office 2016 com ou sem aplicações autónomas  <br/> |Desinstale o Office 2016 MSI.  <br/> |A versão Clique-e-Use de 32 bits do Office 2016 é instalada. As aplicações autónomas não são alteradas  <br/> |
|Instalação do Office 2013 MSI (ou anterior) e/ou aplicações autónomas do Office  <br/> |Nenhuma  <br/> |A versão Clique-e-Use de 32 bits do Office 2016 e a instalação do Office MSI já existente (e aplicações autónomas) existem em simultâneo  <br/> |
||||
   
 **(\*) Nota:** não é atualizada para a versão Clique-e-Use de 32 bits do Office 2016 devido a um erro desconhecido. Está em curso uma correção. 
  
