---
title: Editar ou definir definições de proteção de aplicações para Windows 10 dispositivos
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
description: Saiba como criar ou editar políticas de gestão de aplicações e proteger os ficheiros de trabalho nos dispositivos Windows 10 utilizadores.
ms.openlocfilehash: 6d38d1765e0a331516b2261870112d530ab4ee50f24c6defba95964ea4d9dcfa
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53852669"
---
# <a name="set-or-edit-application-protection-settings-for-windows-10-devices"></a>Definir ou editar as definições de proteção de aplicações para Windows 10 dispositivos

Este artigo aplica-se a Microsoft 365 Empresas Premium.

## <a name="edit-an-app-management-policy-for-windows-10"></a>Editar uma política de gestão de aplicações para Windows 10

1. Vá para o centro de administração em <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .     
2. No navegador esquerdo, selecionar Políticas **de** \> **Dispositivos** .
1. Selecionar uma política Windows aplicação e, em seguida, **Editar.**
1. **Selecionar Editar** junto a uma definição que pretende alterar e, em seguida, **Guardar.**

## <a name="create-an-app-management-policy-for-windows-10"></a>Criar uma política de gestão de aplicações para Windows 10

Se os seus utilizadores tiverem dispositivos Windows 10 pessoais, nos quais realizam tarefas profissionais, também pode proteger os seus dados nesses dispositivos.
  
1. Vá para o centro de administração em <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> . 
2. No navegador esquerdo, selecionar Adicionar **Políticas** \> **de** \> **Dispositivos.**
3. No painel **Adicionar política**, introduza um nome exclusivo para esta política. 
4. Em **Tipo de política**, selecione **Gestão de Aplicações para Windows 10**.
5. Em **Tipo de dispositivo**, escolha Pessoal **ou** Propriedade **da Empresa**.
6. A opção **Encriptar ficheiros de trabalho** é ativada automaticamente. 
7. Defina **Impedir que os utilizadores copiem os dados da empresa para ficheiros pessoais e obrigá-los a guardar os ficheiros de trabalho no OneDrive para Empresas** como **Ativado** se não pretender que os utilizadores guardem ficheiros de trabalho nos respetivos PCs. 
9. Expanda **a ação Recuperar dados em Windows dispositivos**. Recomendamos que a **deslige.**
    Antes de poder aceder à localização do certificado de Agente de Recuperação de Dados, tem de criar um. Para obter instruções, consulte Criar e verificar um certificado de Agente de Recuperação de Dados (DRA) do Sistema de [Encriptação de Ficheiros (EFS).](/windows/security/information-protection/windows-information-protection/create-and-verify-an-efs-dra-certificate)
    
    Por predefinição, os ficheiros de trabalho são encriptados com uma chave secreta que é armazenada no dispositivo e é associada ao perfil do utilizador. Apenas o utilizador pode abrir e desencriptar o ficheiro. No entanto, se um dispositivo for perdido ou um utilizador for removido, um ficheiro pode ficar bloqueado num estado encriptado. Um administrador pode utilizar o certificado de Agente de Recuperação de Dados (DRA) para deciptar o ficheiro.
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. Expanda **a secção** Proteger localizações de rede e de nuvem adicionais se quiser adicionar domínios ou localizações do SharePoint Online para se certificar de que os ficheiros em todas as aplicações listadas estão protegidos. Se precisar de introduzir mais do que um item em cada campo, utilize ponto e vírgula (;) entre os itens.
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. Em seguida, decida **Quem irá ver estas definições?** Se não quiser utilizar o grupo de segurança predefinido, **Todos os Utilizadores**, selecione **Alterar**, selecione os grupos de segurança que irão receber estas definições \> **Selecionar**.
12. Por fim, selecione **Adicionar** para guardar a política e atribua-a a todos os dispositivos.