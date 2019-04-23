---
title: Utilizar o guia passo a passo para adicionar perfis e dispositivos Autopilot
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection:
- M365-subscription-management
- M365-identity-device-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Obter informações sobre como utilizar o piloto automático do Windows para configurar novos dispositivos Windows 10 para a sua empresa.
ms.openlocfilehash: e0802ddcc0964d0b8d102f7dbdb9116b33cdcf58
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32277153"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Utilizar o guia passo a passo para adicionar perfis e dispositivos Autopilot

Pode utilizar o Windows AutoPilot para configurar novos dispositivos com Windows 10 da sua empresa, para que estejam prontos para uma utilização produtiva assim que os der aos seus funcionários.
  
## <a name="device-requirements"></a>Requisitos de dispositivo

Os dispositivos têm de cumprir os seguintes requisitos:
  
- Windows 10, versão 1703 ou posterior.
    
- Novos dispositivos que não tenham tido a experiência de configuração inicial do Windows.
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Utilizar o guia de configuração para criar dispositivos e perfis

Se ainda não tiver criado perfis e grupos de dispositivos, a melhor forma de começar é com o guia passo a passo, mas também pode [adicionar dispositivos](create-and-edit-autopilot-devices.md) e [atribuir perfis](create-and-edit-autopilot-profiles.md) aos mesmos sem utilizar o guia. 
  
1. No centro de administração do Microsoft 365 Business, localize o cartão **Ações do dispositivo** e selecione **Implementar o Windows com o AutoPilot**.
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. Na página **Preparar Windows**, clique ou toque em **Guia de introdução**.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. Na página **Carregar um ficheiro .csv com a lista de dispositivos**, procure uma localização com o ficheiro .CSV preparado e, em seguida, selecione **Abrir** \> **Seguinte**. O ficheiro deverá ter três cabeçalhos:
    
  - Coluna A: Número de Série do Dispositivo
    
  - Coluna B: ID do Produto Windows
    
  - Coluna C: Hash do Hardware
    
    Pode obter esta informação através do fabricante de hardware ou pode utilizar o [script do PowerShell Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) que irá gerar um ficheiro CSV. 
    
    Para obter mais informações, consulte [Ficheiro CSV da lista de dispositivos](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Também pode transferir um ficheiro de exemplo na página **Carregar um ficheiro .csv com a lista de dispositivos**. 
    
4. Na página **Atribuir um perfil**, pode selecionar um perfil existente ou criar um novo. Se ainda não tiver um, ser-lhe-á pedido que crie um novo. 
    
    Um perfil é uma coleção de definições que podem ser aplicadas a um único dispositivo ou a um grupo de dispositivos.
    
    As funcionalidades predefinidas são necessárias e serão configuradas automaticamente. As funcionalidades predefinidas são:
    
  - O registo da Cortana, do OneDrive e do OEM é ignorado.
    
  - Crie uma experiência de início de sessão com a identidade corporativa da sua empresa.
    
  - Os seus dispositivos serão ligados às contas do Azure Active Directory e automaticamente inscritos para serem geridos pelo Microsoft 365 Business.
    
    Para obter mais informações, consulte
    
    [Sobre as definições do Perfil AutoPilot](autopilot-profile-settings.md) . 
    
5. As outras definições são **Ignorar definições de privacidade** e **Não permitir que o utilizador se torne o administrador local**. Ambas estão configuradas como **Desativado** por predefinição. 
    
    Selecione **Seguinte**.
    
6. A página **Concluído** indica que o perfil criado (ou selecionado) será aplicado ao grupo de dispositivos criado ao atualizar a lista de dispositivos. Estas definições entrarão em vigor assim que os utilizadores dos dispositivos iniciarem sessão. Selecione **Fechar**.
    