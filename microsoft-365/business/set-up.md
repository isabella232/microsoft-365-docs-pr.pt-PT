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
- TRN_SMB
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
ms.openlocfilehash: 7ab6ae095ae30f8ceb74be69fcee20f31977ae21
ms.sourcegitcommit: 8fda7852b2a5baa92b8a365865b014ea6d100bbc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/03/2019
ms.locfileid: "39818953"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>Configurar o Microsoft 365 Business no assistente de configuração

Assista a este vídeo para uma visão geral da configuração do Microsoft 365 Business.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Se você achou este vídeo útil, confira a série de [treinamento completo para pequenas empresas e as novas para a Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

## <a name="add-your-domain-users-and-set-up-policies"></a>Adicione seu domínio, usuários e configure políticas

[![Etiqueta que informa que o centro de administração está a mudar e que pode encontrar mais detalhes em aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Quando você compra o Microsoft 365 Business, você tem a opção de usar um domínio que possui ou comprar um durante a [inscrição.](sign-up.md)

- Se você comprou um novo domínio quando se inscreveu, seu domínio está tudo configurado e você pode passar para [adicionar usuários e atribuir licenças.](#add-users-and-assign-licenses)

### <a name="add-your-domain-to-personalize-sign-in"></a>Adicione o seu domínio para personalizar a entrada

1. Entre no [centro de administração da Microsoft 365](https://admin.microsoft.com) usando suas credenciais de administração global. 

2. Escolha **Vá para a configuração** para iniciar o mago.

    ![Selecione Vá para a configuração.](media/gotosetupinadmincenter.png)

3. Na página **de aplicativos install your office,** você pode instalar opcionalmente os aplicativos em seu próprio computador.
    
4. Na etapa de **domínio Adicionar,** digite o nome de domínio que deseja usar (como contoso.com).

    > [!IMPORTANT]
    > Se você comprou um domínio durante a inscrição, você não verá **adicionar um** passo de domínio aqui. Ir para [adicionar usuários](#add-users-and-assign-licenses) em seu lugar.

    ![Captura de tela do Personalize sua página de login.](media/adddomain.png)

    
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

### <a name="connect-your-domain"></a>Ligar o seu domínio

> [!NOTE]
> Se você optar por usar o domínio .onmicrosoft ou usar o AD Connect do Azure para configurar usuários, não verá essa etapa.
  
Para configurar serviços, tem de atualizar alguns registos no seu anfitrião de DNS ou entidade de registo de domínios.
  
1. Normalmente, o assistente de configuração deteta a sua entidade de registo e fornece-lhe uma ligação para instruções passo a passo de forma a atualizar os seus registos NS no site da entidade de registo de domínios. Se isso não o fazer, [alterar nameservers para configurar o Office 365 com qualquer registrador](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2)de domínio . 

    - Se você tiver registros DNS existentes, por exemplo, um site existente, mas seu host DNS está habilitado para [conectar domínio,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)escolha **adicionar registros para mim**. Na página **de serviços on-line Escolha,** aceite todos os padrões e escolha **em seguida**e escolha **autorizar** na página do seu host DNS.
    - Se você tiver registros DNS existentes com outros hosts DNS (não habilitados para conexão de domínio), você deseja gerenciar seus próprios registros de DNS para garantir que os serviços existentes permaneçam conectados. Veja o [básico de domínio](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) para obter mais informações.

        ![Ativar a página de registros.](media/activaterecords.png)

2. Siga os passos no assistente e e-mail e outros serviços serão configurados para você.

### <a name="protect-your-organization"></a>Proteger sua organização 

As políticas que você configura no mago são aplicadas automaticamente a um grupo de [segurança](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) chamado *All Users.* Você também pode criar grupos adicionais para atribuir políticas no centro de administração.

1. Sobre a **proteção de aumento contra ameaças cibernéticas avançadas,** recomenda-se que você aceite os padrões para permitir que o Office [365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) escaneie arquivos e links em aplicativos do Office.

    ![Página de proteção de captura de tela do aumento.](media/increasetreatprotection.png)


2. No **Prevent vazamentos de página de dados confidenciais,** aceite os padrões para ativar a Prevenção de Perdas de Dados (DLP) do Office 365 para rastrear dados confidenciais em aplicativos do Office e evitar o compartilhamento acidental desses fora de sua organização.

3. Nos **dados protect in Office para** página móvel, deixe o gerenciamento de aplicativos móveis, expanda as configurações e os revise e selecione a política de gerenciamento de **aplicativos móveis**do Create.

    ![Captura de tela dos dados de Proteger no Office para página móvel.](media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>PCs seguros do Windows 10

No nav esquerdo, selecione **a configuração** e, em seguida, **sing-in e segurança,** escolha **proteger seus computadores do Windows 10**. Escolha **o View** para começar. Veja [proteger seus computadores do Windows 10](secure-win-10-pcs.md) para instruções completas.

## <a name="deploy-office-365-client-apps"></a>Implantar aplicativos para clientes do Office 365

Se você optar por instalar aplicativos do Office automaticamente durante a configuração, os aplicativos serão instalados nos dispositivos Do Windows 10 assim que os usuários entrarem no AD do Azure a partir de seus dispositivos Windows, usando suas credenciais de trabalho.

Para instalar o Office em dispositivos iOS ou Android móveis, [consulte a configuração de dispositivos móveis para usuários do Microsoft 365 Business.](set-up-mobile-devices.md)

Você também pode instalar o Office individualmente. Consulte [o Office em um PC ou Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) para obter instruções.

## <a name="see-also"></a>See also

[Microsoft 365 Vídeos de treinamento de negócios](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
