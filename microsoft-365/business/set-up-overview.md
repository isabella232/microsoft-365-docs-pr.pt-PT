---
title: Descrição geral da configuração
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Descrição geral do conjunto de passos para o Microsoft 365 Business.
ms.openlocfilehash: ae7ed0aab36a6e759e0f0c1fbc3d3183273a284e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/15/2019
ms.locfileid: "35086382"
---
# <a name="overview-of-setup"></a>Descrição geral do programa de configuração

A maior parte dos passos de configuração pode ser efectuado no Assistente de configuração, mas as outras opções também se encontram listadas.


## <a name="step-1-add-your-domain-and-users"></a>Passo 1: Adicionar o domínio e utilizadores

   - **[Adicionar o domínio](set-up.md#add-your-domain-to-personalize-sign-in)** (se adquiriu o seu domínio durante a [inscrição](sign-up.md), este passo já é efectuado.)

    - **Adicionar utilizadores**. Pode fazê-lo em qualquer uma das três formas:
        - No [Assistente](set-up.md#add-users-in-the-wizard).
        - Utilize a sincronização de directório para [Adicionar utilizadores utilizando Azure AD ligar](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) se tiver no local do Active directory.
        - Também pode [Adicionar utilizadores posteriormente](add-users-m365b.md) no Centro de administração.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Passo 2: Definir políticas de segurança e configurar dispositivos 

  - Utilize o [Assistente de configuração](set-up.md#set-up-security-policies-and-device-configurations) para configurar políticas de segurança e dispositivo. 
  - Também pode adicionar mais ou editá-los mais tarde no [Centro de administração](view-policies-and-devices.md) e no [portal de Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - Além das definições de segurança no Assistente de configuração, pode aumentar a segurança, adicionando as seguintes definições:

      - **Mensagem de correio electrónico de protecção contra malware**
      - **Avançadas hiperligações de seguro de protecção de ameaças (ATP)**
      - **Anexos de segurança de ATP**
      - **ATP anti-phishing**
      - **Arquivo do Exchange Online**
      - **Data Loss Prevention (DLP)**
      - **a protecção de informações azure (Plan1**)

          Para obter iniciado, consulte [Configurar políticas de segurança avançada](set-up-advanced-security.md).

        Consulte também [10 principais formas de proteger o seu negócio de 365 da Microsoft](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) para obter um guia de procedimentos recomendados de segurança.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Passo 3: Configurar e gerir os dispositivos Windows 10

   Quando associa um dispositivo Windows 10 a Azure AD, as políticas que configurar no [passo 2](#step-2-set-up-security-policies-and-configure-devices) são aplicadas ao mesmo.

   - Windows 10 Pro é um [requisito prévio](pre-requisites-for-data-protection.md) para Microsoft 365 Business, mas se tiver o Windows 7 Pro, o Windows 8 Pro ou o Windows 8.1 Pro, sua subscrição lhe permitir para uma [actualização para o Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
    - Utilize o [Assistente de configuração](set-up.md#set-up-security-policies-and-device-configurations) para configurar políticas para Windows 10 dispositivos.

## <a name="stes-4-install-office-365-business"></a>Stes 4: Instalar o Office 365 Business
- Pode instalar automaticamente o Office nos dispositivos Windows utilizando o [Assistente de configuração](set-up.md#deploy-office-365-client-apps).
- Automaticamente a [instalar o Office](auto-install-or-uninstall-office.md) partir do Centro de administração.
- Permitir que os utilizadores [instalar aplicações do Office](https://docs.microsoft.com/office365/admin/setup/install-applications) para o Windows e dispositivos.
     
## <a name="advanced"></a>Avançadas
- **Utilizar o piloto automático para configurar novos dispositivos**
            
     Pode utilizar o [Piloto automático do Windows](add-autopilot-devices-and-profile.md) para pré-configurar automaticamente **novos** dispositivos Windows 10 para um utilizador, mas poderá ser mais fácil obter um [parceiro](https://www.microsoft.com/solution-providers/search) que pode fazer isto por si. Também pode ir para o [Arquivo do Microsoft](https://go.microsoft.com/fwlink/?linkid=874598) e peça um perito em tecnologia nuvem configurar novos dispositivos de compras para si.

- **Aceder a recursos no local**

     - Se a organização utilizar o Windows Server Active Directory no local, pode configurar o Microsoft 365 Business para proteger os dispositivos Windows 10, mantendo o acesso a recursos locais que requerem autenticação local. Siga os passos em [activar dispositivos associados ao domínio de Windows 10 para serem geridos pelo Microsoft 365 Business](manage-windows-devices.md) para configurar esta tarefa. Este é o método preferido e dispositivos neste estado são denominados híbrido Azure AD associado dispositivos.

    - Se a empresa possui um local do Active Directory que contém alguns locais recursos (tais como partilhas de ficheiros e impressoras), pode conceder acesso a dispositivos Azure AD associados a estes recursos seguindo os passos aqui: [acesso local recursos de um Dispositivo Azure AD associados no Microsoft 365 Business](access-resources.md).

  