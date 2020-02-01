---
title: Visão geral da configuração
f1.keywords:
- NOCSH
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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Visão geral dos passos de configuração para o Microsoft 365 Business.
ms.openlocfilehash: 07cbd4fd187f78474783db848ac9b69068d2b44a
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/29/2020
ms.locfileid: "41595071"
---
# <a name="overview-of-setup"></a>Visão geral da configuração

Veja um pequeno vídeo sobre a configuração do Microsoft 365 Business.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Caso tenha considerado este vídeo útil, consulte a [série de formação completa para pequenas empresas e as novidades do Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

A maioria dos passos de configuração podem ser feitos no assistente de configuração, mas as outras opções também estão listadas.

## <a name="step-1-add-your-domain-and-users"></a>Passo 1: Adicione o seu domínio e os utilizadores

   - **[Adicione o seu domínio](set-up.md#add-your-domain-to-personalize-sign-in)** (se comprou o seu domínio durante a [inscrição,](sign-up.md)este passo já está feito.)

    - **Adicione utilizadores**. Pode adicionar utilizadores de qualquer uma das três formas:
        - No [feiticeiro.](set-up.md#add-users-in-the-wizard)
        - Utilize a sincronização do diretório para [adicionar utilizadores utilizando o Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) se tiver um diretório Ativo no local.
        - Também pode [adicionar utilizadores mais tarde](add-users-m365b.md) no centro de administração.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Passo 2: Configurar políticas de segurança e configurar dispositivos 

  - Utilize o assistente de [configuração](set-up.md#protect-your-organization) para configurar as políticas do dispositivo. 
  - Também pode adicioná-los mais ou editá-los mais tarde no [centro de administração](view-policies-and-devices.md) e no [portal Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - O assistente de configuração também criará definições básicas de proteção contra ameaças e prevenção de perdas de dados.
  
  Além das definições de segurança no assistente de configuração, pode aumentar a sua segurança adicionando as seguintes definições:

- **Proteção por e-mail de malware**
- **ATP anti-phishing**
- **Arquivo do Exchange Online**
- **Proteção da Informação Azure (Plano 1)**

Para começar, consulte aumentar a [proteção contra ameaças](increase-threat-protection.md) e [configurar as funcionalidades de conformidade.](set-up-compliance.md)

Consulte também [as 10 melhores formas de garantir o seu Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) para um roteiro das melhores práticas de segurança.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Passo 3: Configurar e gerir dispositivos windows 10

Depois de executar o assistente de configuração, vai querer procectar todos os computadores Windwos 10 da sua organização.
  
- O Windows 10 Pro é um [pré-requisito](pre-requisites-for-data-protection.md) para o Microsoft 365 Business, mas se tiver windows 7 Pro, Windows 8 Pro ou Windows 8.1 Pro, a sua subscrição dá-lhe direito a um [upgrade para o Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
- Siga os passos em [Computadores Seguros do Windows 10](secure-win-10-pcs.md) para definir políticas para dispositivos Windows 10.

Quando se junta a um dispositivo Windows 10 para o Azure AD, as políticas definidas para computadores Windows 10 são aplicadas ao mesmo. Para mais informações, consulte [Configurar dispositivos Windows para utilizadores do Microsoft 365 Business](set-up-windows-devices.md).

## <a name="step-4-install-office-365-business"></a>Passo 4: Instalar escritório 365 Negócios
- Pode instalar automaticamente o Office nos dispositivos Windows utilizando o assistente de [configuração](set-up.md#deploy-office-365-client-apps).
- Deixe os utilizadores [instalarem aplicações do Office](https://docs.microsoft.com/office365/admin/setup/install-applications) para Windows e dispositivos.
     
## <a name="advanced"></a>Avançado
- **Utilize o Autopilot para configurar novos dispositivos**
            
     Pode utilizar o [Windows Autopilot](add-autopilot-devices-and-profile.md) para configurar automaticamente **novos** dispositivos Windows 10 para um utilizador, mas pode ser mais fácil conseguir um [parceiro](https://www.microsoft.com/solution-providers/search) que possa fazê-lo por si. Também pode ir à [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598)e pedir a um especialista em tecnologia na nuvem que crie novos dispositivos que adquira.

- **Acesso aos recursos no local**

     - Se a sua organização utilizar o Diretório Ativo do Windows Server no local, pode configurar o Microsoft 365 Business para proteger os seus dispositivos Windows 10, mantendo ao mesmo tempo o acesso aos recursos no local que requerem autenticação local. Siga os passos em dispositivos Enable [do Windows 10 que serão geridos pelo Microsoft 365 Business](manage-windows-devices.md) para configurar esta configuração. Este é o método preferido, e os dispositivos neste estado são chamados dispositivos híbridos Azure AD.

    - Se o seu negócio tiver um Diretório Ativo local que contenha alguns recursos no local (como ações de ficheiros e impressoras), pode dar aos seus dispositivos ad-ad-join ing e stão a seguir os passos aqui: [Aceder aos recursos no local a partir de um dispositivo azure ad-join no Microsoft 365 Business](access-resources.md).

## <a name="see-also"></a>Consulte também

[Vídeos de formação do Microsoft 365 Business](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
