---
title: Verificar definições de proteção de aplicações em PCs Windows 10
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Obter informações sobre como validar as definições de protecção de aplicações Microsoft 365 Business Windows 10 dispositivos.
ms.openlocfilehash: f00dd380103ad9498d77b0e8814bace3de168df4
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983298"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="26fad-103">Verificar definições de proteção de aplicações em PCs Windows 10</span><span class="sxs-lookup"><span data-stu-id="26fad-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="26fad-104">Confirmar que os utilizadores não conseguem copiar dados da empresa para ficheiros pessoais em dispositivos da empresa</span><span class="sxs-lookup"><span data-stu-id="26fad-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="26fad-p101">Depois de [configurar as políticas de proteção de aplicações](protection-settings-for-windows-10-devices.md), as mesmas poderão demorar algumas horas a entrar em vigor nos dispositivos dos utilizadores. Se tiver mudado para **Ativado**, a definição **Impedir que os utilizadores copiem os dados da empresa para ficheiros pessoais e obrigá-los a guardar os ficheiros de trabalho no OneDrive para Empresas** para dispositivos da empresa, poderá verificá-lo no dispositivo do utilizador após o mesmo ter estabelecido ligação ao Azure AD e iniciado sessão.</span><span class="sxs-lookup"><span data-stu-id="26fad-p101">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices. If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they have connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="26fad-107">**Verificar definições de ligação**</span><span class="sxs-lookup"><span data-stu-id="26fad-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="26fad-p102">Depois de iniciar sessão com as credenciais Microsoft 365 Business e de estabelecer ligação ao Azure AD conforme descrito em [Configurar dispositivos Windows para utilizadores do Microsoft 365 Empresas](set-up-windows-devices.md), aceda a **Definições do Windows** \> **Contas** \> **Aceder a profiss./escolar**. Selecione **Ligado ao Azure AD de \<nome do inquilino\>** e, em seguida, selecione **Informações**.</span><span class="sxs-lookup"><span data-stu-id="26fad-p102">After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="26fad-111">Na página **Gerido por** \<nome do inquilino\>, poderá ver as **Informações de ligação** que incluem um **Endereço do Servidor de Gestão**, tal como o apresentado na imagem seguinte.</span><span class="sxs-lookup"><span data-stu-id="26fad-111">On the **Managed by** \<tenant name\> page you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="26fad-113">**Confirmar que não consegue colar dados da empresa numa aplicação não gerida**</span><span class="sxs-lookup"><span data-stu-id="26fad-113">**Verify that you cannot paste company data to a non-managed app**</span></span>
  
1. <span data-ttu-id="26fad-114">Abra a versão do Outlook 2016 que foi instalada pelo Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="26fad-114">Open Outlook 2016 that was installed by Microsoft 365 Business.</span></span>
    
2. <span data-ttu-id="26fad-115">Abra um e-mail e copie alguns conteúdos do mesmo.</span><span class="sxs-lookup"><span data-stu-id="26fad-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="26fad-116">Abra o Bloco de Notas e tente colar os conteúdos na aplicação.</span><span class="sxs-lookup"><span data-stu-id="26fad-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="26fad-117">Irá receber uma mensagem de erro a indicar que a aplicação não consegue aceder aos conteúdos.</span><span class="sxs-lookup"><span data-stu-id="26fad-117">You will receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="26fad-119">No entanto, poderá colar esses mesmos conteúdos no Word 2016.</span><span class="sxs-lookup"><span data-stu-id="26fad-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="26fad-120">Confirmar que os utilizadores não conseguem copiar dados da empresa para ficheiros em dispositivos pessoais</span><span class="sxs-lookup"><span data-stu-id="26fad-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="26fad-121">**Verificar definições de ligação**</span><span class="sxs-lookup"><span data-stu-id="26fad-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="26fad-122">No dispositivo pessoal Windows 10 onde tiver sessão iniciada como utilizador local, aceda a **Definições do Windows** e clique ou toque em **Contas** \> **Aceder a profiss./escolar**.</span><span class="sxs-lookup"><span data-stu-id="26fad-122">On your Windows 10 personal device where you are logged in as a local user, go to **Windows Settings** and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="26fad-123">Em **Aceder a profiss./escolar**, selecione **Ligar**.</span><span class="sxs-lookup"><span data-stu-id="26fad-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="26fad-124">Introduza a sua credencial Microsoft 365 Business na caixa de diálogo **Configurar uma conta escolar ou profissional** \> **Iniciar sessão**.</span><span class="sxs-lookup"><span data-stu-id="26fad-124">Enter your Microsoft 365 Business credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="26fad-125">Na página **Aceder a profiss./escolar**, selecione a opção **Conta escolar ou profissional** e, em seguida, selecione **Informações**.</span><span class="sxs-lookup"><span data-stu-id="26fad-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Work or school account dalog.](media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="26fad-127">Na página **Aceder a profiss./escolar**, poderá ver as **Informações de ligação** que incluem um **Endereço do Servidor de Gestão**, tal como o apresentado na imagem seguinte, bem como as palavras  *wip*  e  *mam*  .</span><span class="sxs-lookup"><span data-stu-id="26fad-127">On the **Access work or school** page you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="26fad-129">**Confirmar que não consegue colar dados da empresa numa aplicação não gerida**</span><span class="sxs-lookup"><span data-stu-id="26fad-129">**Verify that you cannot paste company data to a non-managed app**</span></span>
  
1. <span data-ttu-id="26fad-130">Abra o Outlook 2016, adicione a sua conta Microsoft 365 Business se necessário e inicie sessão com as suas credenciais Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="26fad-130">Open Outlook 2016 and add your Microsoft 365 Business account if necessary and sign in with your Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="26fad-131">Abra um e-mail e copie alguns conteúdos do mesmo.</span><span class="sxs-lookup"><span data-stu-id="26fad-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="26fad-132">Abra o Bloco de Notas e tente colar os conteúdos na aplicação.</span><span class="sxs-lookup"><span data-stu-id="26fad-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="26fad-133">Irá receber uma mensagem de erro a indicar que a aplicação não consegue aceder aos conteúdos.</span><span class="sxs-lookup"><span data-stu-id="26fad-133">You will receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="26fad-135">No entanto, poderá colar esses mesmos conteúdos no Word 2016.</span><span class="sxs-lookup"><span data-stu-id="26fad-135">You can, however, paste the same content into Word 2016.</span></span>
    

