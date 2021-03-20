---
title: Configurar o Microsoft 365 Business Premium
f1.keywords:
- NOCSH
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
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Descubra os passos de configuração do Microsoft 365 Business Premium, incluindo a adição de um domínio e utilizadores, configurando políticas de segurança, e muito mais.
ms.openlocfilehash: 5b082e78f3dc4067dcce4a96a8088b2347bc3af4
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912576"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a>Configurar o Microsoft 365 Business Premium no assistente de configuração

Veja este vídeo para uma visão geral da configuração do Microsoft 365 Business Premium.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a>Adicione o seu domínio, utilizadores e configurar políticas

Ao comprar o Microsoft 365 Business Premium, tem a opção de utilizar um domínio que possui ou de comprar um durante a [inscrição](sign-up.md).

- Se adquiriu um novo domínio quando se inscreveu, o seu domínio está todo configurado e pode mudar-se para [Adicionar utilizadores e atribuir licenças](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Adicione o seu domínio para personalizar o s-in

1. Inscreva-se no [Microsoft 365 admin center](https://admin.microsoft.com) usando as suas credenciais de administração global. 

2. Escolha **Ir para a configuração** para iniciar o assistente.

    ![Selecione Ir para a configuração.](../media/gotosetupinadmincenter.png)

3. Na página **de aplicações do Office,** pode instalar opcionalmente as aplicações no seu próprio computador.
    
4. No passo de **domínio Adicionar,** insira o nome de domínio que pretende utilizar (como contoso.com).

    > [!IMPORTANT]
    > Se adquiriu um domínio durante a inscrição, não verá **Adicionar um** passo de domínio aqui. Vá a [Adicionar os utilizadores](#add-users-and-assign-licenses) em vez disso.

    ![Screenshot da página De Personalizar o seu sign-in.](../media/adddomain.png)

    
4. Siga os passos no assistente para [criar registos DNS em qualquer fornecedor de hospedagem DNS para o Microsoft 365](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) que verifique que é dono do domínio. Se conhecer o seu anfitrião de domínio, consulte também as [instruções específicas](/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)do anfitrião .

    Se o seu fornecedor de hospedagem for o GoDaddy ou outro anfitrião ativado com [ligação de domínio,](/office365/admin/get-help-with-domains/domain-connect)o processo é fácil e será automaticamente solicitado que faça sessão e deixe a Microsoft autenticar em seu nome.

    ![Na página GoDaddy Confirm Access, selecione Authorize.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Adicionar utilizadores e atribuir licenças

Pode adicionar utilizadores no assistente, mas também pode [adicionar utilizadores mais tarde](../admin/add-users/add-users.md) no centro de administração. Além disso, se tiver um controlador de domínio local, pode adicionar utilizadores ao [Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>Adicionar utilizadores no assistente

Qualquer utilizadores que adicione no assistente recebem automaticamente uma licença Microsoft 365 Business Premium.

![Screenshot da página de novos utilizadores adicionar no assistente](../media/addnewuserspage.png)

1. Se a sua subscrição Microsoft 365 Business Premium tiver utilizadores existentes (por exemplo, se usou o Azure AD Connect), terá agora a opção de lhes atribuir licenças. Continue o processo e adicione licenças aos utilizadores.

2. Depois de adicionar os utilizadores, também terá a opção de partilhar credenciais com os novos utilizadores que adicionou. Pode optar por imprimir, transferir ou enviá-las por e-mail.

### <a name="connect-your-domain"></a>Ligar o seu domínio

> [!NOTE]
> Se optar por utilizar o domínio .onmicrosoft ou utilizar o Azure AD Connect para configurar os utilizadores, não verá este passo.
  
Para configurar serviços, tem de atualizar alguns registos no seu anfitrião de DNS ou entidade de registo de domínios.
  
1. Normalmente, o assistente de configuração deteta a sua entidade de registo e fornece-lhe uma ligação para instruções passo a passo de forma a atualizar os seus registos NS no site da entidade de registo de domínios. Caso não o faça, [altere os serviçais para configurar o Microsoft 365 com qualquer registo de domínio](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md). 

    - Se tiver registos DNS existentes, por exemplo, um web site existente, mas o seu anfitrião DNS está ativado para [a ligação de domínios](/office365/admin/get-help-with-domains/domain-connect), escolha **adicionar registos para mim**. Na página **de serviços online,** aceite todas as predefinições e escolha **Seguinte**, e escolha **'Autorizo'** na página do seu anfitrião DNS.
    - Se tiver registos DNS existentes com outros anfitriões DNS (não habilitados para a ligação de domínios), irá querer gerir os seus próprios registos DNS para garantir que os serviços existentes se mantenham ligados. Consulte [o básico do domínio](/office365/admin/get-help-with-domains/dns-basics) para obter mais informações.

        ![Ativar a página de registos.](../media/activaterecords.png)

2. Siga os passos no assistente e o e-mail e outros serviços serão configurado para si.

### <a name="protect-your-organization"></a>Proteja a sua organização 

As políticas configuradas no assistente são aplicadas automaticamente a um [grupo de Segurança](/office365/admin/create-groups/compare-groups#security-groups) chamado Todos os *Utilizadores*. Também pode criar grupos adicionais para atribuir políticas no centro de administração.

1. Sobre a **proteção do Aumento contra ameaças cibernéticas avançadas,** recomenda-se que aceite os padrãos para permitir que os ficheiros e links [de proteção de ameaças avançadas do Office 365](../security/office-365-security/office-365-atp.md) e links nas aplicações do Office.

    ![Screenshot da página de proteção Aumentar.](../media/increasetreatprotection.png)


2. Na página **Prevent leaks of sensitive data** page, aceite os predefinidos para ligar o Office 365 Data Loss Prevention (DLP) para rastrear dados sensíveis em aplicações do Office e impedir a partilha acidental destes fora da sua organização.

3. Nos **dados** protect in Office para página móvel, deixe a gestão de aplicações móveis, expanda as definições e reveja-as e, em seguida, **selecione Create mobile app management policy**.

    ![Screenshot de Protect datas no Office para página móvel.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Secure Windows 10 PCs

No navegador esquerdo, selecione **Configuração** e, em seguida, **em 'Iniciar s-in e segurança',** escolha **Fixe os computadores Windows 10**. Escolha **a Vista** para começar. Consulte [os computadores Windows 10 para](secure-win-10-pcs.md) obter instruções completas.

## <a name="deploy-office-365-client-apps"></a>Implementar aplicações de clientes 365

Se optar por instalar automaticamente aplicações do Office durante a configuração, as aplicações serão instaladas nos dispositivos Windows 10 assim que os utilizadores tiverem assinado no Azure AD a partir dos seus dispositivos Windows, utilizando as suas credenciais de trabalho.

Para instalar o Office em dispositivos móveis iOS ou Android, consulte [Configurar dispositivos móveis para utilizadores Do Microsoft 365 Business Premium](set-up-mobile-devices.md).

Também pode instalar o Office individualmente. Consulte [o Escritório de Instalação num PC ou Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) para obter instruções.

## <a name="see-also"></a>Consulte também

[Microsoft 365 para vídeos de formação de negócios](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)