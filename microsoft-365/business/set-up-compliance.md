---
title: Aumentar a proteção contra ameaças para o Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
description: Configure recursos de conformidade para evitar a perda de dados e rotular dados confidenciais.
ms.openlocfilehash: 5213c55f4a8ce0e223896f1b960847714d6d06cb
ms.sourcegitcommit: 70e920f76526f47fc849df615de4569e0ac2f4be
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/07/2019
ms.locfileid: "38031421"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="10bb0-103">Configurar recursos de conformidade</span><span class="sxs-lookup"><span data-stu-id="10bb0-103">Set up compliance features</span></span>

<span data-ttu-id="10bb0-104">Seu Microsoft 365 Business vem com recursos para proteger seus dados e dispositivos e ajudá-lo a manter as informações confidenciais dos seus clientes seguras.</span><span class="sxs-lookup"><span data-stu-id="10bb0-104">Your Microsoft 365 Business comes with features to protect your data and devices, and help you keep yours and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="10bb0-105">Configurar recursos de DLP</span><span class="sxs-lookup"><span data-stu-id="10bb0-105">Set up DLP features</span></span>

<span data-ttu-id="10bb0-106">Veja [criar uma política de DLP a partir de um modelo](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) para um exemplo sobre como criar uma política para proteger contra informações de identificação pessoal (PII).</span><span class="sxs-lookup"><span data-stu-id="10bb0-106">See [Create a DLP policy from a template](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="10bb0-107">DLP vem com muitos modelos de política pronto-a-uso para muitos locais diferentes.</span><span class="sxs-lookup"><span data-stu-id="10bb0-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="10bb0-108">Por exemplo, dados financeiros da Austrália, Canada Personal Information Act, Dados Financeiros dos EUA, etc. Veja [o que os modelos](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) de política do DLP incluem para uma lista completa.</span><span class="sxs-lookup"><span data-stu-id="10bb0-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, etc. See [What the DLP policy templates include](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for a full list.</span></span> <span data-ttu-id="10bb0-109">Todos esses modelos podem ser habilitados semelhante sagaz.</span><span class="sxs-lookup"><span data-stu-id="10bb0-109">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="10bb0-110">Configure retenção de e-mail com arquivamento on-line de intercâmbio</span><span class="sxs-lookup"><span data-stu-id="10bb0-110">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="10bb0-111">Os recursos da licença **de arquivamento on-line** de intercâmbio ajudam a manter os padrões regulatórios e de conformidade, preservando o conteúdo de e-mail para o eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="10bb0-111">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="10bb0-112">Ele também ajuda a reduzir o risco em caso de uma ação judicial e fornece uma maneira de recuperar dados após uma violação de segurança, ou quando você precisa recuperar itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="10bb0-112">It also helps reduce your risk in the event of a lawsuit and provides a way to recover data after a security breach, or when you need to recover deleted items.</span></span> <span data-ttu-id="10bb0-113">Você pode usar o litígio para preservar todo o conteúdo de um usuário ou usar políticas de retenção para personalizar o que deseja preservar.</span><span class="sxs-lookup"><span data-stu-id="10bb0-113">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="10bb0-114">**Contenção:** Você pode preservar todo o conteúdo da caixa de correio, incluindo itens excluídos, colocando toda a caixa de correio de um usuário no porão de litígio.</span><span class="sxs-lookup"><span data-stu-id="10bb0-114">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="10bb0-115">Para colocar uma caixa de correio em espera contencioso, no centro de administração:</span><span class="sxs-lookup"><span data-stu-id="10bb0-115">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="10bb0-116">No nav esquerdo, vá para **usuários** \> **ativos.**</span><span class="sxs-lookup"><span data-stu-id="10bb0-116">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="10bb0-117">Selecione um usuário cuja caixa de correio que você deseja colocar em espera de litígio e no painel do usuário expanda **as configurações** do Mail e, ao lado de **mais configurações,** escolha **as propriedades da Edit Exchange.**</span><span class="sxs-lookup"><span data-stu-id="10bb0-117">Select a user whose mailbox you want to place on litigation hold and in the user pane expand **Mail settings** and next to **More settings** choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="10bb0-118">Na página da caixa de correio para o usuário, escolha os recursos de caixa de correio \*\* \*\* na navegação esquerda e, em seguida, escolha o link **Habilitar** a **retenção de Litígio.**</span><span class="sxs-lookup"><span data-stu-id="10bb0-118">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="10bb0-119">No **litígio mantenha** a caixa de diálogo, você pode especificar a duração do litígio no campo de duração de **retenção de litígios,** deixar o campo vazio se você quiser colocar um porão infinito.</span><span class="sxs-lookup"><span data-stu-id="10bb0-119">In the **litigation hold** dialog box you can specify the litigation hold duration in the **Litigation hold duration** field, leave field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="10bb0-120">Você também pode adicionar notas e direcionar o proprietário da caixa de \> correio para um site que você pode ter que explicar mais sobre o litígio hold **Save**.</span><span class="sxs-lookup"><span data-stu-id="10bb0-120">You can also add notes and direct the mail box owner to a website you might have to explain more about the litigation hold \> **Save**.</span></span>
    
<span data-ttu-id="10bb0-121">**Retenção:** Você pode habilitar políticas de retenção personalizadas, por exemplo, preservar por um período de tempo específico ou excluir conteúdo permanentemente no final do período de retenção.</span><span class="sxs-lookup"><span data-stu-id="10bb0-121">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="10bb0-122">Para saber mais, veja [a visão geral das políticas de retenção.](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423)</span><span class="sxs-lookup"><span data-stu-id="10bb0-122">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="10bb0-123">Criar rótulos de sensibilidade</span><span class="sxs-lookup"><span data-stu-id="10bb0-123">Set up Sensitivity labels</span></span>

<span data-ttu-id="10bb0-124">Os rótulos de sensibilidade vêm com o Plano 1 de Proteção de Informações Azure (AIP) e ajudam você a classificar e, opcionalmente, proteger seus documentos e e-mails, aplicando rótulos.</span><span class="sxs-lookup"><span data-stu-id="10bb0-124">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify and optionally, protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="10bb0-125">Os rótulos podem ser aplicados automaticamente por administradores que definem regras e condições, manualmente pelos usuários ou usando uma combinação em que os usuários recebem recomendações.</span><span class="sxs-lookup"><span data-stu-id="10bb0-125">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="10bb0-126">Para configurar rótulos de sensibilidade, veja [criar e gerenciar vídeos](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) de rótulos de sensibilidade.</span><span class="sxs-lookup"><span data-stu-id="10bb0-126">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="10bb0-127">Instale o cliente de Proteção de Informações do Azure manualmente</span><span class="sxs-lookup"><span data-stu-id="10bb0-127">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="10bb0-128">Para instalar manualmente o cliente AIP:</span><span class="sxs-lookup"><span data-stu-id="10bb0-128">To manually install the AIP client:</span></span>

1. <span data-ttu-id="10bb0-129">Baixe **AzinfoProtection_UL.exe** do centro de download da [Microsoft](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="10bb0-129">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="10bb0-130">Você pode verificar se a instalação funcionou visualizando um documento do Word e certificando-se de que a opção **de sensibilidade** está disponível na guia **Home.**</span><span class="sxs-lookup"><span data-stu-id="10bb0-130">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="10bb0-131">![Guia de proteção drop-down em um documento do Word.](media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="10bb0-131">![Protection tab drop-down in a Word document.](media/word-sensitivity.png)</span></span>

<span data-ttu-id="10bb0-132">Para mais informações ver, [instale o cliente.](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3)</span><span class="sxs-lookup"><span data-stu-id="10bb0-132">For more information see, [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
