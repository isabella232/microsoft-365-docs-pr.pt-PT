---
title: Configurar dispositivos Windows para utilizadores Microsoft 365 Business Premium
f1.keywords:
- CSH
ms.author: sharik
author: skjerland
manager: scotv
audience: Admin
ms.topic: article
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
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
- okr_smb
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: Saiba como configurar dispositivos Windows que executam o Windows 10 Pro para utilizadores Do Microsoft 365 Business Premium, permitindo controlos de gestão e segurança centralizados.
ms.openlocfilehash: 9c9ffe5bd74d9e9877a87309757c481576ee89d2
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578133"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="7d12e-103">Configurar dispositivos Windows para utilizadores Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="7d12e-103">Set up Windows devices for Microsoft 365 Business Premium users</span></span>

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="7d12e-104">Pré-requisitos para a configuração de dispositivos Windows para utilizadores Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="7d12e-104">Prerequisites for setting up Windows devices for Microsoft 365 Business Premium users</span></span>

<span data-ttu-id="7d12e-105">Antes de configurar dispositivos Windows para utilizadores Do Microsoft 365 Business Premium, certifique-se de que todos os dispositivos Windows estão a executar o Windows 10 Pro, versão 1703 (Creators Update).</span><span class="sxs-lookup"><span data-stu-id="7d12e-105">Before you can set up Windows devices for Microsoft 365 Business Premium users, make sure all the Windows devices are running Windows 10 Pro, version 1703 (Creators Update).</span></span> <span data-ttu-id="7d12e-106">O Windows 10 Pro é um pré-requisito para a implementação do Windows 10 Business, que é um conjunto de serviços na nuvem e capacidades de gestão de dispositivos que complementam o Windows 10 Pro e permitem os controlos de gestão e segurança centralizados do Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="7d12e-106">Windows 10 Pro is a prerequisite for deploying Windows 10 Business, which is a set of cloud services and device management capabilities that complement Windows 10 Pro and enable the centralized management and security controls of Microsoft 365 Business Premium.</span></span>
  
<span data-ttu-id="7d12e-107">Se tiver dispositivos Windows a executar o Windows 7 Pro, Windows 8 Pro ou Windows 8.1 Pro, a subscrição do Microsoft 365 Business Premium dá-lhe direito a uma atualização do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="7d12e-107">If you have Windows devices running Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your Microsoft 365 Business Premium subscription entitles you to a Windows 10 upgrade.</span></span>
  
<span data-ttu-id="7d12e-108">Para obter mais informações sobre como atualizar dispositivos Windows para a Atualização para Criativos do Windows 10 Pro, siga os passos neste tópico: [Atualizar dispositivos Windows para a Atualização para Criativos do Windows Pro](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="7d12e-108">For more information on how to upgrade Windows devices to Windows 10 Pro Creators Update, follow the steps in this topic: [Upgrade Windows devices to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
  
<span data-ttu-id="7d12e-109">Consulte [Verifique se o dispositivo está ligado à Azure AD](#verify-the-device-is-connected-to-azure-ad) para verificar se tem a atualização ou para se certificar de que a atualização funcionou.</span><span class="sxs-lookup"><span data-stu-id="7d12e-109">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to verify you have the upgrade, or to make sure the upgrade worked.</span></span>

<span data-ttu-id="7d12e-110">Veja um pequeno vídeo sobre a ligação do Windows ao Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7d12e-110">Watch a short video about connecting Windows to Microsoft 365.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

<span data-ttu-id="7d12e-111">Caso tenha considerado este vídeo útil, veja a [série de formação completa para pequenas empresas e as novidades do Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="7d12e-111">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a><span data-ttu-id="7d12e-112">Associar dispositivos Windows 10 ao Azure AD da sua organização</span><span class="sxs-lookup"><span data-stu-id="7d12e-112">Join Windows 10 devices to your organization's Azure AD</span></span>

<span data-ttu-id="7d12e-113">Quando todos os dispositivos Windows da sua organização tiverem sido atualizados para o Windows 10 Pro Creators Update ou já estiverem a executar a Atualização de Criadores Pro Do Windows 10, pode juntar estes dispositivos ao Azure Ative Directory da sua organização.</span><span class="sxs-lookup"><span data-stu-id="7d12e-113">When all Windows devices in your organization have either been upgraded to Windows 10 Pro Creators Update or are already running Windows 10 Pro Creators Update, you can join these devices to your organization's Azure Active Directory.</span></span> <span data-ttu-id="7d12e-114">Assim que os dispositivos forem aderidos, serão automaticamente atualizados para o Windows 10 Business, que faz parte da subscrição do Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="7d12e-114">Once the devices are joined, they'll be automatically upgraded to Windows 10 Business, which is part of your Microsoft 365 Business Premium subscription.</span></span>
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a><span data-ttu-id="7d12e-115">Para um dispositivo Windows 10 Pro novo ou recentemente atualizado</span><span class="sxs-lookup"><span data-stu-id="7d12e-115">For a brand new, or newly upgraded, Windows 10 Pro device</span></span>

<span data-ttu-id="7d12e-116">Para um novo dispositivo a executar a Atualização para Criativos do Windows 10 Pro ou para um dispositivo que foi atualizado para a Atualização para Criativos do Windows 10 Pro, mas cuja configuração do dispositivo Windows 10 não tenha sido efetuada, siga estes passos.</span><span class="sxs-lookup"><span data-stu-id="7d12e-116">For a brand new device running Windows 10 Pro Creators Update, or for a device that was upgraded to Windows 10 Pro Creators Update but has not gone through Windows 10 device setup, follow these steps.</span></span>
  
1. <span data-ttu-id="7d12e-117">Efetue a configuração do dispositivo Windows 10 até aceder à página **Como pretende configurar?**.</span><span class="sxs-lookup"><span data-stu-id="7d12e-117">Go through Windows 10 device setup until you get to the **How would you like to set up?** page.</span></span> 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. <span data-ttu-id="7d12e-119">Aqui, escolha **Configurar para uma organização** e, em seguida, introduzir o seu nome de utilizador e senha para Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="7d12e-119">Here, choose **Set up for an organization** and then enter your username and password for Microsoft 365 Business Premium.</span></span> 
    
3. <span data-ttu-id="7d12e-120">Conclua a configuração do dispositivo Windows 10.</span><span class="sxs-lookup"><span data-stu-id="7d12e-120">Finish Windows 10 device setup.</span></span>
    
   <span data-ttu-id="7d12e-p103">Quando terminar, o utilizador estará ligado ao Azure AD da sua organização. Consulte [Verificar se o dispositivo está ligado ao Azure AD](#verify-the-device-is-connected-to-azure-ad) para garantir que o dispositivo está ligado.</span><span class="sxs-lookup"><span data-stu-id="7d12e-p103">Once you're done, the user will be connected to your organization's Azure AD. See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to make sure.</span></span> 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a><span data-ttu-id="7d12e-123">Para um dispositivo que já esteja configurado e a executar o Windows 10 Pro</span><span class="sxs-lookup"><span data-stu-id="7d12e-123">For a device already set up and running Windows 10 Pro</span></span>

 <span data-ttu-id="7d12e-124">**Ligar utilizadores ao Azure AD:**</span><span class="sxs-lookup"><span data-stu-id="7d12e-124">**Connect users to Azure AD:**</span></span>
  
1. <span data-ttu-id="7d12e-125">No PC Windows do seu utilizador com o Windows 10 Pro, versão 1703 (Atualização para Criativos) (consulte os [pré-requisitos](pre-requisites-for-data-protection.md)), clique no logótipo do Windows e, em seguida, no ícone Definições.</span><span class="sxs-lookup"><span data-stu-id="7d12e-125">In your user's Windows PC, that is running Windows 10 Pro, version 1703 (Creators Update) (see [pre-requisites](pre-requisites-for-data-protection.md)), click the Windows logo, and then the Settings icon.</span></span>
  
   ![In the Start menu, click Windows Settings icon](../media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. <span data-ttu-id="7d12e-127">Nas **Definições**, aceda a **Contas**.</span><span class="sxs-lookup"><span data-stu-id="7d12e-127">In **Settings**, go to **Accounts**.</span></span>
  
   ![In Windows Settings, go to Accounts](../media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. <span data-ttu-id="7d12e-129">Na página **As suas informações**, clique em **Aceder a profiss./escolar** \> **Ligar**.</span><span class="sxs-lookup"><span data-stu-id="7d12e-129">On **Your info** page, click **Access work or school** \> **Connect**.</span></span>
  
   ![Choose Connect under Access work or school](../media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. <span data-ttu-id="7d12e-131">Na caixa de diálogo **Configurar uma conta escolar ou profissional**, em **Ações alternativas**, selecione **Adicionar este dispositivo ao Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="7d12e-131">On the **Set up a work or school account** dialog, under **Alternate actions**, choose **Join this device to Azure Active Directory**.</span></span>
  
   ![Click Join this device to Azure Active Directory](../media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. <span data-ttu-id="7d12e-133">Na página **Vamos iniciar a sua sessão**, introduza a sua conta escolar ou profissional \> **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="7d12e-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span></span>
  
   <span data-ttu-id="7d12e-134">Na página **Introduzir palavra-passe**, introduza a sua palavra-passe \> **Iniciar sessão**.</span><span class="sxs-lookup"><span data-stu-id="7d12e-134">On the **Enter password** page, enter your password \> **Sign in**.</span></span>
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. <span data-ttu-id="7d12e-136">Na página da **organização certifique-se de que esta é** a sua página de organização, verifique se a informação está correta e escolha **'Juntar-se'.**</span><span class="sxs-lookup"><span data-stu-id="7d12e-136">On the **Make sure this is your organization** page, verify that the information is correct, and choose **Join**.</span></span>
  
   <span data-ttu-id="7d12e-137">No **You're all set!**</span><span class="sxs-lookup"><span data-stu-id="7d12e-137">On the **You're all set!**</span></span> <span data-ttu-id="7d12e-138">página, chosse **Done**.</span><span class="sxs-lookup"><span data-stu-id="7d12e-138">page, chosse **Done**.</span></span>
  
   ![No the Certifique-se de que este é o seu ecrã de organização, escolha Junte-se](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
<span data-ttu-id="7d12e-140">Se tiver carregado ficheiros para o OneDrive para Empresas, sincronize-os novamente.</span><span class="sxs-lookup"><span data-stu-id="7d12e-140">If you uploaded files to OneDrive for Business, sync them back down.</span></span> <span data-ttu-id="7d12e-141">Se usou uma ferramenta de terceiros para migrar perfis e ficheiros, também os sincroniza para o novo perfil.</span><span class="sxs-lookup"><span data-stu-id="7d12e-141">If you used a third-party tool to migrate profile and files, also sync those to the new profile.</span></span>
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a><span data-ttu-id="7d12e-142">Verificar se o dispositivo está ligado ao Azure AD</span><span class="sxs-lookup"><span data-stu-id="7d12e-142">Verify the device is connected to Azure AD</span></span>

<span data-ttu-id="7d12e-143">Para verificar o estado da sincronização, na página **de trabalho de acesso ou escola** em **Definições,** selecione a área **Ligada a** _ _ para expor \<organization name\> os botões **Informação** e **Desconexão**.</span><span class="sxs-lookup"><span data-stu-id="7d12e-143">To verify your sync status, on the **Access work or school** page in **Settings**, select the **Connected to** _ \<organization name\> _ area to expose the buttons **Info** and **Disconnect**.</span></span> <span data-ttu-id="7d12e-144">Escolha **Informação** para obter o seu estado de sincronização.</span><span class="sxs-lookup"><span data-stu-id="7d12e-144">Choose **Info** to get your synchronization status.</span></span> 
  
<span data-ttu-id="7d12e-145">Na página de estado do **Sync,** escolha **o Sync** para obter as mais recentes políticas de gestão de dispositivos móveis no PC.</span><span class="sxs-lookup"><span data-stu-id="7d12e-145">On the **Sync status** page, choose **Sync** to get the latest mobile device management policies onto the PC.</span></span>
  
<span data-ttu-id="7d12e-146">Para começar a utilizar a conta Microsoft 365 Business Premium, aceda ao **botão** Iniciar o Windows, clique com o botão correto da sua conta corrente e, em seguida, **a conta Switch**.</span><span class="sxs-lookup"><span data-stu-id="7d12e-146">To start using the Microsoft 365 Business Premium account, go to the Windows **Start** button, right-click your current account picture, and then **Switch account**.</span></span> <span data-ttu-id="7d12e-147">Inicie sessão com o endereço de e-mail e palavra-passe da sua organização.</span><span class="sxs-lookup"><span data-stu-id="7d12e-147">Sign in by using your organization email and password.</span></span>
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-pc-is-upgraded-to-windows-10-business"></a><span data-ttu-id="7d12e-149">Verifique se o PC está atualizado para o Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="7d12e-149">Verify the PC is upgraded to Windows 10 Business</span></span>

<span data-ttu-id="7d12e-150">Verifique se o seu Azure AD aderiu aos dispositivos windows 10 e está atualizado para o Windows 10 Business como parte da subscrição do Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="7d12e-150">Verify that your Azure AD joined Windows 10 devices are upgraded to Windows 10 Business as part of your Microsoft 365 Business Premium subscription.</span></span>
  
1. <span data-ttu-id="7d12e-151">Aceda a **Definições** \> **Sistema** \> **Acerca de**.</span><span class="sxs-lookup"><span data-stu-id="7d12e-151">Go to **Settings** \> **System** \> **About**.</span></span>
    
2. <span data-ttu-id="7d12e-152">Confirme que a **Edição** apresenta **Windows 10 Business**.</span><span class="sxs-lookup"><span data-stu-id="7d12e-152">Confirm that the **Edition** shows **Windows 10 Business**.</span></span>
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a><span data-ttu-id="7d12e-154">Next steps</span><span class="sxs-lookup"><span data-stu-id="7d12e-154">Next steps</span></span>

<span data-ttu-id="7d12e-155">Para configurar os seus dispositivos móveis, consulte [configurar dispositivos móveis para utilizadores Microsoft 365 Business Premium](set-up-mobile-devices.md), Para definir políticas de proteção de dispositivos ou de proteção de aplicações, consulte [Gerir o Microsoft 365 para o negócio](manage.md).</span><span class="sxs-lookup"><span data-stu-id="7d12e-155">To set up your mobile devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md), To set device protection or app protection policies, see [Manage Microsoft 365 for business](manage.md).</span></span>
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a><span data-ttu-id="7d12e-156">Para mais informações sobre a configuração e utilização do Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="7d12e-156">For more on setting up and using Microsoft 365 Business Premium</span></span>

[<span data-ttu-id="7d12e-157">Microsoft 365 para vídeos de formação de negócios</span><span class="sxs-lookup"><span data-stu-id="7d12e-157">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
