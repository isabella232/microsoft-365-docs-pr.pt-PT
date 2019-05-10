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
ms.openlocfilehash: 8c4a14b4b9dcbf7a30c1e6e0bdd53418a1ab8a03
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660691"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Utilizar o guia passo a passo para adicionar perfis e dispositivos Autopilot

Pode utilizar o piloto automático do Windows para configurar **novos** dispositivos Windows 10 para a sua empresa para que estejam prontos para utilização produtiva, logo que lhes atribua aos seus empregados.
  
## <a name="device-requirements"></a>Requisitos de dispositivo

Os dispositivos têm de cumprir os seguintes requisitos:
  
- Windows 10, versão 1703 ou posterior.
    
- Novos dispositivos que não tenham tido a experiência de configuração inicial do Windows.
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Utilizar o guia de configuração para criar dispositivos e perfis

![Faixa que apontam para https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

Se ainda não tiver criado perfis e grupos de dispositivos, a melhor forma de começar é com o guia passo a passo, mas também pode [adicionar dispositivos](create-and-edit-autopilot-devices.md) e [atribuir perfis](create-and-edit-autopilot-profiles.md) aos mesmos sem utilizar o guia. 
  
1. Vá para o Centro de administração no <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.

2. Nav esquerda do escolher **dispositivos** \> **piloto automático**.

    ![No Centro de administração seleccione os dispositivos e, em seguida, o piloto automático.](media/AutoPilot.png)
  
2. Na página **piloto automático** , clique ou toque em **Iniciar guia**.
    
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
    