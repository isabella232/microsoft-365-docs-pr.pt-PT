---
title: Upgrade para Microsoft 365 Business a partir do Office 365 Business Premium
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
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Passos que atualizam o seu negócio do Office 365 Business Premium para o Microsoft 365 Business.
ms.openlocfilehash: e17ac2658c7276ba4a77de371847343866815c42
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/15/2020
ms.locfileid: "42065297"
---
# <a name="upgrade-to-microsoft-365-business-from-office-365-business-premium"></a><span data-ttu-id="b25c8-103">Upgrade para Microsoft 365 Business a partir do Office 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="b25c8-103">Upgrade to Microsoft 365 Business from Office 365 Business Premium</span></span>

<span data-ttu-id="b25c8-104">Se tiver um [Office 365 para subscrição](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2)de negócios , por exemplo, Office 365 Business Premium, pode facilmente fazer upgrade para o Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="b25c8-104">If you have an [Office 365 for business subscription](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2), for example, Office 365 Business Premium, you can easily upgrade to Microsoft 365 Business.</span></span> <span data-ttu-id="b25c8-105">Upgrade para Microsoft 365 Business se quiser adicionar:</span><span class="sxs-lookup"><span data-stu-id="b25c8-105">Upgrade to Microsoft 365 Business if you want to add:</span></span> 
- <span data-ttu-id="b25c8-106">Windows 10 Pro (para PCs que executam o Windows 8 ou mais tarde)</span><span class="sxs-lookup"><span data-stu-id="b25c8-106">Windows 10 Pro (to PCs running Windows 8 or later)</span></span>
- <span data-ttu-id="b25c8-107">Controlos simples que gerem dados empresariais em dispositivos</span><span class="sxs-lookup"><span data-stu-id="b25c8-107">Simple controls that manage business data on devices</span></span>
- <span data-ttu-id="b25c8-108">Capacidades de segurança avançadas.</span><span class="sxs-lookup"><span data-stu-id="b25c8-108">Advanced security capabilities.</span></span>
<span data-ttu-id="b25c8-109">Saiba mais sobre o Microsoft 365 Business em [Microsoft.com](https://www.microsoft.com/microsoft-365/business)</span><span class="sxs-lookup"><span data-stu-id="b25c8-109">Find out more about Microsoft 365 Business at [Microsoft.com](https://www.microsoft.com/microsoft-365/business)</span></span>

## <a name="whats-the-difference-between-office-365-business-premium-and-microsoft-365-business"></a><span data-ttu-id="b25c8-110">Qual é a diferença entre o Office 365 Business Premium e o Microsoft 365 Business?</span><span class="sxs-lookup"><span data-stu-id="b25c8-110">What's the difference between Office 365 Business Premium and Microsoft 365 Business?</span></span>
<span data-ttu-id="b25c8-111">Adicionámos uma comparação lado a lado destes dois planos à Descrição do [Serviço Empresarial Microsoft 365.](https://docs.microsoft.com/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description)</span><span class="sxs-lookup"><span data-stu-id="b25c8-111">We've added a side-by-side comparison of these two plans to the [Microsoft 365 Business Service Description](https://docs.microsoft.com/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description).</span></span> 

## <a name="before-you-get-started"></a><span data-ttu-id="b25c8-112">Antes de começar.</span><span class="sxs-lookup"><span data-stu-id="b25c8-112">Before you get started</span></span>

- <span data-ttu-id="b25c8-113">**Quando devo escolher fazer upgrade?**</span><span class="sxs-lookup"><span data-stu-id="b25c8-113">**When should I choose to upgrade?**</span></span> <span data-ttu-id="b25c8-114">O upgrade é a escolha certa quando pretende atualizar **todos os utilizadores atribuídos** a um único plano.</span><span class="sxs-lookup"><span data-stu-id="b25c8-114">Upgrade is the right choice when you want to upgrade **all users** assigned to a single plan.</span></span> <span data-ttu-id="b25c8-115">Ao optar pela atualização, todos os utilizadores do plano são transferidos para outro plano ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="b25c8-115">When you choose upgrade, all plan users get switched to another plan at the same time.</span></span> <span data-ttu-id="b25c8-116">Se não quiser atualizar todos os designados para um único plano, compre licenças para o novo plano (neste caso Microsoft 365 Business), e [atribua essas licenças individualmente](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) a cada utilizador que pretenda fazer upgrade.</span><span class="sxs-lookup"><span data-stu-id="b25c8-116">If you don't want to upgrade everyone assigned to a single plan, buy licenses for the new plan (in this case Microsoft 365 Business), and [assign those licenses individually](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) to each user that you want to upgrade.</span></span> 
- <span data-ttu-id="b25c8-117">**Alguns addons podem impedir a atualização** Se tentar iniciar uma atualização e tiver um addon que o impeça de continuar, pode remover primeiro o addon e, em seguida, adicioná-lo de volta mais tarde se ainda precisar.</span><span class="sxs-lookup"><span data-stu-id="b25c8-117">**Some add-ons might prevent the upgrade** If you try to start an upgrade and you have an add-on that prevents you from continuing, you can remove the add-on first, and then add it back later if you still need it.</span></span> 
- <span data-ttu-id="b25c8-118">**Se pagou o seu plano de pré-pagamento** Não há um caminho simples de atualização para planos pré-pagos.</span><span class="sxs-lookup"><span data-stu-id="b25c8-118">**If you prepaid your plan** There isn't a straightforward upgrade path for prepaid plans.</span></span> <span data-ttu-id="b25c8-119">Saberá se tem um plano pré-pago porque configura o seu plano usando uma identificação de produto que pode ter comprado numa loja.</span><span class="sxs-lookup"><span data-stu-id="b25c8-119">You'll know if you have a prepaid plan because you set up your plan using a product ID that you might have purchased in a store.</span></span> <span data-ttu-id="b25c8-120">Contacte um parceiro, vá à Microsoft Store ou espere até que o seu plano pré-pago expire para mudar para um novo plano.</span><span class="sxs-lookup"><span data-stu-id="b25c8-120">Contact a partner, go to the Microsoft Store, or wait until your prepaid plan expires to switch to a new plan.</span></span>

## <a name="upgrade-to-microsoft-365-business"></a><span data-ttu-id="b25c8-121">Upgrade para Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="b25c8-121">Upgrade to Microsoft 365 Business</span></span>
<span data-ttu-id="b25c8-122">Compre as suas licenças seguindo estes passos no [novo centro de administração:](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="b25c8-122">Buy your licenses by following these steps in the [new admin center](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview):</span></span>
1. <span data-ttu-id="b25c8-123">Assine no centro de <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>administração em .</span><span class="sxs-lookup"><span data-stu-id="b25c8-123">Sign into the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>
2. <span data-ttu-id="b25c8-124">Vá ao painel de navegação e selecione **Produtos de Faturação** \> **& Serviços**.</span><span class="sxs-lookup"><span data-stu-id="b25c8-124">Go to the navigation pane and select **Billing** \> **Products & Services**.</span></span> <span data-ttu-id="b25c8-125">Encontre a subscrição do Office 365 e selecione-a para ver os detalhes.</span><span class="sxs-lookup"><span data-stu-id="b25c8-125">Find your Office 365 subscription and select it to view the details.</span></span> 

    ![Uma imagem mostra como encontrar e selecionar a sua subscrição no centro de administração.](../media/FindYourSubscription.png)

3. <span data-ttu-id="b25c8-127">Na página seguinte, selecione **Upgrade**.</span><span class="sxs-lookup"><span data-stu-id="b25c8-127">On the next page, select **Upgrade**.</span></span> 

      ![Uma imagem mostra onde selecionar Upgrade no centro de administração.](../media/SelectUpgrade.png)

  > [!NOTE]
  > <span data-ttu-id="b25c8-129">Se vir uma mensagem que diga que atualizar a **sua subscrição não é suportado com licenciamento baseado em grupo no Azure Ative Directory,** pode ignorá-lo com segurança a menos que tenha uma organização muito grande.</span><span class="sxs-lookup"><span data-stu-id="b25c8-129">If you see a message that says **Upgrading your subscription is not supported with group-based licensing in Azure Active Directory**, you can safely ignore this unless you have a very large organization.</span></span> <span data-ttu-id="b25c8-130">As organizações que escolheram esta opção estarão cientes de que estão a usar o licenciamento baseado em grupo.</span><span class="sxs-lookup"><span data-stu-id="b25c8-130">Organizations who have selected this option will be aware that they're using group-based licensing.</span></span>

4. <span data-ttu-id="b25c8-131">Em seguida, pode ver uma lista de planos do Office para os dois.</span><span class="sxs-lookup"><span data-stu-id="b25c8-131">Next, you can view a list of Office plans that you can upgrade to.</span></span> <span data-ttu-id="b25c8-132">Neste caso, encontre o plano de negócios da Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b25c8-132">In this case, find the Microsoft 365 Business plan.</span></span> <span data-ttu-id="b25c8-133">Você pode rolar para baixo se você quiser ver todas as aplicações e serviços do Office que estão incluídos com este plano.</span><span class="sxs-lookup"><span data-stu-id="b25c8-133">You can scroll down if you want to see all the Office apps and services that are included with this plan.</span></span> <span data-ttu-id="b25c8-134">No **Microsoft 365 Business,** selecione **Upgrade** para adicionar o Microsoft 365 Business ao seu carrinho.</span><span class="sxs-lookup"><span data-stu-id="b25c8-134">Under **Microsoft 365 Business**, select **Upgrade** to add Microsoft 365 Business to your cart.</span></span>
5. <span data-ttu-id="b25c8-135">No carrinho:</span><span class="sxs-lookup"><span data-stu-id="b25c8-135">In the cart:</span></span>
    1. <span data-ttu-id="b25c8-136">Vamos automaticamente incluir licenças para todos os seus utilizadores atuais.</span><span class="sxs-lookup"><span data-stu-id="b25c8-136">We'll automatically include licenses for all your current users.</span></span> <span data-ttu-id="b25c8-137">Se precisar de mais ou menos licenças, tem de [comprar e atribuir essas licenças individualmente](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="b25c8-137">If you need more or fewer licenses, you need to [buy and assign those licenses individually](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users).</span></span>  
    2. <span data-ttu-id="b25c8-138">Pode ajustar a forma como gostaria de pagar: mensal ou anualmente.</span><span class="sxs-lookup"><span data-stu-id="b25c8-138">You can adjust how you'd like to pay: monthly or yearly.</span></span> <span data-ttu-id="b25c8-139">Selecione o menu suspenso para fazer a sua escolha.</span><span class="sxs-lookup"><span data-stu-id="b25c8-139">Select the drop-down menu to make your choice.</span></span>
6. <span data-ttu-id="b25c8-140">Selecione **Ir ao Checkout** onde verá um resumo da sua compra, incluindo o método de pagamento desta conta.</span><span class="sxs-lookup"><span data-stu-id="b25c8-140">Select **Go to Checkout** where you'll see a summary of your purchase, including the payment method for this account.</span></span> <span data-ttu-id="b25c8-141">Também pode adicionar um código promocional aqui se tiver um.</span><span class="sxs-lookup"><span data-stu-id="b25c8-141">You can also add a promo code here if you have one.</span></span>
7. <span data-ttu-id="b25c8-142">Selecione **O pedido de lugar** para completar a sua compra.</span><span class="sxs-lookup"><span data-stu-id="b25c8-142">Select **Place order** to complete your purchase.</span></span>
<span data-ttu-id="b25c8-143">A Microsoft leva alguns minutos para configurar os seus novos planos de serviço.</span><span class="sxs-lookup"><span data-stu-id="b25c8-143">It takes Microsoft a few minutes to set up your new service plans.</span></span> <span data-ttu-id="b25c8-144">Para verificar o progresso, selecione Verifique o estado da **atualização**.</span><span class="sxs-lookup"><span data-stu-id="b25c8-144">To check on progress, select **Check upgrade status**.</span></span> 
1. <span data-ttu-id="b25c8-145">Uma vez que o seu plano esteja pronto, você pode precisar completar alguns passos adicionais de configuração no centro de administração.</span><span class="sxs-lookup"><span data-stu-id="b25c8-145">Once your plan is ready, you might need to complete some additional setup steps in the admin center.</span></span> <span data-ttu-id="b25c8-146">No painel de navegação, selecione **Casa** para completar quaisquer passos adicionais de configuração.</span><span class="sxs-lookup"><span data-stu-id="b25c8-146">In the navigation pane, select **Home** to complete any additional setup steps.</span></span>

> [!NOTE]
> <span data-ttu-id="b25c8-147">Receberá um reembolso prostrado pelas 365 licenças do Office que já não precisa.</span><span class="sxs-lookup"><span data-stu-id="b25c8-147">You'll receive a prorated refund for the Office 365 licenses that you no longer need.</span></span> <span data-ttu-id="b25c8-148">A sua conta bancária ou cartão de crédito será cobrada cerca de dois dias após a configuração do novo plano.</span><span class="sxs-lookup"><span data-stu-id="b25c8-148">Your bank account or credit card will be charged about two days after you set up the new plan.</span></span>
  
## <a name="protect-user-devices-and-files"></a><span data-ttu-id="b25c8-149">Proteja os dispositivos e ficheiros do utilizador</span><span class="sxs-lookup"><span data-stu-id="b25c8-149">Protect user devices and files</span></span>

<span data-ttu-id="b25c8-150">Agora que foram atribuídas licenças empresariais da Microsoft 365, completam as etapas para começar a proteger dispositivos e ficheiros.</span><span class="sxs-lookup"><span data-stu-id="b25c8-150">Now that Microsoft 365 Business licenses have been assigned, complete steps to start protecting devices and files.</span></span> <span data-ttu-id="b25c8-151">Você usará algumas novas opções incluídas no painel de navegação do centro de administração.</span><span class="sxs-lookup"><span data-stu-id="b25c8-151">You'll use some new options included in the admin center navigation pane.</span></span>
  
1. <span data-ttu-id="b25c8-152">No centro de administração, no painel de navegação, vá para as **Políticas**de **Dispositivos** \> .</span><span class="sxs-lookup"><span data-stu-id="b25c8-152">In the admin center, in the navigation pane, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="b25c8-153">Na página de políticas do **Dispositivo,** selecione **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="b25c8-153">On the **Device policies** page, select **Add**.</span></span>
    
3. <span data-ttu-id="b25c8-154">No painel de **política Add** dá à política um nome (por exemplo, Proteja os ficheiros de trabalho) e, em seguida, escolha um tipo **de Política** a partir da lista de drop-down.</span><span class="sxs-lookup"><span data-stu-id="b25c8-154">In the **Add policy** pane give the policy a name (for example, Protect work files), and then choose a **Policy type** from the drop-down list.</span></span> 
    
    <span data-ttu-id="b25c8-155">Pode configurar políticas de aplicação para proteger ficheiros em dispositivos Android e iPhone, bem como windows 10, e pode configurar políticas de configuração de dispositivos de configuração de dispositivos Windows 10 da empresa.</span><span class="sxs-lookup"><span data-stu-id="b25c8-155">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="b25c8-156">Consulte os seguintes links para mais detalhes:</span><span class="sxs-lookup"><span data-stu-id="b25c8-156">See the following links for details:</span></span>
    
  - [<span data-ttu-id="b25c8-157">Configurar as definições de proteção de aplicações para dispositivos Android ou iOS</span><span class="sxs-lookup"><span data-stu-id="b25c8-157">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="b25c8-158">Configurar as definições de proteção de aplicações para dispositivos Windows 10</span><span class="sxs-lookup"><span data-stu-id="b25c8-158">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="b25c8-159">Definir definições de proteção do dispositivo para PCs windows 10</span><span class="sxs-lookup"><span data-stu-id="b25c8-159">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
    
  
4. <span data-ttu-id="b25c8-160">Depois de configurar políticas, você e os seus colaboradores podem configurar dispositivos:</span><span class="sxs-lookup"><span data-stu-id="b25c8-160">After you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="b25c8-161">Se os dispositivos Windows ainda não estiverem a utilizar a atualização do Windows Pro Creator, terá de os atualizar para a Atualização dos [Criadores do Windows Pro](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="b25c8-161">If your Windows devices aren't already using the Windows Pro Creator update, you'll need to [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
    
  - <span data-ttu-id="b25c8-162">Consulte [a configuração de dispositivos Windows para utilizadores do Microsoft 365 Business](set-up-windows-devices.md) para obter medidas para dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="b25c8-162">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="b25c8-163">Consulte a [Configuração de dispositivos móveis para os utilizadores do Microsoft 365 Business](set-up-mobile-devices.md) para passos para telemóveis e iPhones Android.</span><span class="sxs-lookup"><span data-stu-id="b25c8-163">See [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 
