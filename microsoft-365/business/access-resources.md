---
title: Acesse recursos locais de um dispositivo azure ad no Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: M365-subscription-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Saiba como ter acesso a recursos locais, como aplicativos line of business, compartilhamentos de arquivos e impressoras de um diretório ativo do Azure, que se juntou ao dispositivo Windows 10.
ms.openlocfilehash: 2af5d4b4f84f39f5b157313e5b38ef030da7263d
ms.sourcegitcommit: 70e920f76526f47fc849df615de4569e0ac2f4be
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/07/2019
ms.locfileid: "38030540"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a><span data-ttu-id="c8286-103">Acesse recursos locais de um dispositivo azure ad no Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="c8286-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>

<span data-ttu-id="c8286-104">Qualquer dispositivo Windows 10 que esteja no Diretório Ativo Do Azure, juntou-se, terá acesso a todos os recursos baseados em nuvem, como seus aplicativos do Office 365, e pode ser protegido pelo Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="c8286-104">Any Windows 10 device that is Azure Active Directory joined will have access to all cloud-based resources such as your Office 365 apps and can be protected by Microsoft 365 Business.</span></span> <span data-ttu-id="c8286-105">Para também permitir o acesso a recursos no local, como aplicativos Line Of Business (LOB), compartilhamentos de arquivos e impressoras, você deve sincronizar seu Diretório Ativo no local com o Diretório Ativo Do Azure usando o [AZure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span><span class="sxs-lookup"><span data-stu-id="c8286-105">To also allow access to on-premises resources like Line Of Business (LOB) apps, file shares, and printers, you must synchronize your on-premises Active Directory with Azure Active Directory by using [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span> 

<span data-ttu-id="c8286-106">Veja [a introdução ao gerenciamento de dispositivos no Diretório Ativo Do Azure](https://docs.microsoft.com/azure/active-directory/device-management-introduction) para saber mais.</span><span class="sxs-lookup"><span data-stu-id="c8286-106">See [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction) to learn more.</span></span>
<span data-ttu-id="c8286-107">As etapas também são resumidas nas seguintes seções.</span><span class="sxs-lookup"><span data-stu-id="c8286-107">The steps are also summarized in the following sections.</span></span>

## <a name="run-azure-ad-connect"></a><span data-ttu-id="c8286-108">Executar azure ad connect</span><span class="sxs-lookup"><span data-stu-id="c8286-108">Run Azure AD Connect</span></span>

<span data-ttu-id="c8286-109">Complete as seguintes etapas para permitir que o AD Azure da sua organização acesse dispositivos para acessar recursos locais.</span><span class="sxs-lookup"><span data-stu-id="c8286-109">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="c8286-110">Para sincronizar seus usuários, grupos e contatos do Diretório Ativo local no Diretório Ativo Do Azure, execute o assistente de sincronização do Diretório e o AD Connect do Azure, conforme descrito na sincronização do diretório para o [Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="c8286-110">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
2. <span data-ttu-id="c8286-111">Depois que a sincronização do diretório tiver sido concluída, certifique-se de que os dispositivos Windows 10 da sua organização estão aderidos ao AD do Azure.</span><span class="sxs-lookup"><span data-stu-id="c8286-111">After the directory synchronization has completed, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="c8286-112">Esta etapa é feita individualmente em cada dispositivo Windows 10.</span><span class="sxs-lookup"><span data-stu-id="c8286-112">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="c8286-113">Veja [configurar dispositivos Windows para usuários do Microsoft 365 Business](set-up-windows-devices.md) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="c8286-113">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="c8286-114">Uma vez que os dispositivos Windows 10 são ajuntados pelo AD Do Azure, cada usuário deve reiniciar seus dispositivos e fazer login com suas credenciais Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="c8286-114">Once the Windows 10 devices are Azure AD joined, each user should reboot their devices and login with their Microsoft 365 Business credentials.</span></span> <span data-ttu-id="c8286-115">Todos os dispositivos terão agora acesso a recursos no local também.</span><span class="sxs-lookup"><span data-stu-id="c8286-115">All devices will now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="c8286-116">Não são necessárias medidas adicionais para ter acesso a recursos locais para dispositivos azure azure ajuntados a AD.</span><span class="sxs-lookup"><span data-stu-id="c8286-116">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="c8286-117">Esta é a funcionalidade incorporada disponível no Windows 10.</span><span class="sxs-lookup"><span data-stu-id="c8286-117">This is built-in functionality available in Windows 10.</span></span> 
  
<span data-ttu-id="c8286-118">Se a sua organização não estiver pronta para ser implantada na configuração do dispositivo adjacente ao AZure Azure descrita acima, considere a configuração da configuração do [dispositivo Hybrid Azure AD Joined](manage-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="c8286-118">If your organization is not ready to deploy in the Azure AD Joined Device Configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a><span data-ttu-id="c8286-119">Considerações ao juntar seus dispositivos Windows ao AD do Azure</span><span class="sxs-lookup"><span data-stu-id="c8286-119">Considerations when joining your Windows devices to Azure AD</span></span>

<span data-ttu-id="c8286-120">Se você é aD do Azure que adere a um dispositivo Windows que já foi unido ou em um grupo de trabalho, você precisa considerar as seguintes limitações:</span><span class="sxs-lookup"><span data-stu-id="c8286-120">If you are Azure AD joining a Windows device that has previously been domain-joined or in a workgroup, you need to consider the following limitations:</span></span>
  
- <span data-ttu-id="c8286-121">Quando um dispositivo azure AD junta, ele cria um novo usuário sem referenciar um perfil existente.</span><span class="sxs-lookup"><span data-stu-id="c8286-121">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="c8286-122">Para corrigir isso, os perfis precisam ser migrados manualmente.</span><span class="sxs-lookup"><span data-stu-id="c8286-122">To fix this, profiles need to be manually migrated.</span></span> <span data-ttu-id="c8286-123">Um perfil de usuário contém informações como favoritos, arquivos locais, configurações do navegador, configurações de menu iniciar, etc. Uma melhor abordagem é encontrar uma ferramenta de terceiros para mapear arquivos e configurações existentes para o novo perfil</span><span class="sxs-lookup"><span data-stu-id="c8286-123">A user profile contains information like favorites, local files, browser settings, Start menu settings, etc. A best approach is to find a third-party tool to map existing files and settings to the new profile</span></span>

- <span data-ttu-id="c8286-124">Se o dispositivo estiver usando objetos de política de grupo (GPO), alguns GPOs podem não ter um provedor de serviço de [configuração](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) comparável (CSP) em sintonia.</span><span class="sxs-lookup"><span data-stu-id="c8286-124">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="c8286-125">Executar a [ferramenta MMAT](https://www.microsoft.com/download/details.aspx?id=45520) para encontrar CSPs comparáveis para GPOs existentes.</span><span class="sxs-lookup"><span data-stu-id="c8286-125">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="c8286-126">Os usuários não poderão autenticar aplicativos que dependem da autenticação do Diretório Ativo.</span><span class="sxs-lookup"><span data-stu-id="c8286-126">Users will not be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="c8286-127">Para lidar com isso avaliar usando um aplicativo legado e considerar a atualização para um aplicativo que usa Auth moderno, se possível.</span><span class="sxs-lookup"><span data-stu-id="c8286-127">To deal with this evaluate using a legacy app and consider updating to an app that uses modern Auth if possible.</span></span>

- <span data-ttu-id="c8286-128">A descoberta ativa da impressora do diretório não funcionará.</span><span class="sxs-lookup"><span data-stu-id="c8286-128">Active Directory printer discovery will not work.</span></span> <span data-ttu-id="c8286-129">Para corrigir isso, forneça caminhos de impressora direta para todos os usuários ou aproveite o [Hybrid Cloud Print.](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)</span><span class="sxs-lookup"><span data-stu-id="c8286-129">To fix this, provide direct printer paths for all users or leverage [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
