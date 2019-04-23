---
title: Verificar definições de proteção de aplicações em PCs Windows 10
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Obter informações sobre como validar as definições de protecção de aplicações Microsoft 365 Business Windows 10 dispositivos.
ms.openlocfilehash: 4f1f0993dff0ef8d3f6858a3749e063c7b5579c7
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32280012"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Verificar definições de proteção de aplicações em PCs Windows 10

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Confirmar que os utilizadores não conseguem copiar dados da empresa para ficheiros pessoais em dispositivos da empresa

Depois de [configurar as políticas de proteção de aplicações](protection-settings-for-windows-10-devices.md), as mesmas poderão demorar algumas horas a entrar em vigor nos dispositivos dos utilizadores. Se tiver mudado para **Ativado**, a definição **Impedir que os utilizadores copiem os dados da empresa para ficheiros pessoais e obrigá-los a guardar os ficheiros de trabalho no OneDrive para Empresas** para dispositivos da empresa, poderá verificá-lo no dispositivo do utilizador após o mesmo ter estabelecido ligação ao Azure AD e iniciado sessão. 
  
 **Verificar definições de ligação**
  
1. Depois de iniciar sessão com as credenciais Microsoft 365 Business e de estabelecer ligação ao Azure AD conforme descrito em [Configurar dispositivos Windows para utilizadores do Microsoft 365 Empresas](set-up-windows-devices.md), aceda a **Definições do Windows** \> **Contas** \> **Aceder a profiss./escolar**. Selecione **Ligado ao Azure AD de \<nome do inquilino\>** e, em seguida, selecione **Informações**.
    
    ![Click or tap Info on the Connected to Azure AD dialog.](media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. Na página **Gerido por** \<nome do inquilino\>, poderá ver as **Informações de ligação** que incluem um **Endereço do Servidor de Gestão**, tal como o apresentado na imagem seguinte. 
    
    ![Managed by page shows connection info of the device manager URL.](media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Confirmar que não consegue colar dados da empresa numa aplicação não gerida**
  
1. Abra a versão do Outlook 2016 que foi instalada pelo Microsoft 365 Business.
    
2. Abra um e-mail e copie alguns conteúdos do mesmo.
    
    Abra o Bloco de Notas e tente colar os conteúdos na aplicação.
    
    Irá receber uma mensagem de erro a indicar que a aplicação não consegue aceder aos conteúdos.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    No entanto, poderá colar esses mesmos conteúdos no Word 2016.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Confirmar que os utilizadores não conseguem copiar dados da empresa para ficheiros em dispositivos pessoais

 **Verificar definições de ligação**
  
1. No dispositivo pessoal Windows 10 onde tiver sessão iniciada como utilizador local, aceda a **Definições do Windows** e clique ou toque em **Contas** \> **Aceder a profiss./escolar**.
    
2. Em **Aceder a profiss./escolar**, selecione **Ligar**.
    
3. Introduza a sua credencial Microsoft 365 Business na caixa de diálogo **Configurar uma conta escolar ou profissional** \> **Iniciar sessão**.
    
4. Na página **Aceder a profiss./escolar**, selecione a opção **Conta escolar ou profissional** e, em seguida, selecione **Informações**.
    
    ![Click or tap Info on the Work or school account dalog.](media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. Na página **Aceder a profiss./escolar**, poderá ver as **Informações de ligação** que incluem um **Endereço do Servidor de Gestão**, tal como o apresentado na imagem seguinte, bem como as palavras  *wip*  e  *mam*  . 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Confirmar que não consegue colar dados da empresa numa aplicação não gerida**
  
1. Abra o Outlook 2016, adicione a sua conta Microsoft 365 Business se necessário e inicie sessão com as suas credenciais Microsoft 365 Business.
    
2. Abra um e-mail e copie alguns conteúdos do mesmo.
    
    Abra o Bloco de Notas e tente colar os conteúdos na aplicação.
    
    Irá receber uma mensagem de erro a indicar que a aplicação não consegue aceder aos conteúdos.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    No entanto, poderá colar esses mesmos conteúdos no Word 2016.
    

