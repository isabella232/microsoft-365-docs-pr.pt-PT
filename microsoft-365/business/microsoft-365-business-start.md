---
title: Começar com a Microsoft 365 para negócios
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Saiba mais sobre o Microsoft 365 para negócios, como configurar e como preparar os dispositivos e Computadores dos seus utilizadores para garantir que estão protegidos pela Microsoft 365 para negócios.
ms.openlocfilehash: 17b142fb704d1b0be088a649490e751effb19517
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/21/2020
ms.locfileid: "43633209"
---
# <a name="get-started-with-microsoft-365-for-business"></a>Começar com a Microsoft 365 para negócios

## <a name="what-is-microsoft-365-for-business"></a>O que é microsoft 365 para negócios

O Microsoft 365 para negócios é um conjunto abrangente de ferramentas de produtividade e colaboração de negócios, como outlook, Word, Excel e outros produtos do Office, que estão sempre atualizados. Pode proteger os seus ficheiros de trabalho em todos os dispositivos iOS, Android e Windows 10 com segurança de qualidade empresarial que é simples de gerir.

Veja este vídeo para uma visão geral rápida do Microsoft 365 para negócios.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
O Microsoft 365 para negócios destina-se a até 300 licenças. Se precisar de mais licenças, consulte a documentação da [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986) para obter mais informações. 
  
## <a name="get-microsoft-365-for-business"></a>Obtenha o Microsoft 365 para negócios

- Se tiver um parceiro, eles receberão o Microsoft 365 para negócios: [Obtenha o Microsoft 365 para negócios a partir do Microsoft Partner Center](get-microsoft-365-business.md).
    
- Se não tiver um parceiro e quiser comprar o Microsoft 365 para negócios, pode [comprá-lo aqui.](https://www.microsoft.com/microsoft-365/business)
    
## <a name="set-up-microsoft-365-for-business"></a>Configurar o Microsoft 365 para negócios

 **Visão geral da Microsoft 365 para business Suite configurada**
  
O diagrama seguinte descreve como os administradores configuram o Microsoft 365 para negócios. Também descreve os passos para preparar os PCs do Windows para o Microsoft 365 para negócios. Também pode adicionar novos dispositivos no centro de administração da Microsoft 365 com o [Windows AutoPilot](add-autopilot-devices-and-profile.md). Pode utilizar o AutoPilot para configurar e configurar novos dispositivos para que estejam prontos para uso produtivo assim que um utilizador se insere com o seu Microsoft 365 para credenciais de negócio.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

Veja este vídeo para uma visão geral do Microsoft 365 para configuração de negócios.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Caso tenha considerado este vídeo útil, consulte a [série de formação completa para pequenas empresas e as novidades do Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

  
### <a name="1-set-up-microsoft-365-for-business-admin"></a>1: Configurar o Microsoft 365 para negócios (Administrador)

Inscreva-se no [Microsoft 365 admin center](https://portal.office.com/adminportal/home) com as suas credenciais de administração global e complete os seguintes passos para configurar o Microsoft 365 para negócios. 
  
1. [Pré-requisitos para proteger dados em dispositivos com microsoft 365 para negócios](pre-requisites-for-data-protection.md)
    
    Leia os pré-requisitos primeiro para se certificar de que os seus dispositivos estão prontos para o Microsoft 365 para negócios.
    
2. [Utilize o assistente de configuração para configurar o Microsoft 365 para negócios](set-up.md)
    
    Se estiver **a mover-se permanentemente de um Diretório Ativo local para a nuvem,** pode ir ao centro de administração da Microsoft 365 e utilizar o assistente de configuração para adicionar os seus utilizadores manualmente, ou pode fazer uma sincronização única com o Azure AD Connect. Existem duas formas de o fazer: 
    
    - Se também tiver um servidor Exchange 2010, Exchange 2013 ou Exchange 2016, pode utilizar o Minimal Hybrid para migrar rapidamente caixas de correio para o [Office 365](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef). Os passos híbridos mínimos incluem uma sincronização única de utilizadores para a AD Azure, e a migração por e-mail de in-instalações para a nuvem. Após a migração por e-mail estar completa, a sincronização do diretório é automaticamente desligada quando utiliza este método.
    
    - Utilize o assistente de sincronização de diretório para sincronizar os seus utilizadores na nuvem. Siga os passos em Configuração da sincronização do diretório para que o [Microsoft 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) complete este processo. Depois de sincronizar os seus utilizadores na nuvem, terá de desligar a sincronização do diretório para o [Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Também terá de dar a cada utilizador que tenha sido adicionado desta forma uma licença para o Microsoft 365 para negócios. Pode fazê-lo no assistente de [configuração](set-up.md) ou pode [atribuir licenças aos utilizadores no Microsoft 365 para negócios](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC).
    
### <a name="2-prepare-mobile-devices"></a>2: Preparar dispositivos móveis

Siga as [etapas em Configurar dispositivos móveis para o Microsoft 365 para que os utilizadores empresariais](set-up-mobile-devices.md) instalem aplicações do Office em dispositivos e certifiquem-se de que estão protegidos pela Microsoft 365 para negócios. 
  
### <a name="3-prepare-pcs"></a>3: Preparar computadores

Os administradores podem pré-seleccionar as definições para novos PCs windows 10 utilizando o [Windows AutoPilot](add-autopilot-devices-and-profile.md). Os utilizadores podem configurar os seus dispositivos Windows 10 existentes ou novos seguindo os passos neste tópico: [Configurar PCs Windows para o Microsoft 365 para utilizadores empresariais](set-up-windows-devices.md). Para dispositivos existentes, os utilizadores podem transferir **opcionalmente** [ficheiros para oneDrive para negócios](move-files-to-onedrive.md). Também podem usar ferramentas de terceiros para mover ficheiros associados ao perfil do Windows para o OneDrive.
  
Se a sua organização utilizar o Diretório Ativo do Windows Server no local, pode configurar o Microsoft 365 para proteger os seus dispositivos Windows 10, mantendo ao mesmo tempo o acesso aos recursos no local que requerem autenticação local. Siga os passos em dispositivos Enable [do Windows 10 que serão geridos pelo Microsoft 365 para que](manage-windows-devices.md) o negócio o possa configurar. Este método é preferido, e os dispositivos neste estado são chamados **dispositivos híbridos azure ad**. 
  
Se mantiver um Diretório Ativo local que contenha alguns recursos no local (como partilhas de ficheiros e impressoras), pode dar aos seus dispositivos ad-ad-ad-ad-in ad-acesso a esses recursos seguindo os passos aqui: [Aceder aos recursos no local a partir de um dispositivo azure ad-join na Microsoft 365 para negócios](access-resources.md). **Azure AD-joined devices**
  
  
## <a name="contact-support"></a>Contactar o suporte

 **Se precisar de contactar o suporte:**
  
- Contacte o seu parceiro.
    
- Como Microsoft 365 para administração de negócios, você tem acesso à nossa equipe de apoio ao cliente: ** [Suporte de contato para produtos empresariais - Admin Help](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b)**
    
## <a name="see-also"></a>Consulte também

[Microsoft 365 para documentação e recursos empresariais](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
Gerir o [Microsoft 365 para negócios](manage.md)[Migrar para a Microsoft 365 para negócios](migrate-to-microsoft-365-business.md)

[Microsoft 365 para vídeos de formação de negócios](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) 
