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
ms.openlocfilehash: acf19a72d994185a35b2e425f8334a73a121ee10
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982828"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="86736-103">Configurar as definições de proteção de aplicações para dispositivos Windows 10</span><span class="sxs-lookup"><span data-stu-id="86736-103">Set application protection settings for Windows 10 devices</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="86736-104">Criar uma política de gestão de aplicações para Windows 10</span><span class="sxs-lookup"><span data-stu-id="86736-104">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="86736-105">Se os seus utilizadores tiverem dispositivos Windows 10 pessoais, nos quais realizam tarefas profissionais, também pode proteger os seus dados nesses dispositivos.</span><span class="sxs-lookup"><span data-stu-id="86736-105">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="86736-p101">Inicie sessão no [Microsoft 365 Business](https://portal.office.com) com as suas credenciais de administrador global. Selecione o mosaico **Administrador** para aceder ao centro de administração.</span><span class="sxs-lookup"><span data-stu-id="86736-p101">Sign in to [Microsoft 365 Business](https://portal.office.com) with global admin credentials. Choose the **Admin** tile to go to the admin center.</span></span> 
    
2. <span data-ttu-id="86736-108">No cartão **Políticas de dispositivos** do portal de administração, selecione **Adicionar política**.</span><span class="sxs-lookup"><span data-stu-id="86736-108">On the **Device policies** card of the admin portal, choose **Add policy**.</span></span>
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. <span data-ttu-id="86736-110">No painel **Adicionar política**, introduza um nome exclusivo para esta política.</span><span class="sxs-lookup"><span data-stu-id="86736-110">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="86736-111">Em **Tipo de política**, selecione **Gestão de Aplicações para Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="86736-111">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
    
5. <span data-ttu-id="86736-112">Em \* \* o tipo de dispositivo \* \*, escolher **pessoal** ou **Propriedade da empresa**.</span><span class="sxs-lookup"><span data-stu-id="86736-112">Under \*\* Device type \*\*, choose either **Personal** or **Company Owned**.</span></span>
    
6. <span data-ttu-id="86736-113">A opção **Encriptar ficheiros de trabalho** é ativada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="86736-113">The **Encrypt work files** is turned on automatically.</span></span> 
    
7. <span data-ttu-id="86736-114">Defina **Impedir que os utilizadores copiem os dados da empresa para ficheiros pessoais e obrigá-los a guardar os ficheiros de trabalho no OneDrive para Empresas** como **Ativado** se não pretender que os utilizadores guardem ficheiros de trabalho nos respetivos PCs.</span><span class="sxs-lookup"><span data-stu-id="86736-114">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
    
8. <span data-ttu-id="86736-p102">Expanda **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos** \> configure as definições de acordo com as suas preferências. A opção **Gerir a forma como os utilizadores acedem a dispositivos do Office em dispositivos móveis** está **Desativada** por predefinição, mas recomenda-se que a defina como **Ativada** e aceite os valores predefinidos. Consulte [Definições disponíveis](protection-settings-for-windows-10-devices.md#bkmk_settings) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="86736-p102">Expand **Manage how users access Office files on devices** \> configure the settings how you would like. The **Manage how users access Office devices on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values. See [Available settings](protection-settings-for-windows-10-devices.md#bkmk_settings) for more information.</span></span> 
    
    <span data-ttu-id="86736-118">Pode sempre utilizar a ligação **Repor predefinições** para regressar à predefinição.</span><span class="sxs-lookup"><span data-stu-id="86736-118">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
9. <span data-ttu-id="86736-119">Expanda a opção **Recuperar dados em dispositivos Windows** e recomendamos que a defina como **Ativada**.</span><span class="sxs-lookup"><span data-stu-id="86736-119">Expand **Recover data on Windows devices** and it is recommended that you turn it **On**.</span></span>
    
    <span data-ttu-id="86736-p103">Antes de poder aceder à localização do certificado de Agente de Recuperação de Dados, tem de criar um. Para obter instruções, consulte [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate (Criar e verificar um certificado de Agente de Recuperação de Dados (DRA) do Sistema de Encriptação de Ficheiros (EFS))](https://go.microsoft.com/fwlink/p/?linkid=853700).</span><span class="sxs-lookup"><span data-stu-id="86736-p103">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one. For instructions see, [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](https://go.microsoft.com/fwlink/p/?linkid=853700).</span></span>
    
    <span data-ttu-id="86736-p104">Por predefinição, os ficheiros de trabalho são encriptados com uma chave secreta que é armazenada no dispositivo e é associada ao perfil do utilizador. Apenas o utilizador pode abrir e desencriptar o ficheiro. No entanto, se um dispositivo for perdido ou um utilizador for removido, um ficheiro pode ficar bloqueado num estado encriptado. Um administrador pode utilizar o certificado de Agente de Recuperação de Dados (DRA) para desencriptar o ficheiro.</span><span class="sxs-lookup"><span data-stu-id="86736-p104">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile. Only the user can open and decrypt the file. However, if a device is lost or a user is removed, a file can be stuck in an encrypted state. The Data Recovery Agent (DRA) certificate can be used by an admin to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="86736-p105">Expanda a opção **Proteger localizações de rede e de nuvem adicionais** se quiser adicionar domínios ou localizações do SharePoint Online para garantir que os ficheiros em todas as aplicações listadas serão protegidos. Se precisar de introduzir mais do que um item em cada campo, utilize ponto e vírgula (;) entre os itens.</span><span class="sxs-lookup"><span data-stu-id="86736-p105">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps will be protected. If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span> 
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="86736-p106">Em seguida, decida **Quem irá ver estas definições?** Se não quiser utilizar o grupo de segurança predefinido, **Todos os Utilizadores**, selecione **Alterar**, selecione os grupos de segurança que irão receber estas definições \> **Selecionar**.</span><span class="sxs-lookup"><span data-stu-id="86736-p106">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
12. <span data-ttu-id="86736-132">Por fim, selecione **Adicionar** para guardar a política e atribua-a a todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="86736-132">Finally, choose **Add** to save the policy, and assign it to devices.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="86736-133">Definições disponíveis</span><span class="sxs-lookup"><span data-stu-id="86736-133">Available settings</span></span>

<span data-ttu-id="86736-134">As seguintes definições estão disponíveis para gerir como os utilizadores acedem a ficheiros de trabalho do Office.</span><span class="sxs-lookup"><span data-stu-id="86736-134">The following settings are available to manage how users access Office work files.</span></span>
  
<span data-ttu-id="86736-135">Para obter mais informações, consulte [Como é que as funcionalidades de proteção no Microsoft 365 Empresas são mapeadas para as definições do Intune](map-protection-features-to-intune-settings.md).</span><span class="sxs-lookup"><span data-stu-id="86736-135">For more information, see [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md).</span></span>
  
|<span data-ttu-id="86736-136">**Definição**</span><span class="sxs-lookup"><span data-stu-id="86736-136">**Setting**</span></span>|<span data-ttu-id="86736-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="86736-137">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="86736-138">Exigir um PIN ou uma impressão digital para aceder às aplicações do Office</span><span class="sxs-lookup"><span data-stu-id="86736-138">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="86736-139">Se esta definição estiver **Ativada**, os utilizadores terão de fornecer outro meio de autenticação, além do nome de utilizador e da palavra-passe, antes de poderem utilizar aplicações do Office nos respetivos dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="86736-139">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="86736-140">Repor o PIN quando o início de sessão falha este número de vezes</span><span class="sxs-lookup"><span data-stu-id="86736-140">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="86736-141">Para impedir um utilizador não autorizado de adivinhar um PIN aleatoriamente, o PIN será reposto após o número de tentativas incorretas que especificar.</span><span class="sxs-lookup"><span data-stu-id="86736-141">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="86736-142">Exigir que o utilizador inicie a sessão novamente após as aplicações do Office estarem inativas durante</span><span class="sxs-lookup"><span data-stu-id="86736-142">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="86736-143">Esta definição determina durante quanto tempo um utilizador pode estar inativo antes de ter de voltar a iniciar sessão.</span><span class="sxs-lookup"><span data-stu-id="86736-143">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
   

