---
title: Visão geral da configuração
f1.keywords:
- NOCSH
ms.author: kwekua
author: kwekua
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Saiba os passos de configuração Microsoft 365 Empresas Premium, desde subscrever, adicionar um domínio e utilizadores, configurar políticas de segurança e muito mais.
ms.openlocfilehash: 7c09dca354781bf92f6bbecca0f3fb9875fb654515fe35c2f96cc780a894a764
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53803228"
---
# <a name="overview-of-setup"></a>Visão geral da configuração

Veja um breve vídeo sobre como Microsoft 365 Empresas Premium configuração.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Caso tenha considerado este vídeo útil, veja a [série de formação completa para pequenas empresas e as novidades do Microsoft 365](../business-video/index.yml).

A maioria dos passos de configuração pode ser feita na configuração guiada, mas as outras opções também são listadas.

## <a name="step-1-add-your-domain-and-users"></a>Passo 1: adicionar o seu domínio e utilizadores

   - **[Adicione o seu domínio](set-up.md#add-your-domain-to-personalize-sign-in)** (se comprou o seu domínio durante a [registo](sign-up.md), este passo já está feito).)

   - **Adicionar utilizadores.** Pode adicionar utilizadores de uma das três formas:
        - Na [configuração guiada](set-up.md#add-users-in-the-wizard).
        - Utilize a sincronização de diretórios para adicionar utilizadores com o [Azure AD Ligação](../enterprise/set-up-directory-synchronization.md) se tiver um Active Directory no local.
        - Também pode [adicionar utilizadores mais tarde](../admin/add-users/add-users.md) no centro de administração.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Passo 2: Configurar políticas de segurança e configurar dispositivos 

  - Utilize a [configuração guiada para](set-up.md#protect-your-organization) configurar políticas de dispositivos. 
  - Também pode adicionar mais ou editá-los mais tarde [no centro de administração e](view-policies-and-devices.md) no portal do [Intune.](/intune/tutorial-walkthrough-intune-portal)
  - O assistente de configuração também irá configurar definições básicas de proteção contra ameaças e prevenção de perda de dados.
  
  Além das definições de segurança no assistente de configuração, pode aumentar a segurança ao adicionar as seguintes definições:

- **Proteção contra software malicónico de e-mail**
- **Anti phishing no Defender para Office 365**
- **Arquivo do Exchange Online**
- **Azure Information Protection (Plano1)**

Para começar, consulte Aumentar [a proteção contra ameaças](increase-threat-protection.md) e [configurar funcionalidades de conformidade.](set-up-compliance.md)

Consulte também [as 10 principais formas de proteger](/office365/admin/security-and-compliance/secure-your-business-data) o Microsoft 365 Empresas Premium para saber mais sobre as melhores práticas de segurança.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Passo 3: configurar e gerir dispositivos Windows 10 dispositivos

Após concluir a configuração guiada, irá querer proteger todos os Windows 10 da sua organização.
  
- Windows 10 Pro é um [](pre-requisites-for-data-protection.md) pré-requisito para o Microsoft 365 Empresas Premium, mas se tiver o Windows 7 Pro, Windows 8 Pro ou Windows 8.1 Pro, a sua subscrição dá-lhe direito a uma atualização para o [Windows 10 Pro.](./upgrade-to-windows-pro-creators-update.md)
- Siga os passos em [PCs Windows 10 segurança](secure-win-10-pcs.md) para configurar políticas para Windows 10 dispositivos.

Quando adere a um Windows 10 Azure AD, as políticas que definir para Windows 10 seus computadores são aplicadas ao mesmo. Para obter mais informações, consulte [Configurar o Windows dispositivos para Microsoft 365 utilizadores.](set-up-windows-devices.md)

## <a name="step-4-install-microsoft-365-apps-for-business"></a>Passo 4: instale o Microsoft 365 Apps para Pequenas e Médias Empresas
- Pode instalar automaticamente os Office dispositivos Windows com o assistente [de configuração.](set-up.md#deploy-office-365-client-apps)
- Permita que [os utilizadores instalem Office](/office365/admin/setup/install-applications) aplicações para Windows dispositivos e dispositivos.
     
## <a name="advanced"></a>Advanced
- **Utilizar o Autopilot para configurar novos dispositivos**
            
     Pode utilizar o [Windows Autopilot](add-autopilot-devices-and-profile.md) para pré-configurar automaticamente novos dispositivos **Windows 10** para um utilizador, [](https://www.microsoft.com/solution-providers/search) mas será mais fácil obter um parceiro que o possa fazer por si. Também pode entrar no Microsoft Store e [pedir](https://go.microsoft.com/fwlink/?linkid=874598)a um especialista em tecnologia da nuvem para configurar os novos dispositivos que comprar.

- **Recursos do Access no local**

     - Se a sua organização utilizar o Windows Server Active Directory no local, pode configurar o Microsoft 365 Empresas Premium para proteger os seus dispositivos Windows 10 e manter o acesso a recursos no local que exigem autenticação local. Siga os passos em [Ativar a gestão Windows 10 dispositivos associados](manage-windows-devices.md) ao domínio Microsoft 365 Empresas Premium configuração. Este é o método preferido e os dispositivos neste estado denominam-se dispositivos associados ao Azure AD Híbrido.

    - Se a sua empresa tiver um Active Directory local que contenha alguns recursos no local (como partilhas de ficheiros e impressoras), pode dar aos seus dispositivos associados ao Azure AD acesso a estes recursos ao seguir os passos aqui: Aceder a recursos no local a partir de um dispositivo associado ao [Azure AD](access-resources.md)no Microsoft 365 Empresas Premium .

## <a name="related-content"></a>Conteúdos relacionados

[Microsoft 365 vídeos de formação para empresas](../business-video/index.yml) (página de ligação)