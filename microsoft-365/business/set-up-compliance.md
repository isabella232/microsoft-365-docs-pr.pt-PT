---
title: Aumentar a proteção contra ameaças Microsoft 365 Empresas Premium
f1.keywords:
- NOCSH
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
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Defina funcionalidades de conformidade para impedir a perda de dados e ajudar a manter as informações confidenciais dos seus clientes e dos seus clientes seguras.
ms.openlocfilehash: 945f8a283b90b89da2fbe67a073e0807b80d198f
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/06/2021
ms.locfileid: "52245090"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="6638b-103">Configurar funcionalidades de conformidade</span><span class="sxs-lookup"><span data-stu-id="6638b-103">Set up compliance features</span></span>

<span data-ttu-id="6638b-104">Os Microsoft 365 Empresas Premium são fornecidos com funcionalidades para proteger os seus dados e dispositivos e ajudá-lo a manter as informações confidenciais dos seus clientes e dos seus clientes seguras.</span><span class="sxs-lookup"><span data-stu-id="6638b-104">Your Microsoft 365 Business Premium comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="6638b-105">Configurar funcionalidades DLP</span><span class="sxs-lookup"><span data-stu-id="6638b-105">Set up DLP features</span></span>

<span data-ttu-id="6638b-106">Consulte [Criar uma política DLP a partir](../compliance/create-a-dlp-policy-from-a-template.md) de um modelo para saber como configurar uma política para proteger contra a perda de dados pessoais.</span><span class="sxs-lookup"><span data-stu-id="6638b-106">See [Create a DLP policy from a template](../compliance/create-a-dlp-policy-from-a-template.md) for an example on how to set up a policy to protect against protect loss of personal data.</span></span> 
  
<span data-ttu-id="6638b-107">O DLP vem com vários modelos de políticas prontos a utilizar para várias localidades diferentes.</span><span class="sxs-lookup"><span data-stu-id="6638b-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="6638b-108">Por exemplo, Dados Financeiros da Austrália, Lei de Informações Pessoais do Canadá, Dados Financeiros dos EUA, entre outros.</span><span class="sxs-lookup"><span data-stu-id="6638b-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="6638b-109">Consulte [O que os modelos de políticas DLP incluem](../compliance/what-the-dlp-policy-templates-include.md) para uma lista completa.</span><span class="sxs-lookup"><span data-stu-id="6638b-109">See [What the DLP policy templates include](../compliance/what-the-dlp-policy-templates-include.md) for a full list.</span></span> <span data-ttu-id="6638b-110">Todos estes modelos podem ser ativados de forma semelhante ao exemplo do modelo PII.</span><span class="sxs-lookup"><span data-stu-id="6638b-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="6638b-111">Configurar a retenção de e-mail com Arquivo de Exchange Online</span><span class="sxs-lookup"><span data-stu-id="6638b-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="6638b-112">**Arquivo de Exchange Online funcionalidades** de licença ajudam a manter as normas de conformidade e regulamentação ao preservar conteúdos de e-mail para Deteção de Dados Eletrónicos.</span><span class="sxs-lookup"><span data-stu-id="6638b-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="6638b-113">Também ajuda a reduzir o risco se houver uma ação judicial e fornece uma forma de recuperar dados após uma violação de segurança ou quando necessitar de recuperar itens eliminados.</span><span class="sxs-lookup"><span data-stu-id="6638b-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="6638b-114">Pode utilizar a retenção de litigações para preservar todos os conteúdos de um utilizador ou utilizar políticas de retenção para personalizar o que pretende preservar.</span><span class="sxs-lookup"><span data-stu-id="6638b-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="6638b-115">**Retenção de litigações:** Pode preservar todo o conteúdo da caixa de correio, incluindo itens eliminados, colocando toda a caixa de correio de um utilizador em espera de litígios.</span><span class="sxs-lookup"><span data-stu-id="6638b-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="6638b-116">Para colocar uma caixa de correio em espera de litigação, no Centro de administração:</span><span class="sxs-lookup"><span data-stu-id="6638b-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="6638b-117">No navegador esquerdo, aceda a **Utilizadores** \> **Ativos.**</span><span class="sxs-lookup"><span data-stu-id="6638b-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="6638b-118">Selecione um utilizador cuja caixa de correio pretende colocar em espera de litigação.</span><span class="sxs-lookup"><span data-stu-id="6638b-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="6638b-119">No painel de utilizador, **expanda** Definições de correio e, junto a Mais definições, selecionar **Editar Exchange propriedades**.</span><span class="sxs-lookup"><span data-stu-id="6638b-119">In the user pane, expand **Mail settings**, and next to **More settings**, choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="6638b-120">Na página da caixa de correio do utilizador, selecionar \*\* funcionalidades  da caixa de correio \*\* no navegador esquerdo e, em seguida, selecionar a ligação Ativar em Retenção **de litígios**.</span><span class="sxs-lookup"><span data-stu-id="6638b-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="6638b-121">Na caixa **de diálogo litigação,** pode especificar a duração da retenção de litigações no campo Duração da **litigação.**</span><span class="sxs-lookup"><span data-stu-id="6638b-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="6638b-122">Deixe o campo em branco se quiser colocar uma posição infinita.</span><span class="sxs-lookup"><span data-stu-id="6638b-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="6638b-123">Também pode adicionar notas e direcionar o proprietário da caixa de correio para um site poderá ter de explicar mais sobre a retenção de litígios.</span><span class="sxs-lookup"><span data-stu-id="6638b-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="6638b-124">\>**Guardar**.</span><span class="sxs-lookup"><span data-stu-id="6638b-124">\> **Save**.</span></span>
    
<span data-ttu-id="6638b-125">**Retenção:** Pode ativar políticas de retenção personalizadas, por exemplo, para preservar durante um período de tempo específico ou eliminar conteúdo permanentemente no final do período de retenção.</span><span class="sxs-lookup"><span data-stu-id="6638b-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="6638b-126">Para saber mais, consulte [o resumo das políticas de retenção.](../compliance/retention.md)</span><span class="sxs-lookup"><span data-stu-id="6638b-126">To learn more, see [Overview of retention policies](../compliance/retention.md).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="6638b-127">Configurar etiquetas de sensibilidade</span><span class="sxs-lookup"><span data-stu-id="6638b-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="6638b-128">As etiquetas de confidencialidade vêm com o Plano 1 do Azure Information Protection (AIP) e ajudam-no a classificar e a proteger opcionalmente os seus documentos e e-mails ao aplicar etiquetas.</span><span class="sxs-lookup"><span data-stu-id="6638b-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="6638b-129">As etiquetas podem ser aplicadas automaticamente por administradores que definam regras e condições, manualmente pelos utilizadores ou através de uma combinação em que os utilizadores recebem recomendações.</span><span class="sxs-lookup"><span data-stu-id="6638b-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="6638b-130">Para configurar etiquetas de Sensibilidade, veja o vídeo Criar e [gerir etiquetas de](../business-video/create-sensitivity-labels.md) sensibilidade.</span><span class="sxs-lookup"><span data-stu-id="6638b-130">To set up Sensitivity labels, view [create and manage sensitivity labels](../business-video/create-sensitivity-labels.md) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="6638b-131">Instalar manualmente o cliente do Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="6638b-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="6638b-132">Para instalar manualmente o cliente AIP:</span><span class="sxs-lookup"><span data-stu-id="6638b-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="6638b-133">**Transfira oAzinfoProtection_UL.exe** centro de [transferências da Microsoft.](https://www.microsoft.com/download/details.aspx?id=53018)</span><span class="sxs-lookup"><span data-stu-id="6638b-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="6638b-134">Pode verificar se a instalação funcionou ao ver um  documento do Word e ao certificar-se de que a opção Confidencialidade está disponível no **separador** Base.</span><span class="sxs-lookup"><span data-stu-id="6638b-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="6638b-135">![Separador Proteção num documento Word.](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="6638b-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="6638b-136">Para obter mais informações, consulte [Instalar o cliente.](/azure/information-protection/infoprotect-tutorial-step3)</span><span class="sxs-lookup"><span data-stu-id="6638b-136">For more information, see [Install the client](/azure/information-protection/infoprotect-tutorial-step3).</span></span>