---
title: Verificar definições de proteção de aplicações em PCs Windows 10
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
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Valide as definições de proteção de aplicações do Microsoft 365 Business em dispositivos Windows 10 e verifique que os utilizadores não podem copiar dados da empresa para ficheiros pessoais ou aplicações não geridas.
ms.openlocfilehash: 5b798e0335188543fc308553f71085bcde8b7752
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/07/2020
ms.locfileid: "42560846"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="1fde0-103">Verificar definições de proteção de aplicações em PCs Windows 10</span><span class="sxs-lookup"><span data-stu-id="1fde0-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="1fde0-104">Confirmar que os utilizadores não conseguem copiar dados da empresa para ficheiros pessoais em dispositivos da empresa</span><span class="sxs-lookup"><span data-stu-id="1fde0-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="1fde0-105">Depois de [configurar as políticas de proteção de aplicações](protection-settings-for-windows-10-devices.md), as mesmas poderão demorar algumas horas a entrar em vigor nos dispositivos dos utilizadores.</span><span class="sxs-lookup"><span data-stu-id="1fde0-105">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="1fde0-106">Se **ligou** o Prevent que os utilizadores **copiassem os dados da empresa para ficheiros pessoais e os obrigasse a guardar ficheiros** de trabalho para a definição de OneDrive for Business para dispositivos da empresa, pode verificar isso no dispositivo do utilizador depois de terem ligado à Azure AD e terem assinado o seu registo.</span><span class="sxs-lookup"><span data-stu-id="1fde0-106">If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they've connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="1fde0-107">**Verificar definições de ligação**</span><span class="sxs-lookup"><span data-stu-id="1fde0-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="1fde0-p102">Depois de iniciar sessão com as credenciais Microsoft 365 Business e de estabelecer ligação ao Azure AD conforme descrito em [Configurar dispositivos Windows para utilizadores do Microsoft 365 Empresas](set-up-windows-devices.md), aceda a **Definições do Windows** \> **Contas** \> **Aceder a profiss./escolar**. Selecione **Ligado ao Azure AD de \<nome do inquilino\>** e, em seguida, selecione **Informações**.</span><span class="sxs-lookup"><span data-stu-id="1fde0-p102">After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="1fde0-111">Na página de \<nome\> do inquilino **gerida,** pode ver a **informação de Ligação** que inclui um Endereço de Servidor de **Gestão** como o mostrado na figura seguinte.</span><span class="sxs-lookup"><span data-stu-id="1fde0-111">On the **Managed by** \<tenant name\> page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="1fde0-113">**Verifique se não pode colar os dados da empresa numa aplicação não gerida**</span><span class="sxs-lookup"><span data-stu-id="1fde0-113">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="1fde0-114">Abra a versão do Outlook 2016 que foi instalada pelo Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="1fde0-114">Open Outlook 2016 that was installed by Microsoft 365 Business.</span></span>
    
2. <span data-ttu-id="1fde0-115">Abra um e-mail e copie alguns conteúdos do mesmo.</span><span class="sxs-lookup"><span data-stu-id="1fde0-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="1fde0-116">Abra o Bloco de Notas e tente colar os conteúdos na aplicação.</span><span class="sxs-lookup"><span data-stu-id="1fde0-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="1fde0-117">Receberá um erro que diz que a aplicação não pode aceder a conteúdos.</span><span class="sxs-lookup"><span data-stu-id="1fde0-117">You'll receive an error that states the app can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="1fde0-119">No entanto, poderá colar esses mesmos conteúdos no Word 2016.</span><span class="sxs-lookup"><span data-stu-id="1fde0-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="1fde0-120">Confirmar que os utilizadores não conseguem copiar dados da empresa para ficheiros em dispositivos pessoais</span><span class="sxs-lookup"><span data-stu-id="1fde0-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="1fde0-121">**Verificar definições de ligação**</span><span class="sxs-lookup"><span data-stu-id="1fde0-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="1fde0-122">No seu dispositivo pessoal do Windows 10, onde está registado como utilizador local, aceda às **Definições do Windows**e clique ou toque em **Contas** \> Aceder ao **trabalho ou à escola.**</span><span class="sxs-lookup"><span data-stu-id="1fde0-122">On your Windows 10 personal device where you're logged in as a local user, go to **Windows Settings**, and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="1fde0-123">Em **Aceder a profiss./escolar**, selecione **Ligar**.</span><span class="sxs-lookup"><span data-stu-id="1fde0-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="1fde0-124">Introduza a sua credencial Microsoft 365 Business na caixa de diálogo **Configurar uma conta escolar ou profissional** \> **Iniciar sessão**.</span><span class="sxs-lookup"><span data-stu-id="1fde0-124">Enter your Microsoft 365 Business credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="1fde0-125">Na página **Aceder a profiss./escolar**, selecione a opção **Conta escolar ou profissional** e, em seguida, selecione **Informações**.</span><span class="sxs-lookup"><span data-stu-id="1fde0-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![Clique ou toque em Informações sobre o diálogo de conta de trabalho ou escola.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="1fde0-127">No trabalho de Acesso ou na página **da escola,** pode ver a **informação de Ligação** que inclui um Endereço de Servidor de **Gestão** como o mostrado na figura seguinte, e inclui as palavras *wip* e *mam* dentro.</span><span class="sxs-lookup"><span data-stu-id="1fde0-127">On the **Access work or school** page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="1fde0-129">**Verifique se não pode colar os dados da empresa numa aplicação não gerida**</span><span class="sxs-lookup"><span data-stu-id="1fde0-129">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="1fde0-130">Abra o Outlook 2016, adicione a sua conta Microsoft 365 Business se necessário e inicie sessão com as suas credenciais Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="1fde0-130">Open Outlook 2016 and add your Microsoft 365 Business account if necessary and sign in with your Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="1fde0-131">Abra um e-mail e copie alguns conteúdos do mesmo.</span><span class="sxs-lookup"><span data-stu-id="1fde0-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="1fde0-132">Abra o Bloco de Notas e tente colar os conteúdos na aplicação.</span><span class="sxs-lookup"><span data-stu-id="1fde0-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="1fde0-133">Receberá um erro que diz que a App não pode aceder a conteúdos.</span><span class="sxs-lookup"><span data-stu-id="1fde0-133">You'll receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="1fde0-135">No entanto, poderá colar esses mesmos conteúdos no Word 2016.</span><span class="sxs-lookup"><span data-stu-id="1fde0-135">You can, however, paste the same content into Word 2016.</span></span>
    

