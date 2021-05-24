---
title: Configurar dispositivos Windows para utilizadores Microsoft 365 Empresas Premium utilizadores
f1.keywords:
- CSH
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
description: Configurar dispositivos Windows com Windows 10 Pro para Microsoft 365 Empresas Premium utilizadores, ativando controlos de segurança e gestão centralizados.
ms.openlocfilehash: 3d32a033a1a1c89d7d4d557cea6a28e24543ab2c
ms.sourcegitcommit: b0d3abbccf4dd37e32d69664d3ebc9ab8dea760d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/21/2021
ms.locfileid: "52594027"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a>Configurar dispositivos Windows para utilizadores Microsoft 365 Empresas Premium utilizadores

## <a name="before-you-begin"></a>Before you begin

Antes de poder configurar dispositivos Windows para utilizadores Microsoft 365 Empresas Premium, certifique-se de que todos os dispositivos Windows estão a ser Windows 10 Pro versão 1703 (Atualização para Criadores). Windows 10 Pro é um pré-requisito para implementar o Windows 10 Business, que é um conjunto de funcionalidades de gestão de dispositivos e serviços na nuvem que complementam o Windows 10 Pro e permitem a gestão centralizada e controlos de segurança do Microsoft 365 Empresas Premium.
  
Se tiver dispositivos Windows a executar o Windows 7 Pro, Windows 8 Pro ou Windows 8.1 Pro, a sua subscrição do Microsoft 365 Empresas Premium dá-lhe direito a Windows 10 atualização.
  
Para obter mais informações sobre como atualizar dispositivos Windows para a Atualização para Criativos do Windows 10 Pro, siga os passos neste tópico: [Atualizar dispositivos Windows para a Atualização para Criativos do Windows Pro](upgrade-to-windows-pro-creators-update.md).
  
Consulte Verificar se o dispositivo está ligado ao [Azure AD](#verify-the-device-is-connected-to-azure-ad) para verificar se tem a atualização ou para se certificar de que a atualização funcionou.

Veja um breve vídeo sobre como ligar Windows a Microsoft 365.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

Caso tenha considerado este vídeo útil, veja a [série de formação completa para pequenas empresas e as novidades do Microsoft 365](../business-video/index.yml).
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>Associar dispositivos Windows 10 ao Azure AD da sua organização

Quando todos os Windows dispositivos da sua organização foram atualizados para a Atualização para Criadores de Windows 10 Pro ou se já estiverem a executar a Atualização para Criadores do Windows 10 Pro, pode associar estes dispositivos à versão Azure Active Directory. Assim que os dispositivos estiverem associados, serão automaticamente atualizados para o Windows 10 Business, que faz parte da sua subscrição Microsoft 365 Empresas Premium dispositivos.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>Para um dispositivo Windows 10 Pro novo ou recentemente atualizado

Para um novo dispositivo a executar a Atualização para Criativos do Windows 10 Pro ou para um dispositivo que foi atualizado para a Atualização para Criativos do Windows 10 Pro, mas cuja configuração do dispositivo Windows 10 não tenha sido efetuada, siga estes passos.
  
1. Efetue a configuração do dispositivo Windows 10 até aceder à página **Como pretende configurar?**. 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. Aqui, **selecionar Configurar para uma organização e,** em seguida, introduza o seu nome de utilizador e palavra-passe Microsoft 365 Empresas Premium. 
    
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
  
6. Na página **Certifique-se de que esta é a sua organização,** verifique se as informações estão corretas e selecionar **Aderir.**
  
   Na **seta Está pronto!** , seleção **de Feito**.
  
   ![No ecrã Certifique-se de que esta é a sua organização, selecionar Aderir](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
Se tiver carregado ficheiros para o OneDrive para Empresas, sincronize-os novamente. Se tiver utilizado uma ferramenta de terceiros para migrar o perfil e os ficheiros, também os sincroniza com o novo perfil.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>Verificar se o dispositivo está ligado ao Azure AD

Para verificar o seu estado  de sincronização, na página Aceder  a trabalhos ou escolares no **Definições**, selecione a área Ligado a _ para expor os botões Informações e \<organization name\> **Desligar**.  **Selecionar Informações** para obter o seu estado de sincronização. 
  
Na página Estado **de sincronização,** selecionar **Sincronização** para obter as mais recentes políticas de gestão de dispositivos móveis no PC.
  
Para começar a utilizar a Microsoft 365 Empresas Premium conta, vá  para o Windows Iniciar, clique com o botão direito do rato na imagem da sua conta atual e, em seguida, **em Mudar de conta**. Inicie sessão com o endereço de e-mail e palavra-passe da sua organização.
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-pc-is-upgraded-to-windows-10-business"></a>Verificar se o PC está atualizado para o Windows 10 Business

Verifique se os dispositivos associados ao Azure AD Windows 10 foram atualizados para os Windows 10 Business como parte da sua subscrição Microsoft 365 Empresas Premium subscrição.
  
1. Aceda a **Definições** \> **Sistema** \> **Acerca de**.
    
2. Confirme que a **Edição** apresenta **Windows 10 Business**.
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>Next steps

Para configurar os seus dispositivos móveis, consulte Configurar dispositivos móveis para utilizadores [Microsoft 365 Empresas Premium](set-up-mobile-devices.md), Para definir políticas de proteção de aplicações ou proteção de dispositivos, consulte Gerir o [Microsoft 365 para empresas.](manage.md)
  
## <a name="related-content"></a>Conteúdos relacionados

[Microsoft 365 vídeos de formação para empresas](../business-video/index.yml) (página de ligação)
