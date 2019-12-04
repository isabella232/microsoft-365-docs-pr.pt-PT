---
title: Introdução ao Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Aprenda a configurar o Microsoft 365 Business.
ms.openlocfilehash: 32bb30208083c4f62dd449290a7c9f5d8c725631
ms.sourcegitcommit: c5ca71d6feb0f033b50ccd4de816fd59b0925007
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/04/2019
ms.locfileid: "39831419"
---
# <a name="get-started-with-microsoft-365-business"></a>Introdução ao Microsoft 365 Business

## <a name="what-is-microsoft-365-business"></a>O que é o Microsoft 365 Business

O Microsoft 365 Business é um conjunto abrangente de ferramentas de produtividade e colaboração de negócios, como Outlook, Word, Excel e outros produtos do Office, que estão sempre atualizados. Você pode proteger seus arquivos de trabalho em todos os seus dispositivos iOS, Android e Windows 10 com segurança de nível corporativo que é simples de gerenciar.

Assista a este vídeo para uma rápida visão geral do Microsoft 365 Business.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Microsoft 365 Business destina-se a até 300 licenças. Se você precisar de mais licenças, consulte a documentação da [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986) para obter mais informações. 
  
## <a name="get-microsoft-365-business"></a>Obter o Microsoft 365 Empresas

- Se você tiver um parceiro, eles receberão o Microsoft 365 Business: obtenha o [Microsoft 365 Business do Microsoft Partner Center.](get-microsoft-365-business.md)
    
- Se não tiver um parceiro e quiser obter o Microsoft 365 Business, pode [comprá-lo aqui](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>Configurar o Microsoft 365 Empresas

 **Visão geral da configuração do Microsoft 365 Business Suite**
  
O diagrama a seguir descreve como os administradores configurar Microsoft 365 Business. Também descreve os passos para preparar os PCs com Windows para o Microsoft 365 Business. Você também pode adicionar novos dispositivos no centro de administração microsoft 365 business com [o Windows AutoPilot.](add-autopilot-devices-and-profile.md) Você pode usar o AutoPilot para configurar e pré-configurar novos dispositivos para que eles estejam prontos para uso produtivo assim que um usuário entrar com suas credenciais microsoft 365 Business.
  
![A diagram that shows the setup and management flow for admins, and also for a user](media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

Assista a este vídeo para uma visão geral da configuração do Microsoft 365 Business.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Se você achou este vídeo útil, confira a série de [treinamento completo para pequenas empresas e as novas para a Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: Configurar o Microsoft 365 Business (Admin)

Entre no [microsoft 365 business admin center](https://portal.office.com/adminportal/home) com suas credenciais de administração global e complete as seguintes etapas para configurar o Microsoft 365 Business. 
  
1. [Pré-requisitos para proteger dados em dispositivos com a Microsoft 365 Business](pre-requisites-for-data-protection.md)
    
    Leia os pré-requisitos primeiro para garantir que seus dispositivos estejam prontos para o Microsoft 365 Business.
    
2. [Use o assistente de configuração para configurar o Microsoft 365 Business](set-up.md)
    
    Se você estiver **permanentemente se movendo de um Diretório Ativo local para a nuvem,** você pode ir para o centro de administração de negócios microsoft 365 e usar o assistente de configuração para adicionar seus usuários manualmente ou você pode fazer uma sincronização única com o AD Connect do Azure. Existem duas formas de o fazer: 
    
    - Se você também tiver um servidor Exchange 2010, Exchange 2013 ou Exchange 2016, você pode usar o Minimal Hybrid para migrar rapidamente as caixas de correio da [Exchange para o Office 365](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef). As etapas híbridas mínimas incluem uma sincronização única dos usuários com o AD do Azure e a migração de e-mail de locais para a nuvem. Depois que a migração de e-mail estiver completa, a sincronização do diretório é desativada automaticamente quando você usa esse método.
    
    - Use o assistente de sincronização do diretório do Office 365 para sincronizar seus usuários com a nuvem. Siga os passos em [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) para concluir este processo. Depois de sincronizar seus usuários com a nuvem, você terá que desligar a [sincronização do diretório para o Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Você também terá que dar a cada usuário que foi adicionado desta forma uma licença para a Microsoft 365 Business. Você pode fazer isso no assistente de [configuração](set-up.md) ou você pode [atribuir licenças aos usuários no Office 365 para negócios.](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC)
    
### <a name="2-prepare-mobile-devices"></a>2: Preparar dispositivos móveis

Siga as [etapas na Configuração de dispositivos móveis para usuários do Microsoft 365 Business](set-up-mobile-devices.md) instalaraplicativos do Office em dispositivos e garantir que eles sejam protegidos pelo Microsoft 365 Business. 
  
### <a name="3-prepare-pcs"></a>3: Preparar PCs

Os administradores podem pré-selecionar configurações para novos PCs do Windows 10 usando o [Windows AutoPilot.](add-autopilot-devices-and-profile.md) Os usuários podem configurar seus dispositivos Windows 10 existentes ou novos seguindo as etapas deste tópico: [configure PCs do Windows para usuários do Microsoft 365 Business.](set-up-windows-devices.md) Para dispositivos existentes, os usuários podem mover **arquivos opcionalmente** [para o OneDrive for Business.](move-files-to-onedrive.md) Eles também podem usar ferramentas de terceiros para mover arquivos associados ao perfil do Windows para o OneDrive.
  
Se a sua organização usar o Diretório Ativo do Windows Server no local, você poderá configurar o Microsoft 365 Business para proteger seus dispositivos Windows 10, mantendo o acesso a recursos no local que exigem autenticação local. Siga as etapas dos [dispositivos Windows 10 incluídos no domínio habilitado para serem gerenciados pelo Microsoft 365 Business](manage-windows-devices.md) para configurar isso. Este método é preferido, e os dispositivos neste estado são chamados dispositivos unidos a **AD híbridos.** 
  
Se você mantiver um Diretório Ativo local que contém alguns recursos no local (como compartilhamentos de arquivos e impressoras), você pode dar aos **dispositivos vinculados a Azure a dispositivos vinculados** a esses recursos seguindo os passos aqui: Acesse [recursos locais de um dispositivo azure vinculado a AD no Microsoft 365 Business](access-resources.md).
  
  
## <a name="contact-support"></a>Contacte o suporte

 **Se precisar de contactar o suporte:**
  
- Contacte o seu parceiro.
    
- Como administrador da Microsoft 365 Business, você tem acesso à nossa equipe de suporte ao cliente: ** [suporte de contato para produtos de negócios - Admin Help](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b)**
    
## <a name="see-also"></a>See also

[Recursos e documentação do Microsoft 365 Empresas](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Gerir o Microsoft 365 Empresas](manage.md)[Migrar para o Microsoft 365 Empresas](migrate-to-microsoft-365-business.md)

[Microsoft 365 Vídeos de treinamento de negócios](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) 
