---
title: Configurar as definições de proteção de aplicações para dispositivos Windows 10
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Saiba como criar uma política de gerenciamento de aplicativos e proteger arquivos de trabalho em dispositivos Windows 10.
ms.openlocfilehash: 0e1221e533418166b80afd94431414016774f247
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575784"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a>Configurar as definições de proteção de aplicações para dispositivos Windows 10

## <a name="create-an-app-management-policy-for-windows-10"></a>Criar uma política de gestão de aplicações para Windows 10

Se os seus utilizadores tiverem dispositivos Windows 10 pessoais, nos quais realizam tarefas profissionais, também pode proteger os seus dados nesses dispositivos.
  
1. Vá para o centro de administração <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>em. 
    
2. No NAV esquerdo, escolha **Adicionar** **políticas** \> de **dispositivos** \> .

3. No painel **Adicionar política**, introduza um nome exclusivo para esta política. 
    
4. Em **Tipo de política**, selecione **Gestão de Aplicações para Windows 10**.
    
5. Em **tipo de dispositivo**, escolha **pessoal** ou **empresa possuída**.
    
6. A opção **Encriptar ficheiros de trabalho** é ativada automaticamente. 
    
7. Defina **Impedir que os utilizadores copiem os dados da empresa para ficheiros pessoais e obrigá-los a guardar os ficheiros de trabalho no OneDrive para Empresas** como **Ativado** se não pretender que os utilizadores guardem ficheiros de trabalho nos respetivos PCs. 
    
9. Expanda a opção **Recuperar dados em dispositivos Windows** e recomendamos que a defina como **Ativada**.
    
    Antes de poder aceder à localização do certificado de Agente de Recuperação de Dados, tem de criar um. Para obter instruções, consulte [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate (Criar e verificar um certificado de Agente de Recuperação de Dados (DRA) do Sistema de Encriptação de Ficheiros (EFS))](https://go.microsoft.com/fwlink/p/?linkid=853700).
    
    Por predefinição, os ficheiros de trabalho são encriptados com uma chave secreta que é armazenada no dispositivo e é associada ao perfil do utilizador. Apenas o utilizador pode abrir e desencriptar o ficheiro. No entanto, se um dispositivo for perdido ou um utilizador for removido, um ficheiro pode ficar bloqueado num estado encriptado. Um administrador pode utilizar o certificado de Agente de Recuperação de Dados (DRA) para desencriptar o ficheiro.
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. Expanda a opção **Proteger localizações de rede e de nuvem adicionais** se quiser adicionar domínios ou localizações do SharePoint Online para garantir que os ficheiros em todas as aplicações listadas serão protegidos. Se precisar de introduzir mais do que um item em cada campo, utilize ponto e vírgula (;) entre os itens.
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. Em seguida, decida **Quem irá ver estas definições?** Se não quiser utilizar o grupo de segurança predefinido, **Todos os Utilizadores**, selecione **Alterar**, selecione os grupos de segurança que irão receber estas definições \> **Selecionar**.
    
12. Por fim, selecione **Adicionar** para guardar a política e atribua-a a todos os dispositivos. 