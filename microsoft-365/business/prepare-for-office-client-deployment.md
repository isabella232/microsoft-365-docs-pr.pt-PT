---
title: Preparar a implementação do cliente do Office pelo Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Saiba como instalar automaticamente os aplicativos do Office de 32 bits nos computadores do Windows 10 e mantê-los atualizados.
ms.openlocfilehash: 09857ddeb28e953da07979045a65f6b91925aeaf
ms.sourcegitcommit: 2c2248b03f7753d64490f2f7e56ec644a235b65a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/15/2019
ms.locfileid: "38640775"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a>Preparar a implementação do cliente do Office pelo Microsoft 365 Business

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Preparar a instalação automática das aplicações do Office em computadores cliente

Você pode usar o Microsoft 365 Business para instalar automaticamente os aplicativos do Office de 32 bits em computadores Windows 10 e mantê-los atualizados com atualizações.
  
A instalação automática funciona melhor se o computador do usuário final estiver no Windows 10 Business e:
  
- Não tiver aplicações de ambiente de trabalho do Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access e OneDrive).
    
    ou
    
- Tiver uma versão do Office Clique-e-Use instalada.
    
Para determinar se tem a versão Clique-e-Use do Office, em qualquer aplicação do Office, aceda a **Ficheiro** \> **Conta** ( **Conta do Office** no Outlook). Se você vir **atualizações do escritório** como mostrado na figura seguinte, então a instalação foi feita usando Clique para Executar. 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Quem se beneficia de ter esse recurso**
  
O utilizador final cujo PC:
  
- **Tem** uma licença de utilizador do Windows 10 Business, uma licença ativa do Microsoft 365 Business, a Atualização para Criativos do Windows 10 e está ligado ao Azure Active Directory. 
    
- **Não tem** aplicativos do Office de 64 bits (exemplo: Word, Excel, PowerPoint). Se são necessários aplicativos do Office de 64 bits, esse recurso não é um bom ajuste porque não há suporte para acionar uma versão clique para execução de 64 bits 2016 do Office do console de administração Microsoft 365 Business. 
    
- **Não tem** quaisquer aplicações autónomas do Windows Installer (MSI) 2016 (por exemplo, o Visio ou Project). O Microsoft 365 Business atualiza o Office para a versão Click-to-Run do Office 2016 e isso não funciona com aplicativos autônomos do Office 2016 MSI. 
    
A tabela a seguir mostra que ação os usuários/administradores finais podem precisar tomar, dependendo de seu estado de início, para ter uma versão clique-a-run bem-sucedida de 32 bits da implantação do Office do console de administração Microsoft 365 Business.
  
|**Estado inicial da instalação do Office**|**Ação a tomar antes da instalação do Office do Microsoft 365 Business**|**Estado final**|
|:-----|:-----|:-----|
|Nenhum conjunto de aplicações do Office instalado  <br/> |Nenhum  <br/> |O Office 2016 de 32 bits é instalado usando clique para execução  <br/> |
|Versão Clique-e-Use de 32 bits do Office (2016 ou anterior) sem aplicações autónomas  <br/> |Nenhum  <br/> |Atualizada para a versão Clique-e-Use de 32 bits mais recente do Office 2016, conforme necessário **\*** <br/> |
|Versão existente de 32 bits do Office e aplicativos autônomos de 32 bits do Office e Click-to-Run de 32 bits ou 64 bits (por exemplo, Visio, Projeto)  <br/> |Nenhum  <br/> |Aplicativos autônomos não são afetados. O conjunto de aplicações é atualizado para a versão Clique-e-Use de 32 bits do Office 2016  <br/> |
|Versão Clique-e-Use de 32 bits do Office e quaisquer aplicações autónomas do Office MSI de 32 ou 64 bits (exceto o 2016)  <br/> |Nenhum  <br/> |Aplicativos autônomos não são afetados. O conjunto de aplicações é atualizado para a versão Clique-e-Use de 32 bits do Office 2016  <br/> ||||
|Qualquer versão Clique-e-Use de 64 bits do Office  <br/> |Desinstale os aplicativos do Office de 64 bits, se não houver problema em substituí-los por aplicativos do Office de 32 bits  <br/> |Se as aplicações do Office de 64 bits forem removidas, a versão Clique-e-Use de 32 bits do Office 2016 é instalada  <br/> |
|Uma instalação MSI do Office 2016 com ou sem aplicações autónomas  <br/> |Desinstale o Office 2016 MSI.  <br/> |A versão Clique-e-Use de 32 bits do Office 2016 é instalada. As aplicações autónomas não são alteradas  <br/> |
|Instalação do Office 2013 MSI (ou anterior) e/ou aplicações autónomas do Office  <br/> |Nenhuma  <br/> |A versão Clique-e-Use de 32 bits do Office 2016 e a instalação do Office MSI já existente (e aplicações autónomas) existem em simultâneo  <br/> |
||||
   
 **(\*) Nota:** não é atualizada para a versão Clique-e-Use de 32 bits do Office 2016 devido a um erro desconhecido. Uma correção está em andamento. 
  