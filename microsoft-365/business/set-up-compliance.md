---
title: Aumentar a proteção contra ameaças para o Microsoft 365 Business Premium
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
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Configurar funcionalidades de conformidade para evitar a perda de dados e ajudar a manter as informações sensíveis dos seus clientes e dos seus clientes seguras.
ms.openlocfilehash: 9b900367c22ec5bb5c2719af63049045ecd5e466
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/27/2020
ms.locfileid: "44402700"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="377fd-103">Configurar funcionalidades de conformidade</span><span class="sxs-lookup"><span data-stu-id="377fd-103">Set up compliance features</span></span>

<span data-ttu-id="377fd-104">O Microsoft 365 Business Premium vem com funcionalidades para proteger os seus dados e dispositivos e ajudá-lo a manter as informações sensíveis dos seus clientes e dos seus clientes seguras.</span><span class="sxs-lookup"><span data-stu-id="377fd-104">Your Microsoft 365 Business Premium comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="377fd-105">Configurar as funcionalidades dLP</span><span class="sxs-lookup"><span data-stu-id="377fd-105">Set up DLP features</span></span>

<span data-ttu-id="377fd-106">Consulte [Criar uma política de DLP](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) a partir de um modelo para um exemplo sobre como criar uma política de proteção contra informações pessoalmente identificáveis (PII).</span><span class="sxs-lookup"><span data-stu-id="377fd-106">See [Create a DLP policy from a template](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="377fd-107">DLP vem com muitos modelos de política prontos a usar para muitos locais diferentes.</span><span class="sxs-lookup"><span data-stu-id="377fd-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="377fd-108">Por exemplo, Australia Financial Data, Canada Personal Information Act, Dados Financeiros dos EUA, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="377fd-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="377fd-109">Veja [o que os modelos de política do DLP incluem](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) para uma lista completa.</span><span class="sxs-lookup"><span data-stu-id="377fd-109">See [What the DLP policy templates include](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) for a full list.</span></span> <span data-ttu-id="377fd-110">Todos estes modelos podem ser ativados semelhantes ao exemplo do modelo PII.</span><span class="sxs-lookup"><span data-stu-id="377fd-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="377fd-111">Configurar a retenção de e-mails com o Arquivo Online de Troca</span><span class="sxs-lookup"><span data-stu-id="377fd-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="377fd-112">**As** funcionalidades de licença de arquivo online exchange ajudam a manter a conformidade e os padrões regulamentares preservando o conteúdo de e-mail para eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="377fd-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="377fd-113">Também ajuda a reduzir o seu risco se houver um processo judicial, e fornece uma maneira de recuperar dados após uma violação de segurança ou quando precisa de recuperar itens apagados.</span><span class="sxs-lookup"><span data-stu-id="377fd-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="377fd-114">Pode utilizar litígios para preservar todo o conteúdo do utilizador ou utilizar políticas de retenção para personalizar o que pretende preservar.</span><span class="sxs-lookup"><span data-stu-id="377fd-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="377fd-115">**Detenção de litígios:** Pode preservar todos os conteúdos da caixa de correio, incluindo itens eliminados, colocando toda a caixa de correio de um utilizador em espera de litígios.</span><span class="sxs-lookup"><span data-stu-id="377fd-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="377fd-116">Para colocar uma caixa de correio em espera de litígios, no centro de Administração:</span><span class="sxs-lookup"><span data-stu-id="377fd-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="377fd-117">Na navegação à esquerda, vá aos **Users** \> **utilizadores ativos.**</span><span class="sxs-lookup"><span data-stu-id="377fd-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="377fd-118">Selecione um utilizador cuja caixa de correio pretende colocar em espera de litígios.</span><span class="sxs-lookup"><span data-stu-id="377fd-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="377fd-119">No painel do utilizador, expandir **as definições de Correio**, e ao lado de mais **configurações,** escolha **propriedades de Edição Exchange**.</span><span class="sxs-lookup"><span data-stu-id="377fd-119">In the user pane, expand **Mail settings**, and next to **More settings**, choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="377fd-120">Na página da caixa de correio para o utilizador, escolha as funcionalidades da caixa de correio \*\* no v ' à esquerda e, em seguida, escolha o link **Enable** sob **a porção de Litígios**.</span><span class="sxs-lookup"><span data-stu-id="377fd-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="377fd-121">Na **litigation hold** caixa de diálogo, pode especificar a duração do processo no campo de duração do **processo.**</span><span class="sxs-lookup"><span data-stu-id="377fd-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="377fd-122">Deixe o campo vazio se quiser colocar um porão infinito.</span><span class="sxs-lookup"><span data-stu-id="377fd-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="377fd-123">Também pode adicionar notas e direcionar o proprietário da caixa de correio para um site que poderá ter de explicar mais sobre o processo.</span><span class="sxs-lookup"><span data-stu-id="377fd-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="377fd-124">\>**Salvar.**</span><span class="sxs-lookup"><span data-stu-id="377fd-124">\> **Save**.</span></span>
    
<span data-ttu-id="377fd-125">**Retenção:** Pode permitir que políticas de retenção personalizadas, por exemplo, preservem por um período de tempo específico ou apaguem conteúdos permanentemente no final do período de retenção.</span><span class="sxs-lookup"><span data-stu-id="377fd-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="377fd-126">Para saber mais, consulte [a visão geral das políticas de retenção.](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)</span><span class="sxs-lookup"><span data-stu-id="377fd-126">To learn more, see [Overview of retention policies](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="377fd-127">Configurar rótulos de sensibilidade</span><span class="sxs-lookup"><span data-stu-id="377fd-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="377fd-128">As etiquetas de sensibilidade vêm com o Plano 1 de Proteção de Informação Azure (AIP) e ajudam-no a classificar e a proteger opcionalmente os seus documentos e e-mails, aplicando etiquetas.</span><span class="sxs-lookup"><span data-stu-id="377fd-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="377fd-129">As etiquetas podem ser aplicadas automaticamente por administradores que definem regras e condições, manualmente pelos utilizadores, ou utilizando uma combinação em que os utilizadores recebem recomendações.</span><span class="sxs-lookup"><span data-stu-id="377fd-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="377fd-130">Para configurar etiquetas de sensibilidade, veja criar e gerir o vídeo das etiquetas de [sensibilidade.](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)</span><span class="sxs-lookup"><span data-stu-id="377fd-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="377fd-131">Instale manualmente o cliente de Proteção de Informação Do Azure</span><span class="sxs-lookup"><span data-stu-id="377fd-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="377fd-132">Para instalar manualmente o cliente AIP:</span><span class="sxs-lookup"><span data-stu-id="377fd-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="377fd-133">Baixe **AzinfoProtection_UL.exe** do centro de [descarregamento](https://www.microsoft.com/download/details.aspx?id=53018)da Microsoft .</span><span class="sxs-lookup"><span data-stu-id="377fd-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="377fd-134">Pode verificar se a instalação funcionou visualizando um documento Word e certificando-se de que a opção **Sensibilidade** está disponível no separador **Home.**</span><span class="sxs-lookup"><span data-stu-id="377fd-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="377fd-135">![A questão da proteção cai num documento word.](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="377fd-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="377fd-136">Para mais informações, consulte [Instalar o cliente.](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3)</span><span class="sxs-lookup"><span data-stu-id="377fd-136">For more information, see [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
