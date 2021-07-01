---
title: Configurar o Microsoft 365 Empresas Premium
f1.keywords:
- NOCSH
ms.author: kwekua
author: kwekua
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
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Descubra os passos de configuração para o Microsoft 365 Empresas Premium, incluindo adicionar um domínio e utilizadores, configurar políticas de segurança e muito mais.
ms.openlocfilehash: 74a98e915577cf86ec32a706bd3b8f558f49db95
ms.sourcegitcommit: 48195345b21b409b175d68acdc25d9f2fc4fc5f1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/30/2021
ms.locfileid: "53227645"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a>Configurar Microsoft 365 Empresas Premium no assistente de configuração

## <a name="watch-overview-of-microsoft-365-setup"></a>Ver: Visão geral Microsoft 365 configuração

Veja este vídeo para ver uma visão geral Microsoft 365 Empresas Premium configuração.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a>Adicionar o seu domínio, utilizadores e configurar políticas

Quando compra um Microsoft 365 Empresas Premium, tem a opção de utilizar um domínio que possui ou de comprar um durante a [registo](sign-up.md).

- Se comprou um novo domínio quando se inscreveu, o seu domínio está configurado e pode aceder a Adicionar utilizadores e atribuir [licenças.](#add-users-and-assign-licenses)

### <a name="add-your-domain-to-personalize-sign-in"></a>Adicionar o seu domínio para personalizar o seu registo

1. Inscreva-se [no](https://admin.microsoft.com) centro de administração do Microsoft 365 com as suas credenciais de administrador global. 

2. **Selecionar Ir para a configuração** para iniciar o assistente.

    ![Selecione Ir para a configuração.](../media/gotosetupinadmincenter.png)

3. Na página **Instalar as Office aplicações,** pode instalar opcionalmente as aplicações no seu computador.
    
4. No passo **Adicionar domínio,** introduza o nome de domínio que pretende utilizar (como contoso.com).

    > [!IMPORTANT]
    > Se comprou um domínio durante a inscrever-se, não verá **Adicionar um passo de** domínio aqui. Em alternativa, [vá para Adicionar](#add-users-and-assign-licenses) utilizadores.

    ![Captura de ecrã a mostra a página Personalizar o seu dia atual.](../media/adddomain.png)

    
4. Siga os passos no assistente para Criar registos DNS em qualquer fornecedor de anfitriões [DNS Microsoft 365](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) que verifique que é o propriedade do domínio. Se conhecer o seu anfitrião do domínio, consulte Também [Adicionar um domínio ao Microsoft 365.](/microsoft-365/admin/setup/add-domain)

    Se o seu fornecedor de domínios for a GoDaddy ou outro anfitrião ativado com ligação de [domínio,](/office365/admin/get-help-with-domains/domain-connect)o processo é fácil e ser-lhe-á automaticamente pedido para o fazer e permitir que a Microsoft se autentique em seu nome.

    ![Na página Confirmar Acesso da GoDaddy, selecione Autorizar.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Adicionar utilizadores e atribuir licenças

Pode adicionar utilizadores no assistente, mas também pode adicionar [utilizadores mais tarde](../admin/add-users/add-users.md) no centro de administração. Além disso, se tiver um controlador de domínio local, pode adicionar utilizadores com o [Azure AD Ligação](/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>Adicionar utilizadores no assistente

Todos os utilizadores que adicionar no assistente receberão automaticamente uma Microsoft 365 Empresas Premium de licenciamento.

![Captura de ecrã da página Adicionar novos utilizadores no assistente](../media/addnewuserspage.png)

1. Se a sua subscrição do Microsoft 365 Empresas Premium tiver utilizadores existentes (por exemplo, se tiver utilizado o Azure AD Ligação), terá uma opção para atribuir licenças aos utilizadores agora. Continue o processo e adicione licenças aos utilizadores.

2. Depois de adicionar os utilizadores, também receberá uma opção para partilhar as credenciais com os novos utilizadores que adicionou. Pode optar por imprimir, transferir ou enviá-las por e-mail.

### <a name="connect-your-domain"></a>Ligar o seu domínio

> [!NOTE]
> Se optou por utilizar o domínio .onmicrosoft ou tiver utilizado o Azure AD Ligação para configurar utilizadores, não verá este passo.
  
Para configurar serviços, tem de atualizar alguns registos no seu anfitrião de DNS ou entidade de registo de domínios.
  
1. Normalmente, o assistente de configuração deteta a sua entidade de registo e fornece-lhe uma ligação para instruções passo a passo de forma a atualizar os seus registos NS no site da entidade de registo de domínios. Se isto não acontecer, altere os servidores de nomes para [configurar o Microsoft 365 de domínios.](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md) 

    - Se tiver registos DNS existentes, por exemplo um site existente, mas o seu anfitrião DNS estiver ativado para ligar o [domínio,](/office365/admin/get-help-with-domains/domain-connect)selecionar Adicionar **registos por mim.** Na página **Escolher os seus serviços online,** aceite todas as  predefinições e selecionar Seguinte e selecionar Autorizar na página do seu anfitrião de DNS.
    - Se tiver registos DNS existentes com outros anfitriões de DNS (não ativado para ligação de domínio), é reflegado para gerir os seus próprios registos DNS para se certificar de que os serviços existentes permanecem ligados. Consulte [as noções básicas de](/office365/admin/get-help-with-domains/dns-basics) domínios para mais informações.

        ![Página Ativar registos.](../media/activaterecords.png)

2. Siga os passos no assistente e o e-mail e outros serviços serão configurados para si.

### <a name="protect-your-organization"></a>Proteger a sua organização 

As políticas que configurar no assistente são aplicadas automaticamente a um Grupo [de segurança denominado](/office365/admin/create-groups/compare-groups#security-groups) *Todos os Utilizadores.* Também pode criar grupos adicionais para atribuir políticas no centro de administração.

1. Em Aumentar a proteção **contra ciberameaces avançadas**, [](../security/office-365-security/defender-for-office-365.md) recomendamos que aceite as predefinições para permitir que Office 365 a Proteção Avançada contra Ameaças analisa ficheiros e ligações em Office aplicações.

    ![Captura de ecrã da página Aumentar proteção.](../media/increasetreatprotection.png)


2. Na página Impedir **fugas** de dados confidenciais, aceite as predefinições para ativo o Office 365 Prevenção de Perda de Dados (DLP) para controlar dados confidenciais em aplicações do Office e impedir a partilha acidental destes dados fora da sua organização.

3. Na página Proteger dados **no Office** para dispositivos móveis, deixe a gestão de aplicações móveis ativada, expanda as definições e reveja-as e, em seguida, selecione Criar política de gestão de aplicações **móveis**.

    ![Captura de ecrã da página Proteger dados no Office para dispositivos móveis.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Proteger Windows 10 PCs

No navegador esquerdo,  selecione Configurar e, em seguida, em **Sign-in and security**, selecione Secure your **Windows 10 .** **Selecionar** Ver para começar. Consulte [Proteger os seus Windows 10 para obter](secure-win-10-pcs.md) instruções completas.

## <a name="deploy-office-365-client-apps"></a>Implementar aplicações Office 365 cliente

Se optou por instalar automaticamente aplicações do Office durante a configuração, as aplicações serão instaladas nos dispositivos Windows 10 assim que os utilizadores tenham feito a loteamento no Azure AD a partir dos respetivos dispositivos Windows, com as respetivos credenciais de trabalho.

Para instalar o Office dispositivos móveis iOS ou Android, consulte Configurar dispositivos [móveis para Microsoft 365 Empresas Premium utilizadores.](set-up-mobile-devices.md)

Também pode instalar o Office individualmente. Consulte [Instalar Office num PC ou Mac para](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) obter instruções.

## <a name="related-content"></a>Conteúdos relacionados

[Microsoft 365 vídeos de formação para empresas](../business-video/index.yml) (página de ligação)
