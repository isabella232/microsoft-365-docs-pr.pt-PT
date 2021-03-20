---
title: Editar ou definir definições de proteção de aplicações para dispositivos Windows 10
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
description: Saiba como criar ou editar políticas de gestão de aplicações e proteger ficheiros de trabalho nos dispositivos pessoais do Windows 10 dos seus utilizadores.
ms.openlocfilehash: 64c6aa620171a373cd7564c7de3abbf4a4546c4e
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912828"
---
# <a name="set-or-edit-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="2e87c-103">Definir ou editar definições de proteção de aplicações para dispositivos Windows 10</span><span class="sxs-lookup"><span data-stu-id="2e87c-103">Set or edit application protection settings for Windows 10 devices</span></span>

<span data-ttu-id="2e87c-104">Este artigo aplica-se ao Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="2e87c-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="edit-an-app-management-policy-for-windows-10"></a><span data-ttu-id="2e87c-105">Editar uma política de gestão de aplicações para o Windows 10</span><span class="sxs-lookup"><span data-stu-id="2e87c-105">Edit an app management policy for Windows 10</span></span>

1. <span data-ttu-id="2e87c-106">Vá ao centro de administração em <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="2e87c-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>     
2. <span data-ttu-id="2e87c-107">No navegador esquerdo, escolha **Políticas de** \> **Dispositivos** .</span><span class="sxs-lookup"><span data-stu-id="2e87c-107">On the left nav, choose **Devices** \> **Policies** .</span></span>
1. <span data-ttu-id="2e87c-108">Escolha uma política de aplicações do Windows existente e, em seguida, **Edite.**</span><span class="sxs-lookup"><span data-stu-id="2e87c-108">Choose an existing Windows app policy and then **Edit**.</span></span>
1. <span data-ttu-id="2e87c-109">Escolha **Editar** ao lado de uma definição que pretende alterar e, em seguida, **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="2e87c-109">Choose **Edit** next to a setting you want to change and then **Save**.</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="2e87c-110">Criar uma política de gestão de aplicações para Windows 10</span><span class="sxs-lookup"><span data-stu-id="2e87c-110">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="2e87c-111">Se os seus utilizadores tiverem dispositivos Windows 10 pessoais, nos quais realizam tarefas profissionais, também pode proteger os seus dados nesses dispositivos.</span><span class="sxs-lookup"><span data-stu-id="2e87c-111">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="2e87c-112">Vá ao centro de administração em <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="2e87c-112">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
2. <span data-ttu-id="2e87c-113">No navegador esquerdo, escolha **Políticas de Dispositivos** \>  \> **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="2e87c-113">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
3. <span data-ttu-id="2e87c-114">No painel **Adicionar política**, introduza um nome exclusivo para esta política.</span><span class="sxs-lookup"><span data-stu-id="2e87c-114">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
4. <span data-ttu-id="2e87c-115">Em **Tipo de política**, selecione **Gestão de Aplicações para Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="2e87c-115">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
5. <span data-ttu-id="2e87c-116">Sob **o tipo dispositivo**, escolha **pessoal** ou **empresa própria.**</span><span class="sxs-lookup"><span data-stu-id="2e87c-116">Under **Device type**, choose either **Personal** or **Company Owned**.</span></span>
6. <span data-ttu-id="2e87c-117">A opção **Encriptar ficheiros de trabalho** é ativada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="2e87c-117">The **Encrypt work files** is turned on automatically.</span></span> 
7. <span data-ttu-id="2e87c-118">Defina **Impedir que os utilizadores copiem os dados da empresa para ficheiros pessoais e obrigá-los a guardar os ficheiros de trabalho no OneDrive para Empresas** como **Ativado** se não pretender que os utilizadores guardem ficheiros de trabalho nos respetivos PCs.</span><span class="sxs-lookup"><span data-stu-id="2e87c-118">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
9. <span data-ttu-id="2e87c-119">Expandir **Recuperar dados em dispositivos Windows**.</span><span class="sxs-lookup"><span data-stu-id="2e87c-119">Expand **Recover data on Windows devices**.</span></span> <span data-ttu-id="2e87c-120">Recomendamos que **o** ligue.</span><span class="sxs-lookup"><span data-stu-id="2e87c-120">We recommend that you turn it **On**.</span></span>
    <span data-ttu-id="2e87c-121">Antes de poder aceder à localização do certificado de Agente de Recuperação de Dados, tem de criar um.</span><span class="sxs-lookup"><span data-stu-id="2e87c-121">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one.</span></span> <span data-ttu-id="2e87c-122">Para obter instruções, consulte [Criar e verificar um certificado de Agente de Recuperação de Dados (EFS) do Sistema de Recolha de Dados encriptante (EFS).](/windows/security/information-protection/windows-information-protection/create-and-verify-an-efs-dra-certificate)</span><span class="sxs-lookup"><span data-stu-id="2e87c-122">For instructions, see [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](/windows/security/information-protection/windows-information-protection/create-and-verify-an-efs-dra-certificate).</span></span>
    
    <span data-ttu-id="2e87c-123">Por predefinição, os ficheiros de trabalho são encriptados com uma chave secreta que é armazenada no dispositivo e é associada ao perfil do utilizador.</span><span class="sxs-lookup"><span data-stu-id="2e87c-123">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile.</span></span> <span data-ttu-id="2e87c-124">Apenas o utilizador pode abrir e desencriptar o ficheiro.</span><span class="sxs-lookup"><span data-stu-id="2e87c-124">Only the user can open and decrypt the file.</span></span> <span data-ttu-id="2e87c-125">No entanto, se um dispositivo for perdido ou um utilizador for removido, um ficheiro pode ficar bloqueado num estado encriptado.</span><span class="sxs-lookup"><span data-stu-id="2e87c-125">However, if a device is lost or a user is removed, a file can be stuck in an encrypted state.</span></span> <span data-ttu-id="2e87c-126">Um administrador pode usar o certificado de Agente de Recuperação de Dados (DRA) para desencriptar o ficheiro.</span><span class="sxs-lookup"><span data-stu-id="2e87c-126">An admin can use the Data Recovery Agent (DRA) certificate to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="2e87c-128">**Expanda-se Proteger localizações adicionais de rede e nuvem** se pretender adicionar domínios adicionais ou localizações online do SharePoint para garantir que os ficheiros em todas as aplicações listadas estão protegidos.</span><span class="sxs-lookup"><span data-stu-id="2e87c-128">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps are protected.</span></span> <span data-ttu-id="2e87c-129">Se precisar de introduzir mais do que um item em cada campo, utilize ponto e vírgula (;) entre os itens.</span><span class="sxs-lookup"><span data-stu-id="2e87c-129">If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span>
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="2e87c-p104">Em seguida, decida **Quem irá ver estas definições?** Se não quiser utilizar o grupo de segurança predefinido, **Todos os Utilizadores**, selecione **Alterar**, selecione os grupos de segurança que irão receber estas definições \> **Selecionar**.</span><span class="sxs-lookup"><span data-stu-id="2e87c-p104">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
12. <span data-ttu-id="2e87c-133">Por fim, selecione **Adicionar** para guardar a política e atribua-a a todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="2e87c-133">Finally, choose **Add** to save the policy, and assign it to devices.</span></span>