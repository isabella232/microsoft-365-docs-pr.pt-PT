---
title: Validar definições de protecção da aplicação em dispositivos Android ou iOS
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
ms.assetid: f3433b6b-02f7-447f-9d62-306bf03638b0
description: 'Learn how to validate the Microsoft 365 Business app protection settings in your Android or iOS devices.  '
ms.openlocfilehash: 5ab16d481bd11ec31a1387a7e94d8b08bb3e0abe
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32287408"
---
# <a name="validate-app-protection-settings-on-android-or-ios-devices"></a><span data-ttu-id="0186f-103">Validar definições de protecção da aplicação em dispositivos Android ou iOS</span><span class="sxs-lookup"><span data-stu-id="0186f-103">Validate app protection settings on Android or iOS devices</span></span>

<span data-ttu-id="0186f-104">Siga as instruções nos separadores para validar as definições de protecção de aplicações em dispositivos Android ou iOS.</span><span class="sxs-lookup"><span data-stu-id="0186f-104">Follow the instructions in the tabs to validate app protection settings on Android or iOS devices.</span></span>
  
## <a name="androidtab"></a>[<span data-ttu-id="0186f-105">Android</span><span class="sxs-lookup"><span data-stu-id="0186f-105">Android</span></span>](#tab/)
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="0186f-106">Verificar se as definições de proteção de aplicações estão a funcionar nos dispositivos dos utilizadores</span><span class="sxs-lookup"><span data-stu-id="0186f-106">Check that the App protection settings are working on user devices</span></span>

<span data-ttu-id="0186f-107">Depois de [definir as configurações das aplicações para dispositivos Android](app-protection-settings-for-android-and-ios.md) para proteger as aplicações, pode seguir estes passos para verificar se as definições que escolheu estão a funcionar.</span><span class="sxs-lookup"><span data-stu-id="0186f-107">After you [set app configurations for Android devices](app-protection-settings-for-android-and-ios.md) to protect the apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="0186f-108">Primeiro, certifique-se de que a política se aplica à aplicação em que a pretende verificar.</span><span class="sxs-lookup"><span data-stu-id="0186f-108">First, make sure that the policy applies to the app in which you are going to validate it.</span></span>
  
1. <span data-ttu-id="0186f-109">No [centro de administração](https://portal.office.com) do Microsoft 365 Business, aceda a **Políticas** \> **Editar política**.</span><span class="sxs-lookup"><span data-stu-id="0186f-109">In the Microsoft 365 Business [admin center](https://portal.office.com) go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="0186f-110">Selecione a opção **Política de aplicação para Android** para as definições que criou na configuração ou para outra política que tenha criado e verifique se a mesma está a ser imposta no Outlook, por exemplo.</span><span class="sxs-lookup"><span data-stu-id="0186f-110">Choose **Application policy for Android** for the settings you created at setup, or another policy you created, and verify that it is enforced for Outlook for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](media/b3be3ddd-f683-4073-8d7a-9c639a636a2c.png)
  
### <a name="validate-require-a-pin-or-a-fingerprint-to-access-office-apps"></a><span data-ttu-id="0186f-112">Verificar a opção para exigir um PIN ou uma impressão digital para aceder às aplicações do Office</span><span class="sxs-lookup"><span data-stu-id="0186f-112">Validate Require a PIN or a fingerprint to access Office apps</span></span>

<span data-ttu-id="0186f-113">No painel **Editar política**, selecione **Editar** junto a **Controlo do acesso a documentos do Office**. Expanda a secção **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis** e certifique-se de que a opção **Exigir um PIN ou impressão digital para aceder às aplicações do Office** está definida como **Ativada**.</span><span class="sxs-lookup"><span data-stu-id="0186f-113">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Make sure that the Require a PIN or fingerprint to acces Office apps is set to On.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="0186f-115">No dispositivo Android do utilizador, abra o Outlook e inicie sessão com as credenciais do Microsoft 365 Business do utilizador.</span><span class="sxs-lookup"><span data-stu-id="0186f-115">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="0186f-116">Também lhe será pedido para introduzir um PIN ou utilizar uma impressão digital.</span><span class="sxs-lookup"><span data-stu-id="0186f-116">You will also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your Android device to access Office apps.](media/9e8ecfee-8122-4a3a-8918-eece80344310.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="0186f-118">Verificar a opção para repor o PIN após um número de tentativas falhadas</span><span class="sxs-lookup"><span data-stu-id="0186f-118">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="0186f-119">No painel **Editar política**, selecione **Editar** junto a **Controlo do acesso a documentos do Office**. Expanda a secção **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis** e certifique-se de que a opção **Repor o PIN após um número de tentativas falhadas** tem um número definido (a predefinição é 5).</span><span class="sxs-lookup"><span data-stu-id="0186f-119">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number - this is 5 by default.</span></span> 
  
1. <span data-ttu-id="0186f-120">No dispositivo Android do utilizador, abra o Outlook e inicie sessão com as credenciais do Microsoft 365 Business do utilizador.</span><span class="sxs-lookup"><span data-stu-id="0186f-120">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="0186f-p101">Introduza um PIN incorreto tantas vezes quanto for especificado pela política. Será apresentado um aviso a indicar **Limite de Tentativas de PIN Atingido** para repor o PIN.</span><span class="sxs-lookup"><span data-stu-id="0186f-p101">Enter an incorrect PIN as many times as specified by the policy. You will see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fca6fcb4-bb5c-477f-af5e-5dc937e8b835.png)
  
3. <span data-ttu-id="0186f-p102">Prima **Repor PIN**. Ser-lhe-á pedido que inicie sessão com as credencias do Microsoft 365 Business do utilizador e, em seguida, que defina um novo PIN.</span><span class="sxs-lookup"><span data-stu-id="0186f-p102">Press **Reset PIN**. You will be prompted to sign in with the user's Microsoft 365 Business credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="0186f-126">Verificar a opção para forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas</span><span class="sxs-lookup"><span data-stu-id="0186f-126">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="0186f-127">No painel **Editar política**, selecione **Editar** junto a **Proteção contra dispositivos perdidos ou roubados**. Expanda a secção **Proteger os ficheiros de trabalho se os dispositivos forem perdidos ou roubados** e certifique-se de que a opção **Forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas** está definida como **Ativada**.</span><span class="sxs-lookup"><span data-stu-id="0186f-127">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="0186f-129">No dispositivo Android do utilizador, abra o Outlook e inicie sessão com as credenciais do Microsoft 365 Business do utilizador e, se lhe for pedido, introduza um PIN.</span><span class="sxs-lookup"><span data-stu-id="0186f-129">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="0186f-130">Abra um e-mail que contenha um anexo e toque no ícone de seta para baixo junto às informações do anexo.</span><span class="sxs-lookup"><span data-stu-id="0186f-130">Open an email that contains an attachment and tap the down arrow icon next to the attachment's information.</span></span>
    
    ![Tap the down arrow next to an attachment to try to save it.](media/b22573bb-91ce-455f-84fa-8feb2846b117.png)
  
    <span data-ttu-id="0186f-132">Será apresentada a mensagem **Não é possível guardar no dispositivo** na parte inferior do ecrã.</span><span class="sxs-lookup"><span data-stu-id="0186f-132">You will see **Cannot save to device** on the bottom of the screen.</span></span> 
    
    ![Warning text that indicates cannot save a file locally to an Android.](media/52ca3f3d-7ed0-4a52-9621-4872da6ea9c5.png)
  
    > [!NOTE]
    > <span data-ttu-id="0186f-134">A opção Guardar no OneDrive para Empresas não se encontra disponível para Android neste momento, por isso, só verá a opção para guardar localmente bloqueada.</span><span class="sxs-lookup"><span data-stu-id="0186f-134">Saving to OneDrive for Business is not enabled for Android at this time, so you can only see that saving locally is blocked.</span></span> 
  
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="0186f-135">Verificar a opção para exigir que o utilizador inicie sessão novamente caso as aplicações do Office estejam inativas durante um período de tempo específico</span><span class="sxs-lookup"><span data-stu-id="0186f-135">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="0186f-136">No painel **Editar política**, selecione **Editar** junto a **Controlo do acesso a documentos do Office**. Expanda a janela **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis** e certifique-se de que a opção **Exigir que os utilizadores iniciem sessão novamente após as aplicações do Office terem estado inativas durante** está definida para um determinado número de minutos (a predefinição é 30 minutos).</span><span class="sxs-lookup"><span data-stu-id="0186f-136">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes - this is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="0186f-137">No dispositivo Android do utilizador, abra o Outlook e inicie sessão com as credenciais do Microsoft 365 Business do utilizador e, se lhe for pedido, introduza um PIN.</span><span class="sxs-lookup"><span data-stu-id="0186f-137">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="0186f-p103">Já deverá ver a caixa de entrada do Outlook. Não faça alterações ao dispositivo Android inativo durante, pelo menos, 30 minutos (ou outro período de tempo superior ao especificado na política). Provavelmente, o ecrã do dispositivo ficará mais escuro.</span><span class="sxs-lookup"><span data-stu-id="0186f-p103">You should now see Outlook's inbox. Let the Android device idle untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="0186f-141">Aceda novamente ao Outlook no dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="0186f-141">Re-access Outlook on the Android device.</span></span>
    
4. <span data-ttu-id="0186f-142">Ser-lhe-á pedido que introduza o seu PIN antes de poder aceder novamente ao Outlook.</span><span class="sxs-lookup"><span data-stu-id="0186f-142">You will be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="0186f-143">Verificar a opção para proteger ficheiros de trabalho com encriptação</span><span class="sxs-lookup"><span data-stu-id="0186f-143">Validate Protect work files with encryption</span></span>

<span data-ttu-id="0186f-144">No painel **Editar política**, selecione **Editar** junto a **Proteção contra dispositivos perdidos ou roubados**. Expanda a janela **Proteger os ficheiros de trabalho se os dispositivos forem perdidos ou roubados** e certifique-se de que a opção **Proteger ficheiros de trabalho com encriptação** está definida como **Ativada** e a opção **Forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas** está definida como **Desativada**.</span><span class="sxs-lookup"><span data-stu-id="0186f-144">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="0186f-145">No dispositivo Android do utilizador, abra o Outlook e inicie sessão com as credenciais do Microsoft 365 Business do utilizador e, se lhe for pedido, introduza um PIN.</span><span class="sxs-lookup"><span data-stu-id="0186f-145">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="0186f-146">Abra um e-mail que contenha alguns anexos de ficheiros de imagem.</span><span class="sxs-lookup"><span data-stu-id="0186f-146">Open an email which contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="0186f-147">Toque no ícone de seta para baixo junto às informações do anexo para guardá-lo.</span><span class="sxs-lookup"><span data-stu-id="0186f-147">Tap the down arrow icon next to the attachment's info to save it.</span></span>
    
    ![Tap the down arrow to save the figure file to the Android device.](media/08a9e21e-4022-45d5-acff-59cface651e7.png)
  
4. <span data-ttu-id="0186f-p104">Poderá ser-lhe pedido para permitir que o Outlook aceda às fotografias, multimédia e ficheiros no seu dispositivo. Toque em **Permitir**.</span><span class="sxs-lookup"><span data-stu-id="0186f-p104">You may be prompted to allow Outlook to access photos, media, and files on your device. Tap **Allow**.</span></span>
    
5. <span data-ttu-id="0186f-151">Na parte inferior do ecrã, selecione **Guardar no Dispositivo** e, em seguida, abra a aplicação **Galeria**.</span><span class="sxs-lookup"><span data-stu-id="0186f-151">At the bottom of the screen, choose to **Save to Device** and then open the **Gallery** app.</span></span> 
    
6. <span data-ttu-id="0186f-p105">Deverá ver uma fotografia encriptada (ou mais, caso tenha guardado múltiplos anexos de ficheiros de imagem) na lista. A fotografia poderá ser apresentada na Lista de imagens como um quadrado cinzento com um ponto de exclamação branco dentro de um círculo branco no centro do quadrado cinzento.</span><span class="sxs-lookup"><span data-stu-id="0186f-p105">You should see an encrypted photo (or more, if you saved multiple image file attachments) in the list. It may appear in the Pictures list as a gray square with a white exclamation point within a white circle in the center of the gray square.</span></span>
    
    ![An encrypted image file in the Gallery app.](media/25936414-bd7e-421d-824e-6e59b877722d.png)
  
## <a name="iostab"></a>[<span data-ttu-id="0186f-155">iOS</span><span class="sxs-lookup"><span data-stu-id="0186f-155">iOS</span></span>](#tab/)
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="0186f-156">Verificar se as definições de proteção de aplicações estão a funcionar nos dispositivos dos utilizadores</span><span class="sxs-lookup"><span data-stu-id="0186f-156">Check that the App protection settings are working on user devices</span></span>

<span data-ttu-id="0186f-157">Depois de [definir as configurações das aplicações para dispositivos iOS](app-protection-settings-for-android-and-ios.md) para proteger as aplicações, pode seguir estes passos para verificar se as definições que escolheu estão a funcionar.</span><span class="sxs-lookup"><span data-stu-id="0186f-157">After you [set app configurations for iOS devices](app-protection-settings-for-android-and-ios.md) to protect apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="0186f-158">Primeiro, certifique-se de que a política se aplica à aplicação em que a pretende verificar.</span><span class="sxs-lookup"><span data-stu-id="0186f-158">First, make sure that the policy applies to the app in which you are going to validate it.</span></span>
  
1. <span data-ttu-id="0186f-159">No [centro de administração](https://portal.office.com) do Microsoft 365 Business, aceda a **Políticas** \> **Editar política**.</span><span class="sxs-lookup"><span data-stu-id="0186f-159">In the Microsoft 365 Business [admin center](https://portal.office.com), go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="0186f-160">Selecione a opção **Política de aplicação para iOS** para as definições que criou na configuração ou para outra política que tenha criado e verifique se a mesma está a ser imposta no Outlook, por exemplo.</span><span class="sxs-lookup"><span data-stu-id="0186f-160">Choose **Application policy for iOS** for the settings you created at setup, or another policy you created, and verify that it is enforced for Outlook for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](media/842441b8-e7b1-4b86-9edd-d94d1f77b6f4.png)
  
### <a name="validate-require-a-pin-to-access-office-apps"></a><span data-ttu-id="0186f-162">Verificar a opção para exigir um PIN para aceder às aplicações do Office</span><span class="sxs-lookup"><span data-stu-id="0186f-162">Validate Require a PIN to access Office apps</span></span>

<span data-ttu-id="0186f-163">No painel **Editar política**, selecione **Editar** junto a **Controlo do acesso a documentos do Office**. Expanda a secção **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis** e certifique-se de que a opção **Exigir um PIN ou impressão digital para aceder às aplicações do Office** está definida como **Ativada**.</span><span class="sxs-lookup"><span data-stu-id="0186f-163">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Make sure that the Require a PIN or fingerprint to acces Office apps is set to On.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="0186f-165">No dispositivo iOS do utilizador, abra o Outlook e inicie sessão com as credenciais do Microsoft 365 Business do utilizador.</span><span class="sxs-lookup"><span data-stu-id="0186f-165">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="0186f-166">Também lhe será pedido para introduzir um PIN ou utilizar uma impressão digital.</span><span class="sxs-lookup"><span data-stu-id="0186f-166">You will also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your IOS device to access Office apps.](media/06fc5cf3-9f19-4090-b23c-14bb59805b7a.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="0186f-168">Verificar a opção para repor o PIN após um número de tentativas falhadas</span><span class="sxs-lookup"><span data-stu-id="0186f-168">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="0186f-169">No painel **Editar política**, selecione **Editar** junto a **Controlo do acesso a documentos do Office**. Expanda a secção **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis** e certifique-se de que a opção **Repor o PIN após um número de tentativas falhadas** tem um número definido (a predefinição é 5).</span><span class="sxs-lookup"><span data-stu-id="0186f-169">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number - this is 5 by default.</span></span> 
  
1. <span data-ttu-id="0186f-170">No dispositivo iOS do utilizador, abra o Outlook e inicie sessão com as credenciais do Microsoft 365 Business do utilizador.</span><span class="sxs-lookup"><span data-stu-id="0186f-170">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="0186f-p106">Introduza um PIN incorreto tantas vezes quanto for especificado pela política. Será apresentado um aviso a indicar **Limite de Tentativas de PIN Atingido** para repor o PIN.</span><span class="sxs-lookup"><span data-stu-id="0186f-p106">Enter an incorrect PIN as many times as specified by the policy. You will see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fab5c089-a4a5-4e8d-8c95-b8eed1dfa262.png)
  
3. <span data-ttu-id="0186f-p107">Prima **OK**. Ser-lhe-á pedido que inicie sessão com as credencias do Microsoft 365 Business do utilizador e, em seguida, que defina um novo PIN.</span><span class="sxs-lookup"><span data-stu-id="0186f-p107">Press **OK**. You will be prompted to sign in with the user's Microsoft 365 Business credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="0186f-176">Verificar a opção para forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas</span><span class="sxs-lookup"><span data-stu-id="0186f-176">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="0186f-177">No painel **Editar política**, selecione **Editar** junto a **Proteção contra dispositivos perdidos ou roubados**. Expanda a secção **Proteger os ficheiros de trabalho se os dispositivos forem perdidos ou roubados** e certifique-se de que a opção **Forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas** está definida como **Ativada**.</span><span class="sxs-lookup"><span data-stu-id="0186f-177">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="0186f-179">No dispositivo iOS do utilizador, abra o Outlook e inicie sessão com as credenciais do Microsoft 365 Business do utilizador e, se lhe for pedido, introduza um PIN.</span><span class="sxs-lookup"><span data-stu-id="0186f-179">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="0186f-180">Abra um e-mail que contenha um anexo, abra o anexo e selecione **Guardar** na parte inferior do ecrã.</span><span class="sxs-lookup"><span data-stu-id="0186f-180">Open an email that contains an attachment, open the attachment and choose **Save** on the bottom of the screen.</span></span> 
    
    ![Tap the Save option after you open an attachment to try to save it.](media/b419b070-1530-4f14-86a8-8d89933a2b25.png)
  
3. <span data-ttu-id="0186f-p108">Deverá ver apenas uma opção para o OneDrive para Empresas. Se não for o caso, toque em **Adicionar Conta** e selecione **OneDrive para Empresas** no ecrã **Adicionar Conta de Armazenamento**. Introduza as credenciais do Microsoft 365 Business do utilizador final para iniciar sessão quando lhe for pedido.</span><span class="sxs-lookup"><span data-stu-id="0186f-p108">You should only see an option for OneDrive for Business. If not If not, tap **Add Account** and select **OneDrive for Business** from the **Add Storage Account** screen. Provide the end user's Microsoft 365 Business to sign in when prompted.</span></span> 
    
    <span data-ttu-id="0186f-185">Toque em **Guardar** e selecione **OneDrive para Empresas**.</span><span class="sxs-lookup"><span data-stu-id="0186f-185">Tap **Save** and select **OneDrive for Business**.</span></span>
    
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="0186f-186">Verificar a opção para exigir que o utilizador inicie sessão novamente caso as aplicações do Office estejam inativas durante um período de tempo específico</span><span class="sxs-lookup"><span data-stu-id="0186f-186">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="0186f-187">No painel **Editar política**, selecione **Editar** junto a **Controlo do acesso a documentos do Office**. Expanda a janela **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis** e certifique-se de que a opção **Exigir que os utilizadores iniciem sessão novamente após as aplicações do Office terem estado inativas durante** está definida para um determinado número de minutos (a predefinição é 30 minutos).</span><span class="sxs-lookup"><span data-stu-id="0186f-187">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes - this is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="0186f-188">No dispositivo iOS do utilizador, abra o Outlook e inicie sessão com as credenciais do Microsoft 365 Business do utilizador e, se lhe for pedido, introduza um PIN.</span><span class="sxs-lookup"><span data-stu-id="0186f-188">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="0186f-p109">Já deverá ver a caixa de entrada do Outlook. Não faça alterações ao dispositivo iOS durante, pelo menos, 30 minutos (ou outro período de tempo superior ao especificado na política). Provavelmente, o ecrã do dispositivo ficará mais escuro.</span><span class="sxs-lookup"><span data-stu-id="0186f-p109">You should now see Outlook's inbox. Let the iOS device untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="0186f-192">Volte a aceder ao Outlook no dispositivo iOS.</span><span class="sxs-lookup"><span data-stu-id="0186f-192">Re-access Outlook on the iOS device.</span></span>
    
4. <span data-ttu-id="0186f-193">Ser-lhe-á pedido que introduza o seu PIN antes de poder aceder novamente ao Outlook.</span><span class="sxs-lookup"><span data-stu-id="0186f-193">You will be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="0186f-194">Verificar a opção para proteger ficheiros de trabalho com encriptação</span><span class="sxs-lookup"><span data-stu-id="0186f-194">Validate Protect work files with encryption</span></span>

<span data-ttu-id="0186f-195">No painel **Editar política**, selecione **Editar** junto a **Proteção contra dispositivos perdidos ou roubados**. Expanda a janela **Proteger os ficheiros de trabalho se os dispositivos forem perdidos ou roubados** e certifique-se de que a opção **Proteger ficheiros de trabalho com encriptação** está definida como **Ativada** e a opção **Forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas** está definida como **Desativada**.</span><span class="sxs-lookup"><span data-stu-id="0186f-195">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="0186f-196">No dispositivo iOS do utilizador, abra o Outlook e inicie sessão com as credenciais do Microsoft 365 Business do utilizador e, se lhe for pedido, introduza um PIN.</span><span class="sxs-lookup"><span data-stu-id="0186f-196">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="0186f-197">Abra um e-mail que contenha alguns anexos de ficheiros de imagem.</span><span class="sxs-lookup"><span data-stu-id="0186f-197">Open an email which contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="0186f-198">Toque no anexo e, em seguida, toque na opção **Guardar** por baixo do mesmo.</span><span class="sxs-lookup"><span data-stu-id="0186f-198">Tap the attachment and then tap the **Save** option under it.</span></span> 
    
4. <span data-ttu-id="0186f-p110">Abra a aplicação **Fotografias** no ecrã principal. Deverá ver uma fotografia (ou mais, se tiver guardado múltiplos anexos de ficheiros de imagem) guardada, embora esteja encriptada.</span><span class="sxs-lookup"><span data-stu-id="0186f-p110">Open **Photos** app from the home screen. You should see an encrypted photo (or more, if you saved multiple image file attachments) saved, but encrypted.</span></span> 
    
---

