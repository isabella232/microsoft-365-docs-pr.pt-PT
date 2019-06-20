---
title: Aumentar a protecção contra ameaças para a Microsoft 365 empresa
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
search.appverid:
- BCS160
- MET150
description: Configurar a protecção de ameaças avançado do Office 365 e proteger dados sensíveis.
ms.openlocfilehash: 53741a7726222bb32329a401953be72257df95cc
ms.sourcegitcommit: 7ac06563c6ff034358e8fd3f9298fc426187ade2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/31/2019
ms.locfileid: "35086384"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="70716-103">Configurar funcionalidades de conformidade</span><span class="sxs-lookup"><span data-stu-id="70716-103">Set up compliance features</span></span>

<span data-ttu-id="70716-104">A Microsoft 365 Business é fornecido com funcionalidades para proteger os dados e dispositivos e ajudar a proteger o seu e informações confidenciais dos clientes.</span><span class="sxs-lookup"><span data-stu-id="70716-104">Your Microsoft 365 Business comes with features to protect your data and devices, and help you keep yours and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="70716-105">Configurar funcionalidades do DLP</span><span class="sxs-lookup"><span data-stu-id="70716-105">Set up DLP features</span></span>

<span data-ttu-id="70716-106">Consulte [criar uma política DLP a partir de um modelo](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) para obter um exemplo sobre como configurar uma política para proteger informações de identificação pessoal (PII).</span><span class="sxs-lookup"><span data-stu-id="70716-106">See [Create a DLP policy from a template](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="70716-107">DLP é fornecido com modelos de política de prontos a utilizar muitos para muitos idiomas diferentes.</span><span class="sxs-lookup"><span data-stu-id="70716-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="70716-108">Por exemplo, dados financeiros da Austrália, Canadá lei de informações pessoais, dados financeiros dos e.u.a., etc. Para obter uma lista completa, consulte a [incluem modelos de política que do DLP](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) .</span><span class="sxs-lookup"><span data-stu-id="70716-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, etc. See [What the DLP policy templates include](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for a full list.</span></span> <span data-ttu-id="70716-109">Todos estes modelos podem ser activados semelhante ao exemplo de modelo do PII.</span><span class="sxs-lookup"><span data-stu-id="70716-109">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="70716-110">Configurar a retenção de correio electrónico com o arquivo Online do Exchange</span><span class="sxs-lookup"><span data-stu-id="70716-110">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="70716-111">Funcionalidades de licença **Online arquivo do Exchange** ajudam a manter a conformidade e normas reguladoras mantiver o correio electrónico conteúdo para detecção de dados electrónicos.</span><span class="sxs-lookup"><span data-stu-id="70716-111">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="70716-112">Também ajuda a reduzir os riscos em caso de uma acção judicial e fornece uma forma de recuperar os dados após uma falha de segurança, ou quando necessitar de recuperar itens eliminados.</span><span class="sxs-lookup"><span data-stu-id="70716-112">It also helps reduce your risk in the event of a lawsuit and provides a way to recover data after a security breach, or when you need to recover deleted items.</span></span> <span data-ttu-id="70716-113">Pode utilizar o litígio suspenso para manter todo o conteúdo de um utilizador, ou utilizar políticas de retenção para personalizar o que pretende preservar.</span><span class="sxs-lookup"><span data-stu-id="70716-113">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="70716-114">**Espera litígio:** Pode preservar todo o conteúdo da caixa de correio reter itens eliminados incluindo colocando a caixa de correio de todo um utilizador no litígio.</span><span class="sxs-lookup"><span data-stu-id="70716-114">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="70716-115">Para colocar uma caixa de correio em espera de litígio, no Centro de administração:</span><span class="sxs-lookup"><span data-stu-id="70716-115">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="70716-116">No nav esquerda, vá para **os utilizadores** \> **os utilizadores activos**.</span><span class="sxs-lookup"><span data-stu-id="70716-116">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="70716-117">Seleccione um utilizador cuja caixa de correio que pretende colocar no litígio mantenha e no painel do utilizador expanda **definições de correio** e junto de **definições mais** escolha **Exchange editar propriedades**.</span><span class="sxs-lookup"><span data-stu-id="70716-117">Select a user whose mailbox you want to place on litigation hold and in the user pane expand **Mail settings** and next to **More settings** choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="70716-118">Na página da caixa de correio do utilizador, seleccione \* \* funcionalidades de correio \* \* no nav esquerda e, em seguida, seleccione a hiperligação **Activar** em **litígio mantenha**.</span><span class="sxs-lookup"><span data-stu-id="70716-118">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="70716-119">Em **litígios mantenha** a caixa de diálogo pode especificar os litígios Mantenha duração no campo **litígio Mantenha duração** , deixe o campo vazio se pretende colocar uma espera infinita.</span><span class="sxs-lookup"><span data-stu-id="70716-119">In the **litigation hold** dialog box you can specify the litigation hold duration in the **Litigation hold duration** field, leave field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="70716-120">Também pode adicionar notas e direccionar o proprietário de caixa de correio para um Web site poderá ter de explicar mais informações sobre os litígios mantém \> **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="70716-120">You can also add notes and direct the mail box owner to a website you might have to explain more about the litigation hold \> **Save**.</span></span>
    
<span data-ttu-id="70716-121">**Retenção:** Pode activar políticas de retenção personalizado como, por exemplo, a preservar de um determinado período de tempo ou eliminar permanentemente o conteúdo no final do período de retenção.</span><span class="sxs-lookup"><span data-stu-id="70716-121">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="70716-122">Para obter mais informações, consulte [Descrição geral de políticas de retenção](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span><span class="sxs-lookup"><span data-stu-id="70716-122">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>

## <a name="set-up-azure-information-protection-features"></a><span data-ttu-id="70716-123">Configurar funcionalidades de protecção de informações de Azure</span><span class="sxs-lookup"><span data-stu-id="70716-123">Set up Azure Information Protection features</span></span>

<span data-ttu-id="70716-124">Protecção de informações Azure (AIP) ajuda a classificar e opcionalmente, proteger os seus documentos e mensagens de correio electrónico, através da aplicação de etiquetas.</span><span class="sxs-lookup"><span data-stu-id="70716-124">Azure Information Protection (AIP) helps you classify and optionally, protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="70716-125">Podem ser aplicados automaticamente rótulos por administradores que definem as regras e condições, manualmente por utilizadores ou utilizando uma combinação de onde os utilizadores tiverem recomendações.</span><span class="sxs-lookup"><span data-stu-id="70716-125">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="70716-126">No Outlook na web pode aplicar as restrições e os seguintes rótulos incorporados para mensagens de correio electrónico:</span><span class="sxs-lookup"><span data-stu-id="70716-126">In Outlook on the web you can apply the following built-in labels and restrictions to your emails:</span></span>
  
- <span data-ttu-id="70716-127">**Não reencaminhar**: os destinatários podem ler a mensagem, mas não é possível reencaminhar, imprimir ou copiar conteúdo</span><span class="sxs-lookup"><span data-stu-id="70716-127">**Do Not Forward**: Recipients can read the message, but they can't forward, print, or copy content</span></span>
    
- <span data-ttu-id="70716-128">**Encriptar**: toda a mensagem está encriptada.</span><span class="sxs-lookup"><span data-stu-id="70716-128">**Encrypt**: The entire message is encrypted.</span></span> <span data-ttu-id="70716-129">Os destinatários têm de confirmar sua identidade antes de aceder a conteúdo encriptado e não é possível remover a encriptação.</span><span class="sxs-lookup"><span data-stu-id="70716-129">Recipients must confirm their identity before accessing encrypted content and can't remove encryption.</span></span>
    
- <span data-ttu-id="70716-130">**Confidencial**: dá os empregados da organização todas as permissões para o conteúdo de correio electrónico e anexos, mas não para pessoas fora da organização.</span><span class="sxs-lookup"><span data-stu-id="70716-130">**Confidential**: Gives the employees in your organization full permissions to the email content and attachments, but not to people outside your organization.</span></span> <span data-ttu-id="70716-131">Proprietários de dados podem controlar e revogar o conteúdo em qualquer altura.</span><span class="sxs-lookup"><span data-stu-id="70716-131">Data owners can track and revoke content at any point.</span></span>
    
- <span data-ttu-id="70716-132">**Altamente confidenciais**: esta restrição pode ser aplicada aos dados altamente confidenciais, permitindo que os empregados ver, editar e responder, mas não reencaminhar, imprimir ou copiar os dados.</span><span class="sxs-lookup"><span data-stu-id="70716-132">**Highly Confidential**: This restriction can be applied to highly confidential data, allowing employees to view, edit, and reply, but not forward, print, or copy the data.</span></span> <span data-ttu-id="70716-133">Proprietários de dados podem controlar e revogar o conteúdo em qualquer altura.</span><span class="sxs-lookup"><span data-stu-id="70716-133">Data owners can track and revoke content at any point.</span></span>

### <a name="make-sure-azure-information-protection-is-activated"></a><span data-ttu-id="70716-134">Garantir a protecção de informações Azure está activada</span><span class="sxs-lookup"><span data-stu-id="70716-134">Make sure Azure Information Protection is activated</span></span>

<span data-ttu-id="70716-135">Para verificar que AIP está activado:</span><span class="sxs-lookup"><span data-stu-id="70716-135">To verify that AIP is activated :</span></span>

1. <span data-ttu-id="70716-136">Iniciar sessão no [Azure portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="70716-136">Sign into [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="70716-137">Seleccione **todos os serviços** e escreva *Azure a protecção de informações* na **Caixa de procura**.</span><span class="sxs-lookup"><span data-stu-id="70716-137">Select **All services** and type in *Azure Information Protection* in the **Search Box**.</span></span>

3. <span data-ttu-id="70716-138">Depois de visualizar os resultados, clique em Iniciar seguinte para **A protecção de informações Azure** para o tornar um favorito e fácil de localizar mais tarde.</span><span class="sxs-lookup"><span data-stu-id="70716-138">Once the results display, click the start next to **Azure Information Protection** to make it a favorite and easy to find later.</span></span>

4. <span data-ttu-id="70716-139">Seleccione **A protecção de informações Azure** \> **a activação de protecção** e certifique-se de que o estado estiver definido para activada.</span><span class="sxs-lookup"><span data-stu-id="70716-139">Select **Azure Information Protection** \> **Protection activation** and make sure the status is set to activated.</span></span> 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a><span data-ttu-id="70716-140">Visualizar as etiquetas de política e a predefinição de protecção de informações de Azure</span><span class="sxs-lookup"><span data-stu-id="70716-140">View the Azure Information Protection policy and default labels</span></span> 

<span data-ttu-id="70716-141">Para ver e modificar, os existentes etiquetas:</span><span class="sxs-lookup"><span data-stu-id="70716-141">To view, and modify, the existing labels:</span></span>

1. <span data-ttu-id="70716-142">No dashboard Azure a protecção de informações, seleccione as **classificações de** \> **etiquetas**.</span><span class="sxs-lookup"><span data-stu-id="70716-142">On the Azure Information Protection dashboard, select **Classifications** \> **Labels**.</span></span> <br/><span data-ttu-id="70716-143">![Etiquetas padrão para a protecção de informações Azure.](media/AIPLabels.png)</span><span class="sxs-lookup"><span data-stu-id="70716-143">![Standard labels for Azure Information Protection.](media/AIPLabels.png)</span></span>

2. <span data-ttu-id="70716-144">Pode escolher qualquer etiqueta para ver opções, pode alterar o nome a apresentar, cores, etc.</span><span class="sxs-lookup"><span data-stu-id="70716-144">You can choose any label to view options, you can change the display name, colors, etc.</span></span>
 
3. <span data-ttu-id="70716-145">Consulte [modificar e criar novos rótulos](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) se pretender criar os seus próprios.</span><span class="sxs-lookup"><span data-stu-id="70716-145">See  [Modify and create new labels](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) if you want to create your own.</span></span> 

### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="70716-146">Instalar manualmente o cliente de protecção de informações de Azure</span><span class="sxs-lookup"><span data-stu-id="70716-146">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="70716-147">Para instalar manualmente o cliente AIP:</span><span class="sxs-lookup"><span data-stu-id="70716-147">To manually install the AIP client:</span></span>

1. <span data-ttu-id="70716-148">Transferir o **AzInfoProtection.exe** do [Centro de transferências da Microsoft](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="70716-148">Download **AzInfoProtection.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="70716-149">Pode verificar que a instalação trabalhou visualizando um documento do Word e certificando-se de que a opção de **protecção** está disponível no separador **base** .</span><span class="sxs-lookup"><span data-stu-id="70716-149">You can verify that the installation worked by viewing a Word document and making sure that the **Protect** option is available on the **Home** tab.</span></span> <br/><span data-ttu-id="70716-150">![Separador protecção pendente num documento do Word.](media/Word_Protect.png)</span><span class="sxs-lookup"><span data-stu-id="70716-150">![Protection tab drop-down in a Word document.](media/Word_Protect.png)</span></span>

<span data-ttu-id="70716-151">Para mais informações, consulte [instalar o cliente](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="70716-151">For more information see, [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
