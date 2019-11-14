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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Saiba como criar, editar ou excluir uma política de gerenciamento de aplicativos e proteger arquivos de trabalho em dispositivos Android ou iOS.
ms.openlocfilehash: 2eebe5b603837d7e4125ab7e88b61792ca3a1e5d
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/14/2019
ms.locfileid: "38321851"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a><span data-ttu-id="f27f6-103">Configurar as definições de proteção de aplicações para dispositivos Android ou iOS</span><span class="sxs-lookup"><span data-stu-id="f27f6-103">Set app protection settings for Android or iOS devices</span></span>

![Banner que https://aka.ms/aboutM365previewapontam para .](media/m365admincenterchanging.png)

## <a name="create-an-app-management-policy"></a><span data-ttu-id="f27f6-105">Criar uma política de gestão de aplicações</span><span class="sxs-lookup"><span data-stu-id="f27f6-105">Create an app management policy</span></span>

1. <span data-ttu-id="f27f6-106">Vá para o centro <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>de administração em .</span><span class="sxs-lookup"><span data-stu-id="f27f6-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="f27f6-107">No nav esquerdo, escolha **políticas** \> dos **dispositivos** \> **adicione.**</span><span class="sxs-lookup"><span data-stu-id="f27f6-107">In the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
  
3. <span data-ttu-id="f27f6-108">No painel **Adicionar política**, introduza um nome exclusivo para esta política.</span><span class="sxs-lookup"><span data-stu-id="f27f6-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="f27f6-109">De acordo com o **tipo de política,** escolha gerenciamento de **aplicativos para Android** ou gerenciamento de **aplicativos para iOS,** dependendo de qual conjunto de políticas você deseja criar.</span><span class="sxs-lookup"><span data-stu-id="f27f6-109">Under **Policy type**, choose **Application Management for Android** or **Application Management for iOS**, depending on which set of policies you want to create.</span></span> 
    
5. <span data-ttu-id="f27f6-110">Expanda os arquivos de **trabalho protect quando os dispositivos são perdidos ou roubados** e **gerencie como os usuários acessam os arquivos do Office em dispositivos móveis.**</span><span class="sxs-lookup"><span data-stu-id="f27f6-110">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices**.</span></span> <span data-ttu-id="f27f6-111">Configure as configurações como você gostaria.</span><span class="sxs-lookup"><span data-stu-id="f27f6-111">Configure the settings how you would like.</span></span> <span data-ttu-id="f27f6-112">**Gerenciar como os usuários acessam os arquivos do Office em dispositivos móveis** está **desligado** por padrão, mas recomendamos que você **os** desligue e aceite os valores padrão.</span><span class="sxs-lookup"><span data-stu-id="f27f6-112">**Manage how users access Office files on mobile devices** is **Off** by default, but we recommend that you turn it **On** and accept the default values.</span></span> <span data-ttu-id="f27f6-113">Para mais informações, consulte [as configurações disponíveis.](#available-settings)</span><span class="sxs-lookup"><span data-stu-id="f27f6-113">For more information, see [Available settings](#available-settings).</span></span> 
    
    <span data-ttu-id="f27f6-114">Pode sempre utilizar a ligação **Repor predefinições** para regressar à predefinição.</span><span class="sxs-lookup"><span data-stu-id="f27f6-114">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. <span data-ttu-id="f27f6-116">Em seguida, decida **Quem irá ver estas definições?**</span><span class="sxs-lookup"><span data-stu-id="f27f6-116">Next decide **Who will get these settings?**</span></span> <span data-ttu-id="f27f6-117">Se você não quiser usar o grupo de segurança padrão **de todos os usuários,** escolha **o Change,** escolha os \> **grupos**de segurança que selecionem essas configurações.</span><span class="sxs-lookup"><span data-stu-id="f27f6-117">If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups that get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="f27f6-118">Por fim, selecione **Concluído** para guardar a política e atribuí-la aos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f27f6-118">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="edit-an-app-management-policy"></a><span data-ttu-id="f27f6-119">Editar uma política de gestão de aplicações</span><span class="sxs-lookup"><span data-stu-id="f27f6-119">Edit an app management policy</span></span>

1. <span data-ttu-id="f27f6-120">No cartão **de Políticas,** escolha **a política de eitar**.</span><span class="sxs-lookup"><span data-stu-id="f27f6-120">On the **Policies** card, choose **Edit policy**.</span></span>
    
2. <span data-ttu-id="f27f6-121">No painel **Editar política**, selecione a política que pretende alterar</span><span class="sxs-lookup"><span data-stu-id="f27f6-121">On the **Edit policy** pane, choose the policy you want to change</span></span> 
    
3. <span data-ttu-id="f27f6-122">Selecione **Editar** junto a cada definição para alterar os valores na política.</span><span class="sxs-lookup"><span data-stu-id="f27f6-122">Choose **Edit** next to each setting to change the values in the policy.</span></span> <span data-ttu-id="f27f6-123">Quando você muda um valor, ele é automaticamente salvo na política.</span><span class="sxs-lookup"><span data-stu-id="f27f6-123">When you change a value, it's automatically saved in the policy.</span></span>
    
4. <span data-ttu-id="f27f6-124">Quando terminar, feche o painel de políticas de **eite.**</span><span class="sxs-lookup"><span data-stu-id="f27f6-124">When you're finished, close the **Edit policy** pane.</span></span> 
    
## <a name="delete-an-app-management-policy"></a><span data-ttu-id="f27f6-125">Eliminar uma política de gestão de aplicações</span><span class="sxs-lookup"><span data-stu-id="f27f6-125">Delete an app management policy</span></span>

1. <span data-ttu-id="f27f6-126">Na página **de Políticas,** escolha uma política e, em seguida, **excluir**.</span><span class="sxs-lookup"><span data-stu-id="f27f6-126">On the **Policies** page, choose a policy and then **Delete**.</span></span>
    
2. <span data-ttu-id="f27f6-127">No painel de **política supressão,** escolha **confirmar** para excluir a política ou as políticas que você escolheu.</span><span class="sxs-lookup"><span data-stu-id="f27f6-127">On the **Delete policy** pane, choose **Confirm** to delete the policy or policies you chose.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="f27f6-128">Definições disponíveis</span><span class="sxs-lookup"><span data-stu-id="f27f6-128">Available settings</span></span>

<span data-ttu-id="f27f6-129">As tabelas a seguir dão informações detalhadas sobre as configurações disponíveis para proteger os arquivos de trabalho em dispositivos e as configurações que controlam como os usuários acessam os arquivos do Office de seus dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="f27f6-129">The following tables give detailed information about settings available to protect work files on devices and the settings that control how users access Office files from their mobile devices.</span></span>
  
 <span data-ttu-id="f27f6-130">Para obter mais informações, consulte [Como é que as funcionalidades de proteção no Microsoft 365 Empresas são mapeadas para as definições do Intune](map-protection-features-to-intune-settings.md).</span><span class="sxs-lookup"><span data-stu-id="f27f6-130">For more information, see [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md).</span></span> 
  
### <a name="settings-that-protect-work-files"></a><span data-ttu-id="f27f6-131">Definições que protegem os ficheiros de trabalho</span><span class="sxs-lookup"><span data-stu-id="f27f6-131">Settings that protect work files</span></span>

<span data-ttu-id="f27f6-132">As seguintes definições para proteger ficheiros de trabalho estarão disponíveis se o dispositivo de um utilizador for perdido ou roubado:</span><span class="sxs-lookup"><span data-stu-id="f27f6-132">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="f27f6-133">Definição</span><span class="sxs-lookup"><span data-stu-id="f27f6-133">Setting</span></span>  <br/> |<span data-ttu-id="f27f6-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="f27f6-134">Description</span></span>  <br/> |
|<span data-ttu-id="f27f6-135">Eliminar ficheiros de trabalho de um dispositivo inativo após este número de dias</span><span class="sxs-lookup"><span data-stu-id="f27f6-135">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="f27f6-136">Se um dispositivo não for usado para o número de dias que você especifica aqui, quaisquer arquivos de trabalho armazenados no dispositivo serão excluídos automaticamente.</span><span class="sxs-lookup"><span data-stu-id="f27f6-136">If a device isn't used for the number of days that you specify here, any work files stored on the device will be deleted automatically.</span></span>  <br/> |
|<span data-ttu-id="f27f6-137">Forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas</span><span class="sxs-lookup"><span data-stu-id="f27f6-137">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="f27f6-138">Se esta configuração estiver **em ação,** o único local disponível para salvar arquivos de trabalho é o OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="f27f6-138">If this setting is **On**, the only available save location for work files is OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="f27f6-139">Encriptar ficheiros de trabalho</span><span class="sxs-lookup"><span data-stu-id="f27f6-139">Encrypt work files</span></span>  <br/> |<span data-ttu-id="f27f6-140">Mantenha esta definição **Ativada** para que os ficheiros de trabalho sejam protegidos por encriptação.</span><span class="sxs-lookup"><span data-stu-id="f27f6-140">Keep this setting **On** so that work files are protected by encryption.</span></span> <span data-ttu-id="f27f6-141">Mesmo que o dispositivo esteja perdido ou roubado, ninguém pode ler os dados da empresa.</span><span class="sxs-lookup"><span data-stu-id="f27f6-141">Even if the device is lost or stolen, no one can read your company data.</span></span>  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="f27f6-142">Definições que controlam a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis</span><span class="sxs-lookup"><span data-stu-id="f27f6-142">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="f27f6-143">As seguintes definições estão disponíveis para gerir como os utilizadores acedem a ficheiros de trabalho do Office:</span><span class="sxs-lookup"><span data-stu-id="f27f6-143">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="f27f6-144">Definição</span><span class="sxs-lookup"><span data-stu-id="f27f6-144">Setting</span></span>  <br/> |<span data-ttu-id="f27f6-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="f27f6-145">Description</span></span>  <br/> |
|<span data-ttu-id="f27f6-146">Exigir um PIN ou uma impressão digital para aceder às aplicações do Office</span><span class="sxs-lookup"><span data-stu-id="f27f6-146">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="f27f6-147">Se essa \*\*\*\* configuração estiver on,00, os usuários devem fornecer outra forma de autenticação, além de seu nome de usuário e senha, antes que eles possam usar aplicativos do Office em seus dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="f27f6-147">If this setting is **On** users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile devices.</span></span><br/> |
|<span data-ttu-id="f27f6-148">Repor o PIN quando o início de sessão falha este número de vezes</span><span class="sxs-lookup"><span data-stu-id="f27f6-148">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="f27f6-149">Para impedir um utilizador não autorizado de adivinhar um PIN aleatoriamente, o PIN será reposto após o número de tentativas incorretas que especificar.</span><span class="sxs-lookup"><span data-stu-id="f27f6-149">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="f27f6-150">Exigir que o utilizador inicie a sessão novamente após as aplicações do Office estarem inativas durante</span><span class="sxs-lookup"><span data-stu-id="f27f6-150">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="f27f6-151">Essa configuração determina quanto tempo um usuário pode ficar ocioso antes de ser solicitado a entrar novamente.</span><span class="sxs-lookup"><span data-stu-id="f27f6-151">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="f27f6-152">Negar o acesso a ficheiros de trabalho em dispositivos desbloqueados por jailbreak ou rooting</span><span class="sxs-lookup"><span data-stu-id="f27f6-152">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="f27f6-p105">Alguns utilizadores podem ter um dispositivo desbloqueado através de jailbreak ou rooting. Isto significa que o utilizador pode modificar o sistema operativo, o que pode tornar o dispositivo mais suscetível a software maligno. Estes dispositivos são bloqueados quando esta definição se encontra **Ativada**.  </span><span class="sxs-lookup"><span data-stu-id="f27f6-p105">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="f27f6-156">Permitir que os utilizadores copiem conteúdos das aplicações do Office para aplicações pessoais</span><span class="sxs-lookup"><span data-stu-id="f27f6-156">Allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="f27f6-157">Nós permitimos isso por padrão, mas se a configuração estiver **on,** o usuário poderá copiar informações em um arquivo de trabalho para um arquivo pessoal.</span><span class="sxs-lookup"><span data-stu-id="f27f6-157">We do allow this by default, but if the setting is **On**, the user could copy information in a work file to a personal file.</span></span> <span data-ttu-id="f27f6-158">Se a configuração estiver **desligada,** o usuário não poderá copiar informações de uma conta de trabalho em um aplicativo pessoal ou conta pessoal.</span><span class="sxs-lookup"><span data-stu-id="f27f6-158">If the setting is **Off**, the user will be unable to copy information from a work account into a personal app or personal account.</span></span>  <br/> |
