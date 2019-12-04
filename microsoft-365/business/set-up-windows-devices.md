---
title: Configurar dispositivos Windows para utilizadores do Microsoft 365 Business
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
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: 'Saiba como configurar dispositivos Windows que executam o Windows 10 Pro para usuários do Microsoft 365 Business. '
ms.openlocfilehash: b377c1e69d117b893b256880cd3b9972e33345c7
ms.sourcegitcommit: 8fda7852b2a5baa92b8a365865b014ea6d100bbc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/03/2019
ms.locfileid: "39812884"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-users"></a><span data-ttu-id="0e2c1-103">Configurar dispositivos Windows para utilizadores do Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="0e2c1-103">Set up Windows devices for Microsoft 365 Business users</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e2c1-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0e2c1-104">Prerequisites</span></span>

<span data-ttu-id="0e2c1-p101">Antes de poder configurar dispositivos Windows para os utilizadores do Microsoft 365 Business, certifique-se de que todos os dispositivos Windows estão a executar o Windows 10 Pro, versão 1703 (Atualização para Criativos). O Windows 10 Pro é um pré-requisito para implementar o Windows 10 Business, que é um conjunto de funcionalidades de gestão de dispositivos e serviços na nuvem que complementam o Windows 10 Pro e permitem a gestão centralizada e os controlos de segurança do Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-p101">Before you can set up Windows devices for Microsoft 365 Business users, make sure all the Windows devices are running Windows 10 Pro, version 1703 (Creators Update). Windows 10 Pro is a prerequisite for deploying Windows 10 Business, which is a set of cloud services and device management capabilities that complement Windows 10 Pro and enable the centralized management and security controls of Microsoft 365 Business.</span></span>
  
<span data-ttu-id="0e2c1-107">Se tiver dispositivos Windows a executar o Windows 7 Pro, Windows 8 Pro ou Windows 8.1 Pro, a sua subscrição do Microsoft 365 Business dá-lhe direito a uma atualização do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-107">If you have Windows devices running Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your Microsoft 365 Business subscription entitles you to a Windows 10 upgrade.</span></span>
  
<span data-ttu-id="0e2c1-108">Para obter mais informações sobre como atualizar dispositivos Windows para a Atualização para Criativos do Windows 10 Pro, siga os passos neste tópico: [Atualizar dispositivos Windows para a Atualização para Criativos do Windows Pro](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="0e2c1-108">For more information on how to upgrade Windows devices to Windows 10 Pro Creators Update, follow the steps in this topic: [Upgrade Windows devices to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
  
<span data-ttu-id="0e2c1-109">[Verifique se o dispositivo está conectado ao AD do Azure](#verify-the-device-is-connected-to-azure-ad) para verificar se você tem a atualização ou para garantir que a atualização funcione.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-109">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to verify you have the upgrade, or to make sure the upgrade worked.</span></span>

<span data-ttu-id="0e2c1-110">Assista a um pequeno vídeo sobre a conexão do Windows com o Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-110">Watch a short video about connecting Windows to Microsoft 365.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

<span data-ttu-id="0e2c1-111">Se você achou este vídeo útil, confira a série de [treinamento completo para pequenas empresas e as novas para a Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="0e2c1-111">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a><span data-ttu-id="0e2c1-112">Associar dispositivos Windows 10 ao Azure AD da sua organização</span><span class="sxs-lookup"><span data-stu-id="0e2c1-112">Join Windows 10 devices to your organization's Azure AD</span></span>

<span data-ttu-id="0e2c1-113">Quando todos os dispositivos Windows da sua organização tiverem sido atualizados para o Windows 10 Pro Creators Update ou já estiverem executando o Windows 10 Pro Creators Update, você pode conectar esses dispositivos ao Diretório Ativo Azure da sua organização.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-113">When all Windows devices in your organization have either been upgraded to Windows 10 Pro Creators Update or are already running Windows 10 Pro Creators Update, you can join these devices to your organization's Azure Active Directory.</span></span> <span data-ttu-id="0e2c1-114">Uma vez que os dispositivos são aderidos, eles serão atualizados automaticamente para o Windows 10 Business, que faz parte da sua assinatura Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-114">Once the devices are joined, they'll be automatically upgraded to Windows 10 Business, which is part of your Microsoft 365 Business subscription.</span></span>
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a><span data-ttu-id="0e2c1-115">Para um dispositivo Windows 10 Pro novo ou recentemente atualizado</span><span class="sxs-lookup"><span data-stu-id="0e2c1-115">For a brand new, or newly upgraded, Windows 10 Pro device</span></span>

<span data-ttu-id="0e2c1-116">Para um novo dispositivo a executar a Atualização para Criativos do Windows 10 Pro ou para um dispositivo que foi atualizado para a Atualização para Criativos do Windows 10 Pro, mas cuja configuração do dispositivo Windows 10 não tenha sido efetuada, siga estes passos.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-116">For a brand new device running Windows 10 Pro Creators Update, or for a device that was upgraded to Windows 10 Pro Creators Update but has not gone through Windows 10 device setup, follow these steps.</span></span>
  
1. <span data-ttu-id="0e2c1-117">Efetue a configuração do dispositivo Windows 10 até aceder à página **Como pretende configurar?**.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-117">Go through Windows 10 device setup until you get to the **How would you like to set up?** page.</span></span> 
    
    ![On the How would you like to set up page, choose Set up for an organization](media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. <span data-ttu-id="0e2c1-119">Selecione **Configurar para uma organização** e, em seguida, introduza o seu nome de utilizador e palavra-passe do Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-119">Here, choose **Set up for an organization** and then enter your username and password for Microsoft 365 Business.</span></span> 
    
3. <span data-ttu-id="0e2c1-120">Conclua a configuração do dispositivo Windows 10.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-120">Finish Windows 10 device setup.</span></span>
    
   <span data-ttu-id="0e2c1-p103">Quando terminar, o utilizador estará ligado ao Azure AD da sua organização. Consulte [Verificar se o dispositivo está ligado ao Azure AD](#verify-the-device-is-connected-to-azure-ad) para garantir que o dispositivo está ligado.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-p103">Once you're done, the user will be connected to your organization's Azure AD. See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to make sure.</span></span> 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a><span data-ttu-id="0e2c1-123">Para um dispositivo que já esteja configurado e a executar o Windows 10 Pro</span><span class="sxs-lookup"><span data-stu-id="0e2c1-123">For a device already set up and running Windows 10 Pro</span></span>

 <span data-ttu-id="0e2c1-124">**Ligar utilizadores ao Azure AD:**</span><span class="sxs-lookup"><span data-stu-id="0e2c1-124">**Connect users to Azure AD:**</span></span>
  
1. <span data-ttu-id="0e2c1-125">No PC Windows do seu utilizador com o Windows 10 Pro, versão 1703 (Atualização para Criativos) (consulte os [pré-requisitos](pre-requisites-for-data-protection.md)), clique no logótipo do Windows e, em seguida, no ícone Definições.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-125">In your user's Windows PC, that is running Windows 10 Pro, version 1703 (Creators Update) (see [pre-requisites](pre-requisites-for-data-protection.md)), click the Windows logo, and then the Settings icon.</span></span>
  
   ![In the Start menu, click Windows Settings icon](media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. <span data-ttu-id="0e2c1-127">Nas **Definições**, aceda a **Contas**.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-127">In **Settings**, go to **Accounts**.</span></span>
  
   ![In Windows Settings, go to Accounts](media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. <span data-ttu-id="0e2c1-129">Na página **As suas informações**, clique em **Aceder a profiss./escolar** \> **Ligar**.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-129">On **Your info** page, click **Access work or school** \> **Connect**.</span></span>
  
   ![Choose Connect under Access work or school](media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. <span data-ttu-id="0e2c1-131">Na caixa de diálogo **Configurar uma conta escolar ou profissional**, em **Ações alternativas**, selecione **Adicionar este dispositivo ao Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-131">On the **Set up a work or school account** dialog, under **Alternate actions**, choose **Join this device to Azure Active Directory**.</span></span>
  
   ![Click Join this device to Azure Active Directory](media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. <span data-ttu-id="0e2c1-133">Na página **Vamos iniciar a sua sessão**, introduza a sua conta escolar ou profissional \> **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span></span>
  
   <span data-ttu-id="0e2c1-134">Na página **Introduzir palavra-passe**, introduza a sua palavra-passe \> **Iniciar sessão**.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-134">On the **Enter password** page, enter your password \> **Sign in**.</span></span>
  
   ![Enter your work or school email on the Let's get you signed in page](media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. <span data-ttu-id="0e2c1-136">No **Verifique se esta é a** página da sua organização, verifique se as informações estão corretas e clique em **Participar.**</span><span class="sxs-lookup"><span data-stu-id="0e2c1-136">On the **Make sure this is your organization** page, verify that the information is correct, and click **Join**.</span></span>
  
   <span data-ttu-id="0e2c1-p104">Na página **Está pronto!**, clique em **Concluído**.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-p104">On the **You're all set!** page, click **Done**.</span></span>
  
   ![On the Make sure this is your organization screen, click Join](media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
<span data-ttu-id="0e2c1-140">Se tiver carregado ficheiros para o OneDrive para Empresas, sincronize-os novamente.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-140">If you uploaded files to OneDrive for Business, sync them back down.</span></span> <span data-ttu-id="0e2c1-141">Se você usou uma ferramenta de terceiros para migrar perfil e arquivos, também sincronizá-los com o novo perfil.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-141">If you used a third-party tool to migrate profile and files, also sync those to the new profile.</span></span>
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a><span data-ttu-id="0e2c1-142">Verificar se o dispositivo está ligado ao Azure AD</span><span class="sxs-lookup"><span data-stu-id="0e2c1-142">Verify the device is connected to Azure AD</span></span>

<span data-ttu-id="0e2c1-p106">Para verificar o seu estado de sincronização, na página **Aceder a profiss./escolar** nas **Definições**, clique na área **Ligado a** _ \<organization name\> _ para revelar os botões **Informações** e **Desligar**. Clique em **Informações** para obter o seu estado de sincronização.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-p106">To verify your sync status, on the **Access work or school** page in **Settings**, click in the **Connected to** _ \<organization name\> _ area to expose the buttons **Info** and **Disconnect**. Click on **Info** to get your synchronization status.</span></span> 
  
<span data-ttu-id="0e2c1-145">Na página Estado de sincronização, clique em Sincronizar para obter as mais recentes políticas de gestão de dispositivos móveis no PC.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-145">On the Sync status page, click Sync to get the latest mobile device management policies onto the PC.</span></span>
  
<span data-ttu-id="0e2c1-146">Para começar a usar a conta Microsoft 365 Business, acesse o botão Windows **Start,** clique na foto da sua conta corrente e, em seguida, **alternar**a conta.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-146">To start using the Microsoft 365 Business account, go to the Windows **Start** button, right-click your current account picture, and then **Switch account**.</span></span> <span data-ttu-id="0e2c1-147">Inicie sessão com o endereço de e-mail e palavra-passe da sua organização.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-147">Sign in by using your organization email and password.</span></span>
  
![Click Info button to view synchronization status](media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-device-is-upgraded-to-windows-10-business"></a><span data-ttu-id="0e2c1-149">Verificar se o dispositivo foi atualizado para o Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="0e2c1-149">Verify the device is upgraded to Windows 10 Business</span></span>

<span data-ttu-id="0e2c1-150">Verifique se os seus dispositivos Windows 10 associados ao Azure AD foram atualizados para o Windows 10 Business como parte da sua subscrição do Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-150">Verify that your Azure AD joined Windows 10 devices were upgraded to Windows 10 Business as part of your Microsoft 365 Business subscription.</span></span>
  
1. <span data-ttu-id="0e2c1-151">Aceda a **Definições** \> **Sistema** \> **Acerca de**.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-151">Go to **Settings** \> **System** \> **About**.</span></span>
    
2. <span data-ttu-id="0e2c1-152">Confirme que a **Edição** apresenta **Windows 10 Business**.</span><span class="sxs-lookup"><span data-stu-id="0e2c1-152">Confirm that the **Edition** shows **Windows 10 Business**.</span></span>
    
    ![Verify that Windows edition is Windows 10 Business.](media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a><span data-ttu-id="0e2c1-154">Next steps</span><span class="sxs-lookup"><span data-stu-id="0e2c1-154">Next steps</span></span>

<span data-ttu-id="0e2c1-155">Para configurar os seus dispositivos móveis, consulte [Configurar dispositivos móveis para utilizadores do Microsoft 365 Business](set-up-mobile-devices.md). Para definir políticas de proteção de aplicações ou proteção de dispositivos, consulte [Gerir o Microsoft 365 Business](manage.md).</span><span class="sxs-lookup"><span data-stu-id="0e2c1-155">To set up your mobile devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md), To set device protection or app protection policies, see [Manage Microsoft 365 Business](manage.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="0e2c1-156">See also</span><span class="sxs-lookup"><span data-stu-id="0e2c1-156">See also</span></span>

[<span data-ttu-id="0e2c1-157">Microsoft 365 Vídeos de treinamento de negócios</span><span class="sxs-lookup"><span data-stu-id="0e2c1-157">Microsoft 365 Business training videos</span></span>](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
