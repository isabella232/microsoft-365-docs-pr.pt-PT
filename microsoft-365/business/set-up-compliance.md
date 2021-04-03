---
title: Aumentar a proteção contra ameaças para o Microsoft 365 Business Premium
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
description: Crie funcionalidades de conformidade para evitar a perda de dados e ajude a manter as informações sensíveis dos seus e dos seus clientes seguras.
ms.openlocfilehash: c0accc37d3dcda9ba75813f01a98a3233c5a8369
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579960"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="79b98-103">Configurar funcionalidades de conformidade</span><span class="sxs-lookup"><span data-stu-id="79b98-103">Set up compliance features</span></span>

<span data-ttu-id="79b98-104">O Microsoft 365 Business Premium vem com funcionalidades para proteger os seus dados e dispositivos e ajudá-lo a manter as informações sensíveis dos seus clientes e dos seus clientes seguras.</span><span class="sxs-lookup"><span data-stu-id="79b98-104">Your Microsoft 365 Business Premium comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="79b98-105">Configurar funcionalidades DLP</span><span class="sxs-lookup"><span data-stu-id="79b98-105">Set up DLP features</span></span>

<span data-ttu-id="79b98-106">Consulte [Criar uma política DLP a partir de um modelo](../compliance/create-a-dlp-policy-from-a-template.md) para um exemplo sobre como configurar uma política para proteger contra a perda de dados pessoais.</span><span class="sxs-lookup"><span data-stu-id="79b98-106">See [Create a DLP policy from a template](../compliance/create-a-dlp-policy-from-a-template.md) for an example on how to set up a policy to protect against protect loss of personal data.</span></span> 
  
<span data-ttu-id="79b98-107">DLP vem com muitos modelos de política prontos a usar para muitos locais diferentes.</span><span class="sxs-lookup"><span data-stu-id="79b98-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="79b98-108">Por exemplo, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="79b98-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="79b98-109">Veja [o que os modelos de política do DLP incluem](../compliance/what-the-dlp-policy-templates-include.md) para uma lista completa.</span><span class="sxs-lookup"><span data-stu-id="79b98-109">See [What the DLP policy templates include](../compliance/what-the-dlp-policy-templates-include.md) for a full list.</span></span> <span data-ttu-id="79b98-110">Todos estes modelos podem ser ativados semelhantes ao exemplo do modelo PII.</span><span class="sxs-lookup"><span data-stu-id="79b98-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="79b98-111">Configurar retenção de e-mail com o Arquivo Online da Bolsa</span><span class="sxs-lookup"><span data-stu-id="79b98-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="79b98-112">As funcionalidades de licença **de arquivamento online de intercâmbio** ajudam a manter os padrões de conformidade e regulamentares, preservando o conteúdo de e-mail para eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="79b98-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="79b98-113">Também ajuda a reduzir o seu risco se houver um processo judicial, e fornece uma forma de recuperar dados após uma falha de segurança ou quando precisa de recuperar itens eliminados.</span><span class="sxs-lookup"><span data-stu-id="79b98-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="79b98-114">Pode utilizar o porão de litígios para preservar todo o conteúdo de um utilizador, ou usar políticas de retenção para personalizar o que pretende preservar.</span><span class="sxs-lookup"><span data-stu-id="79b98-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="79b98-115">**Detenção de litígios:** Pode preservar todos os conteúdos da caixa de correio, incluindo itens eliminados, colocando toda a caixa de correio de um utilizador em porão de litígio.</span><span class="sxs-lookup"><span data-stu-id="79b98-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="79b98-116">Para colocar uma caixa de correio em porão de litígio, no centro de administração:</span><span class="sxs-lookup"><span data-stu-id="79b98-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="79b98-117">No navegador esquerdo, vá aos  \> **utilizadores Utilizadores Ativos**.</span><span class="sxs-lookup"><span data-stu-id="79b98-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="79b98-118">Selecione um utilizador cuja caixa de correio pretende colocar em espera de litígio.</span><span class="sxs-lookup"><span data-stu-id="79b98-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="79b98-119">No painel de utilizador, expanda as **definições de Correio**, e ao lado **de mais definições,** escolha **propriedades de Edit Exchange**.</span><span class="sxs-lookup"><span data-stu-id="79b98-119">In the user pane, expand **Mail settings**, and next to **More settings**, choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="79b98-120">Na página da caixa de correio para o utilizador, escolha as funcionalidades da caixa de correio \*\* na navegação esquerda e, em seguida, escolha o link **Enable** no **porão de Contencioso**.</span><span class="sxs-lookup"><span data-stu-id="79b98-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="79b98-121">Na caixa de diálogo **de detenção de litígios,** pode especificar a duração da duração do litígio no campo de **duração do litígio.**</span><span class="sxs-lookup"><span data-stu-id="79b98-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="79b98-122">Deixe o campo vazio se quiser colocar um domínio infinito.</span><span class="sxs-lookup"><span data-stu-id="79b98-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="79b98-123">Também pode adicionar notas e dirigir o proprietário da caixa de correio para um site que poderá ter de explicar mais sobre o porão de litígios.</span><span class="sxs-lookup"><span data-stu-id="79b98-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="79b98-124">\>**Guardar.**</span><span class="sxs-lookup"><span data-stu-id="79b98-124">\> **Save**.</span></span>
    
<span data-ttu-id="79b98-125">**Retenção:** Pode ativar políticas de retenção personalizadas, por exemplo, para preservar por um determinado período de tempo ou eliminar o conteúdo permanentemente no final do período de retenção.</span><span class="sxs-lookup"><span data-stu-id="79b98-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="79b98-126">Para saber mais, consulte [a visão geral das políticas de retenção.](../compliance/retention.md)</span><span class="sxs-lookup"><span data-stu-id="79b98-126">To learn more, see [Overview of retention policies](../compliance/retention.md).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="79b98-127">Configurar rótulos de sensibilidade</span><span class="sxs-lookup"><span data-stu-id="79b98-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="79b98-128">As etiquetas de sensibilidade vêm com o Plano 1 de Proteção de Informação (AIP) do Azure, e ajudam-no a classificar e a proteger opcionalmente os seus documentos e e-mails, aplicando etiquetas.</span><span class="sxs-lookup"><span data-stu-id="79b98-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="79b98-129">As etiquetas podem ser aplicadas automaticamente por administradores que definem regras e condições, manualmente pelos utilizadores, ou através de uma combinação em que os utilizadores recebem recomendações.</span><span class="sxs-lookup"><span data-stu-id="79b98-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="79b98-130">Para configurar rótulos de sensibilidade, ver [criar e gerir vídeos de etiquetas de sensibilidade.](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)</span><span class="sxs-lookup"><span data-stu-id="79b98-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="79b98-131">Instale manualmente o cliente Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="79b98-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="79b98-132">Para instalar manualmente o cliente AIP:</span><span class="sxs-lookup"><span data-stu-id="79b98-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="79b98-133">Descarregue **AzinfoProtection_UL.exe** do [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="79b98-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="79b98-134">Pode verificar se a instalação funcionou visualizando um documento Word e certificando-se de que a opção **Sensibilidade** está disponível no **separador 'Casa'.**</span><span class="sxs-lookup"><span data-stu-id="79b98-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="79b98-135">![Aba de proteção num documento do Word.](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="79b98-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="79b98-136">Para mais informações, consulte [instalar o cliente.](/azure/information-protection/infoprotect-tutorial-step3)</span><span class="sxs-lookup"><span data-stu-id="79b98-136">For more information, see [Install the client](/azure/information-protection/infoprotect-tutorial-step3).</span></span>