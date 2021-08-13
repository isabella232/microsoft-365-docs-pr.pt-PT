---
title: Sincronizar utilizadores do domínio com a Microsoft 365
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
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
- MOE150
description: Sincronize utilizadores controlados pelo domínio com o Microsoft 365 para empresas.
ms.openlocfilehash: 468fa943df55b12573f0a4f595294e39a146b1850f3c430ac2088a30991c0e60
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53809318"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>Sincronizar utilizadores do domínio com a Microsoft 365

## <a name="1-prepare-for-directory-synchronization"></a>1. Preparar a Sincronização de Diretórios 

Antes de sincronizar os seus utilizadores e computadores a partir do Domínio do Active Directory local, reveja Preparar a [sincronização](../enterprise/prepare-for-directory-synchronization.md)de diretórios para o Microsoft 365 . Em particular:

   - Certifique-se de que não existem duplicados no seu diretório para os seguintes atributos: **mail**, **proxyAddresses** e **userPrincipalName**. Estes valores têm de ser exclusivos e todos os duplicados têm de ser removidos.
   
   - Recomendamos que configure o atributo **userPrincipalName** (UPN) para cada conta de utilizador local para corresponder ao endereço de e-mail principal que corresponde ao utilizador Microsoft 365 licença. Por exemplo: *mary.shelley@contoso.com* em vez de *mary@contoso.local*
   
   - Se o domínio do Active Directory terminar num sufixo não rotativo *como.local* ou *.lan,* em vez de um sufixo de Internet, como *.com* ou *.org,* ajuste primeiro o sufixo UPN das contas de utilizador local conforme descrito em Preparar um domínio não rotativo para a sincronização de [diretórios.](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md) 

O **Executar IdFix** no passo quatro (4) abaixo também irá garantir que o seu Active Directory no local está pronto para sincronização de diretórios.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Instalar e configurar o Azure AD Ligação

Para sincronizar os seus utilizadores, grupos e contactos do Active Directory local para o Azure Active Directory, instale o Azure Active Directory Ligação e configurar a sincronização de diretórios. 

 1. No centro [de administração , selecione](https://go.microsoft.com/fwlink/p/?linkid=2024339) **Configuração** no navegador esquerdo.

 2. Em **Sign-in and security**, selecionar **View**  under **Sync users from your org's directory**.

 3. Na página **Sincronização de utilizadores a partir do diretório da sua** empresa, **selecionar Começar.**

 4. No primeiro passo, execute a ferramenta IdFix para se preparar para a sincronização de diretórios.

 5. Siga os passos do assistente para transferir o Azure AD Ligação e utilize-o para sincronizar os seus utilizadores controlados pelo domínio para Microsoft 365.


Consulte [Configurar a sincronização de diretórios para Microsoft 365](../enterprise/set-up-directory-synchronization.md) mais informações.

À medida que configura as suas opções para o Azure AD Ligação, recomendamos que ative a Sincronização de Palavras-passe , o Sinal de Utilização Única Efetivamente e a funcionalidade de escrita de **palavra-passe,** que também é suportada no Microsoft 365 para empresas.  

> [!NOTE]
> Existem alguns passos adicionais para a escrita de palavras-passe além da caixa de verificação no Azure AD Ligação. Para obter mais informações, consulte [o artigo Como: configurar o writeback da palavra-passe.](/azure/active-directory/authentication/howto-sspr-writeback) 

Se também quiser gerir dispositivos de Windows 10 associados ao domínio, consulte ativar a gestão de dispositivos Windows 10 associados ao domínio pelo [Microsoft 365 Empresas Premium](manage-windows-devices.md) para configurar uma Associação Híbrida do Azure AD.