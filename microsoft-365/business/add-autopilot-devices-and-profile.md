---
title: Utilizar o guia passo a passo para adicionar perfis e dispositivos Autopilot
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
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
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
- AdminTemplateSet
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Saiba como utilizar o Windows AutoPilot para configurar novos dispositivos Windows 10 para a sua empresa, de modo a ficarem prontos para utilização por funcionários.
ms.openlocfilehash: b61ece9a82e12bec088be1b8e2611a13ea7f80d7669911ccaa57df72bf75ee84
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53896464"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Utilizar o guia passo a passo para adicionar perfis e dispositivos Autopilot

Pode utilizar o Windows AutoPilot para configurar novos **dispositivos** Windows 10 para a sua empresa, para que possam ser utilizados quando os der aos seus funcionários.
  
## <a name="device-requirements"></a>Requisitos de dispositivo

Os dispositivos têm de cumprir estes requisitos:
  
- Windows 10, versão 1703 ou posterior
    
- Novos dispositivos que não passaram por Windows experiência prática
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Utilizar o guia de configuração para criar dispositivos e perfis

Se ainda não criou grupos ou perfis de dispositivos, a melhor forma de começar é utilizar o guia passo a passo. Também pode adicionar [dispositivos e](create-and-edit-autopilot-devices.md) [atribuir perfis](create-and-edit-autopilot-profiles.md) aos utilizadores sem utilizar o guia. 
  
1. Vá para o centro de administração em <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .

2. No painel de navegação esquerdo, selecionar **Dispositivos** \> **AutoPilot**.

    ![No centro de administração, selecionar dispositivos e, em seguida, AutoPilot.](../media/AutoPilot.png)
  
2. Na página **AutoPilot,** clique ou toque em **Guia de início**.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. Na página **Carregar .csv** com a lista de dispositivos, navegue para uma localização onde tenha o ficheiro preparado para .CSV e, em seguida, **abrir** \> **Seguinte.** O ficheiro tem de ter três cabeçalhos:
    
    - Coluna A: Número de Série do Dispositivo
    
    - Coluna B: ID do Produto Windows
    
    - Coluna C: Hash do Hardware
    
    Pode obter estas informações com o fornecedor de hardware ou pode utilizar o script do [PowerShell Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) para gerar um ficheiro CSV. 
    
    Para obter mais informações, consulte [Ficheiro CSV da lista de dispositivos](../admin/misc/device-list.md). Também pode transferir um ficheiro de exemplo na página **Carregar um ficheiro .csv com a lista de dispositivos**. 
    
> [!NOTE]
> Este script utiliza WMI para obter as propriedades necessárias para um cliente registar um dispositivo com o Windows Autopilot. Tenha em atenção que é normal que o ficheiro CSV resultante não recolha um valor de ID do Produto Windows (PKID), uma vez que este não é necessário para registar um dispositivo e que o valor PKID seja NULO no CSV de saída está totalmente bem. Só será preenchido o número de série e a hash de hardware.
    
4. Na página **Atribuir um perfil,** pode escolher um perfil existente ou criar um novo. Se ainda não tiver uma, ser-lhe-á pedido para criar uma. 
    
    Um perfil é uma coleção de definições que podem ser aplicadas a um único dispositivo ou a um grupo de dispositivos.
    
    As funcionalidades predefinidas são necessárias e são definidas automaticamente. As funcionalidades predefinidas são:
    
    - Ignorar Cortana, OneDrive e registo OEM.
    
    - Crie uma experiência de início de sessão com a identidade corporativa da sua empresa.
    
    - Ligação seus dispositivos para Azure Active Directory contas e inscreva-os automaticamente para que sejam geridos pelos Microsoft 365 Empresas Premium.
    
    Para obter mais informações, consulte [Acerca das definições do Perfil AutoPilot.](autopilot-profile-settings.md) 
    
5. As outras definições são **Ignorar definições de privacidade** e **Não permitir que o utilizador se torne o administrador local**. Ambas estão configuradas como **Desativado** por predefinição. 
    
    Selecione **Seguinte**.
    
6. **A ação terminar** indica que o perfil que criou (ou que escolheu) será aplicado ao grupo de dispositivos que criou ao carregar a lista de dispositivos. As definições entrarão em vigor assim que os utilizadores dos dispositivos entrarem em ação. Selecione **Fechar**.

## <a name="related-content"></a>Conteúdos relacionados

[Acerca das definições do Perfil AutoPilot](autopilot-profile-settings.md) (artigo)\
[Opções para proteger os seus dispositivos e dados da aplicação](../admin/devices/choose-device-security.md) (artigo)
