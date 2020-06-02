---
title: Configurar as definições de proteção de aplicações para dispositivos Android ou iOS
f1.keywords:
- NOCSH
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Saiba como criar, editar ou eliminar uma política de gestão de aplicações e proteger ficheiros de trabalho em dispositivos Android ou iOS.
ms.openlocfilehash: 67e7aaec5ff5a28f1e2d489913246c1c15c2f7b6
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471205"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a><span data-ttu-id="805cc-103">Configurar as definições de proteção de aplicações para dispositivos Android ou iOS</span><span class="sxs-lookup"><span data-stu-id="805cc-103">Set app protection settings for Android or iOS devices</span></span>

<span data-ttu-id="805cc-104">Este artigo aplica-se ao Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="805cc-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="create-an-app-management-policy"></a><span data-ttu-id="805cc-105">Criar uma política de gestão de aplicações</span><span class="sxs-lookup"><span data-stu-id="805cc-105">Create an app management policy</span></span>

1. <span data-ttu-id="805cc-106">Vá ao centro de administração em <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="805cc-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="805cc-107">No navegador esquerdo, escolha **Políticas de Dispositivos** \> **Policies** \> **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="805cc-107">In the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
  
3. <span data-ttu-id="805cc-108">No painel **Adicionar política**, introduza um nome exclusivo para esta política.</span><span class="sxs-lookup"><span data-stu-id="805cc-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="805cc-109">Sob **o tipo de Política**, escolha **Gestão de Aplicações para Android** ou **Gestão de Aplicações para iOS,** dependendo do conjunto de políticas que pretende criar.</span><span class="sxs-lookup"><span data-stu-id="805cc-109">Under **Policy type**, choose **Application Management for Android** or **Application Management for iOS**, depending on which set of policies you want to create.</span></span> 
    
5. <span data-ttu-id="805cc-110">Expandir **Ficheiros de trabalho quando os dispositivos são perdidos ou roubados** e **Gerir como os utilizadores acedem aos ficheiros do Office em dispositivos móveis**.</span><span class="sxs-lookup"><span data-stu-id="805cc-110">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices**.</span></span> <span data-ttu-id="805cc-111">Configure as definições como gostaria.</span><span class="sxs-lookup"><span data-stu-id="805cc-111">Configure the settings how you would like.</span></span> <span data-ttu-id="805cc-112">**Gerencie a forma como os utilizadores acedem aos ficheiros do Office em dispositivos móveis** **por** padrão, mas recomendamos que o ligue **e** aceite os valores predefinidos.</span><span class="sxs-lookup"><span data-stu-id="805cc-112">**Manage how users access Office files on mobile devices** is **Off** by default, but we recommend that you turn it **On** and accept the default values.</span></span> <span data-ttu-id="805cc-113">Para mais informações, consulte [as definições disponíveis.](#available-settings)</span><span class="sxs-lookup"><span data-stu-id="805cc-113">For more information, see [Available settings](#available-settings).</span></span> 
    
    <span data-ttu-id="805cc-114">Pode sempre utilizar a ligação **Repor predefinições** para regressar à predefinição.</span><span class="sxs-lookup"><span data-stu-id="805cc-114">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Screenshot of Create a policy with Application management for Android selected](../media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. <span data-ttu-id="805cc-116">Em seguida, decida **Quem irá ver estas definições?**</span><span class="sxs-lookup"><span data-stu-id="805cc-116">Next decide **Who will get these settings?**</span></span> <span data-ttu-id="805cc-117">Se não quiser utilizar o grupo de segurança predefinido **Todos os Utilizadores,** escolha **Alterar**, escolha os grupos de segurança que obtêm estas definições \> **Selecione**.</span><span class="sxs-lookup"><span data-stu-id="805cc-117">If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups that get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="805cc-118">Por fim, selecione **Concluído** para guardar a política e atribuí-la aos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="805cc-118">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="edit-an-app-management-policy"></a><span data-ttu-id="805cc-119">Editar uma política de gestão de aplicações</span><span class="sxs-lookup"><span data-stu-id="805cc-119">Edit an app management policy</span></span>

1. <span data-ttu-id="805cc-120">No cartão **Políticas,** escolha **a política de Edição.**</span><span class="sxs-lookup"><span data-stu-id="805cc-120">On the **Policies** card, choose **Edit policy**.</span></span>
    
2. <span data-ttu-id="805cc-121">No painel **Editar política**, selecione a política que pretende alterar</span><span class="sxs-lookup"><span data-stu-id="805cc-121">On the **Edit policy** pane, choose the policy you want to change</span></span> 
    
3. <span data-ttu-id="805cc-122">Selecione **Editar** junto a cada definição para alterar os valores na política.</span><span class="sxs-lookup"><span data-stu-id="805cc-122">Choose **Edit** next to each setting to change the values in the policy.</span></span> <span data-ttu-id="805cc-123">Quando se muda um valor, é automaticamente guardado na apólice.</span><span class="sxs-lookup"><span data-stu-id="805cc-123">When you change a value, it's automatically saved in the policy.</span></span>
    
4. <span data-ttu-id="805cc-124">Quando terminar, feche o painel de política de **edição.**</span><span class="sxs-lookup"><span data-stu-id="805cc-124">When you're finished, close the **Edit policy** pane.</span></span> 
    
## <a name="delete-an-app-management-policy"></a><span data-ttu-id="805cc-125">Eliminar uma política de gestão de aplicações</span><span class="sxs-lookup"><span data-stu-id="805cc-125">Delete an app management policy</span></span>

1. <span data-ttu-id="805cc-126">Na página **Políticas,** escolha uma política e, em seguida, **apague**.</span><span class="sxs-lookup"><span data-stu-id="805cc-126">On the **Policies** page, choose a policy and then **Delete**.</span></span>
    
2. <span data-ttu-id="805cc-127">No painel **de política eliminar,** escolha **Confirmar** para eliminar a política ou as políticas que escolheu.</span><span class="sxs-lookup"><span data-stu-id="805cc-127">On the **Delete policy** pane, choose **Confirm** to delete the policy or policies you chose.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="805cc-128">Definições disponíveis</span><span class="sxs-lookup"><span data-stu-id="805cc-128">Available settings</span></span>

<span data-ttu-id="805cc-129">As seguintes tabelas dão informações detalhadas sobre as definições disponíveis para proteger ficheiros de trabalho em dispositivos e as definições que controlam a forma como os utilizadores acedem aos ficheiros do Office a partir dos seus dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="805cc-129">The following tables give detailed information about settings available to protect work files on devices and the settings that control how users access Office files from their mobile devices.</span></span>
  
 <span data-ttu-id="805cc-130">Para obter mais informações, consulte [como as funcionalidades de proteção no mapa do Microsoft 365 Business Premium para as definições do Intune.](map-protection-features-to-intune-settings.md)</span><span class="sxs-lookup"><span data-stu-id="805cc-130">For more information, see [How do protection features in Microsoft 365 Business Premium map to Intune settings](map-protection-features-to-intune-settings.md).</span></span> 
  
### <a name="settings-that-protect-work-files"></a><span data-ttu-id="805cc-131">Definições que protegem os ficheiros de trabalho</span><span class="sxs-lookup"><span data-stu-id="805cc-131">Settings that protect work files</span></span>

<span data-ttu-id="805cc-132">As seguintes definições para proteger ficheiros de trabalho estarão disponíveis se o dispositivo de um utilizador for perdido ou roubado:</span><span class="sxs-lookup"><span data-stu-id="805cc-132">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="805cc-133">Definição</span><span class="sxs-lookup"><span data-stu-id="805cc-133">Setting</span></span>  <br/> |<span data-ttu-id="805cc-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="805cc-134">Description</span></span>  <br/> |
|<span data-ttu-id="805cc-135">Eliminar ficheiros de trabalho de um dispositivo inativo após este número de dias</span><span class="sxs-lookup"><span data-stu-id="805cc-135">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="805cc-136">Se um dispositivo não for utilizado durante o número de dias que especifica aqui, quaisquer ficheiros de trabalho armazenados no dispositivo serão automaticamente eliminados.</span><span class="sxs-lookup"><span data-stu-id="805cc-136">If a device isn't used for the number of days that you specify here, any work files stored on the device will be deleted automatically.</span></span>  <br/> |
|<span data-ttu-id="805cc-137">Forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas</span><span class="sxs-lookup"><span data-stu-id="805cc-137">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="805cc-138">Se esta definição estiver **on,** a única localização de poupança disponível para ficheiros de trabalho é o OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="805cc-138">If this setting is **On**, the only available save location for work files is OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="805cc-139">Encriptar ficheiros de trabalho</span><span class="sxs-lookup"><span data-stu-id="805cc-139">Encrypt work files</span></span>  <br/> |<span data-ttu-id="805cc-140">Mantenha esta definição **Ativada** para que os ficheiros de trabalho sejam protegidos por encriptação.</span><span class="sxs-lookup"><span data-stu-id="805cc-140">Keep this setting **On** so that work files are protected by encryption.</span></span> <span data-ttu-id="805cc-141">Mesmo que o dispositivo seja perdido ou roubado, ninguém pode ler os dados da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="805cc-141">Even if the device is lost or stolen, no one can read your company data.</span></span>  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="805cc-142">Definições que controlam a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis</span><span class="sxs-lookup"><span data-stu-id="805cc-142">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="805cc-143">As seguintes definições estão disponíveis para gerir como os utilizadores acedem a ficheiros de trabalho do Office:</span><span class="sxs-lookup"><span data-stu-id="805cc-143">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="805cc-144">Definição</span><span class="sxs-lookup"><span data-stu-id="805cc-144">Setting</span></span>  <br/> |<span data-ttu-id="805cc-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="805cc-145">Description</span></span>  <br/> |
|<span data-ttu-id="805cc-146">Exigir um PIN ou uma impressão digital para aceder às aplicações do Office</span><span class="sxs-lookup"><span data-stu-id="805cc-146">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="805cc-147">Se esta definição for **No que** os utilizadores devem fornecer outra forma de autenticação, além do seu nome de utilizador e palavra-passe, antes de poderem utilizar aplicações do Office nos seus dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="805cc-147">If this setting is **On** users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile devices.</span></span><br/> |
|<span data-ttu-id="805cc-148">Repor o PIN quando o início de sessão falha este número de vezes</span><span class="sxs-lookup"><span data-stu-id="805cc-148">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="805cc-149">Para impedir um utilizador não autorizado de adivinhar um PIN aleatoriamente, o PIN será reposto após o número de tentativas incorretas que especificar.</span><span class="sxs-lookup"><span data-stu-id="805cc-149">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="805cc-150">Exigir que o utilizador inicie a sessão novamente após as aplicações do Office estarem inativas durante</span><span class="sxs-lookup"><span data-stu-id="805cc-150">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="805cc-151">Esta definição determina quanto tempo um utilizador pode ficar inativo antes de ser solicitado a iniciar novamente o seu sposição.</span><span class="sxs-lookup"><span data-stu-id="805cc-151">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="805cc-152">Negar o acesso a ficheiros de trabalho em dispositivos desbloqueados por jailbreak ou rooting</span><span class="sxs-lookup"><span data-stu-id="805cc-152">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="805cc-p105">Alguns utilizadores podem ter um dispositivo desbloqueado através de jailbreak ou rooting. Isto significa que o utilizador pode modificar o sistema operativo, o que pode tornar o dispositivo mais suscetível a software maligno. Estes dispositivos são bloqueados quando esta definição se encontra **Ativada**.  </span><span class="sxs-lookup"><span data-stu-id="805cc-p105">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="805cc-156">Não permita que os utilizadores copiem conteúdo de apps do Office em aplicações pessoais</span><span class="sxs-lookup"><span data-stu-id="805cc-156">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="805cc-157">Permitimos isso por predefinição, mas se a definição estiver **em Funcionamento,** o utilizador poderá copiar informações num ficheiro de trabalho para um ficheiro pessoal.</span><span class="sxs-lookup"><span data-stu-id="805cc-157">We do allow this by default, but if the setting is **On**, the user could copy information in a work file to a personal file.</span></span> <span data-ttu-id="805cc-158">Se a definição estiver **desligada,** o utilizador não poderá copiar informação de uma conta de trabalho numa aplicação pessoal ou numa conta pessoal.</span><span class="sxs-lookup"><span data-stu-id="805cc-158">If the setting is **Off**, the user will be unable to copy information from a work account into a personal app or personal account.</span></span>  <br/> |
