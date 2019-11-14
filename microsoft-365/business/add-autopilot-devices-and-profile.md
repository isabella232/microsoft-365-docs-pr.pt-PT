---
title: Utilizar o guia passo a passo para adicionar perfis e dispositivos Autopilot
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Saiba como usar o Windows AutoPilot para configurar novos dispositivos Windows 10 para sua empresa.
ms.openlocfilehash: 5f40dac57285b83da57d4506bac58e562475522c
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/14/2019
ms.locfileid: "38323101"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Utilizar o guia passo a passo para adicionar perfis e dispositivos Autopilot

Você pode usar o Windows AutoPilot para configurar **novos** dispositivos Windows 10 para sua empresa para que eles estejam prontos para uso quando você os dá aos seus funcionários.
  
## <a name="device-requirements"></a>Requisitos de dispositivo

Os dispositivos devem atender a esses requisitos:
  
- Windows 10, versão 1703 ou mais tarde
    
- Novos dispositivos que não passaram pela experiência do Windows fora da caixa
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Utilizar o guia de configuração para criar dispositivos e perfis

[![Etiqueta que informa que o centro de administração está a mudar e que pode encontrar mais detalhes em aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Se você ainda não criou grupos ou perfis de dispositivos, a melhor maneira de começar é usando o guia passo a passo. Você também pode [adicionar dispositivos](create-and-edit-autopilot-devices.md) e [atribuir perfis](create-and-edit-autopilot-profiles.md) a eles sem usar o guia. 
  
1. Vá para o centro <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>de administração em .

2. No painel de navegação esquerdo, escolha **dispositivos** \> **AutoPilot**.

    ![No centro de administração, escolha dispositivos e, em seguida, AutoPilot.](media/AutoPilot.png)
  
2. Na página **AutoPilot,** clique ou toque **no guia Iniciar.**
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. No **arquivo Upload .csv com lista de página de dispositivos,** navegue para um local onde você tenha o preparado. Arquivo CSV, em seguida, **abrir** \> em **seguida**. O arquivo deve ter três cabeçalhos:
    
    - Coluna A: Número de Série do Dispositivo
    
    - Coluna B: ID do Produto Windows
    
    - Coluna C: Hash do Hardware
    
    Você pode obter essas informações do fornecedor de hardware ou pode usar o [script Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) para gerar um arquivo CSV. 
    
    Para obter mais informações, consulte [Ficheiro CSV da lista de dispositivos](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Também pode transferir um ficheiro de exemplo na página **Carregar um ficheiro .csv com a lista de dispositivos**. 
    
4. Na página de **perfil da Atribuição** de uma, você pode escolher um perfil existente ou criar um novo. Se você ainda não tem um, você será solicitado a criar um. 
    
    Um perfil é uma coleção de definições que podem ser aplicadas a um único dispositivo ou a um grupo de dispositivos.
    
    Os recursos padrão são necessários e são definidos automaticamente. As funcionalidades predefinidas são:
    
    - Pule o registro Cortana, OneDrive e OEM.
    
    - Crie uma experiência de início de sessão com a identidade corporativa da sua empresa.
    
    - Conecte seus dispositivos às contas do Diretório Ativo do Azure e os inscrevê-los automaticamente para serem gerenciados pelo Microsoft 365 Business.
    
    Para mais informações, veja sobre as configurações do [perfil do Piloto Automático.](autopilot-profile-settings.md) 
    
5. As outras definições são **Ignorar definições de privacidade** e **Não permitir que o utilizador se torne o administrador local**. Ambas estão configuradas como **Desativado** por predefinição. 
    
    Selecione **Seguinte**.
    
6. **Você está pronto** indica que o perfil que você criou (ou escolheu) será aplicado ao grupo de dispositivos criados por carregar a lista de dispositivos. As configurações estarão em vigor quando os usuários do dispositivo entrarem em seguida. Selecione **Fechar**.
    