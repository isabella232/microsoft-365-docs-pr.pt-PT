---
title: Ativar a gestão, por parte do Microsoft 365 Business, de dispositivos associados ao domínio Windows 10
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
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Saiba como habilitar o Microsoft 365 para proteger o Diretório Ativo local a se juntar aos dispositivos Windows 10.
ms.openlocfilehash: 93e3364fc94f3878bec13d0a87b17a7d3678a4cc
ms.sourcegitcommit: 9a057e70637dcfe06d4f729a96c02be989cf9e25
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/14/2019
ms.locfileid: "38633275"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Ativar a gestão, por parte do Microsoft 365 Business, de dispositivos associados ao domínio Windows 10

Se a sua organização usar o Diretório Ativo do Windows Server no local, você poderá configurar o Microsoft 365 Business para proteger seus dispositivos Windows 10, mantendo o acesso a recursos no local que exigem autenticação local.
Para configurar essa proteção, você pode implementar **dispositivos híbridos azure ajuntados a AD.** Estes dispositivos são unidos ao seu Diretório Ativo no local e ao seu Diretório Ativo Azure.

Este vídeo descreve os passos de como configurar isso para o cenário mais comum, que também é detalhado nas etapas que se seguem.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a>1. Prepare-se para sincronização do diretório 

Antes de sincronizar seus usuários e computadores do Domínio do Diretório Ativo local, revise [prepare-se para sincronização do diretório para o Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). Em particular:

   - Certifique-se de que não existem duplicatas em seu diretório para os seguintes atributos: **e-mail,** **proxyAddresss**e **userPrincipalName**. Esses valores devem ser únicos e quaisquer duplicatas devem ser removidas.
   
   - Recomendamos que você configure o atributo **do usuárioPrincipalName** (UPN) para cada conta de usuário local para combinar o endereço de e-mail principal que corresponde ao usuário licenciado do Microsoft 365. Por exemplo: *mary.shelley@contoso.com* em vez de *mary@contoso.local*
   
   - Se o domínio diretório ativo termina em um sufixo não routable como *.local* ou *.lan*, em vez de um sufixo routable do Internet tal como *.com* ou *.org,* ajuste o sufixo de UPN dos clientes locais primeiramente como descrito em [prepare um non-routable para o synchronization do diretório.](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization) 

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Instalar e configurar Azure AD Connect

Para sincronizar seus usuários, grupos e contatos do Diretório Ativo local no Diretório Ativo Do Azure, instale o Azure Active Directory Connect e configure a sincronização do diretório. Veja [configurar sincronização do diretório para o Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) para saber mais.

> [!NOTE]
> As etapas são exatamente as mesmas para o Microsoft 365 Business. 

Ao configurar suas opções para o AD Connect do Azure, recomendamos que você habilite sincronização por **senha,** **entrada única perfeita**e o recurso de retorno de **senha,** que também é suportado no Microsoft 365 Business.

> [!NOTE]
> Há algumas etapas adicionais para o writeback da senha além da caixa de verificação no ad do AD do Azure conecta. Para mais informações, veja [como fazer: configure](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback)o writeback de senha . 

## <a name="3-configure-hybrid-azure-ad-join"></a>3. Configure Hybrid Azure AD Join 3. Configure Hybrid AD Join

Antes de ativar os dispositivos Windows 10 para ser o AD Híbrido Azure, certifique-se de conhecer os seguintes pré-requisitos:

   - Você está executando a versão mais recente do Azure AD Connect.

   - A conexão Azure AD sincronizado todos os objetos de computador dos dispositivos que você deseja ser híbrido Azure AD juntou. Se os objetos de computador pertencem a unidades organizacionais específicas (OU), certifique-se de que esses OUs sejam definidos para sincronização em AD azure também se conectar.

Para registrar os dispositivos Windows 10 existentes, incluídos em domínio, conforme o AD Híbrido Azure se juntou, siga as etapas do [Tutorial: Configure o Diretório Ativo Azure híbrido junte-se a domínios gerenciados.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) Isso permite que seu Diretório Ativo existente no local se junte aos computadores do Windows 10 e os torne prontos para a nuvem.
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a>4. Ativar a inscrição automática para o Windows 10

 Para inscrever automaticamente os dispositivos Windows 10 para gerenciamento de dispositivos móveis em intune, [consulte o Dispositivo Do Minque um Windows 10 usando automaticamente a Política do Grupo.](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy) Você pode definir a política do grupo em um nível de computador local ou para operações em massa, você pode usar os modelos do Console de Gerenciamento de Políticas de Grupo e ADMX para criar essa configuração de política de grupo em seu controlador de domínio.

## <a name="5-configure-seamless-single-sign-on"></a>5. Configurar o único sinal perfeito

  O SSO sem costura assina automaticamente os usuários em seus recursos de nuvem microsoft 365 quando eles usam computadores corporativos. Basta implantar uma das duas opções de política de grupo descritas no [Azure Active Directory Seamless Single Sign-On: Início rápido](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature). A opção Política de **Grupo** não permite que os usuários alterem suas configurações, enquanto a opção preferência por política do **grupo** define os valores, mas também os deixa configuráveis pelo usuário.

## <a name="6-set-up-windows-hello-for-business"></a>6. Configurar o Windows Hello para negócios

 O Windows Hello for Business substitui senhas por autenticação forte de dois fatores (2FA) por se inscrever em um computador local. Um fator é um par de chaves assimétrico, e o outro é um PIN ou outro gesto local, como impressão digital ou reconhecimento facial, se o dispositivo o suportar. Recomendamos que você substitua senhas por 2FA e Windows Hello for Business sempre que possível.

Para configurar o Hybrid Windows Hello for Business, reveja a [confiança híbrida do Windows Hello para pré-requisitos](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs)de negócios. Em seguida, siga as instruções em [Configurar Híbrido Windows Olá para configurações de confiança-chave do negócio.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings) 
