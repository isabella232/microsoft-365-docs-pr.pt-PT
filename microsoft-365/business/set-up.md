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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Obter informações sobre como configurar o Microsoft 365 Business.
ms.openlocfilehash: ac9c8b828ff131a15bf057fa8bdc0bf56dd00987
ms.sourcegitcommit: 75b97d1ff617bc4b1b0ef9135dfe6a8842ea1b52
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/18/2019
ms.locfileid: "35772573"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>Configurar o Microsoft 365 Business no Assistente de configuração

## <a name="add-your-domain-users-and-set-up-policies"></a>Adicionar o domínio, utilizadores e configurar políticas

![Faixa que apontam para https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

Quando adquirir o Microsoft 365 Business, tem a opção de utilização de um domínio que possui ou comprar uma durante a [inscrição](sign-up.md).

- Se tiver adquirido um novo domínio, quando se inscreve, o domínio é o conjunto de todas as cópias e pode mover para [Adicionar utilizadores e atribuir licenças](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Adicionar o domínio para personalizar o início de sessão

1. Iniciar sessão no [Centro de administração do Microsoft 365](https://admin.microsoft.com) utilizando as credenciais de administrador global. 

2. Optar por **Adicionar um domínio** ou **Adicionar utilizadores** para iniciar o assistente.
    > [!IMPORTANT]
    > Se tiver adquirido um domínio durante a inscrição, irá não consulte **Adicionar um domínio do** passo aqui. Vá para [Adicionar utilizadores](#add-users-and-assign-licenses) em vez disso.

    ![Seleccione Adicionar um domínio.](media/addadomainadmincenter.png)
    
3. No assistente, introduza o nome de domínio que pretende utilizar (por exemplo, contoso.com).


    ![Captura de ecrã de personalizar a página de início de sessão.](media/personalizesignin.png)

    
4. Siga os passos no Assistente para [registos de DNS criar em qualquer fornecedor de alojamento de DNS para o Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) , que verifica que possui o domínio. Se souber o anfitrião de domínio, consulte também as [instruções específicas do anfitrião](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Se o fornecedor de alojamento de GoDaddy, o processo é fácil e será automaticamente solicitado para iniciar sessão e informar a Microsoft autenticar em seu nome:

    ![Na página de acesso de confirmar GoDaddy, seleccione o autorizar.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Adicionar utilizadores e atribuir licenças

Pode adicionar utilizadores no assistente, mas também pode [Adicionar utilizadores posteriormente](add-users-m365b.md) no Centro de administração. Além disso, se tiver um controlador de domínio local, pode adicionar os utilizadores com [Azure AD ligar](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>Adicionar utilizadores no Assistente

Qualquer utilizador que adicione no assistente obter atribui automaticamente uma licença do Microsoft 365 Business.

![Instantâneo da página Adicionar de utilizadores novo no Assistente](media/addnewuserspage.png)

1. Se a sua subscrição do Microsoft 365 Business tem utilizadores existentes (por exemplo, se utilizou Azure ligar AD), receberá uma opção para atribuir-lhes licenças agora. Continue o processo e adicione licenças aos utilizadores.

3. Depois de ter adicionado os utilizadores, também terá a opção de partilhar as credenciais com os novos utilizadores que adicionou. Pode optar por imprimir, transferir ou enviá-las por e-mail.

4. Ignore a migração de mensagens de e-mail e selecione **Seguinte** na página **Migrar as mensagens de e-mail**. 

    Se estiver a mover de outro fornecedor de correio electrónico e pretender copiar os dados mais tarde, pode [Migrar correio-electrónico e contactos para o Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).


### <a name="connect-your-domain"></a>Ligar o seu domínio

> [!NOTE]
> Se optou por utilizar o domínio de .onmicrosoft, ou utilizado Azure AD ligar para configurar utilizadores, não verá este passo.
  
Para configurar serviços, tem de atualizar alguns registos no seu anfitrião de DNS ou entidade de registo de domínios.
  
1. Normalmente, o assistente de configuração deteta a sua entidade de registo e fornece-lhe uma ligação para instruções passo a passo de forma a atualizar os seus registos NS no site da entidade de registo de domínios. Caso contrário, [nameservers de alteração para configurar o Office 365 qualquer registo de domínio](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Se tiver registos DNS existentes, por exemplo um web site existente, irá pretender gerir os seus próprios registos DNS para se certificar de que os serviços existentes permanecem ligados. Consulte [Noções básicas de domínio](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) para obter mais informações.

        ![Ligar o seu domínio página com irá gerir os meus próprios registos DNS.](media/connectyourdomainpage.png)

2. Siga os passos no assistente e correio electrónico e outros serviços serão configurados para si.

### <a name="set-up-security-policies-and-device-configurations"></a>Configurar políticas de segurança e configurações de dispositivo 

As políticas que configura no assistente são aplicadas automaticamente a um [grupo de segurança](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) denominado *Todos os utilizadores*. Também pode criar grupos adicionais para atribuir políticas para no Centro de administração.

1. Na **proteger os ficheiros de trabalho em dispositivos móveis** a opção **proteger ficheiros de trabalho quando dispositivos perdidos ou roubados** está seleccionada por predefinição. Tem uma opção para activar a **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis**, e este procedimento é recomendado.

    ![Captura de ecrã de proteger ficheiros de trabalho na página de dispositivos móveis.](media/protectworkfilesondevices.png)

     - Expanda a **proteger ficheiros de trabalho quando dispositivos perdidos ou roubados** para apresentar os [valores predefinidos](protect-work-files-on-lost-or-stolen-device.md):

        ![Captura de ecrã de valores predefinidos para proteger ficheiros em dispositivos perdidos.](media/protectworkfilesondevicesdefault.png)

    - Seleccione **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis** e expandi-lo para apresentar os [valores predefinidos](manage-user-access-on-mobile-devices.md). Recomendamos que aceite os valores predefinidos durante a configuração para criar políticas de aplicação para Android, iOS e 10 do Windows que se aplicam a todos os utilizadores. Poderá criar políticas adicionais após a configuração estar concluída.

        ![Captura de ecrã de definições de protecção de ficheiros do Office no telemóvel.](media/useraccessonmobile.png)

2. O último passo no proteger os dados e dispositivos permite-lhe definir políticas para proteger o Windows 10 dispositivos. Estas definições são aplicadas automaticamente quando Windows 10 um utilizador liga a sua organização. Pode expandir **Secure Windows 10 dispositivos** para ver e modificar os [valores predefinidos](secure-windows-10-devices.md).
3. Também pode optar por [instalar automaticamente o Office](install-office-on-windows-10-during-setup.md) no Windows 10 dispositivos.

    ![Instantâneo da Definir página de configuração do Windows 10 dispositivo.](media/setwin10config.png)



## <a name="deploy-office-365-client-apps"></a>Implementar aplicações de cliente do Office 365

Se optar por instalar automaticamente aplicações do Office no durante o conjunto de cópias, as aplicações instalará nos dispositivos Windows 10 depois dos utilizadores têm sessão iniciada no Azure AD dos dispositivos do Windows com as respectivas credenciais de trabalho.
Para instalar o Office iOS móvel ou dispositivos Android, consulte [Configurar dispositivos móveis para utilizadores empresariais do Microsoft 365](set-up-mobile-devices.md).

Pode também instalar o Office individualmente. Consulte a [instalar o Office num PC ou Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) para obter instruções.
