---
title: Introdução ao Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 9/20/2018
ms.audience: Admin
ms.topic: overview
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Obter informações sobre como configurar o Microsoft 365 Business.
ms.openlocfilehash: ee15ffa98de032d7936d950124cdf772335949bd
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/16/2019
ms.locfileid: "26983288"
---
# <a name="get-started-with-microsoft-365-business"></a>Introdução ao Microsoft 365 Business

## <a name="what-is-microsoft-365-business"></a>O que é o Microsoft 365 Business

O Microsoft 365 Empresas é um conjunto abrangente de ferramentas de colaboração e produtividade empresarial, como o Outlook, Word, Excel e outros produtos do Office sempre atualizados. Pode proteger os seus ficheiros de trabalho em todos os seus dispositivos iOS, Android e Windows 10 com segurança de nível empresarial que é simples de gerir.
  
Microsoft 365 Business foi concebido para um máximo de 300 licenças. Caso necessite de mais licenças, consulte a documentação sobre o [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986) para obter mais informações. 
  
## <a name="get-microsoft-365-business"></a>Obter o Microsoft 365 Empresas

- Se tiver um parceiro, este obterá o Microsoft 365 Business: [Obter o Microsoft 365 Empresas a partir do Centro de Parceiros da Microsoft](get-microsoft-365-business.md).
    
- Se não tiver um parceiro e quiser obter o Microsoft 365 Business, pode [comprá-lo aqui](https://www.microsoft.com/en-us/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>Configurar o Microsoft 365 Empresas

 **Descrição geral do Microsoft 365 Business Suite, configurar**
  
O diagrama seguinte descreve como administradores configurar o Microsoft 365 Business. Também descreve os passos para preparar computadores com o Windows para o Microsoft 365 Business. Também pode adicionar novos dispositivos no Centro de administração de Microsoft 365 Business com o [Piloto automático do Windows](add-autopilot-devices-and-profile.md). Pode utilizar o piloto automático para pré- configurar novos dispositivos, a prepará-las para utilização produtiva, logo que um utilizador inicia sessão com as respectivas credenciais de Microsoft 365 Business.
  
![A diagram that shows the setup and management flow for admins, and also for a user](media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)
  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: configurar o Microsoft 365 Business (Admin.)

Inicie sessão no [centro de administração do Microsoft 365 Empresas](https://portal.office.com/adminportal/home) com as suas credenciais de administrador global e conclua os passos abaixo para configurar o Microsoft 365 Business. 
  
1. [Pré-requisitos para proteger dados em dispositivos com o Microsoft 365 Empresas](pre-requisites-for-data-protection.md)
    
    Leia os pré-requisitos primeiro para se certificar de que os seus dispositivos estão prontos para o Microsoft 365 Business.
    
2. [Configurar o Microsoft 365 Empresas com o assistente de configuração](set-up.md)
    
    Se estiver **a mover permanentemente de um Active Directory para o cloud local**, pode adicionar utilizadores manualmente no Centro de administração do Microsoft 365 Business utilizando o Assistente de configuração ou pode efectuar uma sincronização pontual com Azure AD ligar. Existem duas formas de efectuar este procedimento: 
    
  - Se também tiver um Exchange 2010, Exchange 2013 ou de 2016 Exchange server, pode [Utilizar híbrido mínima rapidamente migrar caixas de correio do Exchange para o Office 365](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef). Os passos de híbridos mínima incluem uma sincronização de utilizadores a Azure AD única, bem como migração a partir do local para a nuvem de correio electrónico. Uma vez concluída a migração de correio electrónico, a sincronização de directório é automaticamente desactivada quando utilizar este método.
    
  - Utilize o assistente de sincronização de diretórios do Office 365 para sincronizar os seus utilizadores com a nuvem. Siga os passos em [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) para concluir este processo. Depois de sincronizar os seus utilizadores com a nuvem, terá de [Turn off directory synchronization for Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Também terá de atribuir a cada utilizador que tenha sido adicionado esta forma de uma licença para Microsoft 365 Business. Pode fazê-lo no [Assistente de configuração](set-up.md), ou [atribuir licenças aos utilizadores no Office 365 para a empresa](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC).
    
### <a name="2-prepare-mobile-devices"></a>2: preparar dispositivos móveis

Siga os passos no a[Configurar dispositivos móveis para utilizadores empresariais do Microsoft 365](set-up-mobile-devices.md) para instalar aplicações do Office em dispositivos e certificar-se de que estejam protegidos por negócio do Microsoft 365. 
  
### <a name="3-prepare-pcs"></a>3: preparar computadores

Admins previamente pode seleccionar definições para novos dispositivos Windows 10 computadores utilizando o [Piloto automático do Windows](add-autopilot-devices-and-profile.md). Os utilizadores podem configurar os dispositivos Windows 10 novos ou existentes seguindo os passos descritos neste tópico: [Configurar computadores com o Windows para utilizadores empresariais do Microsoft 365](set-up-windows-devices.md). Para dispositivos existentes os utilizadores são também podem **, opcionalmente,**[mover os ficheiros para OneDrive para a empresa](move-files-to-onedrive.md). Eles também podem utilizar ferramentas de outros fabricantes para mover ficheiros associados ao perfil do Windows para OneDrive.
  
Se a organização utilizar o Windows Server Active Directory no local, pode configurar o Microsoft 365 Business para proteger os dispositivos Windows 10, mantendo o acesso a recursos locais que requerem autenticação local. Siga os passos em [activar dispositivos associados ao domínio de Windows 10 para serem geridos pelo Microsoft 365 Business](manage-windows-devices.md) para configurar esta tarefa. Este é o método preferido e dispositivos neste estado são denominados **híbrido Azure AD associado dispositivos**. 
  
Se mantiver um local do Active Directory que contém alguns locais recursos (tais como partilhas de ficheiros e impressoras), pode conceder acesso a **dispositivos Azure AD associados** a estes recursos seguindo os passos aqui: [acesso local recursos de um Dispositivo Azure AD associados no Microsoft 365 Business](access-resources.md).
  
Depois de ter configurado Windows 10 PCs, pode [instalar automaticamente o Office](auto-install-or-uninstall-office.md) para os dispositivos. 
  
## <a name="contact-support"></a>Contacte o suporte

 **Se precisar de contactar o suporte:**
  
- Contacte o seu parceiro.
    
- Como um administrador de Microsoft 365 Business, tem acesso a nossa equipa de suporte de cliente, **, [contacte o suporte para produtos empresariais - ajuda de administração](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b)**
    

