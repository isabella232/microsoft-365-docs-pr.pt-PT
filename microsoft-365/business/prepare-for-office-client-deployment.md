---
title: Preparar a implementação do cliente do Office pelo Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 10/31/2017
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Obter informações sobre como instalar as aplicações do Office de 32 bits para computadores Windows 10 e mantê-los actualizados automaticamente.
ms.openlocfilehash: c8e93746b89925d6b6a928a474fe5736e2834987
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32286663"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a>Preparar a implementação do cliente do Office pelo Microsoft 365 Business

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Preparar a instalação automática das aplicações do Office em computadores cliente

Pode utilizar o Microsoft 365 Business para instalar automaticamente as aplicações do Office de 32 bits em computadores com Windows 10 e mantê-las atualizadas.
  
Isto funciona melhor se o computador do utilizador final tiver o Windows 10 Business e:
  
- Não tiver aplicações de ambiente de trabalho do Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access e OneDrive).
    
    ou
    
- Tiver uma versão do Office Clique-e-Use instalada.
    
Para determinar se tem a versão Clique-e-Use do Office, em qualquer aplicação do Office, aceda a **Ficheiro** \> **Conta** ( **Conta do Office** no Outlook). Se vir as Atualizações do Office conforme apresentado na seguinte imagem, a instalação foi efetuada com a tecnologia Clique-e-Use. 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Quem irá beneficiar desta funcionalidade**
  
O utilizador final cujo PC:
  
- **Tem** uma licença de utilizador do Windows 10 Business, uma licença ativa do Microsoft 365 Business, a Atualização para Criativos do Windows 10 e está ligado ao Azure Active Directory. 
    
- **Não tem** aplicações do Office de 64 bits (por exemplo: Word, Excel, Powerpoint). Se for necessário ter aplicações do Office de 64 bits, esta funcionalidade não é uma boa opção pois não existe suporte para acionar uma versão Clique-e-Use de 64 bits do Office 2016 a partir da consola do administrador do Microsoft 365 Business. 
    
- **Não tem** quaisquer aplicações autónomas do Windows Installer (MSI) 2016 (por exemplo, o Visio ou Project). O Microsoft 365 Business atualiza o Office para a versão Clique-e-Use do Office 2016 e a mesma não funciona com as aplicações autónomas do Office 2016 MSI. 
    
A seguinte tabela indica detalhadamente que ação os utilizadores/administradores poderão ter de efetuar, dependendo do respetivo estado inicial, para realizar uma implementação com êxito da versão Clique-e-Use de 32 bits do Office a partir da consola do administrador do Microsoft 365 Business.
  
|**Estado inicial da instalação do Office**|**Ação a tomar antes da instalação do Office do Microsoft 365 Business**|**Estado final**|
|:-----|:-----|:-----|
|Nenhum conjunto de aplicações do Office instalado  <br/> |Nenhuma  <br/> |Office 2016 de 32 bits instalado com a tecnologia Clique-e-Use  <br/> |
|Versão Clique-e-Use de 32 bits do Office (2016 ou anterior) sem aplicações autónomas  <br/> |Nenhuma  <br/> |Atualizada para a versão Clique-e-Use de 32 bits mais recente do Office 2016, conforme necessário **\*** <br/> |
|Versão Clique-e-Use de 32 bits do Office e aplicações autónomas do Office Clique-e-Use de 32 ou 64 bits (por exemplo, o Visio ou Project)  <br/> |Nenhuma  <br/> |As aplicações autónomas não são afetadas. O conjunto de aplicações é atualizado para a versão Clique-e-Use de 32 bits do Office 2016  <br/> |
|Versão Clique-e-Use de 32 bits do Office e quaisquer aplicações autónomas do Office MSI de 32 ou 64 bits (exceto o 2016)  <br/> |Nenhuma  <br/> |As aplicações autónomas não são afetadas. O conjunto de aplicações é atualizado para a versão Clique-e-Use de 32 bits do Office 2016  <br/> ||||
|Qualquer versão Clique-e-Use de 64 bits do Office  <br/> |Desinstale as aplicações do Office de 64 bits se não houver problema em substitui-las pelas aplicações do Office de 32 bits  <br/> |Se as aplicações do Office de 64 bits forem removidas, a versão Clique-e-Use de 32 bits do Office 2016 é instalada  <br/> |
|Uma instalação MSI do Office 2016 com ou sem aplicações autónomas  <br/> |Desinstale o Office 2016 MSI.  <br/> |A versão Clique-e-Use de 32 bits do Office 2016 é instalada. As aplicações autónomas não são alteradas  <br/> |
|Instalação do Office 2013 MSI (ou anterior) e/ou aplicações autónomas do Office  <br/> |Nenhuma  <br/> |A versão Clique-e-Use de 32 bits do Office 2016 e a instalação do Office MSI já existente (e aplicações autónomas) existem em simultâneo  <br/> |
||||
   
 **(\*) Nota:** não é atualizada para a versão Clique-e-Use de 32 bits do Office 2016 devido a um erro desconhecido. A correção está em curso. 
  


