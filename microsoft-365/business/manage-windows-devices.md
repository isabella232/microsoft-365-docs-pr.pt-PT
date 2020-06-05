---
title: Permitir que dispositivos Windows 10 unidos por domínio sejam geridos pela Microsoft 365 para negócios
f1.keywords:
- CSH
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
description: Saiba como permitir que o Microsoft 365 proteja os dispositivos locais do Windows 10, aderidos ao Active-Directory, em apenas alguns passos.
ms.openlocfilehash: 857651081fb10856d28dd419333ebef655388407
ms.sourcegitcommit: e6e704cbd9a50fc7db1e6a0cf5d3f8c6cbb94363
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/04/2020
ms.locfileid: "44564958"
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

Vá a portal.azure.com e no topo da pesquisa de página para Intune.
Na página Microsoft Intune, selecione **a inscrição** do Dispositivo e na página **'Vista Geral'** certifique-se de que **a autoridade MDM** é **Intune**.

- Se **a autoridade do MDM** não for **nenhuma,** clique na **autoridade do MDM** para defini-la para **Intune**.
- Se **a autoridade do MDM** for o Microsoft Office **365,** vá aos **Devices**  >  **dispositivos de inscrição** de dispositivos e use o diálogo **da autoridade Add MDM** no direito de adicionar a autoridade **Intune MDM** (o diálogo da Autoridade add **MDM** só está disponível se a **Autoridade MDM** estiver definida para o Microsoft Office 365).

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. Verifique se a Azure AD está ativada para unir computadores

- Vá ao centro de administração <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> e selecione **Azure Ative Directory** (selecione Mostrar tudo se o Diretório Ativo Azure não estiver visível) na lista de **centros de administração.** 
- No **centro de administração Azure Ative,** vá ao **Azure Ative Directory,** escolha **Dispositivos** e, em seguida, **configurações do Dispositivo**.
- Verifique se**os utilizadores podem juntar-se a dispositivos para Azure AD** está ativado 
    1. Para ativar todos os utilizadores, desa um pouco de **tudo**.
    2. Para permitir utilizadores específicos, desatado para **selecionar** para permitir um grupo específico de utilizadores.
        - Adicione os utilizadores de domínio desejado sincronizados em Azure AD a um [grupo de segurança](../admin/create-groups/create-groups.md).
        - Escolha **Grupos Selecionados** para ativar o âmbito do utilizador MDM para esse grupo de segurança.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. Verifique se a Azure AD está ativada para o MDM

- Vá ao centro de administração <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> e selecione **Endpoint Managemen**t (selecione **Mostrar tudo** se **o Endpoint Manager** não estiver visível)
- No **centro de administração do Microsoft Endpoint Manager,** aceda a **Inscrições**  >  **Windows**  >  Automáticas de**Inscrição**  >  **no**Windows do Windows .
- Verifique se o âmbito do utilizador DO MDM está ativado.

    1. Para inscrever todos os computadores, descreva para **All** para inscrever automaticamente todos os computadores de utilizador que se unem ao Azure AD e aos novos computadores quando os utilizadores adicionarem uma conta de trabalho ao Windows.
    2. Definir para **Alguns** para inscrever os computadores de um grupo específico de utilizadores.
        -  Adicione os utilizadores de domínio desejado sincronizados em Azure AD a um [grupo de segurança](../admin/create-groups/create-groups.md).
        -  Escolha **Grupos Selecionados** para ativar o âmbito do utilizador MDM para esse grupo de segurança.

## <a name="4-set-up-service-connection-point-scp"></a>4. Configurar o ponto de ligação de serviço (SCP)

Estes passos são simplificados a partir da [configuração híbrida azure ad join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join). Para completar os passos, precisa de utilizar o Azure AD Connect e as suas palavras-passe de administração global e de administração de administração do Microsoft 365 Business Premium.

1.  Inicie o Azure AD Connect e, em seguida, selecione **Configure**.
2.  Na página **de tarefas adicionais,** selecione **opções do dispositivo configurar**e, em seguida, selecione **Seguinte**.
3.  Na página **'Vista Geral',** selecione **Seguinte**.
4.  Na página **Connect to Azure AD,** insira as credenciais de um administrador global para o Microsoft 365 Business Premium.
5.  Na página de opções do **Dispositivo,** selecione **Configure Hybrid Azure AD ,** e, em seguida, selecione **Next**.
6.  Na página **SCP,** para cada floresta onde deseja Azure AD Connect para configurar o SCP, complete os seguintes passos e, em seguida, selecione **Seguinte**:
    - Verifique a caixa ao lado do nome da floresta. A floresta deve ser o seu nome de domínio AD.
    - Sob a coluna **Serviço de Autenticação,** abra o dropdown e selecione o nome de domínio correspondente (deve haver apenas uma opção).
    - **Selecione Adicionar** para introduzir as credenciais de administrador de domínio.  
7.  Na página de **sistemas operativos do Dispositivo,** selecione apenas dispositivos ligados ao domínio do Windows 10 ou posteriormente ligados ao domínio.
8.  Na página **Pronto para configurar,** selecione **Configurar**.
9.  Na página completa da **Configuração,** selecione **Sair**.


## <a name="5-create-a-gpo-for-intune-enrollment--admx-method"></a>5. Criar um GPO para inscrição intune – método ADMX

Utilização . Arquivo de modelo ADMX.

1.  Inicie sessão no servidor AD, procure e abra **Server Manager**  >  **Tools**  >  **gestão de políticas do Grupo**de Ferramentas do Gestor do Servidor .
2.  Selecione o nome de domínio em **Domínios** e clique com o botão direito **Objetos de Política** de Grupo para selecionar **Novos**.
3.  Dê ao novo GPO um nome, por exemplo , "*Cloud_Enrollment*" e, em seguida, selecione **OK**.
4.  Clique com o botão direito no novo GPO em **Objetos de Política de Grupo** e selecione **Editar**.
5.  No Editor de **Gestão de Políticas**de Grupo, aceda a políticas **de configuração de computador**  >  **Policies**  >  **Modelos Administrativos**De Componentes do  >  **Windows**  >  **.**
6. Clique com o botão direito **Ativar a inscrição automática de MDM utilizando credenciais AD Ad predefinidas** e, em seguida, selecione **Enabled**  >  **Enabled OK**. Feche a janela do editor.

> [!IMPORTANT]
> Se não vir a política Ative a **inscrição automática de MDM utilizando credenciais AD predefinidas**, consulte [obter os modelos administrativos mais recentes](#get-the-latest-administrative-templates).

## <a name="6-deploy-the-group-policy"></a>6. Implementar a Política de Grupo

1.  No Gestor do Servidor, em **"Domínios** > objetos de Política de Grupo", selecione o GPO do Passo 3 acima, por exemplo "Cloud_Enrollment".
2.  Selecione o **separador Âmbito** para o seu GPO.
3.  No separador Scope da GPO, clique com o botão direito no link para o domínio em **Links**.
4.  Selecione **Aplicada** para implementar o GPO e, em seguida, **OK** no ecrã de confirmação.

## <a name="get-the-latest-administrative-templates"></a>Obtenha os mais recentes modelos administrativos

Se não vir a política Ative a **inscrição automática de MDM utilizando credenciais AD predefinidas**, pode ser porque não tem o ADMX instalado para o Windows 10, a versão 1803, a versão 1809 ou a versão 1903. Para corrigir o problema, siga estes passos (Nota: o mais recente MDM.admx é compatível com o contrário):

1.  Download: [Modelos Administrativos (.admx) para Windows 10 May 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).
2.  Instale a embalagem no Controlador de Domínio Primário (PDC).
3.  Navegar, dependendo da versão para a pasta: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 maio 2019 Update (1903) v3**.
4.  Rebatize a pasta **Definições de Política** no caminho acima para **Definições de Políticas**.
5.  **Copiar Pasta dedefinições de cópia** para **C:\Windows\SYSVOL\domain\Policies**. 
    -   Se planeia utilizar uma loja de política central para todo o seu domínio, adicione o conteúdo das Definições de Política.
6.  Reinicie o Controlador de Domínio Primário para que a política esteja disponível. Este procedimento funcionará para qualquer versão futura também.

Neste momento, deverá ser capaz de ver a política Ativar a **inscrição automática de MDM utilizando credenciais AD predefinidas** disponíveis.

