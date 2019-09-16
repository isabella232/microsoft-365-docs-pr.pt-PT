---
title: Ativar a gestão, por parte do Microsoft 365 Business, de dispositivos associados ao domínio Windows 10
ms.author: sirkkuw
author: Sirkkuw
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
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Saiba como habilitar o Microsoft 365 para proteger dispositivos do Windows 10 ingressados no AD local.
ms.openlocfilehash: 5cce4bc53f118560e31ad7e6048e4efcb49d662e
ms.sourcegitcommit: c0f769244d05ad019ea2307c38d5543d7b1e5afd
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992235"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Ativar a gestão, por parte do Microsoft 365 Business, de dispositivos associados ao domínio Windows 10

Se sua organização usa o Active Directory do Windows Server no local, você pode configurar o Microsoft 365 Business para proteger seus dispositivos Windows 10, enquanto ainda mantém o acesso a recursos locais que exigem autenticação local. Você pode configurá-lo sincronizando primeiro o Active Directory com o Azure Active Directory, seguido de registrar os dispositivos Windows 10 com o Azure AD e inscrevendo-os para o gerenciamento de dispositivos móveis pelo Microsoft 365 Business.
O vídeo a seguir detalha as etapas de como configurá-lo para o cenário mais comum.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a>Configurar dispositivos ingressados no domínio a serem gerenciados pelo Microsoft 365 Business

Para configurar os dispositivos ingressados no domínio da sua organização para se beneficiarem dos recursos fornecidos pelo Azure Active Directory, além do Active Directory local, você pode implementar **dispositivos ingressados no Azure ad híbridos**. Estes são dispositivos que estão associados ao Active Directory no local e ao Azure Active Directory. Os dispositivos ingressados no Azure AD híbridos podem ser protegidos e gerenciados pelo Microsoft 365 Business. 
  
Conclua as etapas abaixo para tornar seus dispositivos Windows 10 híbridos do Azure AD ingressados e gerenciados pelo Microsoft 365 Business.
  
1. Para sincronizar seus usuários, grupos e contatos do Active Directory local no Active Directory do Azure, execute o assistente de sincronização de diretórios e o Azure Active Directory Connect, conforme descrito em [Configurar a sincronização de diretórios para o Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
    > [!NOTE]
    > As etapas são exatamente as mesmas para o Microsoft 365 Business. 
  
2. Antes de concluir a etapa 3 para permitir que os dispositivos Windows 10 sejam ingressados no Azure AD híbrido, você precisa certificar-se de que atende aos seguintes pré-requisitos:

   - Você está executando a versão mais recente do Azure AD Connect.

   - O Azure AD Connect sincronizou todos os objetos de computador dos dispositivos que você deseja que sejam ingressados no Azure AD híbrido. Se os objetos de computador pertencerem a unidades organizacionais específicas (UO), certifique-se de que essas OUs estão definidas para sincronização no Azure AD conectar também.
    
3. Registre dispositivos existentes do Windows 10 ingressados no domínio para ser híbrido do Azure AD ingressado e inscrevê-los para gerenciamento de dispositivos móveis pelo Intune (Microsoft 365 Business):
    
4. Siga as instruções passo a passo em [como configurar os dispositivos ingressados no Azure Active Directory híbrido](https://go.microsoft.com/fwlink/p/?linkid=872870). Isso permitirá a sincronização de seu Active Directory local ingressado em computadores com Windows 10 e disponibilizá-los na nuvem.
    
5. Para inscrever um dispositivo Windows 10 para gerenciamento de dispositivos móveis, consulte [inscrever um dispositivo Windows 10 com o Intune usando uma política de grupo](https://go.microsoft.com/fwlink/p/?linkid=872871) para obter instruções. Você pode definir a diretiva de grupo em um nível de computador local ou para operações em massa, você pode criar essa configuração de diretiva de grupo no seu servidor de controlador de domínio.