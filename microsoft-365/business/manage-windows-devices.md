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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Saiba como habilitar o Microsoft 365 para proteger dispositivos do Windows 10 ingressados no AD local.
ms.openlocfilehash: d1dbfc6a35d54db653ae0f911fad05ac2ce0a993
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288041"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Ativar a gestão, por parte do Microsoft 365 Business, de dispositivos associados ao domínio Windows 10

Se sua organização usa o Active Directory do Windows Server no local, você pode configurar o Microsoft 365 Business para proteger seus dispositivos Windows 10, enquanto ainda mantém o acesso a recursos locais que exigem autenticação local.
Para configurar isso, você pode implementar **dispositivos ingressados no Azure ad híbridos**. Estes são dispositivos que estão associados ao Active Directory no local e ao Azure Active Directory.

O vídeo a seguir detalha as etapas de como configurá-lo para o cenário mais comum que também é detalhado nas etapas a seguir.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a>1. Prepare-se para a sincronização de diretórios 

Antes de sincronizar seus usuários e computadores do domínio local do Active Directory, revise [Prepare-se para a sincronização de diretórios para o Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). Em particular:

   - Certifique-se de que não existem duplicados no directório para os seguintes atributos: **mail**, **proxyAddresses**e **userPrincipalName**. Esses valores devem ser exclusivos e quaisquer duplicatas devem ser removidas..
   
   - É recomendável que o atributo **userPrincipalName** (UPN) para cada conta de usuário local esteja configurado para corresponder ao endereço de email principal que corresponde ao usuário licenciado do Microsoft 365. Por exemplo, *Mary. Shelley<span>@ Contoso<span> . com* em vez de *Mary @ contoso. local*
   
   - Se o domínio do Active Directory terminar em um sufixo não roteável como *. local* ou *. LAN*, em vez de um sufixo roteável da Internet, como *. com* ou *. org*, será necessário ajustar o sufixo UPN das contas de usuário local primeiro, conforme descrito em [Prepare um domínio não roteável para a sincronização de diretórios](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

## <a name="2-install-and-configure-azure-ad-connect"></a>2. instalar e configurar o Azure AD Connect

Para sincronizar seus usuários, grupos e contatos do Active Directory local para o Active Directory do Azure, instale o Azure Active Directory Connect e configure a sincronização de diretórios. Consulte [Configurar a sincronização de diretórios para o Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) para saber mais.

> [!NOTE]
> As etapas são exatamente as mesmas para o Microsoft 365 Business. 

À medida que você configura suas opções para o Azure AD Connect, recomendamos habilitar a **sincronização de senha** e o **logon único sem emenda**, bem como o recurso de **write-back de senha** , que também é suportado no Microsoft 365 Business.

> [!NOTE]
> Existem algumas etapas adicionais para Write-back de senha além da caixa de seleção no Azure AD Connect. Para obter mais informações, consulte [como fazer: configurar o Write-back de senha](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

## <a name="3-configure-hybrid-azure-ad-join"></a>3. configurar a associação híbrida do Azure AD

Antes de habilitar os dispositivos do Windows 10 para serem ingressados no Azure AD híbrido, você deve se certificar de que atende aos seguintes pré-requisitos:

   - Você está executando a versão mais recente do Azure AD Connect.

   - O Azure AD Connect sincronizou todos os objetos de computador dos dispositivos que você deseja que sejam ingressados no Azure AD híbrido. Se os objetos de computador pertencerem a unidades organizacionais específicas (UO), certifique-se de que essas OUs estão definidas para sincronização no Azure AD conectar também.

Para registrar dispositivos existentes do Windows 10 ingressados no domínio como ingressado no Azure AD híbrido, siga as etapas no [tutorial: configurar junção híbrida do Azure Active Directory para domínios gerenciados](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join). Isso habilitará o híbrido para que seu Active Directory local existente ingresse em computadores com Windows 10 e torne-os prontos para a nuvem.
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a>4. habilitar o registro automático para o Windows 10

 Para inscrever automaticamente dispositivos Windows 10 para gerenciamento de dispositivo móvel no Intune, consulte [inscrever um dispositivo Windows 10 automaticamente usando a diretiva de grupo](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy). Você pode definir a diretiva de grupo em um nível de computador local ou para operações em massa, você pode criar essa configuração de diretiva de grupo no seu controlador de domínio usando o console de gerenciamento de diretiva de grupo e modelos ADMX.

## <a name="5-configure-seamless-single-sign-on"></a>5. configurar o início de sessão único sem emenda

  O SSO sem emenda assinará automaticamente os usuários em seus recursos de nuvem do Microsoft 365 quando usarem computadores corporativos. Basta implementar uma das duas opções de política de grupo descritas no [Azure Active Directory sem costura único Sign-on: início rápido](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature). A opção **de diretiva de grupo** não permite que os usuários alterem suas configurações, enquanto a opção **de preferência de diretiva de grupo** define os valores, mas também os deixa configuráveis pelo usuário.

## <a name="6-set-up-windows-hello-for-business"></a>6. configurar o Windows Hello para empresas

 O Windows Hello para empresas substitui senhas com autenticação de dois fatores forte (2FA) para fazer login em um computador local. Um fator é um par de chaves assimétrica, e o outro é um PIN ou outro gesto local, como impressão digital ou reconhecimento facial, se o seu dispositivo o suportar. Recomendamos que você substitua senhas com 2FA e Windows Hello para empresas sempre que possível.

Para configurar o Windows Hello para empresas híbrida, examine os [pré-requisitos de confiança de chave híbrida do Windows Hello para empresas](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs). Em seguida, siga as instruções em [configurar as configurações de confiança de chave híbrida do Windows Hello para empresas](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings). 
