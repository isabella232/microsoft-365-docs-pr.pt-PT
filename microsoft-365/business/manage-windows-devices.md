---
title: Permitir a gestão de dispositivos Windows 10 associados ao domínio pelo Microsoft 365 para empresas
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
description: Saiba como ativar o Microsoft 365 para proteger dispositivos Windows 10 locais associados ao Active-Directory em apenas alguns passos.
ms.openlocfilehash: c9f5a21d993200abcf9ecf1fa236879245e1c153
ms.sourcegitcommit: 4076b43a4b661de029f6307ddc1a989ab3108edb
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2021
ms.locfileid: "51939508"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>Permitir a gestão de dispositivos Windows 10 associados ao domínio pelo Microsoft 365 Business Premium

Se a sua organização utilizar o Windows Server Active Directory no local, pode configurar o Microsoft 365 Business Premium para proteger os seus dispositivos com Windows 10, ao mesmo tempo que mantém o acesso a recursos no local que exigem autenticação local.
Para configurar esta proteção, pode implementar dispositivos **associados ao Azure AD Híbrido.** Estes dispositivos estão associados ao Seu Active Directory no local e ao seu Azure Active Directory.

Este vídeo descreve os passos sobre como configurar esta configuração para o cenário mais comum, que também está detalhado nos passos que se seguem.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a>Antes de começar, certifique-se de que conclui estes passos:
- Sincronize os utilizadores com o Azure AD com o Azure AD Connect.
- Concluir a sincronização da Unidade Organizacional do Azure AD Connect (OU).
- Certifique-se de que todos os utilizadores do domínio que sincroniza têm licenças para o Microsoft 365 Empresas Premium.

Consulte [Sincronizar utilizadores de domínio com a Microsoft](manage-domain-users.md) para ver os passos.

## <a name="1-verify-mdm-authority-in-intune"></a>1. Verificar a Autoridade de MDM no Intune

Vá para [Gestor](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) de Pontos Finais e, na página Microsoft Intune, selecione Inscrição de dispositivos **e,** em seguida, na página **Overview,** certifique-se de que a autoridade **MDM** é **o Intune.**

- Se **a autoridade MDM** for **Nenhuma**, clique na autoridade **de MDM** para a definir como **Intune.**
- Se a **autoridade MDM** for Microsoft Office  **365,** vá para Dispositivos Inscrever dispositivos e utilize a caixa de diálogo Adicionar autoridade MDM à direita para adicionar autoridade MDM do Intune (a caixa de diálogo Adicionar Autoridade MDM só está disponível se a Autoridade de MDM estiver definida para Microsoft Office  >   365).    

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. Verificar se o Azure AD está ativado para aderir a computadores

- Vá para o centro de administração em e selecione <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **Azure Active Directory** (selecione Mostrar tudo se o Azure Active Directory não estiver visível) na lista **Centros de** administração. 
- No centro de **administração do Azure Active Directory,** vá para  **O Azure Active Directory** , selecionar Dispositivos e, em seguida, **Definições do dispositivo**.
- Verificar se os **utilizadores podem associar dispositivos ao Azure AD** está ativado 
    1. Para ativar todos os utilizadores, defina para **Todos.**
    2. Para ativar utilizadores específicos, defina para **Selecionado** para ativar um grupo específico de utilizadores.
        - Adicione os utilizadores de domínio pretendidos sincronizados no Azure AD a um grupo [de segurança](../admin/create-groups/create-groups.md).
        - **Selecione Selecionar** grupos para ativar o âmbito de utilizador da MDM para esse grupo de segurança.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. Verificar se o Azure AD está ativado para a MDM

- Vá para o centro de administração em e selecione <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **Endpoint Managemen** t (selecione Mostrar tudo se o Gestor de Pontos  **Finais** não estiver visível)
- No centro **de administração do Microsoft Endpoint Manager, vá a** **Dispositivos Inscrição** Automática do  >    >  **Windows Windows.**  >  
- Verifique se o âmbito de utilizador da MDM está ativado.

    1. Para inscrever todos  os computadores, defina para Todos para inscrever automaticamente todos os computadores dos utilizadores associados ao Azure AD e a novos computadores quando os utilizadores adicionarem uma conta escolar ao Windows.
    2. Defina **para Alguns** para inscrever os computadores de um grupo de utilizadores específico.
        -  Adicione os utilizadores de domínio pretendidos sincronizados no Azure AD a um grupo [de segurança](../admin/create-groups/create-groups.md).
        -  **Selecione Selecionar** grupos para ativar o âmbito de utilizador da MDM para esse grupo de segurança.

## <a name="4-create-the-required-resources"></a>4. Crie os recursos necessários 

O desempenho das tarefas necessárias para configurar a associação híbrida do [Azure AD](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) foi simplificado através da utilização do cmdlet [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) que se encontra no módulo [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) powerShell. Ao invocar este cmdlet, este irá criar e configurar a política de grupo e o ponto de ligação de serviço necessários.

Pode instalar este módulo ao invocar o seguinte a partir de uma instância do PowerShell:

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> Recomendamos que instale este módulo no Windows Server a executar o Azure AD Connect.

Para criar a política de grupo e o ponto de ligação de serviço necessários, invoque o cmdlet [Initialize-SecMgmtHybirdDeviceEnrollment.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) Irá precisar das suas credenciais de administrador global do Microsoft 365 Empresas Premium quando realizar esta tarefa. Quando estiver pronto para criar os recursos, invoque o seguinte:

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

O primeiro comando estabelecerá uma ligação com a nuvem da Microsoft e, quando lhe for pedido, especifique as suas credenciais de administrador global do Microsoft 365 Empresas - Versão Premium.

## <a name="5-link-the-group-policy"></a>5. Associar a Política de Grupo

1. Na Consola de Gestão da Política de Grupo (GPMC), clique com o botão direito do rato na localização onde quer ligar a política e selecione Ligar um *GPO existente...* no menu de contexto.
2. Selecione a política criada no passo acima e, em seguida, clique **em OK.**

## <a name="get-the-latest-administrative-templates"></a>Obter os Modelos Administrativos mais recentes

Se não vir a política Ativar a inscrição automática da MDM utilizando as credenciais do **Azure AD** predefinida, é possível que não tenha o ADMX instalado para Windows 10, versão 1803 ou posterior. Para corrigir o problema, siga estes passos (Nota: a MDM.admx mais recente é retrocompatível):

1.  Transferir: [Modelos Administrativos (.admx) para Windows 10 de Outubro de 2020 Atualização (20H2).](https://www.microsoft.com/download/102157)
2.  Instale o pacote num Controlador de Domínio.
3.  Navegue, consoante a versão Modelos Administrativos para a pasta: **C:\Programas (x86)\Política de Grupo da Microsoft\Atualização de Outubro de 2020 (20H2)**.
4.  Rename **the Policy Definitions** folder in the above path to **PolicyDefinitions.**
5.  Copie a **pasta PolicyDefinitions** para a sua partilha SYSVOL, por predefinição localizada em **C:\Windows\SYSVOL\domain\Policies.** 
    -   Se tenciona utilizar um loja de políticas central para todo o domínio, adicione os conteúdos da PolicyDefinitions aí.
6.  Caso tenha vários Controladores de Domínio, aguarde até que a replicação do SYSVOL esteja disponível para que as políticas sejam disponibilizadas. Este procedimento também funcionará em qualquer versão futura dos Modelos Administrativos.

Neste momento, deverá conseguir ver a política Ativar a inscrição automática de MDM utilizando **as credenciais do Azure AD predefinida** disponíveis.

## <a name="related-content"></a>Conteúdo relacionado

Sincronizar utilizadores do domínio com o [Microsoft 365](manage-domain-users.md) (artigo) Criar um grupo no tutorial do centro de administração (artigo): Configurar [a](../admin/create-groups/create-groups.md) associação híbrida do [Azure Active Directory](/azure/active-directory/devices/hybrid-azuread-join-managed-domains.md) para domínios geridos (artigo)