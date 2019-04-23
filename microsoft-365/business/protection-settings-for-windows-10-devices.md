---
title: Configurar as definições de proteção de aplicações para dispositivos Windows 10
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
f1_keywords:
- Win10AppPolicy
- O365E_Win10AppPolicy
- BCS365_Win10AppPolicy
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Obter informações sobre como criar uma política de gestão de aplicações e proteger os ficheiros de trabalho no Windows 10 dispositivos.
ms.openlocfilehash: 289c6a74f6ccb53f6a833612a7b4a5bcddd3ea56
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32278194"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a>Configurar as definições de proteção de aplicações para dispositivos Windows 10

## <a name="create-an-app-management-policy-for-windows-10"></a>Criar uma política de gestão de aplicações para Windows 10

Se os seus utilizadores tiverem dispositivos Windows 10 pessoais, nos quais realizam tarefas profissionais, também pode proteger os seus dados nesses dispositivos.
  
1. Iniciar sessão no [Centro de administração](https://go.microsoft.com/fwlink/p/?linkid=837890) com credenciais de administrador global. Selecione o mosaico **Administrador** para aceder ao centro de administração. 
    
2. Nav esquerda, escolher **dispositivos** \> **políticas** \> **Adicionar**.

3. No painel **Adicionar política**, introduza um nome exclusivo para esta política. 
    
4. Em **Tipo de política**, selecione **Gestão de Aplicações para Windows 10**.
    
5. Under ** Device type **, choose either **Personal** or **Company Owned**.
    
6. A opção **Encriptar ficheiros de trabalho** é ativada automaticamente. 
    
7. Defina **Impedir que os utilizadores copiem os dados da empresa para ficheiros pessoais e obrigá-los a guardar os ficheiros de trabalho no OneDrive para Empresas** como **Ativado** se não pretender que os utilizadores guardem ficheiros de trabalho nos respetivos PCs. 
    
8. Expanda **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos** \> configure as definições de acordo com as suas preferências. A opção **Gerir a forma como os utilizadores acedem a dispositivos do Office em dispositivos móveis** está **Desativada** por predefinição, mas recomenda-se que a defina como **Ativada** e aceite os valores predefinidos. Para mais informações, consulte [as definições disponíveis](#available-settings). 
    
    Pode sempre utilizar a ligação **Repor predefinições** para regressar à predefinição. 
    
9. Expanda a opção **Recuperar dados em dispositivos Windows** e recomendamos que a defina como **Ativada**.
    
    Antes de poder aceder à localização do certificado de Agente de Recuperação de Dados, tem de criar um. Para obter instruções, consulte [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate (Criar e verificar um certificado de Agente de Recuperação de Dados (DRA) do Sistema de Encriptação de Ficheiros (EFS))](https://go.microsoft.com/fwlink/p/?linkid=853700).
    
    Por predefinição, os ficheiros de trabalho são encriptados com uma chave secreta que é armazenada no dispositivo e é associada ao perfil do utilizador. Apenas o utilizador pode abrir e desencriptar o ficheiro. No entanto, se um dispositivo for perdido ou um utilizador for removido, um ficheiro pode ficar bloqueado num estado encriptado. Um administrador pode utilizar o certificado de Agente de Recuperação de Dados (DRA) para desencriptar o ficheiro.
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. Expanda a opção **Proteger localizações de rede e de nuvem adicionais** se quiser adicionar domínios ou localizações do SharePoint Online para garantir que os ficheiros em todas as aplicações listadas serão protegidos. Se precisar de introduzir mais do que um item em cada campo, utilize ponto e vírgula (;) entre os itens. 
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. Em seguida, decida **Quem irá ver estas definições?** Se não quiser utilizar o grupo de segurança predefinido, **Todos os Utilizadores**, selecione **Alterar**, selecione os grupos de segurança que irão receber estas definições \> **Selecionar**.
    
12. Por fim, selecione **Adicionar** para guardar a política e atribua-a a todos os dispositivos. 
    
## <a name="available-settings"></a>Definições disponíveis

As seguintes definições estão disponíveis para gerir como os utilizadores acedem a ficheiros de trabalho do Office.
  
Para obter mais informações, consulte [Como é que as funcionalidades de proteção no Microsoft 365 Empresas são mapeadas para as definições do Intune](map-protection-features-to-intune-settings.md).
  
|**Definição**|**Descrição**|
|:-----|:-----|
|Exigir um PIN ou uma impressão digital para aceder às aplicações do Office  <br/> |Se esta definição estiver **Ativada**, os utilizadores terão de fornecer outro meio de autenticação, além do nome de utilizador e da palavra-passe, antes de poderem utilizar aplicações do Office nos respetivos dispositivos móveis.  <br/> |
|Repor o PIN quando o início de sessão falha este número de vezes  <br/> |Para impedir um utilizador não autorizado de adivinhar um PIN aleatoriamente, o PIN será reposto após o número de tentativas incorretas que especificar.  <br/> |
|Exigir que o utilizador inicie a sessão novamente após as aplicações do Office estarem inativas durante  <br/> |Esta definição determina durante quanto tempo um utilizador pode estar inativo antes de ter de voltar a iniciar sessão.  <br/> |
   

