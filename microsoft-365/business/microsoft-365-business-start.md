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
ms.openlocfilehash: ed302a79d125ffc9c6203d902f437749a5b0f8d4
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575904"
---
# <a name="get-started-with-microsoft-365-business"></a>Introdução ao Microsoft 365 Business

## <a name="what-is-microsoft-365-business"></a>O que é o Microsoft 365 Business

O Microsoft 365 Empresas é um conjunto abrangente de ferramentas de colaboração e produtividade empresarial, como o Outlook, Word, Excel e outros produtos do Office sempre atualizados. Pode proteger os seus ficheiros de trabalho em todos os seus dispositivos iOS, Android e Windows 10 com segurança de nível empresarial que é simples de gerir.
  
Microsoft 365 Business foi concebido para um máximo de 300 licenças. Caso necessite de mais licenças, consulte a documentação sobre o [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986) para obter mais informações. 
  
## <a name="get-microsoft-365-business"></a>Obter o Microsoft 365 Empresas

- Se tiver um parceiro, este obterá o Microsoft 365 Business: [Obter o Microsoft 365 Empresas a partir do Centro de Parceiros da Microsoft](get-microsoft-365-business.md).
    
- Se não tiver um parceiro e quiser obter o Microsoft 365 Business, pode [comprá-lo aqui](https://www.microsoft.com/en-us/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>Configurar o Microsoft 365 Empresas

 **Visão geral do Microsoft 365 Business Suite configurada**
  
O diagrama a seguir descreve como os administradores configurar o Microsoft 365 Business. Também descreve os passos para preparar os PCs com Windows para o Microsoft 365 Business. Também pode adicionar novos dispositivos no centro de administração do Microsoft 365 Business com o [Windows AutoPilot](add-autopilot-devices-and-profile.md). Pode utilizar o AutoPilot para configurar e pré-configurar novos dispositivos e prepará-los para uma utilização produtiva assim que o utilizador iniciar sessão com as respetivas credenciais do Microsoft 365 Business.
  
![A diagram that shows the setup and management flow for admins, and also for a user](media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)
  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: configurar o Microsoft 365 Business (admin)

Inicie sessão no [centro de administração do Microsoft 365 Empresas](https://portal.office.com/adminportal/home) com as suas credenciais de administrador global e conclua os passos abaixo para configurar o Microsoft 365 Business. 
  
1. [Pré-requisitos para proteger dados em dispositivos com o Microsoft 365 Empresas](pre-requisites-for-data-protection.md)
    
    Leia os pré-requisitos primeiro para se certificar de que os seus dispositivos estão prontos para o Microsoft 365 Business.
    
2. [Configurar o Microsoft 365 Empresas com o assistente de configuração](set-up.md)
    
    Se você estiver se **movendo permanentemente de um Active Directory local para a nuvem**, você pode adicionar seus usuários manualmente no centro de administração do Microsoft 365 Business usando o assistente de instalação, ou você pode fazer uma sincronização única com o Azure ad Connect. Existem duas formas de o fazer: 
    
  - Se você também tiver um Exchange 2010, Exchange 2013 ou Exchange 2016 servidor, você pode [usar híbrido mínimo para migrar rapidamente caixas de correio do Exchange para o Office 365](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef). Os passos de migração híbrida mínima incluem uma sincronização única dos utilizadores para o Azure AD, bem como a migração de e-mails do servidor no local para a nuvem. Após a conclusão da migração de e-mails, a sincronização de diretórios será automaticamente desativada com este método.
    
  - Utilize o assistente de sincronização de diretórios do Office 365 para sincronizar os seus utilizadores com a nuvem. Siga os passos em [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) para concluir este processo. Depois de sincronizar os seus utilizadores com a nuvem, terá de [Turn off directory synchronization for Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Também terá de atribuir uma licença do Microsoft 365 Empresas a cada um dos utilizadores que adicionou desta forma. Você pode fazer isso no [Assistente de instalação](set-up.md)ou nas [licenças atribuir a usuários no Office 365 para empresas](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC).
    
### <a name="2-prepare-mobile-devices"></a>2: Prepare dispositivos móveis

Siga as etapas em[configurar dispositivos móveis para usuários do microsoft 365 Business](set-up-mobile-devices.md) para instalar aplicativos do Office em dispositivos e certificando-se de que eles estão protegidos pelo Microsoft 365 Business. 
  
### <a name="3-prepare-pcs"></a>3: Prepare PCs

Os administradores podem pré-selecionar configurações para novos dispositivos Windows 10 PCs usando o [Windows AutoPilot](add-autopilot-devices-and-profile.md). Os usuários podem configurar seus dispositivos Windows 10 existentes ou novos seguindo as etapas neste tópico: [Configurar PCs Windows para usuários do Microsoft 365 Business](set-up-windows-devices.md). Para dispositivos existentes, os usuários também podem **opcionalmente**[mover arquivos para o onedrive for Business](move-files-to-onedrive.md). Eles também podem usar ferramentas de terceiros para mover arquivos associados ao perfil do Windows para o OneDrive.
  
Se sua organização usa o Active Directory do Windows Server no local, você pode configurar o Microsoft 365 Business para proteger seus dispositivos Windows 10, enquanto ainda mantém o acesso a recursos locais que exigem autenticação local. Siga as etapas em [habilitar dispositivos do Windows 10 ingressados no domínio para serem gerenciados pelo Microsoft 365 Business](manage-windows-devices.md) para configurá-lo. Esse é o método preferencial e os dispositivos nesse estado são chamados de **dispositivos ingressados no Azure ad híbrido**. 
  
Se você manter um Active Directory local que contenha alguns recursos locais (como compartilhamentos de arquivos e impressoras), poderá conceder aos **dispositivos associados ao AD do Azure** acesso a esses recursos seguindo as etapas aqui: [acessar recursos locais de um Dispositivo ingressado no Azure AD no Microsoft 365 Business](access-resources.md).
  
Depois de configurar o Windows 10 PCs, você pode [instalar automaticamente o Office](auto-install-or-uninstall-office.md) para os dispositivos. 
  
## <a name="contact-support"></a>Contacte o suporte

 **Se precisar de contactar o suporte:**
  
- Contacte o seu parceiro.
    
- Como administrador do Microsoft 365 Business, você tem acesso à nossa equipe de suporte ao cliente, ** [contate o suporte para produtos corporativos-ajuda do administrador](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b)**
    
## <a name="related-topics"></a>Tópicos relacionados
[Recursos e documentação do Microsoft 365 Empresas](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Gerir o Microsoft 365 Empresas](manage.md)[Migrar para o Microsoft 365 Empresas](migrate-to-microsoft-365-business.md)
  

