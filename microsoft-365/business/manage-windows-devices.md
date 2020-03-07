---
title: Ativar a gestão, por parte do Microsoft 365 Business, de dispositivos associados ao domínio Windows 10
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
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Saiba como permitir que o Microsoft 365 proteja os dispositivos locais do Windows 10 em apenas alguns passos.
ms.openlocfilehash: 625eb7ac344b060409101d650ff30044d073f5bf
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561466"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Ativar a gestão, por parte do Microsoft 365 Business, de dispositivos associados ao domínio Windows 10

Se a sua organização utilizar o Diretório Ativo do Windows Server no local, pode configurar o Microsoft 365 Business para proteger os seus dispositivos Windows 10, mantendo ao mesmo tempo o acesso aos recursos no local que requerem autenticação local.
Para configurar esta proteção, pode implementar **dispositivos ad ad ad híbridos Azure**. Estes dispositivos juntam-se tanto ao diretório ativo no local como ao seu Diretório Ativo Azure.

Este vídeo descreve os passos para configurar isto para o cenário mais comum, que também é detalhado nos passos que se seguem.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a>1. Preparar para sincronização de diretório 

Antes de sincronizar os seus utilizadores e computadores do domínio de diretório ativo local, reveja [prepare-se para sincronização de diretório sincronia para o Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). Em especial:

   - Certifique-se de que não existem duplicados no seu diretório para os seguintes atributos: **correio,** **proxyAddresss**, e **userPrincipalName**. Estes valores devem ser únicos e quaisquer duplicados devem ser removidos.
   
   - Recomendamos que configure o atributo do **userPrincipalName** (UPN) para cada conta de utilizador local para corresponder ao endereço de e-mail primário que corresponde ao utilizador licenciado da Microsoft 365. Por exemplo: *mary.shelley@contoso.com* em vez de *mary@contoso.local*
   
   - Se o domínio do Diretório Ativo terminar num sufixo não repreensível como *.local* ou *.lan*, em vez de um sufixo resaída à Internet, como *.com* ou *.org,* ajuste primeiro o sufixo UPN das contas de utilizador local, tal como descrito na [Prepare um domínio não repreensível para sincronização](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization)de diretórios. 

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Instale e configure a Ligação AD Azure

Para sincronizar os seus utilizadores, grupos e contactos do Diretório Ativo local em Azure Ative Directory, instale o Azure Ative Directory Connect e instale sincronização de diretórios. Consulte a [sincronização do diretório para o Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) para saber mais.

> [!NOTE]
> Os passos são exatamente os mesmos para o Microsoft 365 Business. 

À medida que configura as suas opções para O Azure AD Connect, recomendamos que ative a **Sincronização**de Passwords, **Um Único Sinal**perfeito e a funcionalidade de redação de **palavra-passe,** que também é suportada no Microsoft 365 Business.

> [!NOTE]
> Existem alguns passos adicionais para a reescrita de palavra-passe para além da caixa de verificação no Azure AD Connect. Para mais informações, consulte [Como: configurar a reescrita da palavra-passe](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

## <a name="3-configure-hybrid-azure-ad-join"></a>3. Configure Hybrid Azure AD Aderir

Antes de ativar os dispositivos Do Windows 10 para ser Hybrid Azure AD, certifique-se de que cumpre os seguintes pré-requisitos:

   - Estás a executar a versão mais recente do Azure AD Connect.

   - A ligação Azure AD sincronizou todos os objetos informáticos dos dispositivos que pretende ser híbrido Azure AD. Se os objetos informáticos pertencerem a unidades organizacionais específicas (OU), certifique-se de que estas OUs estão definidas para sincronização em Azure AD connect também.

Para registar os dispositivos Windows 10 existentes à medida que o Hybrid Azure AD se juntou, siga os passos no [Tutorial: Configure hybrid Azure Ative Directory juntam-se para domínios geridos](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join). Este diretório ativo no local permite que o seu Diretório Ativo no local se junte aos computadores Windows 10 e os torne em nuvem prontas.
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a>4. Ativar a inscrição automática para o Windows 10

 Para inscrever automaticamente os dispositivos do Windows 10 para gestão de dispositivos móveis em Intune, consulte [Inscrever automaticamente um dispositivo Windows 10 utilizando automaticamente a Política de Grupo](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy). Pode definir a Política de Grupo a nível de computador local, ou para operações a granel, pode utilizar os modelos de Consola de Gestão de Políticas de Grupo e DEM para criar esta definição de Política de Grupo no seu Controlador de Domínio.

## <a name="5-configure-seamless-single-sign-on"></a>5. Configurar um único signo sem emenda

  O SSO SSO sem emenda sintetmente assina automaticamente os utilizadores nos seus recursos na nuvem Microsoft 365 quando utilizam computadores corporativos. Basta implementar uma das duas opções de Política de Grupo descritas no [Azure Ative Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature). A opção Política de **Grupo** não permite que os utilizadores alterem as suas definições, enquanto a opção **De Preferência** política do grupo define os valores, mas também os deixa configurados pelo utilizador.

## <a name="6-set-up-windows-hello-for-business"></a>6. Configurar o Windows Hello for Business

 O Windows Hello for Business substitui as palavras-passe por uma autenticação forte de dois fatores (2FA) para a assinatura num computador local. Um fator é um par de chaves assimétrica, e o outro é um PIN ou outro gesto local, como impressão digital ou reconhecimento facial se o seu dispositivo o suportar. Recomendamos que substitua as palavras-passe por 2FA e Windows Hello for Business sempre que possível.

Para configurar o Hybrid Windows Hello for Business, reveja a [chave híbrida do Windows Hello for Business Pré-requisitos.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs) Em seguida, siga as instruções em [Configurar as definições](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings)de confiança da chave Híbrida Configure Hello for Business . 
