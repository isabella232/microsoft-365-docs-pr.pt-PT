---
title: Configurar as definições de proteção de aplicações para dispositivos Android ou iOS
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Obter informações sobre como criar, editar ou eliminar uma política de gestão de aplicações e proteger ficheiros de trabalho em dispositivos Android ou iOS.
ms.openlocfilehash: 21cc1d91c2952c6e9414d3742c26547fc36016a5
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/15/2019
ms.locfileid: "34073516"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a><span data-ttu-id="4ae2f-103">Configurar as definições de proteção de aplicações para dispositivos Android ou iOS</span><span class="sxs-lookup"><span data-stu-id="4ae2f-103">Set app protection settings for Android or iOS devices</span></span>

![Faixa que apontam para https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

## <a name="create-an-app-management-policy"></a><span data-ttu-id="4ae2f-105">Criar uma política de gestão de aplicações</span><span class="sxs-lookup"><span data-stu-id="4ae2f-105">Create an app management policy</span></span>

1. <span data-ttu-id="4ae2f-106">Vá para o Centro de administração no <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="4ae2f-107">Nav esquerda, escolher **dispositivos** \> **políticas** \> **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-107">In the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
  
3. <span data-ttu-id="4ae2f-108">No painel **Adicionar política**, introduza um nome exclusivo para esta política.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="4ae2f-109">Em **Tipo de política**, selecione **Gestão de Aplicações para Android** ou **Gestão de Aplicações para iOS** consoante o conjunto de políticas que pretende criar.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-109">Under **Policy type**, choose **Application Management for Android** or **Application Management for iOS** depending on which set of policies you want to create.</span></span> 
    
5. <span data-ttu-id="4ae2f-110">Expanda as opções **Proteger os ficheiros de trabalho se os dispositivos forem perdidos ou roubados** e **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis** \> configure as definições como pretende.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-110">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** \> configure the settings how you would like.</span></span> <span data-ttu-id="4ae2f-111">A opção **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis** está **Desativada** por predefinição, mas recomenda-se que a defina como **Ativada** e aceite os valores predefinidos.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-111">The **Manage how users access Office files on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values.</span></span> <span data-ttu-id="4ae2f-112">Para mais informações, consulte [as definições disponíveis](#available-settings) .</span><span class="sxs-lookup"><span data-stu-id="4ae2f-112">See [Available settings](#available-settings)  for more information.</span></span> 
    
    <span data-ttu-id="4ae2f-113">Pode sempre utilizar a ligação **Repor predefinições** para regressar à predefinição.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-113">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. <span data-ttu-id="4ae2f-p102">Em seguida, decida **Quem irá ver estas definições?** Se não quiser utilizar o grupo de segurança predefinido, **Todos os Utilizadores**, selecione **Alterar**, selecione os grupos de segurança que irão receber estas definições \> **Selecionar**.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-p102">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="4ae2f-117">Por fim, selecione **Concluído** para guardar a política e atribuí-la aos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-117">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="edit-an-app-management-policy"></a><span data-ttu-id="4ae2f-118">Editar uma política de gestão de aplicações</span><span class="sxs-lookup"><span data-stu-id="4ae2f-118">Edit an app management policy</span></span>

1. <span data-ttu-id="4ae2f-119">Na ficha de **políticas** , escolha **Editar política**.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-119">On the **Policies** card, choose **Edit policy**.</span></span>
    
2. <span data-ttu-id="4ae2f-120">No painel **Editar política**, selecione a política que pretende alterar</span><span class="sxs-lookup"><span data-stu-id="4ae2f-120">On the **Edit policy** pane, choose the policy you want to change</span></span> 
    
3. <span data-ttu-id="4ae2f-p103">Selecione **Editar** junto a cada definição para alterar os valores na política. Ao alterar um valor, este é guardado automaticamente na política</span><span class="sxs-lookup"><span data-stu-id="4ae2f-p103">Choose **Edit** next to each setting to change the values in the policy. When you change a value, it is automatically saved into the policy</span></span> 
    
4. <span data-ttu-id="4ae2f-123">Quando tiver terminado, feche o painel **Editar política**.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-123">When you are finished, close the **Edit policy** pane.</span></span> 
    
## <a name="delete-an-app-management-policy"></a><span data-ttu-id="4ae2f-124">Eliminar uma política de gestão de aplicações</span><span class="sxs-lookup"><span data-stu-id="4ae2f-124">Delete an app management policy</span></span>

1. <span data-ttu-id="4ae2f-125">Na página **políticas** , escolha uma política e, em seguida, **Eliminar**.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-125">On the **Policies** page, choose a policy and then **Delete**.</span></span>
    
2. <span data-ttu-id="4ae2f-126">No painel de **Eliminar política** escolha **Confirmar** ao eliminar a política ou políticas que escolheu.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-126">On the **Delete policy** pane choose **Confirm** to delete the policy or policies you chose.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="4ae2f-127">Definições disponíveis</span><span class="sxs-lookup"><span data-stu-id="4ae2f-127">Available settings</span></span>

<span data-ttu-id="4ae2f-128">As tabelas seguintes fornecem informações detalhadas sobre as definições disponíveis para proteger ficheiros de trabalho em dispositivos e as definições que controlam a forma como os utilizadores acedem a ficheiros do Office a partir dos respetivos dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-128">The following tables give detailed information about the available settings to protect work files on devices and the settings that control how users access Office files from their mobile devices.</span></span>
  
 <span data-ttu-id="4ae2f-129">Consulte o artigo [Como é que as funcionalidades de proteção no Microsoft 365 Business são mapeadas às definições do Intune](map-protection-features-to-intune-settings.md) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-129">See [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md) for more information.</span></span> 
  
### <a name="settings-that-protect-work-files"></a><span data-ttu-id="4ae2f-130">Definições que protegem os ficheiros de trabalho</span><span class="sxs-lookup"><span data-stu-id="4ae2f-130">Settings that protect work files</span></span>

<span data-ttu-id="4ae2f-131">As seguintes definições para proteger ficheiros de trabalho estarão disponíveis se o dispositivo de um utilizador for perdido ou roubado:</span><span class="sxs-lookup"><span data-stu-id="4ae2f-131">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="4ae2f-132">Definição</span><span class="sxs-lookup"><span data-stu-id="4ae2f-132">Setting</span></span>  <br/> |<span data-ttu-id="4ae2f-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ae2f-133">Description</span></span>  <br/> |
|<span data-ttu-id="4ae2f-134">Eliminar ficheiros de trabalho de um dispositivo inativo após este número de dias</span><span class="sxs-lookup"><span data-stu-id="4ae2f-134">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="4ae2f-135">Se determinado dispositivo não for utilizado durante o número de dias que especificar aqui, todos os ficheiros de trabalho armazenados no dispositivo serão eliminados automaticamente.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-135">If a device is not used for the number of days that you specify here, any work files stored on the device will automatically be deleted.</span></span>  <br/> |
|<span data-ttu-id="4ae2f-136">Forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas</span><span class="sxs-lookup"><span data-stu-id="4ae2f-136">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="4ae2f-137">Se esta definição estiver **Ativada**, a única localização disponível para guardar ficheiros de trabalho será o OneDrive para Empresas.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-137">If this setting is **On**, the only available save location for work files will be OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="4ae2f-138">Encriptar ficheiros de trabalho</span><span class="sxs-lookup"><span data-stu-id="4ae2f-138">Encrypt work files</span></span>  <br/> |<span data-ttu-id="4ae2f-p104">Mantenha esta definição **Ativada** para que os ficheiros de trabalho sejam protegidos por encriptação. Mesmo que o dispositivo seja perdido ou roubado, os dados da sua empresa não poderão ser lidos por outras pessoas.  </span><span class="sxs-lookup"><span data-stu-id="4ae2f-p104">Keep this setting **On** so that work files are protected by encryption. Even if the device is lost or stolen, no one will be able to read your company data.  </span></span><br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="4ae2f-141">Definições que controlam a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis</span><span class="sxs-lookup"><span data-stu-id="4ae2f-141">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="4ae2f-142">As seguintes definições estão disponíveis para gerir como os utilizadores acedem a ficheiros de trabalho do Office:</span><span class="sxs-lookup"><span data-stu-id="4ae2f-142">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="4ae2f-143">Definição</span><span class="sxs-lookup"><span data-stu-id="4ae2f-143">Setting</span></span>  <br/> |<span data-ttu-id="4ae2f-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ae2f-144">Description</span></span>  <br/> |
|<span data-ttu-id="4ae2f-145">Exigir um PIN ou uma impressão digital para aceder às aplicações do Office</span><span class="sxs-lookup"><span data-stu-id="4ae2f-145">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="4ae2f-146">Se esta definição estiver **Ativada**, os utilizadores terão de fornecer outro meio de autenticação, além do nome de utilizador e da palavra-passe, antes de poderem utilizar aplicações do Office nos respetivos dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-146">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="4ae2f-147">Repor o PIN quando o início de sessão falha este número de vezes</span><span class="sxs-lookup"><span data-stu-id="4ae2f-147">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="4ae2f-148">Para impedir um utilizador não autorizado de adivinhar um PIN aleatoriamente, o PIN será reposto após o número de tentativas incorretas que especificar.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-148">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="4ae2f-149">Exigir que o utilizador inicie a sessão novamente após as aplicações do Office estarem inativas durante</span><span class="sxs-lookup"><span data-stu-id="4ae2f-149">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="4ae2f-150">Esta definição determina durante quanto tempo um utilizador pode estar inativo antes de ter de voltar a iniciar sessão.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-150">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="4ae2f-151">Negar o acesso a ficheiros de trabalho em dispositivos desbloqueados por jailbreak ou rooting</span><span class="sxs-lookup"><span data-stu-id="4ae2f-151">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="4ae2f-p105">Alguns utilizadores podem ter um dispositivo desbloqueado através de jailbreak ou rooting. Isto significa que o utilizador pode modificar o sistema operativo, o que pode tornar o dispositivo mais suscetível a software maligno. Estes dispositivos são bloqueados quando esta definição se encontra **Ativada**.  </span><span class="sxs-lookup"><span data-stu-id="4ae2f-p105">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="4ae2f-155">Permitir que os utilizadores copiem conteúdos das aplicações do Office para aplicações pessoais</span><span class="sxs-lookup"><span data-stu-id="4ae2f-155">Allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="4ae2f-156">Vamos permitir isto por predefinição, mas se a definição estiver **activa**, o utilizador pode copiar informações num ficheiro de trabalho para um ficheiro pessoal.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-156">We do allow this by default, but if the setting is **On**, the user could copy information in a work file to a personal file.</span></span> <span data-ttu-id="4ae2f-157">Se a definição estiver **desactivada**, o utilizador será não é possível copiar informações de uma conta de trabalho para uma conta pessoal ou app pessoal.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-157">If the setting is **Off**, the user will be unable to copy information from a work account into a personal app or personal account.</span></span>  <br/> |
   

  

