---
title: Valide as definições de proteção de aplicativos em dispositivos Android ou iOS
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
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: f3433b6b-02f7-447f-9d62-306bf03638b0
description: Saiba como validar as definições de proteção de aplicações Microsoft 365 Business Premium nos seus dispositivos Android ou iOS.
ms.openlocfilehash: d25a23bc8eb56e05bd74f7bf4658ee9e18dc41f8
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/21/2020
ms.locfileid: "43635730"
---
# <a name="validate-app-protection-settings-on-android-or-ios-devices"></a><span data-ttu-id="2d9db-103">Valide as definições de proteção de aplicativos em dispositivos Android ou iOS</span><span class="sxs-lookup"><span data-stu-id="2d9db-103">Validate app protection settings on Android or iOS devices</span></span>

<span data-ttu-id="2d9db-104">Siga as instruções nas seguintes secções para validar as definições de proteção de aplicações em dispositivos Android ou iOS.</span><span class="sxs-lookup"><span data-stu-id="2d9db-104">Follow the instructions in the following sections to validate app protection settings on Android or iOS devices.</span></span>
  
## <a name="android"></a><span data-ttu-id="2d9db-105">Android</span><span class="sxs-lookup"><span data-stu-id="2d9db-105">Android</span></span>
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="2d9db-106">Verifique se as definições de proteção de aplicações estão a funcionar em dispositivos de utilizador</span><span class="sxs-lookup"><span data-stu-id="2d9db-106">Check that the app protection settings are working on user devices</span></span>

<span data-ttu-id="2d9db-107">Depois de [definir as configurações das aplicações para dispositivos Android](app-protection-settings-for-android-and-ios.md) para proteger as aplicações, pode seguir estes passos para verificar se as definições que escolheu estão a funcionar.</span><span class="sxs-lookup"><span data-stu-id="2d9db-107">After you [set app configurations for Android devices](app-protection-settings-for-android-and-ios.md) to protect the apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="2d9db-108">Em primeiro lugar, certifique-se de que a apólice se aplica à aplicação na qual a vai validar.</span><span class="sxs-lookup"><span data-stu-id="2d9db-108">First, make sure that the policy applies to the app in which you're going to validate it.</span></span>
  
1. <span data-ttu-id="2d9db-109">No [centro de administração](https://portal.office.com)Microsoft 365 Business Premium, vá para a **política de edição**de **políticas.** \></span><span class="sxs-lookup"><span data-stu-id="2d9db-109">In the Microsoft 365 Business Premium [admin center](https://portal.office.com), go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="2d9db-110">Escolha **a política de Aplicação para Android** para as definições que criou na configuração, ou outra política que criou, e verifique se é aplicada para o Outlook, por exemplo.</span><span class="sxs-lookup"><span data-stu-id="2d9db-110">Choose **Application policy for Android** for the settings you created at setup, or another policy you created, and verify that it's enforced for Outlook, for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](../media/b3be3ddd-f683-4073-8d7a-9c639a636a2c.png)
  
### <a name="validate-require-a-pin-or-a-fingerprint-to-access-office-apps"></a><span data-ttu-id="2d9db-112">Verificar a opção para exigir um PIN ou uma impressão digital para aceder às aplicações do Office</span><span class="sxs-lookup"><span data-stu-id="2d9db-112">Validate Require a PIN or a fingerprint to access Office apps</span></span>

<span data-ttu-id="2d9db-113">No painel **Editar política**, selecione **Editar** junto a **Controlo do acesso a documentos do Office**. Expanda a secção **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis** e certifique-se de que a opção **Exigir um PIN ou impressão digital para aceder às aplicações do Office** está definida como **Ativada**.</span><span class="sxs-lookup"><span data-stu-id="2d9db-113">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Certifique-se de que o Requer um PIN ou uma impressão digital para aceder às aplicações do Office está definido para On.](../media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="2d9db-115">No dispositivo Android do utilizador, abra o Outlook e inscreva-se com as credenciais Microsoft 365 Business Premium do utilizador.</span><span class="sxs-lookup"><span data-stu-id="2d9db-115">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="2d9db-116">Também será solicitado a introduzir um PIN ou a utilizar uma impressão digital.</span><span class="sxs-lookup"><span data-stu-id="2d9db-116">You'll also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your Android device to access Office apps.](../media/9e8ecfee-8122-4a3a-8918-eece80344310.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="2d9db-118">Verificar a opção para repor o PIN após um número de tentativas falhadas</span><span class="sxs-lookup"><span data-stu-id="2d9db-118">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="2d9db-119">No painel de **política edite,** escolha **Editar** ao lado do controlo de acesso de **documentos do Office,** expandir **Gerir a forma como os utilizadores acedem aos ficheiros do Office em dispositivos móveis,** e certifique-se de que **o Reset PIN após o número de tentativas falhadas** está definido para algum número.</span><span class="sxs-lookup"><span data-stu-id="2d9db-119">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number.</span></span> <span data-ttu-id="2d9db-120">Este é 5 por defeito.</span><span class="sxs-lookup"><span data-stu-id="2d9db-120">This is 5 by default.</span></span> 
  
1. <span data-ttu-id="2d9db-121">No dispositivo Android do utilizador, abra o Outlook e inscreva-se com as credenciais Microsoft 365 Business Premium do utilizador.</span><span class="sxs-lookup"><span data-stu-id="2d9db-121">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="2d9db-122">Introduza um PIN incorreto tantas vezes quanto for especificado pela política.</span><span class="sxs-lookup"><span data-stu-id="2d9db-122">Enter an incorrect PIN as many times as specified by the policy.</span></span> <span data-ttu-id="2d9db-123">Verá uma solicitação que indica **pin tente limite atingido** para redefinir o PIN.</span><span class="sxs-lookup"><span data-stu-id="2d9db-123">You'll see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](../media/fca6fcb4-bb5c-477f-af5e-5dc937e8b835.png)
  
3. <span data-ttu-id="2d9db-125">Prima **Repor PIN**.</span><span class="sxs-lookup"><span data-stu-id="2d9db-125">Press **Reset PIN**.</span></span> <span data-ttu-id="2d9db-126">Será solicitado a iniciar sessão com as credenciais Microsoft 365 Business Premium do utilizador e, em seguida, obrigado a definir um novo PIN.</span><span class="sxs-lookup"><span data-stu-id="2d9db-126">You'll be prompted to sign in with the user's Microsoft 365 Business Premium credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="2d9db-127">Verificar a opção para forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas</span><span class="sxs-lookup"><span data-stu-id="2d9db-127">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="2d9db-128">No painel **Editar política**, selecione **Editar** junto a **Proteção contra dispositivos perdidos ou roubados**. Expanda a secção **Proteger os ficheiros de trabalho se os dispositivos forem perdidos ou roubados** e certifique-se de que a opção **Forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas** está definida como **Ativada**.</span><span class="sxs-lookup"><span data-stu-id="2d9db-128">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](../media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="2d9db-130">No dispositivo Android do utilizador, abra o Outlook e inscreva-se com as credenciais Microsoft 365 Business Premium do utilizador e introduza um PIN se solicitado.</span><span class="sxs-lookup"><span data-stu-id="2d9db-130">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="2d9db-131">Abra um e-mail que contenha um anexo e toque no ícone de seta para baixo junto às informações do anexo.</span><span class="sxs-lookup"><span data-stu-id="2d9db-131">Open an email that contains an attachment and tap the down arrow icon next to the attachment's information.</span></span>
    
    ![Tap the down arrow next to an attachment to try to save it.](../media/b22573bb-91ce-455f-84fa-8feb2846b117.png)
  
    <span data-ttu-id="2d9db-133">Não pode **ser que se atire na** parte inferior do ecrã.</span><span class="sxs-lookup"><span data-stu-id="2d9db-133">You'll see **Cannot save to device** on the bottom of the screen.</span></span> 
    
    ![Warning text that indicates cannot save a file locally to an Android.](../media/52ca3f3d-7ed0-4a52-9621-4872da6ea9c5.png)
  
    > [!NOTE]
    > <span data-ttu-id="2d9db-135">A opção Guardar no OneDrive para Empresas não se encontra disponível para Android neste momento, por isso, só verá a opção para guardar localmente bloqueada.</span><span class="sxs-lookup"><span data-stu-id="2d9db-135">Saving to OneDrive for Business is not enabled for Android at this time, so you can only see that saving locally is blocked.</span></span> 
  
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="2d9db-136">Verificar a opção para exigir que o utilizador inicie sessão novamente caso as aplicações do Office estejam inativas durante um período de tempo específico</span><span class="sxs-lookup"><span data-stu-id="2d9db-136">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="2d9db-137">No painel de **política edite,** escolha **Editar** ao lado do controlo de acesso de **documentos do Office,** expandir **Gerir a forma como os utilizadores acedem aos ficheiros do Office em dispositivos móveis,** e certifique-se de que os utilizadores voltam a fazer o início depois de as aplicações do Office terem sido **inativas,** está definida para alguns minutos.</span><span class="sxs-lookup"><span data-stu-id="2d9db-137">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes.</span></span> <span data-ttu-id="2d9db-138">São 30 minutos por defeito.</span><span class="sxs-lookup"><span data-stu-id="2d9db-138">This is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="2d9db-139">No dispositivo Android do utilizador, abra o Outlook e inscreva-se com as credenciais Microsoft 365 Business Premium do utilizador e introduza um PIN se solicitado.</span><span class="sxs-lookup"><span data-stu-id="2d9db-139">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="2d9db-p105">Já deverá ver a caixa de entrada do Outlook. Não faça alterações ao dispositivo Android inativo durante, pelo menos, 30 minutos (ou outro período de tempo superior ao especificado na política). Provavelmente, o ecrã do dispositivo ficará mais escuro.</span><span class="sxs-lookup"><span data-stu-id="2d9db-p105">You should now see Outlook's inbox. Let the Android device idle untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="2d9db-143">Access Outlook no dispositivo Android novamente.</span><span class="sxs-lookup"><span data-stu-id="2d9db-143">Access Outlook on the Android device again.</span></span>
    
4. <span data-ttu-id="2d9db-144">Será solicitado a introduzir o seu PIN antes de poder aceder novamente ao Outlook.</span><span class="sxs-lookup"><span data-stu-id="2d9db-144">You'll be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="2d9db-145">Verificar a opção para proteger ficheiros de trabalho com encriptação</span><span class="sxs-lookup"><span data-stu-id="2d9db-145">Validate Protect work files with encryption</span></span>

<span data-ttu-id="2d9db-146">No painel **Editar política**, selecione **Editar** junto a **Proteção contra dispositivos perdidos ou roubados**. Expanda a janela **Proteger os ficheiros de trabalho se os dispositivos forem perdidos ou roubados** e certifique-se de que a opção **Proteger ficheiros de trabalho com encriptação** está definida como **Ativada** e a opção **Forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas** está definida como **Desativada**.</span><span class="sxs-lookup"><span data-stu-id="2d9db-146">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="2d9db-147">No dispositivo Android do utilizador, abra o Outlook e inscreva-se com as credenciais Microsoft 365 Business Premium do utilizador e introduza um PIN se solicitado.</span><span class="sxs-lookup"><span data-stu-id="2d9db-147">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="2d9db-148">Abra um e-mail que contenha alguns anexos de ficheiros de imagem.</span><span class="sxs-lookup"><span data-stu-id="2d9db-148">Open an email that contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="2d9db-149">Toque no ícone de seta para baixo junto às informações do anexo para guardá-lo.</span><span class="sxs-lookup"><span data-stu-id="2d9db-149">Tap the down arrow icon next to the attachment's info to save it.</span></span>
    
    ![Tap the down arrow to save the figure file to the Android device.](../media/08a9e21e-4022-45d5-acff-59cface651e7.png)
  
4. <span data-ttu-id="2d9db-p106">Poderá ser-lhe pedido para permitir que o Outlook aceda às fotografias, multimédia e ficheiros no seu dispositivo. Toque em **Permitir**.</span><span class="sxs-lookup"><span data-stu-id="2d9db-p106">You may be prompted to allow Outlook to access photos, media, and files on your device. Tap **Allow**.</span></span>
    
5. <span data-ttu-id="2d9db-153">Na parte inferior do ecrã, selecione **Guardar no Dispositivo** e, em seguida, abra a aplicação **Galeria**.</span><span class="sxs-lookup"><span data-stu-id="2d9db-153">At the bottom of the screen, choose to **Save to Device** and then open the **Gallery** app.</span></span> 
    
6. <span data-ttu-id="2d9db-p107">Deverá ver uma fotografia encriptada (ou mais, caso tenha guardado múltiplos anexos de ficheiros de imagem) na lista. A fotografia poderá ser apresentada na Lista de imagens como um quadrado cinzento com um ponto de exclamação branco dentro de um círculo branco no centro do quadrado cinzento.</span><span class="sxs-lookup"><span data-stu-id="2d9db-p107">You should see an encrypted photo (or more, if you saved multiple image file attachments) in the list. It may appear in the Pictures list as a gray square with a white exclamation point within a white circle in the center of the gray square.</span></span>
    
    ![An encrypted image file in the Gallery app.](../media/25936414-bd7e-421d-824e-6e59b877722d.png)
  
## <a name="ios"></a><span data-ttu-id="2d9db-157">iOS</span><span class="sxs-lookup"><span data-stu-id="2d9db-157">iOS</span></span>
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="2d9db-158">Verificar se as definições de proteção de aplicações estão a funcionar nos dispositivos dos utilizadores</span><span class="sxs-lookup"><span data-stu-id="2d9db-158">Check that the App protection settings are working on user devices</span></span>

<span data-ttu-id="2d9db-159">Depois de [definir as configurações das aplicações para dispositivos iOS](app-protection-settings-for-android-and-ios.md) para proteger as aplicações, pode seguir estes passos para verificar se as definições que escolheu estão a funcionar.</span><span class="sxs-lookup"><span data-stu-id="2d9db-159">After you [set app configurations for iOS devices](app-protection-settings-for-android-and-ios.md) to protect apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="2d9db-160">Em primeiro lugar, certifique-se de que a apólice se aplica à aplicação na qual a vai validar.</span><span class="sxs-lookup"><span data-stu-id="2d9db-160">First, make sure that the policy applies to the app in which you're going to validate it.</span></span>
  
1. <span data-ttu-id="2d9db-161">No [centro de administração](https://portal.office.com)Microsoft 365 Business Premium, vá para a **política de edição**de **políticas.** \></span><span class="sxs-lookup"><span data-stu-id="2d9db-161">In the Microsoft 365 Business Premium [admin center](https://portal.office.com), go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="2d9db-162">Escolha a política de **Aplicação para iOS** para as definições que criou na configuração, ou outra política que criou, e verifique se é aplicada para o Outlook, por exemplo.</span><span class="sxs-lookup"><span data-stu-id="2d9db-162">Choose **Application policy for iOS** for the settings you created at setup, or another policy you created, and verify that it's enforced for Outlook for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](../media/842441b8-e7b1-4b86-9edd-d94d1f77b6f4.png)
  
### <a name="validate-require-a-pin-to-access-office-apps"></a><span data-ttu-id="2d9db-164">Verificar a opção para exigir um PIN para aceder às aplicações do Office</span><span class="sxs-lookup"><span data-stu-id="2d9db-164">Validate Require a PIN to access Office apps</span></span>

<span data-ttu-id="2d9db-165">No painel **Editar política**, selecione **Editar** junto a **Controlo do acesso a documentos do Office**. Expanda a secção **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis** e certifique-se de que a opção **Exigir um PIN ou impressão digital para aceder às aplicações do Office** está definida como **Ativada**.</span><span class="sxs-lookup"><span data-stu-id="2d9db-165">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Certifique-se de que o Requer um PIN ou uma impressão digital para aceder às aplicações do Office está definido para On.](../media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="2d9db-167">No dispositivo iOS do utilizador, abra o Outlook e inscreva-se com as credenciais Microsoft 365 Business Premium do utilizador.</span><span class="sxs-lookup"><span data-stu-id="2d9db-167">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="2d9db-168">Também será solicitado a introduzir um PIN ou a utilizar uma impressão digital.</span><span class="sxs-lookup"><span data-stu-id="2d9db-168">You'll also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your IOS device to access Office apps.](../media/06fc5cf3-9f19-4090-b23c-14bb59805b7a.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="2d9db-170">Verificar a opção para repor o PIN após um número de tentativas falhadas</span><span class="sxs-lookup"><span data-stu-id="2d9db-170">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="2d9db-171">No painel de **política edite,** escolha **Editar** ao lado do controlo de acesso de **documentos do Office,** expandir **Gerir a forma como os utilizadores acedem aos ficheiros do Office em dispositivos móveis,** e certifique-se de que **o Reset PIN após o número de tentativas falhadas** está definido para algum número.</span><span class="sxs-lookup"><span data-stu-id="2d9db-171">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number.</span></span> <span data-ttu-id="2d9db-172">Este é 5 por defeito.</span><span class="sxs-lookup"><span data-stu-id="2d9db-172">This is 5 by default.</span></span> 
  
1. <span data-ttu-id="2d9db-173">No dispositivo iOS do utilizador, abra o Outlook e inscreva-se com as credenciais Microsoft 365 Business Premium do utilizador.</span><span class="sxs-lookup"><span data-stu-id="2d9db-173">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="2d9db-174">Introduza um PIN incorreto tantas vezes quanto for especificado pela política.</span><span class="sxs-lookup"><span data-stu-id="2d9db-174">Enter an incorrect PIN as many times as specified by the policy.</span></span> <span data-ttu-id="2d9db-175">Verá uma solicitação que indica **pin tente limite atingido** para redefinir o PIN.</span><span class="sxs-lookup"><span data-stu-id="2d9db-175">You'll see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](../media/fab5c089-a4a5-4e8d-8c95-b8eed1dfa262.png)
  
3. <span data-ttu-id="2d9db-177">Prima **OK**.</span><span class="sxs-lookup"><span data-stu-id="2d9db-177">Press **OK**.</span></span> <span data-ttu-id="2d9db-178">Será solicitado a iniciar sessão com as credenciais Microsoft 365 Business Premium do utilizador e, em seguida, obrigado a definir um novo PIN.</span><span class="sxs-lookup"><span data-stu-id="2d9db-178">You'll be prompted to sign in with the user's Microsoft 365 Business Premium credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="2d9db-179">Verificar a opção para forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas</span><span class="sxs-lookup"><span data-stu-id="2d9db-179">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="2d9db-180">No painel **Editar política**, selecione **Editar** junto a **Proteção contra dispositivos perdidos ou roubados**. Expanda a secção **Proteger os ficheiros de trabalho se os dispositivos forem perdidos ou roubados** e certifique-se de que a opção **Forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas** está definida como **Ativada**.</span><span class="sxs-lookup"><span data-stu-id="2d9db-180">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](../media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="2d9db-182">No dispositivo iOS do utilizador, abra o Outlook e inscreva-se com as credenciais Microsoft 365 Business Premium do utilizador e introduza um PIN se solicitado.</span><span class="sxs-lookup"><span data-stu-id="2d9db-182">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="2d9db-183">Abra um e-mail que contenha um anexo, abra o anexo e selecione **Guardar** na parte inferior do ecrã.</span><span class="sxs-lookup"><span data-stu-id="2d9db-183">Open an email that contains an attachment, open the attachment and choose **Save** on the bottom of the screen.</span></span> 
    
    ![Tap the Save option after you open an attachment to try to save it.](../media/b419b070-1530-4f14-86a8-8d89933a2b25.png)
  
3. <span data-ttu-id="2d9db-185">Deverá ver apenas uma opção para o OneDrive para Empresas.</span><span class="sxs-lookup"><span data-stu-id="2d9db-185">You should only see an option for OneDrive for Business.</span></span> <span data-ttu-id="2d9db-186">Caso contrário, toque em **Adicionar Conta** e selecione **OneDrive para Negócios** a partir do ecrã **da Conta de Armazenamento Adicionar.**</span><span class="sxs-lookup"><span data-stu-id="2d9db-186">If not, tap **Add Account** and select **OneDrive for Business** from the **Add Storage Account** screen.</span></span> <span data-ttu-id="2d9db-187">Forneça ao Microsoft 365 Business Premium do utilizador final para iniciar sessão quando solicitado.</span><span class="sxs-lookup"><span data-stu-id="2d9db-187">Provide the end user's Microsoft 365 Business Premium to sign in when prompted.</span></span> 
    
    <span data-ttu-id="2d9db-188">Toque em **Guardar** e selecione **OneDrive para Empresas**.</span><span class="sxs-lookup"><span data-stu-id="2d9db-188">Tap **Save** and select **OneDrive for Business**.</span></span>
    
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="2d9db-189">Verificar a opção para exigir que o utilizador inicie sessão novamente caso as aplicações do Office estejam inativas durante um período de tempo específico</span><span class="sxs-lookup"><span data-stu-id="2d9db-189">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="2d9db-190">No painel de **política edite,** escolha **Editar** ao lado do controlo de acesso de **documentos do Office,** expandir **Gerir a forma como os utilizadores acedem aos ficheiros do Office em dispositivos móveis,** e certifique-se de que os utilizadores voltam a fazer o início depois de as aplicações do Office terem sido **inativas,** está definida para alguns minutos.</span><span class="sxs-lookup"><span data-stu-id="2d9db-190">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes.</span></span> <span data-ttu-id="2d9db-191">São 30 minutos por defeito.</span><span class="sxs-lookup"><span data-stu-id="2d9db-191">This is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="2d9db-192">No dispositivo iOS do utilizador, abra o Outlook e inscreva-se com as credenciais Microsoft 365 Business Premium do utilizador e introduza um PIN se solicitado.</span><span class="sxs-lookup"><span data-stu-id="2d9db-192">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="2d9db-p113">Já deverá ver a caixa de entrada do Outlook. Não faça alterações ao dispositivo iOS durante, pelo menos, 30 minutos (ou outro período de tempo superior ao especificado na política). Provavelmente, o ecrã do dispositivo ficará mais escuro.</span><span class="sxs-lookup"><span data-stu-id="2d9db-p113">You should now see Outlook's inbox. Let the iOS device untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="2d9db-196">Acesso Outlook no dispositivo iOS novamente.</span><span class="sxs-lookup"><span data-stu-id="2d9db-196">Access Outlook on the iOS device again.</span></span>
    
4. <span data-ttu-id="2d9db-197">Será solicitado a introduzir o seu PIN antes de poder aceder novamente ao Outlook.</span><span class="sxs-lookup"><span data-stu-id="2d9db-197">You'll be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="2d9db-198">Verificar a opção para proteger ficheiros de trabalho com encriptação</span><span class="sxs-lookup"><span data-stu-id="2d9db-198">Validate Protect work files with encryption</span></span>

<span data-ttu-id="2d9db-199">No painel **Editar política**, selecione **Editar** junto a **Proteção contra dispositivos perdidos ou roubados**. Expanda a janela **Proteger os ficheiros de trabalho se os dispositivos forem perdidos ou roubados** e certifique-se de que a opção **Proteger ficheiros de trabalho com encriptação** está definida como **Ativada** e a opção **Forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas** está definida como **Desativada**.</span><span class="sxs-lookup"><span data-stu-id="2d9db-199">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="2d9db-200">No dispositivo iOS do utilizador, abra o Outlook e inscreva-se com as credenciais Microsoft 365 Business Premium do utilizador e introduza um PIN se solicitado.</span><span class="sxs-lookup"><span data-stu-id="2d9db-200">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="2d9db-201">Abra um e-mail que contenha alguns anexos de ficheiros de imagem.</span><span class="sxs-lookup"><span data-stu-id="2d9db-201">Open an email that contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="2d9db-202">Toque no anexo e, em seguida, toque na opção **Guardar** por baixo do mesmo.</span><span class="sxs-lookup"><span data-stu-id="2d9db-202">Tap the attachment and then tap the **Save** option under it.</span></span> 
    
4. <span data-ttu-id="2d9db-p114">Abra a aplicação **Fotografias** no ecrã principal. Deverá ver uma fotografia (ou mais, se tiver guardado múltiplos anexos de ficheiros de imagem) guardada, embora esteja encriptada.</span><span class="sxs-lookup"><span data-stu-id="2d9db-p114">Open **Photos** app from the home screen. You should see an encrypted photo (or more, if you saved multiple image file attachments) saved, but encrypted.</span></span> 
    
---

