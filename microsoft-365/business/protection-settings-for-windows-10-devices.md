---
title: Configurar as definições de proteção de aplicações para dispositivos Windows 10
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- Win10AppPolicy
- O365E_Win10AppPolicy
- BCS365_Win10AppPolicy
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Saiba como criar uma política de gestão de aplicações e proteja ficheiros de trabalho nos dispositivos pessoais do Windows 10 dos seus utilizadores.
ms.openlocfilehash: df10470c6bd7aad2f35700a267c4d24d949f569c
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/01/2020
ms.locfileid: "44470873"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="75b59-103">Configurar as definições de proteção de aplicações para dispositivos Windows 10</span><span class="sxs-lookup"><span data-stu-id="75b59-103">Set application protection settings for Windows 10 devices</span></span>

<span data-ttu-id="75b59-104">Este artigo aplica-se ao Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="75b59-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="75b59-105">Criar uma política de gestão de aplicações para Windows 10</span><span class="sxs-lookup"><span data-stu-id="75b59-105">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="75b59-106">Se os seus utilizadores tiverem dispositivos Windows 10 pessoais, nos quais realizam tarefas profissionais, também pode proteger os seus dados nesses dispositivos.</span><span class="sxs-lookup"><span data-stu-id="75b59-106">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="75b59-107">Vá ao centro de administração em <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="75b59-107">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="75b59-108">No navegador esquerdo, escolha **Políticas de Dispositivos** \> **Policies** \> **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="75b59-108">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>

3. <span data-ttu-id="75b59-109">No painel **Adicionar política**, introduza um nome exclusivo para esta política.</span><span class="sxs-lookup"><span data-stu-id="75b59-109">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="75b59-110">Em **Tipo de política**, selecione **Gestão de Aplicações para Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="75b59-110">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
    
5. <span data-ttu-id="75b59-111">Sob **o tipo dispositivo**, escolha **pessoal** ou **empresa própria.**</span><span class="sxs-lookup"><span data-stu-id="75b59-111">Under **Device type**, choose either **Personal** or **Company Owned**.</span></span>
    
6. <span data-ttu-id="75b59-112">A opção **Encriptar ficheiros de trabalho** é ativada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="75b59-112">The **Encrypt work files** is turned on automatically.</span></span> 
    
7. <span data-ttu-id="75b59-113">Defina **Impedir que os utilizadores copiem os dados da empresa para ficheiros pessoais e obrigá-los a guardar os ficheiros de trabalho no OneDrive para Empresas** como **Ativado** se não pretender que os utilizadores guardem ficheiros de trabalho nos respetivos PCs.</span><span class="sxs-lookup"><span data-stu-id="75b59-113">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
    
9. <span data-ttu-id="75b59-114">Expandir **Recuperar dados em dispositivos Windows**.</span><span class="sxs-lookup"><span data-stu-id="75b59-114">Expand **Recover data on Windows devices**.</span></span> <span data-ttu-id="75b59-115">Recomendamos que **o**ligue.</span><span class="sxs-lookup"><span data-stu-id="75b59-115">We recommend that you turn it **On**.</span></span>
    
    <span data-ttu-id="75b59-116">Antes de poder aceder à localização do certificado de Agente de Recuperação de Dados, tem de criar um.</span><span class="sxs-lookup"><span data-stu-id="75b59-116">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one.</span></span> <span data-ttu-id="75b59-117">Para obter instruções, consulte [Criar e verificar um certificado de Agente de Recuperação de Dados (EFS) do Sistema de Recolha de Dados encriptante (EFS).](https://go.microsoft.com/fwlink/p/?linkid=853700)</span><span class="sxs-lookup"><span data-stu-id="75b59-117">For instructions, see [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](https://go.microsoft.com/fwlink/p/?linkid=853700).</span></span>
    
    <span data-ttu-id="75b59-118">Por predefinição, os ficheiros de trabalho são encriptados com uma chave secreta que é armazenada no dispositivo e é associada ao perfil do utilizador.</span><span class="sxs-lookup"><span data-stu-id="75b59-118">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile.</span></span> <span data-ttu-id="75b59-119">Apenas o utilizador pode abrir e desencriptar o ficheiro.</span><span class="sxs-lookup"><span data-stu-id="75b59-119">Only the user can open and decrypt the file.</span></span> <span data-ttu-id="75b59-120">No entanto, se um dispositivo for perdido ou um utilizador for removido, um ficheiro pode ficar bloqueado num estado encriptado.</span><span class="sxs-lookup"><span data-stu-id="75b59-120">However, if a device is lost or a user is removed, a file can be stuck in an encrypted state.</span></span> <span data-ttu-id="75b59-121">Um administrador pode usar o certificado de Agente de Recuperação de Dados (DRA) para desencriptar o ficheiro.</span><span class="sxs-lookup"><span data-stu-id="75b59-121">An admin can use the Data Recovery Agent (DRA) certificate to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="75b59-123">**Expanda-se Proteger localizações adicionais de rede e nuvem** se pretender adicionar domínios adicionais ou localizações online do SharePoint para garantir que os ficheiros em todas as aplicações listadas estão protegidos.</span><span class="sxs-lookup"><span data-stu-id="75b59-123">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps are protected.</span></span> <span data-ttu-id="75b59-124">Se precisar de introduzir mais do que um item em cada campo, utilize ponto e vírgula (;) entre os itens.</span><span class="sxs-lookup"><span data-stu-id="75b59-124">If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span>
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="75b59-p105">Em seguida, decida **Quem irá ver estas definições?** Se não quiser utilizar o grupo de segurança predefinido, **Todos os Utilizadores**, selecione **Alterar**, selecione os grupos de segurança que irão receber estas definições \> **Selecionar**.</span><span class="sxs-lookup"><span data-stu-id="75b59-p105">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
12. <span data-ttu-id="75b59-128">Por fim, selecione **Adicionar** para guardar a política e atribua-a a todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="75b59-128">Finally, choose **Add** to save the policy, and assign it to devices.</span></span> 
