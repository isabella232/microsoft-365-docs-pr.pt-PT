---
title: Upgrade para Microsoft 365 Business Premium a partir do Microsoft 365 Business Standard
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Saiba a diferença entre o Microsoft 365 Business Standard e o Microsoft 365 Business Premium e como pode fazer upgrade para o Microsoft 365 Business Premium.
ms.openlocfilehash: ef3d929164f83d4e48157065eb1ae1d2a1a9452e
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912928"
---
# <a name="upgrade-to-microsoft-365-business-premium-from-microsoft-365-business-standard"></a><span data-ttu-id="ee685-103">Upgrade para Microsoft 365 Business Premium a partir do Microsoft 365 Business Standard</span><span class="sxs-lookup"><span data-stu-id="ee685-103">Upgrade to Microsoft 365 Business Premium from Microsoft 365 Business Standard</span></span>

<span data-ttu-id="ee685-104">Se tiver um [Microsoft 365 para subscrição de negócios](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2), por exemplo, Microsoft 365 Business Standard, pode facilmente fazer upgrade para o Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="ee685-104">If you have a [Microsoft 365 for business subscription](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2), for example, Microsoft 365 Business Standard, you can easily upgrade to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="ee685-105">Upgrade para Microsoft 365 Business Premium se quiser adicionar:</span><span class="sxs-lookup"><span data-stu-id="ee685-105">Upgrade to Microsoft 365 Business Premium if you want to add:</span></span>

- <span data-ttu-id="ee685-106">Windows 10 Pro (para PCs com o Windows 8 ou mais tarde)</span><span class="sxs-lookup"><span data-stu-id="ee685-106">Windows 10 Pro (to PCs running Windows 8 or later)</span></span>

- <span data-ttu-id="ee685-107">Controlos simples que gerem dados empresariais em dispositivos</span><span class="sxs-lookup"><span data-stu-id="ee685-107">Simple controls that manage business data on devices</span></span>

- <span data-ttu-id="ee685-108">Capacidades avançadas de segurança.</span><span class="sxs-lookup"><span data-stu-id="ee685-108">Advanced security capabilities.</span></span>
<span data-ttu-id="ee685-109">Saiba mais sobre o Microsoft 365 Business Premium em [Microsoft.com](https://www.microsoft.com/microsoft-365/business)</span><span class="sxs-lookup"><span data-stu-id="ee685-109">Find out more about Microsoft 365 Business Premium at [Microsoft.com](https://www.microsoft.com/microsoft-365/business)</span></span>

## <a name="whats-the-difference-between-microsoft-365-business-standard-and-microsoft-365-business-premium"></a><span data-ttu-id="ee685-110">Qual é a diferença entre o Microsoft 365 Business Standard e o Microsoft 365 Business Premium?</span><span class="sxs-lookup"><span data-stu-id="ee685-110">What's the difference between Microsoft 365 Business Standard and Microsoft 365 Business Premium?</span></span>

<span data-ttu-id="ee685-111">Adicionámos uma comparação lado a lado destes dois planos à Descrição do [Serviço Premium de Negócios Microsoft 365.](/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description)</span><span class="sxs-lookup"><span data-stu-id="ee685-111">We've added a side-by-side comparison of these two plans to the [Microsoft 365 Business Premium Service Description](/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description).</span></span> 

## <a name="before-you-get-started"></a><span data-ttu-id="ee685-112">Antes de começar.</span><span class="sxs-lookup"><span data-stu-id="ee685-112">Before you get started</span></span>

- <span data-ttu-id="ee685-113">**Quando devo escolher fazer upgrade?**</span><span class="sxs-lookup"><span data-stu-id="ee685-113">**When should I choose to upgrade?**</span></span> <span data-ttu-id="ee685-114">A atualização é a escolha certa quando pretende atualizar **todos os utilizadores** designados para um único plano.</span><span class="sxs-lookup"><span data-stu-id="ee685-114">Upgrade is the right choice when you want to upgrade **all users** assigned to a single plan.</span></span> <span data-ttu-id="ee685-115">Ao escolher o upgrade, todos os utilizadores do plano são mudados para outro plano ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="ee685-115">When you choose upgrade, all plan users get switched to another plan at the same time.</span></span> <span data-ttu-id="ee685-116">Se não quiser atualizar todos os que estão designados para um único plano, compre licenças para o novo plano (neste caso, o Microsoft 365 Business Premium) e [atribua essas licenças individualmente](../admin/manage/assign-licenses-to-users.md) a cada utilizador que pretende atualizar.</span><span class="sxs-lookup"><span data-stu-id="ee685-116">If you don't want to upgrade everyone assigned to a single plan, buy licenses for the new plan (in this case Microsoft 365 Business Premium), and [assign those licenses individually](../admin/manage/assign-licenses-to-users.md) to each user that you want to upgrade.</span></span>

- <span data-ttu-id="ee685-117">**Alguns addons podem impedir a atualização** Se tentar iniciar uma atualização e tiver um addon que o impeça de continuar, pode remover primeiro o addon e, em seguida, adicioná-lo mais tarde, se ainda precisar.</span><span class="sxs-lookup"><span data-stu-id="ee685-117">**Some add-ons might prevent the upgrade** If you try to start an upgrade and you have an add-on that prevents you from continuing, you can remove the add-on first, and then add it back later if you still need it.</span></span>

- <span data-ttu-id="ee685-118">**Se você pré-pago o seu plano** Não há um caminho simples de atualização para planos pré-pagos.</span><span class="sxs-lookup"><span data-stu-id="ee685-118">**If you prepaid your plan** There isn't a straightforward upgrade path for prepaid plans.</span></span> <span data-ttu-id="ee685-119">Saberá se tem um plano pré-pago porque estabeleceu o seu plano usando uma identificação de produto que pode ter comprado numa loja.</span><span class="sxs-lookup"><span data-stu-id="ee685-119">You'll know if you have a prepaid plan because you set up your plan using a product ID that you might have purchased in a store.</span></span> <span data-ttu-id="ee685-120">Contacte um parceiro, vá à Microsoft Store ou aguarde até que o seu plano pré-pago expire para mudar para um novo plano.</span><span class="sxs-lookup"><span data-stu-id="ee685-120">Contact a partner, go to the Microsoft Store, or wait until your prepaid plan expires to switch to a new plan.</span></span>

## <a name="upgrade-to-microsoft-365-business-premium"></a><span data-ttu-id="ee685-121">Upgrade para Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="ee685-121">Upgrade to Microsoft 365 Business Premium</span></span>

1. <span data-ttu-id="ee685-122">Inscreva-se no centro de administração em <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="ee685-122">Sign into the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="ee685-123">Vá ao painel de navegação e selecione **Faturar** \> **os seus produtos.**</span><span class="sxs-lookup"><span data-stu-id="ee685-123">Go to the navigation pane and select **Billing** \> **Your products**.</span></span> <span data-ttu-id="ee685-124">Encontre a sua subscrição atual e selecione-a para ver os detalhes.</span><span class="sxs-lookup"><span data-stu-id="ee685-124">Find your current subscription and select it to view the details.</span></span>

3. <span data-ttu-id="ee685-125">Na página seguinte, selecione **Upgrade**.</span><span class="sxs-lookup"><span data-stu-id="ee685-125">On the next page, select **Upgrade**.</span></span>

  > [!NOTE]
  > <span data-ttu-id="ee685-126">Se vir uma mensagem que diga que **atualizar a sua subscrição não é suportado com licenças baseadas em grupo no Azure Ative Directory,** pode ignorar com segurança esta mensagem, a menos que tenha uma organização muito grande.</span><span class="sxs-lookup"><span data-stu-id="ee685-126">If you see a message that says **Upgrading your subscription is not supported with group-based licensing in Azure Active Directory**, you can safely ignore this unless you have a very large organization.</span></span> <span data-ttu-id="ee685-127">As organizações que escolheram esta opção estarão cientes de que estão a usar licenças baseadas em grupo.</span><span class="sxs-lookup"><span data-stu-id="ee685-127">Organizations who have selected this option will be aware that they're using group-based licensing.</span></span>

4. <span data-ttu-id="ee685-128">Em seguida, pode ver uma lista de planos para os que pode atualizar.</span><span class="sxs-lookup"><span data-stu-id="ee685-128">Next, you can view a list of plans that you can upgrade to.</span></span> <span data-ttu-id="ee685-129">Neste caso, encontre o plano Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="ee685-129">In this case, find the Microsoft 365 Business Premium plan.</span></span> <span data-ttu-id="ee685-130">Pode descer se quiser ver todas as aplicações e serviços incluídos neste plano.</span><span class="sxs-lookup"><span data-stu-id="ee685-130">You can scroll down if you want to see all the apps and services that are included with this plan.</span></span> <span data-ttu-id="ee685-131">De acordo com **o Microsoft 365 Business Premium,** selecione **Upgrade** para adicionar Microsoft 365 Business Premium ao seu carrinho.</span><span class="sxs-lookup"><span data-stu-id="ee685-131">Under **Microsoft 365 Business Premium**, select **Upgrade** to add Microsoft 365 Business Premium to your cart.</span></span>

5. <span data-ttu-id="ee685-132">No carrinho:</span><span class="sxs-lookup"><span data-stu-id="ee685-132">In the cart:</span></span>

    1. <span data-ttu-id="ee685-133">Iremos automaticamente incluir licenças para todos os seus utilizadores atuais.</span><span class="sxs-lookup"><span data-stu-id="ee685-133">We'll automatically include licenses for all your current users.</span></span> <span data-ttu-id="ee685-134">Se precisar de mais ou menos licenças, tem de [comprar e atribuir essas licenças individualmente.](../admin/manage/assign-licenses-to-users.md)</span><span class="sxs-lookup"><span data-stu-id="ee685-134">If you need more or fewer licenses, you need to [buy and assign those licenses individually](../admin/manage/assign-licenses-to-users.md).</span></span>  
    2. <span data-ttu-id="ee685-135">Pode ajustar como gostaria de pagar: mensalmente ou anualmente.</span><span class="sxs-lookup"><span data-stu-id="ee685-135">You can adjust how you'd like to pay: monthly or yearly.</span></span> <span data-ttu-id="ee685-136">Selecione o menu suspenso para fazer a sua escolha.</span><span class="sxs-lookup"><span data-stu-id="ee685-136">Select the drop-down menu to make your choice.</span></span>

6. <span data-ttu-id="ee685-137">Selecione **Ir ao Checkout** onde verá um resumo da sua compra, incluindo o método de pagamento desta conta.</span><span class="sxs-lookup"><span data-stu-id="ee685-137">Select **Go to Checkout** where you'll see a summary of your purchase, including the payment method for this account.</span></span> <span data-ttu-id="ee685-138">Também pode adicionar um código promocional aqui se tiver um.</span><span class="sxs-lookup"><span data-stu-id="ee685-138">You can also add a promo code here if you have one.</span></span>

7. <span data-ttu-id="ee685-139">Selecione **Fazer o pedido** para concluir a sua compra.</span><span class="sxs-lookup"><span data-stu-id="ee685-139">Select **Place order** to complete your purchase.</span></span>\
<span data-ttu-id="ee685-140">A Microsoft leva alguns minutos para definir os seus novos planos de serviço.</span><span class="sxs-lookup"><span data-stu-id="ee685-140">It takes Microsoft a few minutes to set up your new service plans.</span></span> <span data-ttu-id="ee685-141">Para verificar o progresso, **selecione Verifique o estado da atualização**.</span><span class="sxs-lookup"><span data-stu-id="ee685-141">To check on progress, select **Check upgrade status**.</span></span>

8. <span data-ttu-id="ee685-142">Quando o seu plano estiver pronto, poderá necessitar de completar alguns passos adicionais de configuração no centro de administração.</span><span class="sxs-lookup"><span data-stu-id="ee685-142">When your plan is ready, you might need to complete some additional setup steps in the admin center.</span></span> <span data-ttu-id="ee685-143">No painel de navegação, selecione **Home** para completar quaisquer etapas de configuração adicionais.</span><span class="sxs-lookup"><span data-stu-id="ee685-143">In the navigation pane, select **Home** to complete any additional setup steps.</span></span>

> [!NOTE]
> <span data-ttu-id="ee685-144">Receberá um reembolso prostimado para as licenças Microsoft 365 de que já não precisa.</span><span class="sxs-lookup"><span data-stu-id="ee685-144">You'll receive a prorated refund for the Microsoft 365 licenses that you no longer need.</span></span> <span data-ttu-id="ee685-145">A sua conta bancária ou cartão de crédito será cobrado cerca de dois dias após a sua configuração do novo plano.</span><span class="sxs-lookup"><span data-stu-id="ee685-145">Your bank account or credit card will be charged about two days after you set up the new plan.</span></span>
  
## <a name="protect-user-devices-and-files"></a><span data-ttu-id="ee685-146">Proteger dispositivos e ficheiros do utilizador</span><span class="sxs-lookup"><span data-stu-id="ee685-146">Protect user devices and files</span></span>

<span data-ttu-id="ee685-147">Agora que foram atribuídas licenças Microsoft 365 Business Premium, são dados passos completos para começar a proteger dispositivos e ficheiros.</span><span class="sxs-lookup"><span data-stu-id="ee685-147">Now that Microsoft 365 Business Premium licenses have been assigned, complete steps to start protecting devices and files.</span></span> <span data-ttu-id="ee685-148">Você usará algumas novas opções incluídas no painel de navegação do centro de administração.</span><span class="sxs-lookup"><span data-stu-id="ee685-148">You'll use some new options included in the admin center navigation pane.</span></span>
  
1. <span data-ttu-id="ee685-149">No centro de administração, no painel de navegação, vá às Políticas **de Dispositivos.** \> </span><span class="sxs-lookup"><span data-stu-id="ee685-149">In the admin center, in the navigation pane, go to **Devices** \> **Policies**.</span></span>

2. <span data-ttu-id="ee685-150">Na página de políticas do **Dispositivo,** selecione **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="ee685-150">On the **Device policies** page, select **Add**.</span></span>

3. <span data-ttu-id="ee685-151">No painel **de política Add** dê à política um nome (por exemplo, proteja os ficheiros de trabalho) e, em seguida, escolha um tipo de **Política** da lista de drop-down.</span><span class="sxs-lookup"><span data-stu-id="ee685-151">In the **Add policy** pane give the policy a name (for example, Protect work files), and then choose a **Policy type** from the drop-down list.</span></span>

    <span data-ttu-id="ee685-152">Pode configurar políticas de aplicações para proteger ficheiros em dispositivos Android e iPhone, bem como windows 10, e pode configurar políticas de configuração de dispositivos para dispositivos do Windows 10 da empresa.</span><span class="sxs-lookup"><span data-stu-id="ee685-152">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="ee685-153">Consulte os seguintes links para mais detalhes:</span><span class="sxs-lookup"><span data-stu-id="ee685-153">See the following links for details:</span></span>

    - [<span data-ttu-id="ee685-154">Configurar as definições de proteção de aplicações para dispositivos Android ou iOS</span><span class="sxs-lookup"><span data-stu-id="ee685-154">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)

    - [<span data-ttu-id="ee685-155">Configurar as definições de proteção de aplicações para dispositivos Windows 10</span><span class="sxs-lookup"><span data-stu-id="ee685-155">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)

    - [<span data-ttu-id="ee685-156">Definir definições de proteção do dispositivo para PCs do Windows 10</span><span class="sxs-lookup"><span data-stu-id="ee685-156">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)

4. <span data-ttu-id="ee685-157">Depois de definir políticas, você e os seus colaboradores podem configurar dispositivos:</span><span class="sxs-lookup"><span data-stu-id="ee685-157">After you set up policies, you and your employees can set up devices:</span></span>

    - <span data-ttu-id="ee685-158">Se os seus dispositivos Windows ainda não estiverem a utilizar a atualização do Windows Pro Creator, terá de [os atualizar para a Atualização de Criadores do Windows Pro](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="ee685-158">If your Windows devices aren't already using the Windows Pro Creator update, you'll need to [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

    - <span data-ttu-id="ee685-159">Consulte [configurar dispositivos Windows para utilizadores Do Microsoft 365 Business Premium](set-up-windows-devices.md) para etapas para dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="ee685-159">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span>

    - <span data-ttu-id="ee685-160">Consulte [configurar dispositivos móveis para utilizadores Do Microsoft 365 Business Premium](set-up-mobile-devices.md) para passos para telemóveis e iPhones Android.</span><span class="sxs-lookup"><span data-stu-id="ee685-160">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span>