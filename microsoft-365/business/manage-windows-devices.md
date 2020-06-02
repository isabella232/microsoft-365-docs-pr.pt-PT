---
title: Permitir que dispositivos Windows 10 unidos por domínio sejam geridos pela Microsoft 365 para negócios
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Saiba como permitir que o Microsoft 365 proteja os dispositivos locais do Windows 10, aderidos ao Active-Directory, em apenas alguns passos.
ms.openlocfilehash: 7bfe5da8701a17712fa249eac99a22b8d5a1b2d1
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471053"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>Permitir que dispositivos Windows 10 unidos por domínio sejam geridos pelo Microsoft 365 Business Premium

Se a sua organização utilizar o Windows Server Ative Directory no local, pode configurar o Microsoft 365 Business Premium para proteger os seus dispositivos Windows 10, mantendo ao mesmo tempo o acesso a recursos no local que requerem autenticação local.
Para configurar esta proteção, pode implementar **dispositivos híbridos Azure AD.** Estes dispositivos estão ligados tanto ao seu Ative Directory como ao seu Diretório Ativo Azure.

Este vídeo descreve os passos para como configurar isto para o cenário mais comum, que também é detalhado nos passos que se seguem.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a>1. Preparar para a sincronização do diretório 

Antes de sincronizar os seus utilizadores e computadores a partir do domínio do Diretório Ativo local, [reveja Prepare-se para sincronização de diretórios para o Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). Em particular:

   - Certifique-se de que não existem duplicados no seu diretório para os seguintes atributos: **correio,** **proxyAddresses**e **userPrincipalName**. Estes valores devem ser únicos e quaisquer duplicados devem ser removidos.
   
   - Recomendamos que configuure o atributo **userPrincipalName** (UPN) para cada conta de utilizador local para corresponder ao endereço de e-mail primário que corresponde ao utilizador licenciado microsoft 365. Por exemplo: *mary.shelley@contoso.com* em vez *de mary@contoso.local*
   
   - Se o domínio ative Directory terminar num sufixo não-encaminhável como *.local* ou *.lan*, em vez de um sufixo de internet rotable como *.com* ou *.org*, ajuste o sufixo UPN das contas de utilizador locais primeiro como descrito na [Prepare um domínio não-encaminhável para sincronização de diretórios](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Instalar e configurar a Azure AD Connect

Para sincronizar os seus utilizadores, grupos e contactos do Diretório Ativo local no Azure Ative Directory, instale o Azure Ative Directory Connect e crie sincronização de diretórios. Consulte [a sincronização do diretório configurado para o Office 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) para saber mais.

> [!NOTE]
> Os passos são exatamente os mesmos para o Microsoft 365 para negócios. 

Ao configurar as suas opções para Azure AD Connect, recomendamos que ative a **sincronização de passwords**, **o Sign-On único sem emenda**e a funcionalidade de writeback de **palavra-passe,** que também é suportada no Microsoft 365 para negócios.

> [!NOTE]
> Existem alguns passos adicionais para a gravação de palavras-passe para além da caixa de verificação no Azure AD Connect. Para obter mais informações, consulte [Como-a-fazer: configurar a gravação da palavra-passe](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

## <a name="3-configure-hybrid-azure-ad-join"></a>3. Configurar híbrido Azure Ad Join

Antes de ativar os dispositivos do Windows 10 para serem híbridos Azure AD, certifique-se de que cumpre os seguintes requisitos:

   - Estás a executar a versão mais recente do Azure AD Connect.

   - A ligação AD AD azure sincronizou todos os objetos de computador dos dispositivos que pretende ser híbrido Azure AD ligados. Se os objetos do computador pertencerem a unidades organizacionais específicas (OU), certifique-se de que estas OUs estão definidas para sincronização em Azure AD connect também.

Para registar os dispositivos existentes do Windows 10 unidos como Híbrido Azure AD aderiu, siga os passos no [Tutorial: Configure híbrido Azure Ative Directy junte-se a domínios geridos](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join). Isto permite que o seu Ative Directory existente no local se junte aos computadores windows 10 e os torne em nuvem.
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a>4. Permitir a inscrição automática para o Windows 10

 Para inscrever automaticamente dispositivos Windows 10 para gestão de dispositivos móveis no Intune, consulte [inscrever automaticamente um dispositivo Windows 10 utilizando a Política de Grupo](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy). Pode definir a Política de Grupo a nível de computador local, ou para operações a granel, pode utilizar os modelos de Consola de Gestão de Políticas de Grupo e ADMX para criar esta definição de Política de Grupo no seu Controlador de Domínio.

## <a name="5-configure-seamless-single-sign-on"></a>5. Configurar um único sinal sem emenda

  O Seamless SSO assina automaticamente os utilizadores nos seus recursos em nuvem Microsoft 365 quando utilizam computadores corporativos. Basta implementar uma das duas opções de Política de Grupo descritas no [Azure Ative Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature). A opção **Política de Grupo** não permite que os utilizadores alterem as suas definições, enquanto a opção De Preferência de Política de **Grupo** define os valores, mas também os deixa configuráveis pelo utilizador.

## <a name="6-set-up-windows-hello-for-business"></a>6. Configurar o Windows Hello para o Negócio

 O Windows Hello for Business substitui as palavras-passe por uma autenticação forte de dois fatores (2FA) para iniciar sessão num computador local. Um fator é um par de chave assimétrica, e o outro é um PIN ou outro gesto local, como impressão digital ou reconhecimento facial se o seu dispositivo o suportar. Recomendamos que substitua as palavras-passe por 2FA e Windows Hello para Negócios sempre que possível.

Para configurar o Hybrid Windows Hello for Business, reveja o [fundo híbrido Windows Hello for Business Prerequisites](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs). Em seguida, siga as instruções em [Configurar Híbrido Windows Hello for Business key trust settings](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings). 
