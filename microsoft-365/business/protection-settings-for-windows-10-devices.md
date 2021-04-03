---
title: Editar ou definir definições de proteção de aplicações para dispositivos Windows 10
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
manager: scotv
audience: Admin
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
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Saiba como criar ou editar políticas de gestão de aplicações e proteger ficheiros de trabalho nos dispositivos pessoais do Windows 10 dos seus utilizadores.
ms.openlocfilehash: aa270c563e6bdce6fd48f8713d7db3ce23921925
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580020"
---
# <a name="set-or-edit-application-protection-settings-for-windows-10-devices"></a>Definir ou editar definições de proteção de aplicações para dispositivos Windows 10

Este artigo aplica-se ao Microsoft 365 Business Premium.

## <a name="edit-an-app-management-policy-for-windows-10"></a>Editar uma política de gestão de aplicações para o Windows 10

1. Vá ao centro de administração em <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .     
2. No navegador esquerdo, escolha **Políticas de** \> **Dispositivos** .
1. Escolha uma política de aplicações do Windows existente e, em seguida, **Edite.**
1. Escolha **Editar** ao lado de uma definição que pretende alterar e, em seguida, **Guardar**.

## <a name="create-an-app-management-policy-for-windows-10"></a>Criar uma política de gestão de aplicações para Windows 10

Se os seus utilizadores tiverem dispositivos Windows 10 pessoais, nos quais realizam tarefas profissionais, também pode proteger os seus dados nesses dispositivos.
  
1. Vá ao centro de administração em <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> . 
2. No navegador esquerdo, escolha **Políticas de Dispositivos** \>  \> **Adicionar**.
3. No painel **Adicionar política**, introduza um nome exclusivo para esta política. 
4. Em **Tipo de política**, selecione **Gestão de Aplicações para Windows 10**.
5. Sob **o tipo dispositivo**, escolha **pessoal** ou **empresa própria.**
6. A opção **Encriptar ficheiros de trabalho** é ativada automaticamente. 
7. Defina **Impedir que os utilizadores copiem os dados da empresa para ficheiros pessoais e obrigá-los a guardar os ficheiros de trabalho no OneDrive para Empresas** como **Ativado** se não pretender que os utilizadores guardem ficheiros de trabalho nos respetivos PCs. 
9. Expandir **Recuperar dados em dispositivos Windows**. Recomendamos que **o** ligue.
    Antes de poder aceder à localização do certificado de Agente de Recuperação de Dados, tem de criar um. Para obter instruções, consulte [Criar e verificar um certificado de Agente de Recuperação de Dados (EFS) do Sistema de Recolha de Dados encriptante (EFS).](/windows/security/information-protection/windows-information-protection/create-and-verify-an-efs-dra-certificate)
    
    Por predefinição, os ficheiros de trabalho são encriptados com uma chave secreta que é armazenada no dispositivo e é associada ao perfil do utilizador. Apenas o utilizador pode abrir e desencriptar o ficheiro. No entanto, se um dispositivo for perdido ou um utilizador for removido, um ficheiro pode ficar bloqueado num estado encriptado. Um administrador pode usar o certificado de Agente de Recuperação de Dados (DRA) para desencriptar o ficheiro.
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. **Expanda-se Proteger localizações adicionais de rede e nuvem** se pretender adicionar domínios adicionais ou localizações online do SharePoint para garantir que os ficheiros em todas as aplicações listadas estão protegidos. Se precisar de introduzir mais do que um item em cada campo, utilize ponto e vírgula (;) entre os itens.
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. Em seguida, decida **Quem irá ver estas definições?** Se não quiser utilizar o grupo de segurança predefinido, **Todos os Utilizadores**, selecione **Alterar**, selecione os grupos de segurança que irão receber estas definições \> **Selecionar**.
12. Por fim, selecione **Adicionar** para guardar a política e atribua-a a todos os dispositivos.