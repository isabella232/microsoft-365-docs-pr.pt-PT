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
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Aprenda a configurar o Microsoft 365 Business.
ms.openlocfilehash: 4c744d6a900dba3c11ee51e75602a430268e15bb
ms.sourcegitcommit: 70e920f76526f47fc849df615de4569e0ac2f4be
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/07/2019
ms.locfileid: "38029110"
---
# <a name="get-started-with-microsoft-365-business"></a>Introdução ao Microsoft 365 Business

## <a name="what-is-microsoft-365-business"></a>O que é o Microsoft 365 Business

O Microsoft 365 Empresas é um conjunto abrangente de ferramentas de colaboração e produtividade empresarial, como o Outlook, Word, Excel e outros produtos do Office sempre atualizados. Pode proteger os seus ficheiros de trabalho em todos os seus dispositivos iOS, Android e Windows 10 com segurança de nível empresarial que é simples de gerir.
  
Microsoft 365 Business foi concebido para um máximo de 300 licenças. Caso necessite de mais licenças, consulte a documentação sobre o [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986) para obter mais informações. 
  
## <a name="get-microsoft-365-business"></a>Obter o Microsoft 365 Empresas

- Se tiver um parceiro, este obterá o Microsoft 365 Business: [Obter o Microsoft 365 Empresas a partir do Centro de Parceiros da Microsoft](get-microsoft-365-business.md).
    
- Se não tiver um parceiro e quiser obter o Microsoft 365 Business, pode [comprá-lo aqui](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>Configurar o Microsoft 365 Empresas

 **Visão geral da configuração do Microsoft 365 Business Suite**
  
O diagrama a seguir descreve como os administradores configurar Microsoft 365 Business. Também descreve os passos para preparar os PCs com Windows para o Microsoft 365 Business. Também pode adicionar novos dispositivos no centro de administração do Microsoft 365 Business com o [Windows AutoPilot](add-autopilot-devices-and-profile.md). Pode utilizar o AutoPilot para configurar e pré-configurar novos dispositivos e prepará-los para uma utilização produtiva assim que o utilizador iniciar sessão com as respetivas credenciais do Microsoft 365 Business.
  
![A diagram that shows the setup and management flow for admins, and also for a user](media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)
  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: Configurar o Microsoft 365 Business (Admin)

Inicie sessão no [centro de administração do Microsoft 365 Empresas](https://portal.office.com/adminportal/home) com as suas credenciais de administrador global e conclua os passos abaixo para configurar o Microsoft 365 Business. 
  
1. [Pré-requisitos para proteger dados em dispositivos com o Microsoft 365 Empresas](pre-requisites-for-data-protection.md)
    
    Leia os pré-requisitos primeiro para se certificar de que os seus dispositivos estão prontos para o Microsoft 365 Business.
    
2. [Configurar o Microsoft 365 Empresas com o assistente de configuração](set-up.md)
    
    Se você estiver **permanentemente se movendo de um Diretório Ativo local para a nuvem,** você pode adicionar seus usuários manualmente no centro de administração microsoft 365 Business usando o assistente de configuração ou pode fazer uma sincronização única com o AD Connect do Azure. Existem duas formas de o fazer: 
    
  - Se você também tiver um servidor Exchange 2010, Exchange 2013 ou Exchange 2016, você pode usar o Minimal Hybrid para migrar rapidamente as caixas de correio da [Exchange para o Office 365](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef). Os passos de migração híbrida mínima incluem uma sincronização única dos utilizadores para o Azure AD, bem como a migração de e-mails do servidor no local para a nuvem. Após a conclusão da migração de e-mails, a sincronização de diretórios será automaticamente desativada com este método.
    
  - Utilize o assistente de sincronização de diretórios do Office 365 para sincronizar os seus utilizadores com a nuvem. Siga os passos em [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) para concluir este processo. Depois de sincronizar os seus utilizadores com a nuvem, terá de [Turn off directory synchronization for Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Também terá de atribuir uma licença do Microsoft 365 Empresas a cada um dos utilizadores que adicionou desta forma. Você pode fazer isso no assistente de [configuração,](set-up.md)ou nas [licenças de design para usuários no Office 365 para negócios.](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC)
    
### <a name="2-prepare-mobile-devices"></a>2: Preparar dispositivos móveis

Siga as etapas na Configuração de[dispositivos móveis para usuários corporativos do Microsoft 365](set-up-mobile-devices.md) instalarem aplicativos do Office em dispositivos e garantir que eles sejam protegidos pelo Microsoft 365 Business. 
  
### <a name="3-prepare-pcs"></a>3: Preparar PCs

Os administradores podem pré-selecionar configurações para novos dispositivos com PCs do Windows 10 usando o [Windows AutoPilot.](add-autopilot-devices-and-profile.md) Os usuários podem configurar seus dispositivos Windows 10 existentes ou novos seguindo as etapas deste tópico: [configure PCs do Windows para usuários do Microsoft 365 Business.](set-up-windows-devices.md) Para dispositivos existentes, os usuários também podem mover arquivos **opcionalmente**[para o OneDrive for Business.](move-files-to-onedrive.md) Eles também podem usar ferramentas de terceiros para mover arquivos associados ao perfil do Windows para o OneDrive.
  
Se a sua organização usar o Diretório Ativo do Windows Server no local, você poderá configurar o Microsoft 365 Business para proteger seus dispositivos Windows 10, mantendo o acesso a recursos no local que exigem autenticação local. Siga as etapas dos [dispositivos Windows 10 incluídos no domínio habilitado para serem gerenciados pelo Microsoft 365 Business](manage-windows-devices.md) para configurar isso. Este é o método preferido e os dispositivos neste estado são chamados dispositivos unidos a **AD híbridos.** 
  
Se você mantiver um Diretório Ativo local que contém alguns recursos no local (como compartilhamentos de arquivos e impressoras), você pode dar aos seus **dispositivos azure ad** acesso a esses recursos seguindo os passos aqui: [Acesse recursos no local Dispositivo azure ad-joined no negócio de Microsoft 365.](access-resources.md)
  
Depois de configurar pCs do Windows 10, você pode [instalar automaticamente](auto-install-or-uninstall-office.md) o Office para os dispositivos. 
  
## <a name="contact-support"></a>Contacte o suporte

 **Se precisar de contactar o suporte:**
  
- Contacte o seu parceiro.
    
- Como administrador da Microsoft 365 Business, você tem acesso à nossa equipe de suporte ao cliente, ** [suporte de contato para produtos de negócios - Admin Help](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b)**
    
## <a name="related-topics"></a>Tópicos relacionados
[Recursos e documentação do Microsoft 365 Empresas](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Gerir o Microsoft 365 Empresas](manage.md)[Migrar para o Microsoft 365 Empresas](migrate-to-microsoft-365-business.md)
  

