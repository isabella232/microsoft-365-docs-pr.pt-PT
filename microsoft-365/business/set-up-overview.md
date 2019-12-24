---
title: Visão geral da configuração
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
description: Visão geral das etapas de configuração para o Microsoft 365 Business.
ms.openlocfilehash: 4aca617015cceb85ca35c8d8ada7b83d1416d959
ms.sourcegitcommit: 178ecb21cacdeaf440f3df2fe6e539e9127fcf15
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/23/2019
ms.locfileid: "40850810"
---
# <a name="overview-of-setup"></a>Visão geral da configuração

Assista a um pequeno vídeo sobre a configuração do Microsoft 365 Business.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Se você achou este vídeo útil, confira a série de [treinamento completo para pequenas empresas e as novas para a Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

A maioria das etapas de configuração pode ser feita no assistente de configuração, mas as outras opções também estão listadas.

## <a name="step-1-add-your-domain-and-users"></a>Etapa 1: Adicione seu domínio e usuários

   - **[Adicione o seu domínio](set-up.md#add-your-domain-to-personalize-sign-in)** (se você comprou o seu domínio durante a [inscrição,](sign-up.md)esta etapa já está feito.)

    - **Adicionar usuários.** Você pode adicionar usuários de qualquer uma das três maneiras:
        - No [mago.](set-up.md#add-users-in-the-wizard)
        - Use sincronização do diretório para adicionar usuários usando o AD Connect do [Azure](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) se você tiver um diretório ativo no local.
        - Você também pode [adicionar usuários mais tarde](add-users-m365b.md) no centro de administração.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Etapa 2: Configurar políticas de segurança e configurar dispositivos 

  - Use o assistente de [configuração](set-up.md#protect-your-organization) para configurar as políticas do dispositivo. 
  - Você também pode adicionar mais ou editá-los mais tarde no centro de [administração](view-policies-and-devices.md) e no [portal Intune.](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)
  - O assistente de configuração também criará configurações básicas de proteção contra ameaças e prevenção de perdas de dados.
  
  Além das configurações de segurança no assistente de configuração, você pode aumentar sua segurança adicionando as seguintes configurações:

- **Proteção de malware por e-mail**
- **Atp anti-phishing ATP anti-phishing**
- **Arquivo do Exchange Online**
- **Proteção da Informação Azure (Plan1**)

Para começar, veja a criação de políticas de [segurança avançadas.](set-up-advanced-security.md)

Veja também [as 10 principais maneiras de proteger seu Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) para um roteiro das melhores práticas de segurança.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Etapa 3: Configurar e gerenciar dispositivos Windows 10

Depois de executar o assistente configurar, você vai querer proctect todos os windwos 10 computadores em sua organização.
  
- O Windows 10 Pro é um [pré-requisito](pre-requisites-for-data-protection.md) para o Microsoft 365 Business, mas se você tiver o Windows 7 Pro, o Windows 8 Pro ou o Windows 8.1 Pro, sua assinatura lhe dá direito a uma atualização para o [Windows 10 Pro.](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update)
- Siga as etapas em [PCs do Windows 10 seguros](secure-win-10-pcs.md) para configurar políticas para dispositivos Windows 10.

Quando você junta um dispositivo Windows 10 ao AD do Azure, as políticas que você define para computadores Windows 10 são aplicadas a ele. Para mais informações, consulte [dispositivos Windows para usuários do Microsoft 365 Business.](set-up-windows-devices.md)

## <a name="step-4-install-office-365-business"></a>Etapa 4: Instale o escritório 365 negócio
- Você pode instalar automaticamente o Office nos dispositivos Windows usando o assistente de [configuração.](set-up.md#deploy-office-365-client-apps)
- Permita que os usuários [instalem aplicativos do Office](https://docs.microsoft.com/office365/admin/setup/install-applications) para Windows e dispositivos.
     
## <a name="advanced"></a>Avançado
- **Use o piloto automático para configurar novos dispositivos**
            
     Você pode usar o [Windows Autopilot](add-autopilot-devices-and-profile.md) para pré-configurar automaticamente **novos** dispositivos Windows 10 para um usuário, mas pode ser mais fácil conseguir um [parceiro](https://www.microsoft.com/solution-providers/search) que possa fazer isso por você. Você também pode ir à [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598)e pedir a um especialista em tecnologia de nuvem para configurar novos dispositivos que você compra.

- **Acesso a recursos no local**

     - Se a sua organização usar o Diretório Ativo do Windows Server no local, você poderá configurar o Microsoft 365 Business para proteger seus dispositivos Windows 10, mantendo o acesso a recursos no local que exigem autenticação local. Siga as etapas dos [dispositivos Windows 10 incluídos no domínio habilitado para serem gerenciados pelo Microsoft 365 Business](manage-windows-devices.md) para configurar isso. Este é o método preferido, e os dispositivos neste estado são chamados dispositivos unidos a Anúncio híbrido sucateado a AD.

    - Se a sua empresa tiver um Diretório Ativo local que contém alguns recursos no local (como compartilhamentos de arquivos e impressoras), você poderá dar aos dispositivos vinculados a Azure a dispositivos vinculados a esses recursos seguindo os passos aqui: [acesse recursos locais de um dispositivo azure vinculado a AD no Microsoft 365 Business](access-resources.md).

## <a name="see-also"></a>See also

[Microsoft 365 Vídeos de treinamento de negócios](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
