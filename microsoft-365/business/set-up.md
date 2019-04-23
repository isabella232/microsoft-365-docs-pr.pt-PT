---
title: Configurar o Microsoft 365 Business através do assistente de configuração
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Obter informações sobre como configurar o Microsoft 365 Business, concluindo os quatro passos.
ms.openlocfilehash: a1c8a41c3e291983276280a063248bdd10a7f85a
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32283941"
---
# <a name="set-up-microsoft-365-business-by-using-the-setup-wizard"></a>Configurar o Microsoft 365 Business através do assistente de configuração

Conclua os passos 1 a 4 abaixo.
  
### <a name="set-up-microsoft-365-business"></a>Configurar o Microsoft 365 Business

Ver um vídeo sobre como configurar o Microsoft 365 Business quando não tiver um local, Active Directory:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/0705c337-f3e8-4d28-bb6c-530cd28e99f2?autoplay=false]
  
Os passos de configuração incluem informações sobre configurações que incluem o local do Active Directory. Se pretender continuar a aceder a dispositivos associados ao domínio, leia os seguintes artigos para dois outra forma de permitir que e conclua os passos antes de executar o Assistente de configuração:
  
- [Ativar a gestão, por parte do Microsoft 365 Business, de dispositivos associados ao domínio Windows 10](manage-windows-devices.md)
    
    -Esta é a forma recomendada.
    
- [Acesso local recursos a partir de um dispositivo associado AD Azure no Microsoft 365 Business](access-resources.md)
    
### <a name="step-1-personalize-sign-in"></a>Passo 1: Personalizar o início de sessão

1. Inicie sessão no [Microsoft 365 Business](https://portal.microsoft.com) com as suas credenciais de administrador global. Selecione o mosaico **Administrador** para aceder ao centro de administração. 
    
2. Selecione **Iniciar a configuração** (consoante o seu estado, poderá ver a opção **Continuar configuração**) no centro de administração para iniciar o assistente. 
    
3. Introduza o nome do domínio que pretende utilizar (como contoso.com)
    
    Continue o processo e introduza o seu domínio mesmo que já o tenha verificado quando utilizou o Azure AD Connect, por exemplo. Os dois passos seguintes não se aplicam ao utilizador se tiver utilizado Azure AD ligar para verificar se o domínio.
    
4. Siga os passos no Assistente para [registos de DNS criar em qualquer fornecedor de alojamento de DNS para o Office 365](https://support.office.com/article/7b7b075d-79f9-4e37-8a9e-fb60c1d95166) , que verifica que possui o domínio. 
    
    Pode ver um vídeo de exemplo do [vídeo: configuração do Office 365 no novo Centro de administração do](https://support.office.com/article/a8c2002a-34bc-4ab3-93d8-9b5156c48bf8). Tenha em atenção que este vídeo não inclui os passos de proteção de dados do Microsoft 365 Business.
    
    ![Screenshot of the Business Cloud Suite setup wizard.](media/3c4fd40c-2de1-4a87-8ee0-78d3928c7bb7.png)
  
### <a name="step-2-add-users-and-assign-licenses"></a>Passo 2: Adicionar utilizadores e atribuir licenças

1. Pode adicionar utilizadores aqui ou [adicionar utilizadores mais tarde](add-users-m365b.md) no centro de administração. 
    
    Será atribuída automaticamente uma licença do Microsoft 365 Business a todos os utilizadores que adicionar.
    
2. Se a sua subscrição do Microsoft 365 Business já tiver utilizadores existentes (por exemplo, se utilizou o Azure AD Connect), verá uma opção para atribuir licenças aos mesmos agora. Continue o processo e adicione licenças aos utilizadores.
    
3. Também verá uma opção para partilhar credenciais com os novos utilizadores adicionados. Pode optar por imprimir, transferir ou enviá-las por e-mail.
    
4. Ignore a migração de mensagens de e-mail e selecione **Seguinte** na página **Migrar as mensagens de e-mail**. 
    
    Se estiver a mover de outro fornecedor de correio electrónico e pretender copiar os dados mais tarde, pode [Migrar correio-electrónico e contactos para o Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).
    
    ![Screenshot of two new users added in the setup wizard](media/8f729967-5c65-4ceb-b737-18119db40564.png)
  
### <a name="step-3-connect-your-domain"></a>Passo 3: Ligar ao domínio

> [!NOTE]
> Se optou por utilizar o domínio de .onmicrosoft, ou utilizado Azure AD ligar, não verá este passo. 
  
Para configurar serviços, tem de atualizar alguns registos no seu anfitrião de DNS ou entidade de registo de domínios.
  
1. Normalmente, o assistente de configuração deteta a sua entidade de registo e fornece-lhe uma ligação para instruções passo a passo de forma a atualizar os seus registos NS no site da entidade de registo de domínios. Caso contrário, [nameservers de alteração para configurar o Office 365 qualquer registo de domínio](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).
    
2. O e-mail e os restantes serviços serão configurados automaticamente
    
### <a name="step-4-manage-devices-and-work-files"></a>Passo 4: Gerir dispositivos e ficheiros de trabalho

1. Na página **Proteger ficheiros de trabalho nos seus dispositivos móveis**, altere as definições **Proteger os ficheiros de trabalho se os dispositivos forem perdidos ou roubados** e **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis** para **Ativada**. Também pode aceder a cada sub definição clicando em divisas ao lado de cada definição.
  
  Todos os ficheiros de trabalho dos utilizadores licenciados estão agora protegidos iOS e dos dispositivos Android, logo [instalar aplicações do Office](set-up-mobile-devices.md) (e autenticar com as respectivas credenciais de Microsoft 365 Business). 
  
  ![Screenshot of protect work files on your mobile devices page](media/3139a9aa-6228-4e74-8166-c6a886d7319f.PNG)
  
2. Na página **configuração do dispositivo Windows 10 definido** , defina **Proteger dispositivos 10 do Windows** como **no**.
  
   Também pode aceder a cada sub definição clicando nas divisas junto da mesma.
  
3. Altere a definição **Instalar o Office em dispositivos Windows 10** para **Sim** se todos os seus utilizadores tiverem computadores com o Windows 10, mas sem uma instalação do Office ou uma instalação do Office com tecnologia Clique-e-Use. Se este não for o caso, defina esta opção para **Não**. Pode [instalar automaticamente o Office](auto-install-or-uninstall-office.md) mais tarde a partir do centro de administração após ter preparado os computadores dos utilizadores. Para obter instruções, consulte a [preparar a instalação de cliente do Office](prepare-for-office-client-deployment.md).
  
    Ficheiros de trabalho dos utilizadores licenciados em dispositivos de Windows 10 vão ser projectados, logo a [associar o seu dispositivo Windows 10](set-up-windows-devices.md) a um domínio do Microsoft 365 Business Azure AD ou, em seguida, [instalar o Windows 10 num novo computador](https://support.office.com/article/c654bd23-d256-4ac7-8fba-0c993bf5a771.aspx) ao aderir ao mesmo tempo o Microsoft 365 Domínio de Azure AD de negócio. 
  
4. Clique em **Seguinte** para terminar a configuração. 
  
    Dê-nos o seu feedback neste passo para nos ajudar a melhorar a experiência.
  
    ![Screenshot of Prepare Windows 10 devices page](media/bff701c1-48a3-44f4-aa95-9d959d57c85b.PNG)
  
## <a name="additional-security-settings"></a>Definições de segurança adicionais

Para além da segurança e a definição de conformidade no Assistente de configuração, pode também configurar as seguintes definições adicionais:
  
- Configure a protecção contra anexos não seguros. **Avançada protecção contra ameaças** (ATP) identifica o conteúdo malicioso e, em seguida, bloqueia a entrega de anexos inseguros, ajudando a proteger o computador contra infecções de ransomware e esquemas de phishing. Para activar a protecção do anexo, consulte [Configurar políticas de anexos seguros do Office 365 ATP](https://support.office.com/article/078eb946-819a-4e13-8673-fe0c0ad3a775#setpolicy).
    
- Proteger o ambiente, quando os utilizadores clicam em hiperligações maliciosas. ATP examina hiperligações na mensagem de correio electrónico quando que um utilizador clica-los. Se uma hiperligação não é segura, o utilizador é avisado não a visitar o site ou informado que o site foi bloqueado. Isto ajuda a proteger contra esquemas de phishing. [Configurar políticas de segurança ligações do Office 365 ATP](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#reveddefaultscc) ou [configurar as políticas de segurança ligações do Office 365 ATP](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#addemailpolscc).
    
- Pode preservar incluindo itens eliminados, colocando o correio todo um utilizador no **litígio mantenha**todo o conteúdo da caixa de correio. Para obter instruções, consulte 
- [Configurar a retenção de correio electrónico com o arquivo Online do Exchange](security-features.md#set-up-email-retention-with-exchange-online-archiving).
    
- Configurar **políticas de retenção**de personalizadas, por exemplo, para manter durante um período específico de tempo ou eliminar permanentemente o conteúdo no final do período de retenção. Pode activar políticas de retenção personalizada no Centro de conformidade, vá para a **governação de dados** de valores mobiliários e \> **retenção**e, em seguida, siga os passos no assistente. Para obter mais informações, consulte [Descrição geral de políticas de retenção](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).
    
## <a name="next-steps"></a>Next steps

Para os utilizadores que têm licenças, o próximo passo é configurar os dispositivos.<br/> Consulte [Configurar dispositivos Windows para utilizadores do Microsoft 365 Business](set-up-windows-devices.md) e [Configurar dispositivos móveis para utilizadores do Microsoft 365 Business](set-up-mobile-devices.md). <br/>Consulte [Gerir o Microsoft 365 Business](manage.md) para obter ligações para tópicos sobre como definir políticas de proteção de aplicações e de dispositivos e como remover dados de dispositivos do utilizador. 
  


