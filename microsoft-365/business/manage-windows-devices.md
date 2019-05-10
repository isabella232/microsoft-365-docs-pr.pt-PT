---
title: Ativar a gestão, por parte do Microsoft 365 Business, de dispositivos associados ao domínio Windows 10
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
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Obter informações sobre como activar o Microsoft 365 proteger local AD associado Windows 10 dispositivos.
ms.openlocfilehash: 661e5bf8205a661eb4382b4bdd8fcf3a54ecc12f
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660354"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Ativar a gestão, por parte do Microsoft 365 Business, de dispositivos associados ao domínio Windows 10

Se a organização utilizar o Windows Server Active Directory no local, pode configurar o Microsoft 365 Business para proteger os dispositivos Windows 10, mantendo o acesso a recursos locais que requerem autenticação local. Pode configurar esta tarefa pela primeira sincronização do Active Directory com Azure Active Directory, seguido de registar os dispositivos de 10 de Windows Azure AD e inscrição-los para gestão do dispositivo móvel pelo Microsoft 365 Business.
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a>Configurar dispositivos de domínio a ser gerido pelo Microsoft 365 Business

Para configurar dispositivos de domínio da organização para beneficiar as capacidades fornecidas pelo Azure Active Directory para além do Active Directory no local, pode implementar **híbrido Azure AD associado dispositivos**. Estes são dispositivos que estão associados no local, Active Directory e o Azure Active Directory. Híbrido AD Azure associado dispositivos que podem ser protegidos e geridos pelo Microsoft 365 Business. 
  
Conclua os passos abaixo para certificar os dispositivos Windows 10 híbrido AD Azure associado e geridos pelo Microsoft 365 Business.
  
1. Para sincronizar a utilizadores, grupos e contactos a partir do Active Directory local do Active Directory Azure, execute o Assistente de sincronização de directório e Azure Active Directory ligar conforme descrito em [Configurar a sincronização de directório para o Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
    > [!NOTE]
    > Os passos são exactamente o mesmo para o Microsoft 365 Business. 
  
2. Antes de concluir o passo 3 para permitir que dispositivos Windows 10 ser híbrido Azure AD associado, tem de certificar-se de que cumpre os seguintes pré-requisitos:

   - Tem a versão mais recente do Azure AD ligar.

   - Ligar Azure AD sincronizou todos os objectos de computador dos dispositivos que pretende ser híbrido Azure AD associado. Se os objectos de computador pertencem a unidades organizacionais específicas (UO), em seguida, certifique-se que estes UOs são definidos para sincronização no Azure AD ligar bem.
    
3. Registe existentes associados ao domínio Windows 10 dispositivos ser híbrido Azure AD associado e inscrevê-los para gestão do dispositivo móvel pelo Intune (Microsoft 365 Business):
    
4. Siga as instruções passo a passo de [como configurar dispositivos de Azure do Active Directory associado híbrida](https://go.microsoft.com/fwlink/p/?linkid=872870). Isto permitirá a sincronização do Active Directory no local associado a computadores Windows 10 e torná-los cloud preparado.
    
5. Para inscrever um dispositivo Windows 10 para a gestão do dispositivo móvel, consulte a [Inscrever-se um dispositivo Windows 10 com Intune, utilizando uma política de grupo](https://go.microsoft.com/fwlink/p/?linkid=872871) para obter instruções. Pode definir a política de grupo no computador local nível ou para operações em massa, pode criar esta definição de política de grupo no seu servidor de controlador de domínio.