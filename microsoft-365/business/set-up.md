---
title: Configurar o Microsoft 365 Business
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
description: Obter informações sobre como configurar o Microsoft 365 Business.
ms.openlocfilehash: e635b828609fc47cd8b92bb179a25bcc43cb0a1a
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660875"
---
# <a name="set-up-microsoft-365-business"></a>Configurar o Microsoft 365 Business

Antes de começar, consulte [Obter Microsoft 365 Business](get-microsoft-365-business.md) para detalhes de inscrição.

Ver um [vídeo de curta duração sobre como configurar o Microsoft 365 Business](https://support.office.com/article/38003e30-9d10-44cf-b596-f1b5f662bfa1) utilizando o conjunto de cópias de segurança assistente e quando não tiver um local, Active Directory
  

## <a name="overview"></a>Descrição Geral

A maior parte dos passos de configuração pode ser efectuado no Assistente de configuração, mas as outras opções também se encontram listadas.

1. [Adicionar o domínio](#add-your-domain-to-personalize-sign-in) (se adquiriu o seu domínio durante a [inscrição](sign-up.md), este passo já é efectuado.)
2. Adicione utilizadores. Pode fazê-lo em qualquer uma das três formas:
    - No [Assistente de configuração](#add-users-in-the-wizard).
    - Utilize a sincronização de directório para [Adicionar utilizadores utilizando Azure AD ligar](#add-users-by-using-azure-ad-connect) se tiver no local do Active directory.
    - Também pode [Adicionar utilizadores posteriormente](add-users-m365b.md) no Centro de administração.
3. Configurar políticas de segurança e configurar dispositivos. Pode fazê-lo em qualquer uma das três formas:
    - No [Assistente de configuração](#set-up-policies-in-the-wizard).  
    - No [Centro de administração](#modify-or-add-policies-in-the-admin-center).
    - No [Centro de administração de Intune](https://docs.microsoft.com/intune/what-is-device-management).
4. Configurar e gerir os dispositivos Windows 10.

    Quando associa um dispositivo WIndows 10 a Azure AD, todas as políticas são aplicadas ao mesmo.
    - Defina configurações de dispositivo do Windows 10 no [Assistente de configuração](#set-up-policies-in-the-wizard).
    - Associe um [novo dispositivo de Windows 10](set-up-windows-devices.md#for-a-brand-new-or-newly-upgraded-windows-10-pro-device) a Azure AD.
    - Associe um [dispositivo existente do Windows 10](set-up-windows-devices.md#for-a-device-already-set-up-and-running-windows-10-pro) a Azure AD.
1. Instale o Office 365 Business.
    - Pode instalar automaticamente o Office nos dispositivos Windows utilizando o [Assistente de configuração](#set-up-policies-in-the-wizard).
    - Automaticamente a [instalar o Office](auto-install-or-uninstall-office.md) partir do Centro de administração.
    - Permitir que os utilizadores [instalar aplicações do Office](https://docs.microsoft.com/office365/admin/setup/install-applications) para o Windows e dispositivos.
     
1. Configure segurança adicional.
    - O Assistente de configuração adiciona políticas para proteger os dispositivos, mas também pode tirar partido das capacidades de [segurança adicionais](#additional-security-settings) para ajuda a proteger os dados, contas e mensagens de correio electrónico. 

## <a name="add-your-domain-users-and-set-up-policies"></a>Adicionar o domínio, utilizadores e configurar políticas

![Faixa que apontam para https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

Quando adquirir o Microsoft 365 Business, tem a opção de utilização de um domínio que possui ou comprar uma durante a [inscrição](sign-up.md).

- Se tiver adquirido um novo domínio, quando se inscreve, o domínio é o conjunto de todas as cópias e pode mover para [Adicionar utilizadores e atribuir licenças](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Adicionar o domínio para personalizar o início de sessão

1. Iniciar sessão no [Centro de administração do Microsoft 365](https://admin.microsoft.com) utilizando as credenciais de administrador global. 

2. Seleccione **Adicionar um domínio** para iniciar o assistente.

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
Se tiver um controlador de domínio local e estiver a utilizar o Active Directory, consulte [como os utilizadores de ddd utilizando Azure AD ligar](#add-users-by-using-azure-ad-connect).

![Instantâneo da página Adicionar de utilizadores novo no Assistente](media/addnewuserspage.png)

1. Se a sua subscrição do Microsoft 365 Business já tiver utilizadores existentes (por exemplo, se utilizou o Azure AD Connect), verá uma opção para atribuir licenças aos mesmos agora. Continue o processo e adicione licenças aos utilizadores.

3. Depois de ter adicionado os utilizadores, também terá a opção de partilhar as credenciais com os novos utilizadores que adicionou. Pode optar por imprimir, transferir ou enviá-las por e-mail.

4. Ignore a migração de mensagens de e-mail e selecione **Seguinte** na página **Migrar as mensagens de e-mail**. 

    Se estiver a mover de outro fornecedor de correio electrónico e pretender copiar os dados mais tarde, pode [Migrar correio-electrónico e contactos para o Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).

#### <a name="add-users-by-using-azure-ad-connect"></a>Adicionar utilizadores utilizando Azure ligar AD

 Se tiver um controlador de domínio local com o Active Directory, sincronizar os utilizadores com o Microsoft 365 Business utilizando [Azure AD ligar](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express). Preencha esta opção antes de iniciar o Assistente de configuração. Pode transferi-lo no Centro de administração:

- Vá para **os utilizadores** \> **utilizadores activos**, seleccione nas reticências na parte superior da página e, em seguida, seleccione **sincronização de directórios** para transferir Azure AD ligar.

    ![Na página utilizadores do Active seleccione elipses > directório snchronization.](media/setupdirsync.png)

    > [!IMPORTANT]
    > Se criar os utilizadores desta forma, ainda terá de atribuir licenças aos mesmos no Centro de administração.

##### <a name="continue-to-access-domain-joined-apps-and-devices"></a>Continuar a aceder a dispositivos e aplicações associado ao domínio

Se pretender continuar a aceder a dispositivos e aplicações associado ao domínio, consulte os seguintes artigos para dois outra forma de permitir que:
  
- [Ativar a gestão, por parte do Microsoft 365 Business, de dispositivos associados ao domínio Windows 10](manage-windows-devices.md)
    - Esta é a forma recomendada.

- [Acesso local recursos a partir de um dispositivo associado AD Azure no Microsoft 365 Business](access-resources.md)

### <a name="connect-your-domain"></a>Ligar o seu domínio

> [!NOTE]
> Se optou por utilizar o domínio de .onmicrosoft, ou utilizado Azure AD ligar para configurar utilizadores, não verá este passo.
  
Para configurar serviços, tem de atualizar alguns registos no seu anfitrião de DNS ou entidade de registo de domínios.
  
1. Normalmente, o assistente de configuração deteta a sua entidade de registo e fornece-lhe uma ligação para instruções passo a passo de forma a atualizar os seus registos NS no site da entidade de registo de domínios. Caso contrário, [nameservers de alteração para configurar o Office 365 qualquer registo de domínio](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Se tiver registos DNS existentes, por exemplo um web site existente, irá pretender gerir os seus próprios registos DNS para se certificar de que os serviços existentes permanecem ligados. Consulte [Noções básicas de domínio](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) para obter mais informações.

        ![Ligar o seu domínio página com irá gerir os meus próprios registos DNS.](media/connectyourdomainpage.png)

2. Siga os passos no assistente e correio electrónico e outros serviços serão configurados para si.

### <a name="set-up-security-policies-and-device-configurations"></a>Configurar políticas de segurança e configurações de dispositivo 

Estas políticas aplicam-se para cada utilizador fornecer uma licença para ou a um grupo de utilizadores se optar por atribuir diferentes políticas a um conjunto de utilizadores.

#### <a name="set-up-policies-in-the-wizard"></a>Configurar políticas no Assistente

As políticas que configura no assistente são aplicadas automaticamente a um [grupo de segurança](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) denominado *Todos os utilizadores*.

1. Na **proteger os ficheiros de trabalho em dispositivos móveis** a opção **proteger ficheiros de trabalho quando dispositivos perdidos ou roubados** está seleccionada por predefinição. Tem uma opção para activar a **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis**, e este procedimento é recomendado.

    ![Captura de ecrã de proteger ficheiros de trabalho na página de dispositivos móveis.](media/protectworkfilesondevices.png)

     - Se expandir **proteger ficheiros de trabalho quando dispositivos perdidos ou roubados**, os [valores predefinidos](protect-work-files-on-lost-or-stolen-device.md) estão pré-seleccionadas:

        ![Captura de ecrã de valores predefinidos para proteger ficheiros em dispositivos perdidos.](media/protectworkfilesondevicesdefault.png)

    - Se seleccionar a **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis** e expandi-lo, os [valores predefinidos](manage-user-access-on-mobile-devices.md) são apresentados. Recomendamos que aceite os valores predefinidos durante a configuração para criar políticas de aplicações para Android, iOS e Windows 10 que se apliquem a todos os utilizadores. Poderá criar políticas adicionais após a configuração estar concluída.

        ![Captura de ecrã de definições de protecção de ficheiros do Office no telemóvel.](media/useraccessonmobile.png)

2. O último passo no proteger os dados e dispositivos permite-lhe definir políticas para proteger o Windows 10 dispositivos. Estas definições são aplicadas automaticamente quando Windows 10 um utilizador liga a sua organização. Pode expandir **Secure Windows 10 dispositivos** para ver e modificar os [valores predefinidos](secure-windows-10-devices.md).
3. Também pode optar por [instalar automaticamente o Office](install-office-on-windows-10-during-setup.md) no Windows 10 dispositivos.

    ![Instantâneo da Definir página de configuração do Windows 10 dispositivo.](media/setwin10config.png)

#### <a name="modify-or-add-policies-in-the-admin-center"></a>Modificar ou adicionar políticas no Centro de administração

Consulte [Gerir Microsoft 365 Business](manage.md) para ligações a tópicos sobre como visualizar e modificar a protecção de dispositivo e aplicação de políticas e como remover dados a partir de ou repor dispositivos de utilizador.

## <a name="deploy-and-manage-windows-10"></a>Implementar e gerir o Windows 10
Consulte [Configurar dispositivos do Windows para utilizadores empresariais do Microsoft 365](set-up-windows-devices.md) para ligar manualmente a Azure AD, quer durante a configuração para novos computadores, ou alterando o perfil de início de sessão para os computadores existentes. 

### <a name="use-autopilot-to-set-up-new-devices"></a>Utilizar o piloto automático para configurar novos dispositivos

Pode utilizar o [Piloto automático do Windows](add-autopilot-devices-and-profile.md) para pré-configurar automaticamente **novos** dispositivos Windows 10 para um utilizador, mas poderá ser mais fácil obter um [parceiro](https://www.microsoft.com/solution-providers/search) que pode fazer isto por si. Também pode ir para o [Arquivo do Microsoft](https://go.microsoft.com/fwlink/?linkid=874598) e peça um perito em tecnologia nuvem configurar novos dispositivos de compras para si.

### <a name="access-on-premises-resources"></a>Aceder a recursos no local

Se a organização utilizar o Windows Server Active Directory no local, pode configurar o Microsoft 365 Business para proteger os dispositivos Windows 10, mantendo o acesso a recursos locais que requerem autenticação local. Siga os passos em [activar dispositivos associados ao domínio de Windows 10 para serem geridos pelo Microsoft 365 Business](manage-windows-devices.md) para configurar esta tarefa. Este é o método preferido e dispositivos neste estado são denominados híbrido Azure AD associado dispositivos.

Se a empresa possui um local do Active Directory que contém alguns locais recursos (tais como partilhas de ficheiros e impressoras), pode conceder acesso a dispositivos Azure AD associados a estes recursos seguindo os passos aqui: [acesso local recursos de um Dispositivo Azure AD associados no Microsoft 365 Business](access-resources.md).

## <a name="deploy-office-365-client-apps"></a>Implementar aplicações de cliente do Office 365

Se optar por instalar automaticamente aplicações do Office no durante o conjunto de cópias, as aplicações instalará nos dispositivos Windows 10 depois dos utilizadores têm sessão iniciada no Azure AD dos dispositivos do Windows com as respectivas credenciais de trabalho.
Para instalar o Office iOS móvel ou dispositivos Android, consulte [Configurar dispositivos móveis para utilizadores empresariais do Microsoft 365](set-up-mobile-devices.md).

Pode também instalar o Office individualmente. Consulte a [instalar o Office num PC ou Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) para obter instruções.

## <a name="additional-security-settings"></a>Definições de segurança adicionais

Para além da segurança e a definição de conformidade no Assistente de configuração, pode também configurar as seguintes definições adicionais:
  
- **Mensagem de correio electrónico de protecção contra malware**
- **Anexos seguros de protecção (ATP) ameaça avançadas**
- **Hiperligações de seguro de ATP**
- **APT anti-phishing**
- **Arquivo do Exchange Online**
- **Prevenção de perda de dados (DLP)**
- **Protecção de informações Azure** (Planear 1)
- **Disponibilidade de portal Intune**

Para obter iniciado, consulte [Configurar políticas de segurança avançada](set-up-advanced-security.md).

Consulte também [10 principais formas de proteger o seu negócio de 365 da Microsoft](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) para obter um guia de procedimentos recomendados de segurança.