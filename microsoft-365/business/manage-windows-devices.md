---
title: Permitir que dispositivos Windows 10 unidos por domínio sejam geridos pela Microsoft 365 para negócios
f1.keywords:
- CSH
ms.author: efrene
author: efrene
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
description: Saiba como permitir que o Microsoft 365 proteja os dispositivos locais do Windows 10, aderidos ao Active-Directory, em apenas alguns passos.
ms.openlocfilehash: 8a45c6959bee368491c5c6424e3713300c443779
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580140"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>Permitir que dispositivos Windows 10 unidos por domínio sejam geridos pelo Microsoft 365 Business Premium

Se a sua organização utilizar o Windows Server Ative Directory no local, pode configurar o Microsoft 365 Business Premium para proteger os seus dispositivos Windows 10, mantendo ao mesmo tempo o acesso a recursos no local que requerem autenticação local.
Para configurar esta proteção, pode implementar **dispositivos híbridos Azure AD.** Estes dispositivos estão ligados tanto ao seu Ative Directory como ao seu Diretório Ativo Azure.

Este vídeo descreve os passos para como configurar isto para o cenário mais comum, que também é detalhado nos passos que se seguem.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a>Antes de começar, certifique-se de completar estes passos:
- Sincronizar os utilizadores para Azure AD com Azure AD Connect.
- Sincronização completa da Unidade Organizacional de Ligação Azure (OU).
- Certifique-se de que todos os utilizadores de domínio sincronizados têm licenças para o Microsoft 365 Business Premium.

Consulte [os utilizadores de domínio sincronizados com a Microsoft](manage-domain-users.md) para os passos.

## <a name="1-verify-mdm-authority-in-intune"></a>1. Verificar a Autoridade MDM em Intune

Vá ao [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) e na página Microsoft Intune, selecione **a inscrição** do Dispositivo , em seguida, na página **'Vista Geral',** certifique-se de que **a autoridade MDM** está **Intune**.

- Se **a autoridade do MDM** não for **nenhuma,** clique na **autoridade do MDM** para defini-la para **Intune**.
- Se **a autoridade do MDM** for o Microsoft Office **365,** vá aos   >  **dispositivos de inscrição** de dispositivos e use o diálogo **da autoridade Add MDM** no direito de adicionar a autoridade **Intune MDM** (o diálogo da Autoridade add **MDM** só está disponível se a **Autoridade MDM** estiver definida para o Microsoft Office 365).

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. Verifique se a Azure AD está ativada para unir computadores

- Vá ao centro de administração <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> e selecione **Azure Ative Directory** (selecione Mostrar tudo se o Diretório Ativo Azure não estiver visível) na lista de **centros de administração.** 
- No **centro de administração Azure Ative,** vá ao **Azure Ative Directory,** escolha **Dispositivos** e, em seguida, **configurações do Dispositivo**.
- Verifique se **os utilizadores podem juntar-se a dispositivos para Azure AD** está ativado 
    1. Para ativar todos os utilizadores, desa um pouco de **tudo**.
    2. Para permitir utilizadores específicos, desatado para **selecionar** para permitir um grupo específico de utilizadores.
        - Adicione os utilizadores de domínio desejado sincronizados em Azure AD a um [grupo de segurança](../admin/create-groups/create-groups.md).
        - Escolha **Grupos Selecionados** para ativar o âmbito do utilizador MDM para esse grupo de segurança.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. Verifique se a Azure AD está ativada para o MDM

- Vá ao centro de administração <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  e selecione **Endpoint Managemen** t (selecione **Mostrar tudo** se **o Endpoint Manager** não estiver visível)
- No **centro de administração do Microsoft Endpoint Manager,** aceda a **Inscrições**  >    >  Automáticas de **Inscrição**  >  **no** Windows do Windows .
- Verifique se o âmbito do utilizador DO MDM está ativado.

    1. Para inscrever todos os computadores, descreva para **All** para inscrever automaticamente todos os computadores de utilizador que se unem ao Azure AD e aos novos computadores quando os utilizadores adicionarem uma conta de trabalho ao Windows.
    2. Definir para **Alguns** para inscrever os computadores de um grupo específico de utilizadores.
        -  Adicione os utilizadores de domínio desejado sincronizados em Azure AD a um [grupo de segurança](../admin/create-groups/create-groups.md).
        -  Escolha **Grupos Selecionados** para ativar o âmbito do utilizador MDM para esse grupo de segurança.

## <a name="4-create-the-required-resources"></a>4. Criar os recursos necessários 

A execução das tarefas necessárias para configurar a [junção híbrida Azure AD](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) foi simplificada através da utilização do cmdlet [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) encontrado no módulo [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell. Quando invocar este cmdlet, criará e configurará o ponto de ligação de serviço e a política de grupo necessários.

Pode instalar este módulo invocando o seguinte a partir de uma instância do PowerShell:

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> Recomenda-se que instale este módulo no Servidor do Windows que executa o Azure AD Connect.

Para criar o ponto de ligação de serviço e a política de grupo necessários, irá invocar o cmdlet [Initialize-SecMgmtHybirdDeviceEnrollment.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) Vai precisar das suas credenciais de administração global Microsoft 365 Business Premium ao realizar esta tarefa. Quando estiver pronto para criar os recursos, invoque o seguinte:

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

O primeiro comando estabelecerá uma ligação com a nuvem microsoft, e quando for solicitado, especifique as suas credenciais de administração global Microsoft 365 Business Premium.

## <a name="5-link-the-group-policy"></a>5. Ligue a Política de Grupo

1. Na Consola de Gestão de Políticas de Grupo (GPMC), clique à direita no local onde pretende ligar a política e selecione *Link um GPO existente...* a partir do menu de contexto.
2. Selecione a política criada no passo acima e, em seguida, clique **em OK**.

## <a name="get-the-latest-administrative-templates"></a>Obtenha os mais recentes modelos administrativos

Se não vir a política Ative a **inscrição automática de MDM utilizando credenciais AD predefinidas**, pode ser porque não tem o ADMX instalado para o Windows 10, versão 1803 ou mais tarde. Para corrigir o problema, siga estes passos (Nota: o mais recente MDM.admx é compatível com o contrário):

1.  Download: [Modelos Administrativos (.admx) para atualização do Windows 10 de outubro de 2020 (20H2)](https://www.microsoft.com/download/102157).
2.  Instale a embalagem num controlador de domínio.
3.  Navegue, dependendo da versão De Modelos Administrativos para a pasta: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 outubro 2020 Update (20H2)**.
4.  Rebatize a pasta **Definições de Política** no caminho acima para **Definições de Políticas**.
5.  Copie a pasta **PolicyDefinitions** para a sua quota SYSVOL, por padrão localizada em **C:\Windows\SYSVOL\domain\Policies**. 
    -   Se planeia utilizar uma loja de política central para todo o seu domínio, adicione o conteúdo das Definições de Política.
6.  Caso tenha vários Controladores de Domínio, aguarde que o SYSVOL se reproduza para que as políticas estejam disponíveis. Este procedimento funcionará para qualquer versão futura dos Modelos Administrativos também.

Neste momento, deverá ser capaz de ver a política Ativar a **inscrição automática de MDM utilizando credenciais AD predefinidas** disponíveis.