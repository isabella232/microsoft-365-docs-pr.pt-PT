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
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Verifique se Microsoft 365 Empresas Premium proteção de aplicações em Windows 10 dispositivos e verifique se os utilizadores não conseguem copiar dados da empresa para ficheiros pessoais ou aplicações não geridas.
ms.openlocfilehash: ab084ded5ef052a7b85839f0debb96eb1bc5bdf332230293613396825c7263f0
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53861761"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Verificar definições de proteção de aplicações em PCs Windows 10

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Confirmar que os utilizadores não conseguem copiar dados da empresa para ficheiros pessoais em dispositivos da empresa

Depois de [configurar as políticas de proteção de aplicações](protection-settings-for-windows-10-devices.md), as mesmas poderão demorar algumas horas a entrar em vigor nos dispositivos dos utilizadores. Se tiver  ativado a definição Impedir que os utilizadores copiem dados da empresa para ficheiros pessoais e os force a guardar ficheiros de trabalho no **OneDrive para Empresas** para dispositivos da empresa, pode verificar esta situação no dispositivo do utilizador depois de se ligarem ao Azure AD e de se ligarem ao Azure AD e de se ligarem ao mesmo. 
  
 **Verificar definições de ligação**
  
1. Depois de entrar com as credenciais Microsoft 365 Empresas Premium e de estabelecer ligação ao Azure AD conforme descrito em Configurar dispositivos Windows para utilizadores do [Microsoft 365 Empresas Premium](set-up-windows-devices.md), aceda **Windows Definições** Contas Aceder a escolar ou \>  \> profissionais. **Selecionar Ligado \<tenant name\> ao Azure AD e,** em seguida, **selecionar Informações**.
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. Na página **Gerido por,** pode ver as Informações de ligação que incluem um Endereço do Servidor de Gestão como o apresentado \<tenant name\> na figura  seguinte.  
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Verificar se não consegue colar dados da empresa numa aplicação não gerida**
  
1. Abra Outlook 2016 que foi instalado pelo Microsoft 365 Empresas Premium.
    
2. Abra um e-mail e copie alguns conteúdos do mesmo.
    
    Abra o Bloco de Notas e tente colar os conteúdos na aplicação.
    
    Irá receber uma mensagem de erro a indicar que a aplicação não consegue aceder aos conteúdos.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    No entanto, poderá colar esses mesmos conteúdos no Word 2016.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Confirmar que os utilizadores não conseguem copiar dados da empresa para ficheiros em dispositivos pessoais

 **Verificar definições de ligação**
  
1. No seu Windows 10 pessoal onde tem sessão sessão de utilizador local, aceda a **Windows Definições**  e clique ou toque em Contas \> **Access escolar ou escolar.**
    
2. Em **Aceder a profiss./escolar**, selecione **Ligar**.
    
3. Introduza a Microsoft 365 Empresas Premium credencial na caixa de diálogo Configurar uma conta escolar **ou** escolarIntroduza \> **a sua conta.**
    
4. Na página **Aceder a profiss./escolar**, selecione a opção **Conta escolar ou profissional** e, em seguida, selecione **Informações**.
    
    ![Clique ou toque em Informações na caixa de diálogo Conta escolar ou pessoal.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. Na página **Aceder** **a** trabalhos ou  escolares, pode ver as Informações de ligação que incluem um Endereço do Servidor de Gestão, tal como o apresentado na imagem seguinte, e inclui as palavras *wip* e *mam.* 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Verificar se não consegue colar dados da empresa numa aplicação não gerida**
  
1. Abra Outlook 2016, adicione a sua Microsoft 365 Empresas Premium conta de utilizador se necessário e instale-a com as Microsoft 365 Empresas Premium dados.
    
2. Abra um e-mail e copie alguns conteúdos do mesmo.
    
    Abra o Bloco de Notas e tente colar os conteúdos na aplicação.
    
    Irá receber uma mensagem de erro a indicar que a aplicação não consegue aceder aos conteúdos.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    No entanto, poderá colar esses mesmos conteúdos no Word 2016.
    

