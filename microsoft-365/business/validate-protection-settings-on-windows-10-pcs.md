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
description: Valide as definições de proteção de aplicações Do Microsoft 365 Business Premium em dispositivos Windows 10 e verifique que os utilizadores não podem copiar dados da empresa para ficheiros pessoais ou aplicações não geridas.
ms.openlocfilehash: 20b2e43ae53486c046440ff1066d241ec9661888
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/21/2020
ms.locfileid: "43635750"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="9e70d-103">Verificar definições de proteção de aplicações em PCs Windows 10</span><span class="sxs-lookup"><span data-stu-id="9e70d-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="9e70d-104">Confirmar que os utilizadores não conseguem copiar dados da empresa para ficheiros pessoais em dispositivos da empresa</span><span class="sxs-lookup"><span data-stu-id="9e70d-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="9e70d-105">Depois de [configurar as políticas de proteção de aplicações](protection-settings-for-windows-10-devices.md), as mesmas poderão demorar algumas horas a entrar em vigor nos dispositivos dos utilizadores.</span><span class="sxs-lookup"><span data-stu-id="9e70d-105">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="9e70d-106">Se **ligou** o Prevent que os utilizadores **copiassem os dados da empresa para ficheiros pessoais e os obrigasse a guardar ficheiros** de trabalho para a definição de OneDrive for Business para dispositivos da empresa, pode verificar isso no dispositivo do utilizador depois de terem ligado à Azure AD e terem assinado o seu registo.</span><span class="sxs-lookup"><span data-stu-id="9e70d-106">If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they've connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="9e70d-107">**Verificar definições de ligação**</span><span class="sxs-lookup"><span data-stu-id="9e70d-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="9e70d-108">Depois de iniciar sessão com credenciais Microsoft 365 Business Premium e ligar-se ao Azure AD conforme descrito na Configuração de [dispositivos Windows para utilizadores Microsoft 365 Business Premium](set-up-windows-devices.md), vá para as contas **de Definições** \> **Accounts** \> do Windows **O trabalho ou a escola**.</span><span class="sxs-lookup"><span data-stu-id="9e70d-108">After you sign in with Microsoft 365 Business Premium credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**.</span></span> <span data-ttu-id="9e70d-109">Selecione **Ligado ao Azure AD de \<nome do inquilino\>** e, em seguida, selecione **Informações**.</span><span class="sxs-lookup"><span data-stu-id="9e70d-109">Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="9e70d-111">Na página de \<nome\> do inquilino **gerida,** pode ver a **informação de Ligação** que inclui um Endereço de Servidor de **Gestão** como o mostrado na figura seguinte.</span><span class="sxs-lookup"><span data-stu-id="9e70d-111">On the **Managed by** \<tenant name\> page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="9e70d-113">**Verifique se não pode colar os dados da empresa numa aplicação não gerida**</span><span class="sxs-lookup"><span data-stu-id="9e70d-113">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="9e70d-114">Open Outlook 2016 que foi instalado pelo Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="9e70d-114">Open Outlook 2016 that was installed by Microsoft 365 Business Premium.</span></span>
    
2. <span data-ttu-id="9e70d-115">Abra um e-mail e copie alguns conteúdos do mesmo.</span><span class="sxs-lookup"><span data-stu-id="9e70d-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="9e70d-116">Abra o Bloco de Notas e tente colar os conteúdos na aplicação.</span><span class="sxs-lookup"><span data-stu-id="9e70d-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="9e70d-117">Receberá um erro que diz que a aplicação não pode aceder a conteúdos.</span><span class="sxs-lookup"><span data-stu-id="9e70d-117">You'll receive an error that states the app can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="9e70d-119">No entanto, poderá colar esses mesmos conteúdos no Word 2016.</span><span class="sxs-lookup"><span data-stu-id="9e70d-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="9e70d-120">Confirmar que os utilizadores não conseguem copiar dados da empresa para ficheiros em dispositivos pessoais</span><span class="sxs-lookup"><span data-stu-id="9e70d-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="9e70d-121">**Verificar definições de ligação**</span><span class="sxs-lookup"><span data-stu-id="9e70d-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="9e70d-122">No seu dispositivo pessoal do Windows 10, onde está registado como utilizador local, aceda às **Definições do Windows**e clique ou toque em **Contas** \> Aceder ao **trabalho ou à escola.**</span><span class="sxs-lookup"><span data-stu-id="9e70d-122">On your Windows 10 personal device where you're logged in as a local user, go to **Windows Settings**, and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="9e70d-123">Em **Aceder a profiss./escolar**, selecione **Ligar**.</span><span class="sxs-lookup"><span data-stu-id="9e70d-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="9e70d-124">Insira a sua credencial Microsoft 365 Business Premium na **Configuração de um diálogo** \> de conta de trabalho ou de conta escolar **.**</span><span class="sxs-lookup"><span data-stu-id="9e70d-124">Enter your Microsoft 365 Business Premium credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="9e70d-125">Na página **Aceder a profiss./escolar**, selecione a opção **Conta escolar ou profissional** e, em seguida, selecione **Informações**.</span><span class="sxs-lookup"><span data-stu-id="9e70d-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![Clique ou toque em Informações sobre o diálogo de conta de trabalho ou escola.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="9e70d-127">No trabalho de Acesso ou na página **da escola,** pode ver a **informação de Ligação** que inclui um Endereço de Servidor de **Gestão** como o mostrado na figura seguinte, e inclui as palavras *wip* e *mam* dentro.</span><span class="sxs-lookup"><span data-stu-id="9e70d-127">On the **Access work or school** page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="9e70d-129">**Verifique se não pode colar os dados da empresa numa aplicação não gerida**</span><span class="sxs-lookup"><span data-stu-id="9e70d-129">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="9e70d-130">Abra o Outlook 2016 e adicione a sua conta Microsoft 365 Business Premium se necessário e inscreva-se com as suas credenciais Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="9e70d-130">Open Outlook 2016 and add your Microsoft 365 Business Premium account if necessary and sign in with your Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="9e70d-131">Abra um e-mail e copie alguns conteúdos do mesmo.</span><span class="sxs-lookup"><span data-stu-id="9e70d-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="9e70d-132">Abra o Bloco de Notas e tente colar os conteúdos na aplicação.</span><span class="sxs-lookup"><span data-stu-id="9e70d-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="9e70d-133">Receberá um erro que diz que a App não pode aceder a conteúdos.</span><span class="sxs-lookup"><span data-stu-id="9e70d-133">You'll receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="9e70d-135">No entanto, poderá colar esses mesmos conteúdos no Word 2016.</span><span class="sxs-lookup"><span data-stu-id="9e70d-135">You can, however, paste the same content into Word 2016.</span></span>
    

