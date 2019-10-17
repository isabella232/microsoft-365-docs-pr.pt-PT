---
title: Configurar o Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Saiba como configurar o Microsoft 365 Business.
ms.openlocfilehash: cd59570cbcb9b027780e160117b44be88770d6b9
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575554"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>Configurar o Microsoft 365 Business no assistente de configuração

## <a name="add-your-domain-users-and-set-up-policies"></a>Adicionar seu domínio, usuários e configurar políticas

[![Label para que você saiba que o centro de administração está mudando e você pode encontrar mais detalhes em aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Quando você compra o Microsoft 365 Business, você tem a opção de usar um domínio que você possui ou comprar um durante a [inscrição](sign-up.md).

- Se você adquiriu um novo domínio quando se inscreveu, seu domínio está configurado e você pode mover para [Adicionar usuários e atribuir licenças](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Adicione seu domínio para personalizar o login

1. Entre no [centro de administração do Microsoft 365](https://admin.microsoft.com) usando suas credenciais de administrador global. 

2. Escolha **Adicionar um domínio** ou **Adicionar usuários** para iniciar o assistente.
    > [!IMPORTANT]
    > Se você adquiriu um domínio durante a inscrição, não verá **Adicionar uma etapa de domínio** aqui. Vá para [Adicionar usuários](#add-users-and-assign-licenses) em vez disso.

    ![Selecione ir para a configuração.](media/gotosetupinadmincenter.png)
    
3. No assistente, digite o nome de domínio que você deseja usar (como contoso.com).


    ![Screenshot do Personalize sua página de login.](media/personalizesignin.png)

    
4. Siga as etapas no Assistente para [criar registros DNS em qualquer provedor de hospedagem DNS para o Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) que verifica se você possui o domínio. Se você souber seu host de domínio, consulte também as [instruções específicas do host](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Se o seu provedor de hospedagem é GoDaddy, ou outro host habilitado com o [domínio de conexão](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), o processo é fácil e você será automaticamente solicitado a entrar e permitir que a Microsoft autenticar em seu nome:

    ![Na página Confirmar acesso da GoDaddy, selecione autorizar.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Adicionar utilizadores e atribuir licenças

Você pode adicionar usuários no assistente, mas você também pode [Adicionar usuários posteriormente](add-users-m365b.md) no centro de administração. Além disso, se tiver um controlador de domínio local, pode adicionar utilizadores com o [Azure ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>Adicionar usuários no assistente

Todos os usuários que você adicionar no assistente recebem automaticamente uma licença do Microsoft 365 Business atribuída.

![Screenshot da página Adicionar novos usuários no assistente](media/addnewuserspage.png)

1. Se sua assinatura do Microsoft 365 Business tiver usuários existentes (por exemplo, se você usou o Azure AD Connect), você terá uma opção para atribuir licenças a eles agora. Continue o processo e adicione licenças aos utilizadores.

2. Depois de adicionar os usuários, você também receberá uma opção para compartilhar credenciais com os novos usuários que você adicionou. Pode optar por imprimir, transferir ou enviá-las por e-mail.

3. Na criar equipes para sua organização, você pode optar por adicionar equipes e adicionar usuários a eles. Você também pode fazer isso mais tarde. Para obter mais informações, consulte [criar uma equipe de toda a empresa](https://support.office.com/article/037bb27a-bcc9-48fe-8d72-44d9482420a3).

4. Ignore a migração de mensagens de e-mail e selecione **Seguinte** na página **Migrar as mensagens de e-mail**. 

    Se você estiver movendo de outro provedor de email e quiser copiar seus dados mais tarde, você pode [migrar emails e contatos para o Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).


### <a name="connect-your-domain"></a>Ligar o seu domínio

> [!NOTE]
> Se você optou por usar o domínio. onmicrosoft ou usou o Azure AD Connect para configurar usuários, você não verá esta etapa.
  
Para configurar serviços, tem de atualizar alguns registos no seu anfitrião de DNS ou entidade de registo de domínios.
  
1. Normalmente, o assistente de configuração deteta a sua entidade de registo e fornece-lhe uma ligação para instruções passo a passo de forma a atualizar os seus registos NS no site da entidade de registo de domínios. Se isso não for possível, altere os servidores [de nomes para configurar o Office 365 com qualquer registrador de domínio](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Se você tiver registros DNS existentes, por exemplo, um site da Web existente, mas o host DNS estiver habilitado para [conexão de domínio](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), escolha **adicionar registros para mim**. Na página **escolher seus serviços online** , aceite todos os padrões e escolha **Avançar**e escolha **autorizar** na página do host DNS.
    - Se você tiver registros DNS existentes com outros hosts DNS (não habilitados para conexão de domínio), você desejará gerenciar seus próprios registros DNS para garantir que os serviços existentes fiquem conectados. Consulte [noções básicas do domínio](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) para obter mais informações.

        ![Conecte sua página de domínio com eu gerencio meus próprios registros DNS.](media/connectyourdomainpage.png)

2. Siga as etapas no assistente e e-mail e outros serviços serão configurados para você.

### <a name="protect-data-and-devices"></a>Proteja dados e dispositivos 

As diretivas configuradas no assistente são aplicadas automaticamente a um [grupo de segurança](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) chamado todos os *usuários*. Você também pode criar grupos adicionais para atribuir políticas no centro de administração.

1. Na **proteger seus arquivos de trabalho em dispositivos móveis** a opção **proteger arquivos de trabalho quando os dispositivos são perdidos ou roubados** é selecionado por padrão. Você tem uma opção para ativar **gerenciar como os usuários acessam arquivos do Office em dispositivos móveis**, e isso é recomendado.

    ![Screenshot de proteger arquivos de trabalho na página de dispositivos móveis.](media/protectworkfilesondevices.png)

     - Expanda **proteger arquivos de trabalho quando os dispositivos são perdidos ou roubados** para exibir os [valores padrão](protect-work-files-on-lost-or-stolen-device.md):

        ![Captura de tela de valores padrão para proteger arquivos em dispositivos perdidos.](media/protectworkfilesondevicesdefault.png)

    - Selecione **gerenciar como os usuários acessam arquivos do Office em dispositivos móveis** e expandi-lo para exibir os [valores padrão](manage-user-access-on-mobile-devices.md). Recomendamos que você aceite os valores padrão durante a instalação para criar diretivas de aplicativo para Android, iOS e Windows 10 que se aplicam a todos os usuários. Poderá criar políticas adicionais após a configuração estar concluída.

        ![Screenshot de configurações de proteção para arquivos do Office no celular.](media/useraccessonmobile.png)

2. A última etapa na proteção de dados e dispositivos permite que você configure políticas para proteger dispositivos Windows 10. Essas configurações são aplicadas automaticamente quando o Windows 10 de um usuário se conecta à sua organização. Você pode expandir os **dispositivos Windows 10 seguros** para ver e modificar os [valores padrão](secure-windows-10-devices.md).
3. Você também pode optar por [instalar automaticamente o Office](install-office-on-windows-10-during-setup.md) em dispositivos Windows 10.

    ![Screenshot do conjunto Windows 10 página de configuração do dispositivo.](media/setwin10config.png)


## <a name="deploy-office-365-client-apps"></a>Implantar aplicativos cliente do Office 365

Se você optou por instalar automaticamente os aplicativos do Office durante a instalação, os aplicativos serão instalado nos dispositivos Windows 10 depois que os usuários fizerem logon no Azure AD a partir de seus dispositivos Windows com suas credenciais de trabalho.
Para instalar o Office em dispositivos móveis iOS ou Android, consulte [configurar dispositivos móveis para usuários do Microsoft 365 Business](set-up-mobile-devices.md).

Você também pode instalar o Office individualmente. Consulte [instalar o Office em um PC ou Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) para obter instruções.
