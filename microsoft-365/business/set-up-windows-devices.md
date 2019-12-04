---
title: Configurar dispositivos Windows para utilizadores do Microsoft 365 Business
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
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: 'Saiba como configurar dispositivos Windows que executam o Windows 10 Pro para usuários do Microsoft 365 Business. '
ms.openlocfilehash: 1e160d624ce5150a1fb74899949aca824589d908
ms.sourcegitcommit: c5ca71d6feb0f033b50ccd4de816fd59b0925007
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/04/2019
ms.locfileid: "39831349"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-users"></a>Configurar dispositivos Windows para utilizadores do Microsoft 365 Business

## <a name="prerequisites"></a>Pré-requisitos

Antes de poder configurar dispositivos Windows para os utilizadores do Microsoft 365 Business, certifique-se de que todos os dispositivos Windows estão a executar o Windows 10 Pro, versão 1703 (Atualização para Criativos). O Windows 10 Pro é um pré-requisito para implementar o Windows 10 Business, que é um conjunto de funcionalidades de gestão de dispositivos e serviços na nuvem que complementam o Windows 10 Pro e permitem a gestão centralizada e os controlos de segurança do Microsoft 365 Business.
  
Se tiver dispositivos Windows a executar o Windows 7 Pro, Windows 8 Pro ou Windows 8.1 Pro, a sua subscrição do Microsoft 365 Business dá-lhe direito a uma atualização do Windows 10.
  
Para obter mais informações sobre como atualizar dispositivos Windows para a Atualização para Criativos do Windows 10 Pro, siga os passos neste tópico: [Atualizar dispositivos Windows para a Atualização para Criativos do Windows Pro](upgrade-to-windows-pro-creators-update.md).
  
[Verifique se o dispositivo está conectado ao AD do Azure](#verify-the-device-is-connected-to-azure-ad) para verificar se você tem a atualização ou para garantir que a atualização funcione.

Assista a um pequeno vídeo sobre a conexão do Windows com o Microsoft 365.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

Se você achou este vídeo útil, confira a série de [treinamento completo para pequenas empresas e as novas para a Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>Associar dispositivos Windows 10 ao Azure AD da sua organização

Quando todos os dispositivos Windows da sua organização tiverem sido atualizados para o Windows 10 Pro Creators Update ou já estiverem executando o Windows 10 Pro Creators Update, você pode conectar esses dispositivos ao Diretório Ativo Azure da sua organização. Uma vez que os dispositivos são aderidos, eles serão atualizados automaticamente para o Windows 10 Business, que faz parte da sua assinatura Microsoft 365 Business.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>Para um dispositivo Windows 10 Pro novo ou recentemente atualizado

Para um novo dispositivo a executar a Atualização para Criativos do Windows 10 Pro ou para um dispositivo que foi atualizado para a Atualização para Criativos do Windows 10 Pro, mas cuja configuração do dispositivo Windows 10 não tenha sido efetuada, siga estes passos.
  
1. Efetue a configuração do dispositivo Windows 10 até aceder à página **Como pretende configurar?**. 
    
    ![On the How would you like to set up page, choose Set up for an organization](media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. Selecione **Configurar para uma organização** e, em seguida, introduza o seu nome de utilizador e palavra-passe do Microsoft 365 Business. 
    
3. Conclua a configuração do dispositivo Windows 10.
    
   Quando terminar, o utilizador estará ligado ao Azure AD da sua organização. Consulte [Verificar se o dispositivo está ligado ao Azure AD](#verify-the-device-is-connected-to-azure-ad) para garantir que o dispositivo está ligado. 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a>Para um dispositivo que já esteja configurado e a executar o Windows 10 Pro

 **Ligar utilizadores ao Azure AD:**
  
1. No PC Windows do seu utilizador com o Windows 10 Pro, versão 1703 (Atualização para Criativos) (consulte os [pré-requisitos](pre-requisites-for-data-protection.md)), clique no logótipo do Windows e, em seguida, no ícone Definições.
  
   ![In the Start menu, click Windows Settings icon](media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. Nas **Definições**, aceda a **Contas**.
  
   ![In Windows Settings, go to Accounts](media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. Na página **As suas informações**, clique em **Aceder a profiss./escolar** \> **Ligar**.
  
   ![Choose Connect under Access work or school](media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. Na caixa de diálogo **Configurar uma conta escolar ou profissional**, em **Ações alternativas**, selecione **Adicionar este dispositivo ao Azure Active Directory**.
  
   ![Click Join this device to Azure Active Directory](media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. Na página **Vamos iniciar a sua sessão**, introduza a sua conta escolar ou profissional \> **Seguinte**.
  
   Na página **Introduzir palavra-passe**, introduza a sua palavra-passe \> **Iniciar sessão**.
  
   ![Enter your work or school email on the Let's get you signed in page](media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. No **Verifique se esta é a** página da sua organização, verifique se as informações estão corretas e clique em **Participar.**
  
   Na página **Está pronto!**, clique em **Concluído**.
  
   ![On the Make sure this is your organization screen, click Join](media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
Se tiver carregado ficheiros para o OneDrive para Empresas, sincronize-os novamente. Se você usou uma ferramenta de terceiros para migrar perfil e arquivos, também sincronizá-los com o novo perfil.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>Verificar se o dispositivo está ligado ao Azure AD

Para verificar o seu estado de sincronização, na página **Aceder a profiss./escolar** nas **Definições**, clique na área **Ligado a** _ \<organization name\> _ para revelar os botões **Informações** e **Desligar**. Clique em **Informações** para obter o seu estado de sincronização. 
  
Na página Estado de sincronização, clique em Sincronizar para obter as mais recentes políticas de gestão de dispositivos móveis no PC.
  
Para começar a usar a conta Microsoft 365 Business, acesse o botão Windows **Start,** clique na foto da sua conta corrente e, em seguida, **alternar**a conta. Inicie sessão com o endereço de e-mail e palavra-passe da sua organização.
  
![Click Info button to view synchronization status](media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-device-is-upgraded-to-windows-10-business"></a>Verificar se o dispositivo foi atualizado para o Windows 10 Business

Verifique se os seus dispositivos Windows 10 associados ao Azure AD foram atualizados para o Windows 10 Business como parte da sua subscrição do Microsoft 365 Business.
  
1. Aceda a **Definições** \> **Sistema** \> **Acerca de**.
    
2. Confirme que a **Edição** apresenta **Windows 10 Business**.
    
    ![Verify that Windows edition is Windows 10 Business.](media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>Next steps

Para configurar os seus dispositivos móveis, consulte [Configurar dispositivos móveis para utilizadores do Microsoft 365 Business](set-up-mobile-devices.md). Para definir políticas de proteção de aplicações ou proteção de dispositivos, consulte [Gerir o Microsoft 365 Business](manage.md).
  
## <a name="see-also"></a>See also

[Microsoft 365 Vídeos de treinamento de negócios](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
