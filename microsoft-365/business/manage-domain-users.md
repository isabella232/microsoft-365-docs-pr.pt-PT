---
title: Sincronizar os utilizadores de domínio para o Microsoft 365
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
description: Sincronizar utilizadores controlados por domínios com o Microsoft 365 para o negócio.
ms.openlocfilehash: b477b8a1f35a790d6c49937c973c141ad9f90ad4
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578413"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>Sincronizar os utilizadores de domínio para o Microsoft 365

## <a name="1-prepare-for-directory-synchronization"></a>1. Preparar para a sincronização do diretório 

Antes de sincronizar os seus utilizadores e computadores a partir do domínio do Diretório Ativo local, [reveja Prepare-se para sincronização de diretórios para o Microsoft 365](../enterprise/prepare-for-directory-synchronization.md). Em particular:

   - Certifique-se de que não existem duplicados no seu diretório para os seguintes atributos: **correio,** **proxyAddresses** e **userPrincipalName**. Estes valores devem ser únicos e quaisquer duplicados devem ser removidos.
   
   - Recomendamos que configuure o atributo **userPrincipalName** (UPN) para cada conta de utilizador local para corresponder ao endereço de e-mail primário que corresponde ao utilizador licenciado microsoft 365. Por exemplo: *mary.shelley@contoso.com* em vez *de mary@contoso.local*
   
   - Se o domínio do Diretório Ativo terminar num sufixo não-rotineiro como *.local* ou *.lan*, em vez de um sufixo de internet roteable como *.com* ou *.org*, ajuste o sufixo UPN das contas de utilizador locais primeiro como descrito na [Prepare um domínio não-encaminhável para a sincronização](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md)do diretório . 

O **Run IdFix** no quarto passo (4) abaixo, também garantirá que o seu Diretório Ativo no local está pronto para a sincronização do diretório.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Instalar e configurar a Azure AD Connect

Para sincronizar os seus utilizadores, grupos e contactos do Diretório Ativo local no Azure Ative Directory, instale o Azure Ative Directory Connect e crie sincronização de diretórios. 

 1. No [centro de administração](https://go.microsoft.com/fwlink/p/?linkid=2024339), selecione **Configurar** no navegador esquerdo.

 2. Em **Iniciar sposição e segurança,** escolha **Ver** os **utilizadores do Sync a partir do diretório do seu org.**

 3. No **Sync dos utilizadores da página de diretório do seu org,** escolha **Começar a trabalhar**.

 4. No primeiro passo, a ferramenta IdFix para preparar a sincronização do Diretório.

 5. Siga os passos do assistente para descarregar o Azure AD Connect e use-o para sincronizar os seus utilizadores controlados pelo domínio para o Microsoft 365.


Consulte [a sincronização de diretórios configurar para o Microsoft 365](../enterprise/set-up-directory-synchronization.md) para saber mais.

Ao configurar as suas opções para Azure AD Connect, recomendamos que ative a **sincronização de passwords**, **o Sign-On único sem emenda** e a funcionalidade de writeback de **palavra-passe,** que também é suportada no Microsoft 365 para negócios.

> [!NOTE]
> Existem alguns passos adicionais para a gravação de palavras-passe para além da caixa de verificação no Azure AD Connect. Para obter mais informações, consulte [Como-a-fazer: configurar a gravação da palavra-passe](/azure/active-directory/authentication/howto-sspr-writeback). 

Se também pretende gerir dispositivos Windows 10 unidos por domínio, consulte [ativar dispositivos Windows 10 unidos por domínio para serem geridos pelo Microsoft 365 Business Premium](manage-windows-devices.md) para configurar um AD AD AD Híbrido.