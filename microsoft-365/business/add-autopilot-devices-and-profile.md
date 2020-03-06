---
title: Utilizar o guia passo a passo para adicionar perfis e dispositivos Autopilot
f1.keywords:
- NOCSH
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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Saiba como utilizar o Windows AutoPilot para configurar novos dispositivos Windows 10 para o seu negócio, para que estejam prontos para uso dos colaboradores.
ms.openlocfilehash: 8449d5a3672a20b0cd1ba61bbda863073138c04c
ms.sourcegitcommit: 26e4d5091583765257b7533b5156daa373cd19fe
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/06/2020
ms.locfileid: "42550393"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Utilizar o guia passo a passo para adicionar perfis e dispositivos Autopilot

Pode utilizar o Windows AutoPilot para configurar **novos** dispositivos Windows 10 para o seu negócio, para que estejam prontos a ser utilizados quando os entregar aos seus colaboradores.
  
## <a name="device-requirements"></a>Requisitos de dispositivo

Os dispositivos devem satisfazer estes requisitos:
  
- Windows 10, versão 1703 ou mais tarde
    
- Novos dispositivos que não passaram pela experiência do Windows fora da caixa
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Utilizar o guia de configuração para criar dispositivos e perfis

[![Etiqueta que informa que o centro de administração está a mudar e que pode encontrar mais detalhes em aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Se ainda não criou grupos de dispositivos ou perfis, a melhor maneira de começar é utilizando o guia passo a passo. Também pode [adicionar dispositivos](create-and-edit-autopilot-devices.md) e [atribuir-lhes perfis](create-and-edit-autopilot-profiles.md) sem utilizar o guia. 
  
1. Vá ao centro de <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>administração em .

2. No painel de navegação à esquerda, escolha **Dispositivos** \> **AutoPilot**.

    ![No centro de administração, escolha os dispositivos e, em seguida, o AutoPilot.](../media/AutoPilot.png)
  
2. Na página **AutoPilot,** clique ou toque no **guia Iniciar**.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. No **ficheiro Upload .csv com página de dispositivos,** navegue para um local onde tenha o preparado . Ficheiro CSV, em **seguida, Abrir** \> **Seguinte**. O ficheiro deve ter três cabeçalhos:
    
    - Coluna A: Número de Série do Dispositivo
    
    - Coluna B: ID do Produto Windows
    
    - Coluna C: Hash do Hardware
    
    Pode obter esta informação do seu fornecedor de hardware, ou pode utilizar o [script Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) para gerar um ficheiro CSV. 
    
    Para obter mais informações, consulte [Ficheiro CSV da lista de dispositivos](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Também pode transferir um ficheiro de exemplo na página **Carregar um ficheiro .csv com a lista de dispositivos**. 
    
4. Na página de atribuir uma página de **perfil,** pode escolher um perfil existente ou criar um novo. Se ainda não tiver um, será solicitado a criar um. 
    
    Um perfil é uma coleção de definições que podem ser aplicadas a um único dispositivo ou a um grupo de dispositivos.
    
    As funcionalidades predefinidas são necessárias e são definidas automaticamente. As funcionalidades predefinidas são:
    
    - Skip Cortana, OneDrive e registo OEM.
    
    - Crie uma experiência de início de sessão com a identidade corporativa da sua empresa.
    
    - Ligue os seus dispositivos às contas do Diretório Ativo Do Azure e inscreva-os automaticamente para serem geridos pelo Microsoft 365 Business.
    
    Para mais informações, consulte as definições de [Perfil AutoPilot](autopilot-profile-settings.md). 
    
5. As outras definições são **Ignorar definições de privacidade** e **Não permitir que o utilizador se torne o administrador local**. Ambas estão configuradas como **Desativado** por predefinição. 
    
    Selecione **Seguinte**.
    
6. **Está feito** indica que o perfil que criou (ou escolheu) será aplicado ao grupo de dispositivos que criou através do upload da lista de dispositivos. As definições estarão em vigor quando os utilizadores do dispositivo iniciarem o seu inicio. Selecione **Fechar**.
    
