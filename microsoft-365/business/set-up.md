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
ms.openlocfilehash: f29dbdb61636fdfe573a1a6920d0aed963b737ad
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/19/2019
ms.locfileid: "38721495"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>Configurar o Microsoft 365 Business no assistente de configuração

## <a name="add-your-domain-users-and-set-up-policies"></a>Adicione seu domínio, usuários e configure políticas

[![Etiqueta que informa que o centro de administração está a mudar e que pode encontrar mais detalhes em aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Quando você compra o Microsoft 365 Business, você tem a opção de usar um domínio que possui ou comprar um durante a [inscrição.](sign-up.md)

- Se você comprou um novo domínio quando se inscreveu, seu domínio está tudo configurado e você pode passar para [adicionar usuários e atribuir licenças.](#add-users-and-assign-licenses)

### <a name="add-your-domain-to-personalize-sign-in"></a>Adicione o seu domínio para personalizar a entrada

1. Entre no [centro de administração da Microsoft 365](https://admin.microsoft.com) usando suas credenciais de administração global. 

2. Escolha **Adicionar um domínio** ou adicionar **usuários** para iniciar o assistente.
    > [!IMPORTANT]
    > Se você comprou um domínio durante a inscrição, você não verá **adicionar um** passo de domínio aqui. Ir para [adicionar usuários](#add-users-and-assign-licenses) em seu lugar.

    ![Selecione Vá para a configuração.](media/gotosetupinadmincenter.png)
    
3. No mago, digite o nome de domínio que você deseja usar (como contoso.com).


    ![Captura de tela do Personalize sua página de login.](media/personalizesignin.png)

    
4. Siga os passos no mago para [criar registros DeNS em qualquer provedor de hospedagem dns para o Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) que verifica o seu próprio domínio. Se você conhece o seu anfitrião de domínio, consulte também as instruções específicas do [anfitrião.](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)

    Se o seu provedor de hospedagem é GoDaddy ou outro host habilitado com [conectar domínio,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)o processo é fácil e você será automaticamente solicitado a entrar e deixar microsoft autenticar em seu nome.

    ![Na página GoDaddy Confirm Access, selecione Authorize.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Adicionar utilizadores e atribuir licenças

Você pode adicionar usuários no mago, mas você também pode [adicionar usuários mais tarde](add-users-m365b.md) no centro de administração. Além disso, se você tiver um controlador de domínio local, você pode adicionar usuários ao [Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

#### <a name="add-users-in-the-wizard"></a>Adicionar usuários no mago

Todos os usuários que você adicionar no assistente obter automaticamente atribuído uma licença de negócios Microsoft 365.

![Screenshot da página adicionar novos usuários no mago](media/addnewuserspage.png)

1. Se sua assinatura Microsoft 365 Business tiver usuários existentes (por exemplo, se você usar o AD Connect do Azure), você receberá uma opção para atribuir licenças a eles agora. Continue o processo e adicione licenças aos utilizadores.

2. Depois de adicionar os usuários, você também terá a opção de compartilhar credenciais com os novos usuários que você adicionou. Pode optar por imprimir, transferir ou enviá-las por e-mail.

3. Nas Equipes de Criação para sua organização, você pode optar por adicionar equipes e adicionar usuários a elas. Você também pode fazer isso mais tarde. Para mais informações, veja [criar uma equipe em toda a empresa.](https://support.office.com/article/037bb27a-bcc9-48fe-8d72-44d9482420a3)

4. Ignore a migração de mensagens de e-mail e selecione **Seguinte** na página **Migrar as mensagens de e-mail**. 

    Se você estiver se movendo de outro provedor de e-mail e quiser copiar seus dados mais tarde, poderá [migrar e-mails e contatos para o Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).


### <a name="connect-your-domain"></a>Ligar o seu domínio

> [!NOTE]
> Se você optar por usar o domínio .onmicrosoft ou usar o AD Connect do Azure para configurar usuários, não verá essa etapa.
  
Para configurar serviços, tem de atualizar alguns registos no seu anfitrião de DNS ou entidade de registo de domínios.
  
1. Normalmente, o assistente de configuração deteta a sua entidade de registo e fornece-lhe uma ligação para instruções passo a passo de forma a atualizar os seus registos NS no site da entidade de registo de domínios. Se isso não o fazer, [alterar nameservers para configurar o Office 365 com qualquer registrador](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2)de domínio . 

    - Se você tiver registros DNS existentes, por exemplo, um site existente, mas seu host DNS está habilitado para [conectar domínio,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)escolha **adicionar registros para mim**. Na página **de serviços on-line Escolha,** aceite todos os padrões e escolha **em seguida**e escolha **autorizar** na página do seu host DNS.
    - Se você tiver registros DNS existentes com outros hosts DNS (não habilitados para conexão de domínio), você deseja gerenciar seus próprios registros de DNS para garantir que os serviços existentes permaneçam conectados. Veja o [básico de domínio](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) para obter mais informações.

        ![Conecte sua página de domínio com eu gerenciarei meus próprios registros de DNS.](media/connectyourdomainpage.png)

2. Siga os passos no assistente e e-mail e outros serviços serão configurados para você.

### <a name="protect-data-and-devices"></a>Proteger dados e dispositivos 

As políticas que você configura no mago são aplicadas automaticamente a um grupo de [segurança](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) chamado *All Users.* Você também pode criar grupos adicionais para atribuir políticas no centro de administração.

1. No **Protect your work files em dispositivos móveis,** a opção Protect arquivos de trabalho quando os **dispositivos são perdidos ou roubados** é selecionada por padrão. Você tem a opção de ativar **gerenciar como os usuários acessam os arquivos do Office em dispositivos móveis,** e isso é recomendado.

    ![Captura de tela dos arquivos de trabalho Protect na página de dispositivos móveis.](media/protectworkfilesondevices.png)

     - Expanda os arquivos de trabalho protect quando os **dispositivos são perdidos ou roubados** para exibir os [valores padrão:](protect-work-files-on-lost-or-stolen-device.md)

        ![Captura de tela dos valores padrão para proteger arquivos em dispositivos perdidos.](media/protectworkfilesondevicesdefault.png)

    - Selecione **Gerenciar como os usuários acessam arquivos do Office em dispositivos móveis** e expandi-los para exibir os [valores padrão](manage-user-access-on-mobile-devices.md). Recomendamos que você aceite os valores padrão durante a configuração para criar políticas de aplicativos para Android, iOS e Windows 10 que se aplicam a todos os usuários. Poderá criar políticas adicionais após a configuração estar concluída.

        ![Captura de tela das configurações de proteção para arquivos do Office em dispositivos móveis.](media/useraccessonmobile.png)

2. A última etapa para proteger dados e dispositivos permite configurar políticas para proteger os dispositivos Windows 10. Essas configurações são aplicadas automaticamente quando o Windows 10 de um usuário se conecta à sua organização. Você pode expandir **dispositivos Secure Windows 10** para ver e modificar os [valores padrão.](secure-windows-10-devices.md)
3. Você também pode optar por [instalar automaticamente](install-office-on-windows-10-during-setup.md) o Office em dispositivos Windows 10.

    ![Captura de tela da página de configuração do dispositivo Conjunto Windows 10.](media/setwin10config.png)


## <a name="deploy-office-365-client-apps"></a>Implantar aplicativos para clientes do Office 365

Se você optar por instalar aplicativos do Office automaticamente durante a configuração, os aplicativos serão instalados nos dispositivos Do Windows 10 assim que os usuários entrarem no AD do Azure a partir de seus dispositivos Windows, usando suas credenciais de trabalho.

Para instalar o Office em dispositivos iOS ou Android móveis, [consulte a configuração de dispositivos móveis para usuários do Microsoft 365 Business.](set-up-mobile-devices.md)

Você também pode instalar o Office individualmente. Consulte [o Office em um PC ou Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) para obter instruções.
