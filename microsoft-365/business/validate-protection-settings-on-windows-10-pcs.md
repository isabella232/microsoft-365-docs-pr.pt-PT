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
description: Valide as definições de proteção de aplicações Business Premium do Microsoft 365 em dispositivos Windows 10 e verifique se os utilizadores não podem copiar dados da empresa para ficheiros pessoais ou aplicações não geridas.
ms.openlocfilehash: e319ffa5149f055b5de45078facc8899acffc223
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579868"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Verificar definições de proteção de aplicações em PCs Windows 10

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Confirmar que os utilizadores não conseguem copiar dados da empresa para ficheiros pessoais em dispositivos da empresa

Depois de [configurar as políticas de proteção de aplicações](protection-settings-for-windows-10-devices.md), as mesmas poderão demorar algumas horas a entrar em vigor nos dispositivos dos utilizadores. Se **ligar** os **utilizadores prevent de copiar dados da empresa para ficheiros pessoais e forçá-los a guardar ficheiros de trabalho para a** definição oneDrive para business para dispositivos da empresa, pode verificar isso no dispositivo do utilizador depois de estes terem ligado ao Azure AD e terem assinado. 
  
 **Verificar definições de ligação**
  
1. Depois de iniciar sôs com as credenciais Do Microsoft 365 Business Premium e ligar-se ao Azure AD como descrito no [Configurar dispositivos Windows para utilizadores Do Microsoft 365 Business Premium,](set-up-windows-devices.md)vá ao Trabalho de Acesso ou escola de Contas **do Windows** \> **Settings.** \>  Escolha **Connected to \<tenant name\> Azure AD** e, em seguida, escolha **Informações**.
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. Na **página Gerida por** \<tenant name\> página, pode ver a **informação de Ligação** que inclui um **Endereço do Servidor de Gestão** como o mostrado na figura seguinte. 
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Verifique se não é possível colar os dados da empresa numa aplicação não gerida**
  
1. Open Outlook 2016 que foi instalado pelo Microsoft 365 Business Premium.
    
2. Abra um e-mail e copie alguns conteúdos do mesmo.
    
    Abra o Bloco de Notas e tente colar os conteúdos na aplicação.
    
    Receberá um erro que diz que a aplicação não pode aceder ao conteúdo.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    No entanto, poderá colar esses mesmos conteúdos no Word 2016.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Confirmar que os utilizadores não conseguem copiar dados da empresa para ficheiros em dispositivos pessoais

 **Verificar definições de ligação**
  
1. No seu dispositivo pessoal do Windows 10, onde está a iniciar sessão como utilizador local, vá às **Definições** do Windows e clique ou toque em **Contas** \> **Access ou escola**.
    
2. Em **Aceder a profiss./escolar**, selecione **Ligar**.
    
3. Introduza a sua credencial Microsoft 365 Business Premium na **Configuração de um diálogo de trabalho ou conta escolar** Iniciar \> **.**
    
4. Na página **Aceder a profiss./escolar**, selecione a opção **Conta escolar ou profissional** e, em seguida, selecione **Informações**.
    
    ![Clique ou toque em Informações sobre o diálogo de conta de trabalho ou escola.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. Na página de **Access work ou school,** pode ver a **informação de Ligação** que inclui um **Endereço do Servidor de Gestão** como o mostrado na figura seguinte, e inclui as palavras  *wip*  e  *mam*  dentro. 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Verifique se não é possível colar os dados da empresa numa aplicação não gerida**
  
1. Abra o Outlook 2016 e adicione a sua conta Microsoft 365 Business Premium se necessário e inscreva-se com as suas credenciais Microsoft 365 Business Premium.
    
2. Abra um e-mail e copie alguns conteúdos do mesmo.
    
    Abra o Bloco de Notas e tente colar os conteúdos na aplicação.
    
    Receberá um erro que diz que a App não pode aceder aos conteúdos.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    No entanto, poderá colar esses mesmos conteúdos no Word 2016.
    

