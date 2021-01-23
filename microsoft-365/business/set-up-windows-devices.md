---
title: Configurar dispositivos Windows para utilizadores Microsoft 365 Business Premium
f1.keywords:
- CSH
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
- seo-marvel-mar
- AdminSurgePortfolio
- okr_smb
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: Saiba como configurar dispositivos Windows que executam o Windows 10 Pro para utilizadores Do Microsoft 365 Business Premium, permitindo controlos de gestão e segurança centralizados.
ms.openlocfilehash: b1877d83f113a2ba23d0db374967e0afcd7fe067
ms.sourcegitcommit: 855719ee21017cf87dfa98cbe62806763bcb78ac
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/22/2021
ms.locfileid: "49928730"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a>Configurar dispositivos Windows para utilizadores Microsoft 365 Business Premium

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-premium-users"></a>Pré-requisitos para a configuração de dispositivos Windows para utilizadores Microsoft 365 Business Premium

Antes de configurar dispositivos Windows para utilizadores Do Microsoft 365 Business Premium, certifique-se de que todos os dispositivos Windows estão a executar o Windows 10 Pro, versão 1703 (Creators Update). O Windows 10 Pro é um pré-requisito para a implementação do Windows 10 Business, que é um conjunto de serviços na nuvem e capacidades de gestão de dispositivos que complementam o Windows 10 Pro e permitem os controlos de gestão e segurança centralizados do Microsoft 365 Business Premium.
  
Se tiver dispositivos Windows a executar o Windows 7 Pro, Windows 8 Pro ou Windows 8.1 Pro, a subscrição do Microsoft 365 Business Premium dá-lhe direito a uma atualização do Windows 10.
  
Para obter mais informações sobre como atualizar dispositivos Windows para a Atualização para Criativos do Windows 10 Pro, siga os passos neste tópico: [Atualizar dispositivos Windows para a Atualização para Criativos do Windows Pro](upgrade-to-windows-pro-creators-update.md).
  
Consulte [Verifique se o dispositivo está ligado à Azure AD](#verify-the-device-is-connected-to-azure-ad) para verificar se tem a atualização ou para se certificar de que a atualização funcionou.

Veja um pequeno vídeo sobre a ligação do Windows ao Microsoft 365.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

Caso tenha considerado este vídeo útil, veja a [série de formação completa para pequenas empresas e as novidades do Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>Associar dispositivos Windows 10 ao Azure AD da sua organização

Quando todos os dispositivos Windows da sua organização tiverem sido atualizados para o Windows 10 Pro Creators Update ou já estiverem a executar a Atualização de Criadores Pro Do Windows 10, pode juntar estes dispositivos ao Azure Ative Directory da sua organização. Assim que os dispositivos forem aderidos, serão automaticamente atualizados para o Windows 10 Business, que faz parte da subscrição do Microsoft 365 Business Premium.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>Para um dispositivo Windows 10 Pro novo ou recentemente atualizado

Para um novo dispositivo a executar a Atualização para Criativos do Windows 10 Pro ou para um dispositivo que foi atualizado para a Atualização para Criativos do Windows 10 Pro, mas cuja configuração do dispositivo Windows 10 não tenha sido efetuada, siga estes passos.
  
1. Efetue a configuração do dispositivo Windows 10 até aceder à página **Como pretende configurar?**. 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. Aqui, escolha **Configurar para uma organização** e, em seguida, introduzir o seu nome de utilizador e senha para Microsoft 365 Business Premium. 
    
3. Conclua a configuração do dispositivo Windows 10.
    
   Quando terminar, o utilizador estará ligado ao Azure AD da sua organização. Consulte [Verificar se o dispositivo está ligado ao Azure AD](#verify-the-device-is-connected-to-azure-ad) para garantir que o dispositivo está ligado. 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a>Para um dispositivo que já esteja configurado e a executar o Windows 10 Pro

 **Ligar utilizadores ao Azure AD:**
  
1. No PC Windows do seu utilizador com o Windows 10 Pro, versão 1703 (Atualização para Criativos) (consulte os [pré-requisitos](pre-requisites-for-data-protection.md)), clique no logótipo do Windows e, em seguida, no ícone Definições.
  
   ![In the Start menu, click Windows Settings icon](../media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. Nas **Definições**, aceda a **Contas**.
  
   ![In Windows Settings, go to Accounts](../media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. Na página **As suas informações**, clique em **Aceder a profiss./escolar** \> **Ligar**.
  
   ![Choose Connect under Access work or school](../media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. Na caixa de diálogo **Configurar uma conta escolar ou profissional**, em **Ações alternativas**, selecione **Adicionar este dispositivo ao Azure Active Directory**.
  
   ![Click Join this device to Azure Active Directory](../media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. Na página **Vamos iniciar a sua sessão**, introduza a sua conta escolar ou profissional \> **Seguinte**.
  
   Na página **Introduzir palavra-passe**, introduza a sua palavra-passe \> **Iniciar sessão**.
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. Na página da **organização certifique-se de que esta é** a sua página de organização, verifique se a informação está correta e escolha **'Juntar-se'.**
  
   No **You're all set!** página, chosse **Done**.
  
   ![No the Certifique-se de que este é o seu ecrã de organização, escolha Junte-se](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
Se tiver carregado ficheiros para o OneDrive para Empresas, sincronize-os novamente. Se usou uma ferramenta de terceiros para migrar perfis e ficheiros, também os sincroniza para o novo perfil.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>Verificar se o dispositivo está ligado ao Azure AD

Para verificar o estado da sincronização, na página **de trabalho de acesso ou escola** em **Definições,** selecione a área **Ligada a** _ _ para expor \<organization name\> os botões **Informação** e **Desconexão**. Escolha **Informação** para obter o seu estado de sincronização. 
  
Na página de estado do **Sync,** escolha **o Sync** para obter as mais recentes políticas de gestão de dispositivos móveis no PC.
  
Para começar a utilizar a conta Microsoft 365 Business Premium, aceda ao **botão** Iniciar o Windows, clique com o botão correto da sua conta corrente e, em seguida, **a conta Switch**. Inicie sessão com o endereço de e-mail e palavra-passe da sua organização.
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-pc-is-upgraded-to-windows-10-business"></a>Verifique se o PC está atualizado para o Windows 10 Business

Verifique se o seu Azure AD aderiu aos dispositivos windows 10 e está atualizado para o Windows 10 Business como parte da subscrição do Microsoft 365 Business Premium.
  
1. Aceda a **Definições** \> **Sistema** \> **Acerca de**.
    
2. Confirme que a **Edição** apresenta **Windows 10 Business**.
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>Next steps

Para configurar os seus dispositivos móveis, consulte [configurar dispositivos móveis para utilizadores Microsoft 365 Business Premium](set-up-mobile-devices.md), Para definir políticas de proteção de dispositivos ou de proteção de aplicações, consulte [Gerir o Microsoft 365 para o negócio](manage.md).
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a>Para mais informações sobre a configuração e utilização do Microsoft 365 Business Premium

[Microsoft 365 para vídeos de formação de negócios](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
