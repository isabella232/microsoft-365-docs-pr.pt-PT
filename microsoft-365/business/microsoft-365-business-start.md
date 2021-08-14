---
title: Começar a trabalhar com o Microsoft 365 para empresas
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- TRN_SMB
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Saiba mais sobre Microsoft 365 para empresas, como o configurar e como preparar os dispositivos e PCs dos seus utilizadores para garantir que estão protegidos pelo Microsoft 365 para empresas.
ms.openlocfilehash: 3ac8ec3c831d14cfa6d0018340458b2b494b2dd746a7f2bd61d2eba0b4eaf0a1
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53837907"
---
# <a name="get-started-with-microsoft-365-for-business"></a>Começar a trabalhar com o Microsoft 365 para empresas

## <a name="what-is-microsoft-365-for-business"></a>O que é Microsoft 365 para empresas

O Microsoft 365 para empresas é um conjunto abrangente de ferramentas de colaboração e produtividade empresarial, tais como o Outlook, Word, Excel e outros produtos Office, sempre actualizados. Pode proteger os seus ficheiros de trabalho em todos os seus dispositivos iOS, Android e Windows 10 com segurança de nível empresarial que é simples de gerir.

## <a name="watch-what-is-microsoft-365-business-premium"></a>Ver: O que é o Microsoft 365 Empresas Premium

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Microsoft 365 para empresas destina-se a até 300 licenças. Caso necessite de mais licenças, consulte a documentação sobre o [Microsoft 365 Enterprise](../enterprise/index.yml) para obter mais informações. 
  
## <a name="get-microsoft-365-for-business"></a>Obter o Microsoft 365 para empresas

- Se tiver um parceiro, este obterá o Microsoft 365 para empresas: Obter o Microsoft 365 para Empresas a partir do Centro de [Parceiros da Microsoft](get-microsoft-365-business.md).
    
- Se não tiver um parceiro e quiser obter o Microsoft 365 para empresas, pode [comprá-lo aqui.](https://www.microsoft.com/microsoft-365/business)
    
## <a name="set-up-microsoft-365-for-business"></a>Configurar o Microsoft 365 para empresas

 **Overview of Microsoft 365 for business Suite set up**
  
O seguinte diagrama descreve como os administradores configuram o Microsoft 365 para empresas. Também descreve os passos para preparar Windows PCs para Microsoft 365 para empresas. Também pode adicionar novos dispositivos na aumente centro de administração do Microsoft 365 com [Windows AutoPilot.](add-autopilot-devices-and-profile.md) Pode utilizar o AutoPilot para configurar e pré-configurar novos dispositivos para que estejam prontos para uma utilização produtiva assim que um utilizador começar a trabalhar com as respetivas credenciais do Microsoft 365 para empresas.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

## <a name="watch-set-up-microsoft-365-business"></a>Ver: Configurar o Microsoft 365 Empresas

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Caso tenha considerado este vídeo útil, veja a [série de formação completa para pequenas empresas e as novidades do Microsoft 365](../business-video/index.yml).

  
### <a name="1-set-up-microsoft-365-for-business-admin"></a>1: Configurar o Microsoft 365 para empresas (Administradores)

Indique-centro de administração do Microsoft 365 com as suas credenciais de administrador global e conclua os seguintes passos para configurar o Microsoft 365 para empresas. [](https://admin.microsoft.com/adminportal/home) 
  
1. [Pré-requisitos para proteger dados em dispositivos com o Microsoft 365 para empresas](pre-requisites-for-data-protection.md)
    
    Leia primeiro os pré-requisitos para se certificar de que os seus dispositivos estão prontos para Microsoft 365 para empresas.
    
2. [Utilizar o assistente de configuração para configurar o Microsoft 365 para empresas](set-up.md)
    
    Se mudar permanentemente do **Active Directory local** para a nuvem, pode aceder ao centro de administração do Microsoft 365 e utilizar o assistente de configuração para adicionar os seus utilizadores manualmente ou pode fazer uma sincronização única com o Azure AD Ligação. Existem duas formas de o fazer: 
    
    - Se também tiver um servidor do Exchange 2010, Exchange 2013 ou do Exchange 2016, pode Utilizar uma Migração Híbrida Mínima para migrar rapidamente caixas de correio Exchange para [o Microsoft 365.](/Exchange/mailbox-migration/use-minimal-hybrid-to-quickly-migrate) Os passos híbridos mínimos incluem uma sincronização única de utilizadores com o Azure AD e a migração de e-mails do local para a nuvem. Quando a migração de e-mail estiver concluída, a sincronização de diretórios será desativada automaticamente quando utilizar este método.
    
    - Utilize o assistente de sincronização de diretórios para sincronizar os seus utilizadores com a nuvem. Siga os passos em [Configurar a sincronização de diretórios Microsoft 365](../enterprise/set-up-directory-synchronization.md) para concluir este processo. Após sincronizar os seus utilizadores com a nuvem, terá de Desarmar a [sincronização](../enterprise/turn-off-directory-synchronization.md)de diretórios para o Microsoft 365 .
    
    Também terá de dar a cada utilizador que foi adicionada desta forma uma licença para o Microsoft 365 para empresas. Pode fazê-lo no assistente [de configuração](set-up.md) ou pode [Atribuir licenças a utilizadores.](../admin/manage/assign-licenses-to-users.md)
    
### <a name="2-prepare-mobile-devices"></a>2: Preparar dispositivos móveis

Siga os passos em Configurar dispositivos móveis para o [Microsoft 365](set-up-mobile-devices.md) para utilizadores empresariais instalarem aplicações Office em dispositivos e garantirem que estão protegidos pelo Microsoft 365 para empresas. 
  
### <a name="3-prepare-pcs"></a>3: Preparar PCs

Os administradores podem pré-selecionar definições para novos PCs Windows 10 com [o Windows AutoPilot.](add-autopilot-devices-and-profile.md) Os utilizadores podem configurar as suas novas Windows 10 dispositivos ao seguir os passos neste tópico: Configurar [PCs de Windows](set-up-windows-devices.md)para utilizadores empresariais Microsoft 365. Nos dispositivos existentes, os utilizadores podem **mover ficheiros** [para o OneDrive para Empresas](move-files-to-onedrive.md). Também podem utilizar ferramentas de terceiros para mover ficheiros associados Windows perfil a OneDrive.
  
Se a sua organização utilizar o Windows Server Active Directory no local, pode configurar o Microsoft 365 para empresas para proteger os seus dispositivos Windows 10, mantendo, ao mesmo tempo, o acesso aos recursos no local que exigem autenticação local. Siga os passos em [Ativar a gestão Windows 10](manage-windows-devices.md) dispositivos associados ao domínio pelo Microsoft 365 para empresas para configurar esta configuração. Este método é preferencial e os dispositivos neste estado denominam-se dispositivos associados **ao Azure AD Híbrido.** 
  
Se reter um Active Directory local que contenha alguns recursos no local (como partilhas de ficheiros e impressoras), pode dar aos seus dispositivos associados ao **Azure AD** acesso a estes recursos ao seguir os passos aqui: Aceder a recursos no local a partir de um dispositivo associado ao [Azure AD](access-resources.md)no Microsoft 365 para empresas.
  
  
## <a name="contact-support"></a>Contactar o suporte

 **Se precisar de contactar o suporte:**
  
- Contacte o seu parceiro.
    
- Enquanto administrador Microsoft 365 para empresas, tem acesso à nossa equipa de suporte ao cliente: Contactar o suporte a produtos empresariais **[– Ajuda para Administradores](../business-video/get-help-support.md)**
    
## <a name="related-content"></a>Conteúdos relacionados

[Microsoft 365 para recursos e documentação empresarial](./index.yml) (página de ligação)\
[Gerir Microsoft 365 para empresas](manage.md) (artigo)\
[Migrar para a Microsoft 365 para empresas](migrate-to-microsoft-365-business.md) (artigo)\
[Microsoft 365 vídeos de formação para empresas](../business-video/index.yml) (página de ligação)