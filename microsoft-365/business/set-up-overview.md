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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Aprenda os passos de configuração para o Microsoft 365 Business Premium, desde a subscrição, até adicionar um domínio e utilizadores, até à configuração de políticas de segurança, e muito mais.
ms.openlocfilehash: 46370166a9d5e8c9308b8947513e631c159f0b86
ms.sourcegitcommit: 815229e39a0f905d9f06717f00dc82e2a028fa7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/03/2020
ms.locfileid: "48842136"
---
# <a name="overview-of-setup"></a>Visão geral da configuração

Veja um pequeno vídeo sobre a configuração do Microsoft 365 Business Premium.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Caso tenha considerado este vídeo útil, veja a [série de formação completa para pequenas empresas e as novidades do Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

A maioria dos passos de configuração pode ser feito na configuração guiada, mas as outras opções também estão listadas.

## <a name="step-1-add-your-domain-and-users"></a>Passo 1: Adicione o seu domínio e os seus utilizadores

   - **[Adicione o seu domínio](set-up.md#add-your-domain-to-personalize-sign-in)** (se comprou o seu domínio durante [a inscrição,](sign-up.md)este passo já está feito.)

   - **Adicione os utilizadores**. Pode adicionar utilizadores de qualquer uma das três formas:
        - Na [configuração guiada](set-up.md#add-users-in-the-wizard).
        - Utilize a sincronização do diretório para [adicionar utilizadores utilizando o Azure AD Connect](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) se tiver um diretório ativo no local.
        - Também pode [adicionar utilizadores mais tarde](add-users-m365b.md) no centro de administração.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Passo 2: Configurar políticas de segurança e configurar dispositivos 

  - Utilize a [configuração guiada](set-up.md#protect-your-organization) para configurar as políticas do dispositivo. 
  - Também pode adicionar mais ou editá-los mais tarde no [centro de administração](view-policies-and-devices.md) e no [portal Intune.](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)
  - O assistente de configuração também configurará definições básicas de proteção contra ameaças e prevenção de perdas de dados.
  
  Além das definições de segurança no assistente de configuração, pode aumentar a sua segurança adicionando as seguintes definições:

- **Proteção de malware de e-mail**
- **Anti-phishing no Defender para o Office 365**
- **Arquivo do Exchange Online**
- **Proteção da Informação Azure (Plano 1)**

Para começar, consulte [aumentar a proteção contra ameaças](increase-threat-protection.md) e [configurar funcionalidades de conformidade](set-up-compliance.md).

Consulte também [as 10 melhores formas de garantir o seu Microsoft 365 Business Premium](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) para um roteiro das melhores práticas de segurança.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Passo 3: Configurar e gerir dispositivos do Windows 10

Depois de completar a configuração guiada, irá querer proteger todos os computadores Windows 10 da sua organização.
  
- O Windows 10 Pro é um [pré-requisito](pre-requisites-for-data-protection.md) para o Microsoft 365 Business Premium, mas se tiver o Windows 7 Pro, Windows 8 Pro ou Windows 8.1 Pro, a sua subscrição dá-lhe direito a um [upgrade para o Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
- Siga os passos em [PCs seguros do Windows 10](secure-win-10-pcs.md) para configurar políticas para dispositivos Windows 10.

Quando se junta um dispositivo Do Windows 10 ao Azure AD, as políticas que definiu para computadores Windows 10 são aplicadas ao mesmo. Para obter mais informações, consulte [configurar dispositivos Windows para utilizadores microsoft 365](set-up-windows-devices.md).

## <a name="step-4-install-microsoft-365-apps-for-business"></a>Passo 4: Instalar aplicações microsoft 365 para negócios
- Pode instalar automaticamente o Office nos dispositivos Windows utilizando o [assistente de configuração](set-up.md#deploy-office-365-client-apps).
- Deixe que os utilizadores [instalem aplicações do Office](https://docs.microsoft.com/office365/admin/setup/install-applications) para Windows e dispositivos.
     
## <a name="advanced"></a>Advanced
- **Use o Autopilot para configurar novos dispositivos**
            
     Pode utilizar [o Windows Autopilot](add-autopilot-devices-and-profile.md) para configurar automaticamente **novos** dispositivos Windows 10 para um utilizador, mas pode ser mais fácil obter um [parceiro](https://www.microsoft.com/solution-providers/search) que possa fazê-lo por si. Também pode ir à [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598)e pedir a um especialista em tecnologia na nuvem para configurar novos dispositivos que compra.

- **Acesso aos recursos no local**

     - Se a sua organização utilizar o Windows Server Ative Directory no local, pode configurar o Microsoft 365 Business Premium para proteger os seus dispositivos Windows 10, mantendo ao mesmo tempo o acesso a recursos no local que requerem autenticação local. Siga os passos em [Ativar dispositivos do Windows 10 que se juntam ao domínio para serem geridos pelo Microsoft 365 Business Premium](manage-windows-devices.md) para configurar isto. Este é o método preferido, e os dispositivos neste estado são chamados dispositivos híbridos Azure AD.

    - Se o seu negócio tiver um Ative Directory local que contenha alguns recursos no local (como partilhas de ficheiros e impressoras), pode dar aos seus dispositivos AD ad-ad a estes recursos seguindo os passos aqui: [Aceda aos recursos no local a partir de um dispositivo aderido a Ad AZure no Microsoft 365 Business Premium.](access-resources.md)

## <a name="see-also"></a>Consulte também

[Microsoft 365 para vídeos de formação de negócios](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
