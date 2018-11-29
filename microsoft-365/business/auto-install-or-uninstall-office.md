---
title: Instalar ou desinstalar o Office em dispositivos Windows 10 automaticamente
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
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
ms.assetid: cbc6bfe5-565a-4fb8-95f0-b06e7b74ac46
description: 'Instalar ou desinstalar o Office no Windows 10 dispositivos partir do Centro de administração do Microsoft 365 Business. '
ms.openlocfilehash: 997c001ed1520f1ac989255632d36f9b7bedd16c
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983338"
---
# <a name="automatically-install-or-uninstall-office-on-windows-10-devices"></a>Instalar ou desinstalar o Office em dispositivos Windows 10 automaticamente

Pode instalar o Office em PCs Windows 10 de forma rápida e fácil a partir do centro de administração do Microsoft 365 Business.
  
Para compreender como este processo funciona em aplicações do Office instaladas anteriormente, leia o artigo [Prepare for Office client installation (Preparar a instalação do cliente do Office)](prepare-for-office-client-deployment.md) antes de começar. 
  
## <a name="manage-office-deployments"></a>Gerir as implementações do Office

1. Inicie sessão no [centro de administração](https://aka.ms/bcsportal) com as suas credenciais de administrador global. 
    
2. Na ficha de **dispositivos** , seleccione **Gerir a implementação do Office**.    Se não vir o cartão de **Acções do dispositivo** no centro **doméstica** página admin, clique em **Adicionar** (+) para o adicionar à sua home page de administração.
    
    ![Screenshot of the Devices card in the admin center](media/9982e784-dbf9-4a76-a159-bb3e2e5aa23f.png)
  
3. No painel **Gerir a implementação do Office** aberto, selecione **Adicionar um grupo** e, em seguida, selecione os grupos que pretende utilizar.
    
4. Após ter adicionado os grupos que pretende utilizar, no menu pendente **Ação de Implementação**, selecione **Instalar o Office o mais rápido possível** ou **Desinstalar o Office**.
    
    ![In the Manage Office deployment pane, choose either Install Office as soon as possible, or Uninstall Office.](media/00f24a61-1848-40c0-b037-78d726c7d757.png)
  
5. Selecione **Seguinte** \> reveja as definições e, em seguida, selecione **Confirmar**.
    
Uma versão de 32 bits do Office será instalada ou desinstalada automaticamente nos dispositivos pertencentes aos utilizadores especificados pelos grupos que utilizou.
  
Para verificar se a operação foi concluída, pode abrir o Gestor de Tarefas num computador selecionado para a instalação do Office e procurar o processo Microsoft Office Clique-e-Use.
  


