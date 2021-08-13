---
title: Preparar para Office de cliente por parte do Microsoft 365 para empresas
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
description: Saiba como instalar automaticamente as aplicações Office de 32 bits em Windows 10 computadores e mantê-las atualizadas.
ms.openlocfilehash: 134d5f2918e3f28c2025b282b9ae0325b64fe0474ae8123d0637bb43c4730c55
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53803570"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a>Preparar para Office de cliente por parte do Microsoft 365 para empresas

Este artigo aplica-se a Microsoft 365 Empresas Premium.

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Preparar a instalação automática das aplicações do Office em computadores cliente

Pode utilizar o Microsoft 365 Empresas Premium para instalar automaticamente as aplicações de versão de Office de 32 bits em Windows 10 computadores e mantê-las atualizadas.
  
A instalação automática funciona melhor se o computador do utilizador final estiver no Windows 10 Business e:
  
- Não tiver aplicações de ambiente de trabalho do Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access e OneDrive).
    
    ou
    
- Tiver uma versão do Office Clique-e-Use instalada.
    
Para determinar se tem a versão Clique-e-Use do Office, em qualquer aplicação do Office, aceda a **Ficheiro** \> **Conta** ( **Conta do Office** no Outlook). Se vir **Atualizações Office conforme** apresentado na seguinte imagem, a instalação foi e feita com a versão Clique-e-Use. 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Quem vantagens de ter esta funcionalidade**
  
O utilizador final cujo PC:
  
- **Tem** uma licença Windows 10 Business de utilizador, uma licença do Microsoft 365 para empresas, Atualização para Criativos do Windows 10 e está associado a Azure Active Directory. 
    
- **Não tem aplicações** de Office de 64 bits (por exemplo: Word, Excel, PowerPoint). Se for necessário ter aplicações de Office de 64 bits, esta funcionalidade não é uma boa forma de o fazer porque não existe suporte para ativar uma versão Clique-e-Run de 64 bits do Office da consola do administrador do Microsoft 365 para empresas. 
    
- **Não tem** quaisquer aplicações autónomas do Windows Installer (MSI) 2016 (por exemplo, o Visio ou Project). Microsoft 365 para empresas, Office para a versão Clique-e-Run do Office 2016 e que não funcionam com as aplicações aleacionais do Office 2016 MSI. 
    
A seguinte tabela mostra que ação os utilizadores/administradores finais poderão ter de ecorrer, dependendo do respetiva estado inicial, para que a implementação da versão Clique-e-Run de 32 bits da Office tenha êxito Office partir da consola do administrador do Microsoft 365 para empresas.<br/>


|Estado inicial da instalação do Office|Ação a tomar antes Microsoft 365 para empresas Office instalar|Estado final|
|:-----|:-----|:-----|
|Nenhum conjunto de aplicações do Office instalado  <br/> |Nenhuma  <br/> |Office 32 bits do 2016 é instalado com a instalação Clique-e-Use  <br/> |
|Versão Clique-e-Use de 32 bits do Office (2016 ou anterior) sem aplicações autónomas  <br/> |Nenhuma  <br/> |Atualizada para a versão Clique-e-Use de 32 bits mais recente do Office 2016, conforme necessário **\*** <br/> |
|Versão Clique-e-Utilize de 32 bits do Office e aplicações de Office versão Clique-e-Utilize de 32 bits ou 64 bits (por exemplo, Visio, Project)  <br/> |Nenhum  <br/> |As aplicações a standalone não são afetadas. O conjunto de aplicações é atualizado para a versão Clique-e-Use de 32 bits do Office 2016  <br/> |
|Versão Clique-e-Use de 32 bits do Office e quaisquer aplicações autónomas do Office MSI de 32 ou 64 bits (exceto o 2016)  <br/> |Nenhuma  <br/> |As aplicações a standalone não são afetadas. O conjunto de aplicações é atualizado para a versão Clique-e-Use de 32 bits do Office 2016  <br/> |
|Qualquer versão Clique-e-Use de 64 bits do Office  <br/> |Desinstale as aplicações de Office de 64 bits, se não se importar de substituí-las por aplicações Office de 32 bits  <br/> |Se as aplicações do Office de 64 bits forem removidas, a versão Clique-e-Use de 32 bits do Office 2016 é instalada  <br/> |
|Uma instalação MSI do Office 2016 com ou sem aplicações autónomas  <br/> |Desinstale o Office 2016 MSI.  <br/> |A versão Clique-e-Use de 32 bits do Office 2016 é instalada. As aplicações autónomas não são alteradas  <br/> |
|Instalação do Office 2013 MSI (ou anterior) e/ou aplicações autónomas do Office  <br/> |Nenhuma  <br/> |A versão Clique-e-Use de 32 bits do Office 2016 e a instalação do Office MSI já existente (e aplicações autónomas) existem em simultâneo  <br/> |
||||
   
 **(\*) Nota:** não é atualizada para a versão Clique-e-Use de 32 bits do Office 2016 devido a um erro desconhecido. Está em curso uma correção. 
  
