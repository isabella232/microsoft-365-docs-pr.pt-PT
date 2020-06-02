---
title: Aceder aos recursos no local a partir de um dispositivo AD AZure ligado ao Microsoft 365 Business
f1.keywords:
- NOCSH
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Saiba como obter acesso a recursos no local, como linha de aplicações empresariais, partilhas de ficheiros e impressoras de um Azure Ative Directory que aderiu ao dispositivo Windows 10.
ms.openlocfilehash: 9615ecc9469992d3e5a7479f4799c610db11fb41
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471257"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a><span data-ttu-id="c33b2-103">Aceder aos recursos no local a partir de um dispositivo AD AD Azure no Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="c33b2-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium</span></span>

<span data-ttu-id="c33b2-104">Este artigo aplica-se ao Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="c33b2-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="c33b2-105">Qualquer dispositivo do Windows 10 que seja a aderido ao Azure Ative Directory tem acesso a todos os recursos baseados na nuvem, como as suas aplicações Microsoft 365, e pode ser protegido pelo Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="c33b2-105">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Microsoft 365 apps, and can be protected by Microsoft 365 Business Premium.</span></span> <span data-ttu-id="c33b2-106">Também pode permitir o acesso a recursos no local, como aplicações de linha de negócios (LOB), partilhas de ficheiros e impressoras.</span><span class="sxs-lookup"><span data-stu-id="c33b2-106">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="c33b2-107">Para permitir o acesso, utilize [o Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) para sincronizar o seu Ative Directory no local com o Azure Ative Directory.</span><span class="sxs-lookup"><span data-stu-id="c33b2-107">To allow access, use [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="c33b2-108">Para saber mais, consulte [Introdução à gestão de dispositivos no Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span><span class="sxs-lookup"><span data-stu-id="c33b2-108">To learn more, see [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="c33b2-109">Os passos são também resumidos nas seguintes secções.</span><span class="sxs-lookup"><span data-stu-id="c33b2-109">The steps are also summarized in the following sections.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c33b2-110">Este procedimento só é aplicável à OAuth e à NTLM.</span><span class="sxs-lookup"><span data-stu-id="c33b2-110">This procedure is only applicable to OAuth and NTLM.</span></span> <span data-ttu-id="c33b2-111">Kerberos não é apoiado.</span><span class="sxs-lookup"><span data-stu-id="c33b2-111">Kerberos is not supported.</span></span>
 
## <a name="run-azure-ad-connect"></a><span data-ttu-id="c33b2-112">Executar Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="c33b2-112">Run Azure AD Connect</span></span>

<span data-ttu-id="c33b2-113">Complete os seguintes passos para permitir que os dispositivos Azure AD da sua organização tenham acesso aos recursos no local.</span><span class="sxs-lookup"><span data-stu-id="c33b2-113">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="c33b2-114">Para sincronizar os seus utilizadores, grupos e contactos do Diretório Ativo local para o Azure Ative Directory, executar o assistente de sincronização do Diretório e a Azure AD Connect, conforme descrito na [sincronização do diretório configurado para o Office 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="c33b2-114">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization).</span></span>
    
2. <span data-ttu-id="c33b2-115">Depois de concluída a sincronização do diretório, certifique-se de que os dispositivos windows 10 da sua organização estão unidos a Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c33b2-115">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="c33b2-116">Este passo é feito individualmente em cada dispositivo Windows 10.</span><span class="sxs-lookup"><span data-stu-id="c33b2-116">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="c33b2-117">Consulte [os dispositivos Windows para os utilizadores Do Microsoft 365 Business Premium](set-up-windows-devices.md) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="c33b2-117">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="c33b2-118">Uma vez que os dispositivos Windows 10 estejam ligados ao Azure AD, cada utilizador deve reiniciar os seus dispositivos e iniciar sôs com as suas credenciais Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="c33b2-118">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business Premium credentials.</span></span> <span data-ttu-id="c33b2-119">Todos os dispositivos têm agora acesso a recursos no local também.</span><span class="sxs-lookup"><span data-stu-id="c33b2-119">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="c33b2-120">Não são necessárias medidas adicionais para ter acesso aos recursos no local para dispositivos aderidos a Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c33b2-120">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="c33b2-121">Esta funcionalidade encontra-se integrada no Windows 10.</span><span class="sxs-lookup"><span data-stu-id="c33b2-121">This functionality is built into Windows 10.</span></span> 

<span data-ttu-id="c33b2-122">Se tiver planos para iniciar sessão no dispositivo AADJ que não seja o método de senha Como PIN/Bio-métrica via login credencial WHFB e, em seguida, aceder a recursos no local (partilhas,impressoras.. etc), por favor, sigahttps://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span><span class="sxs-lookup"><span data-stu-id="c33b2-122">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares,printers..etc), please follow https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span></span>
  
<span data-ttu-id="c33b2-123">Se a sua organização não estiver pronta para implantar na configuração do dispositivo azure AD descrita acima, considere configurar a [configuração do dispositivo AD AD Ad Hybrid Azure](manage-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="c33b2-123">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="c33b2-124">Considerações quando se junta dispositivos Windows ao Azure AD</span><span class="sxs-lookup"><span data-stu-id="c33b2-124">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="c33b2-125">Se o dispositivo Windows a que aD Azure-AD aderiu foi previamente agrupado por domínio ou num grupo de trabalho, considere as seguintes limitações:</span><span class="sxs-lookup"><span data-stu-id="c33b2-125">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="c33b2-126">Quando um dispositivo Azure AD se junta, cria um novo utilizador sem se referir a um perfil existente.</span><span class="sxs-lookup"><span data-stu-id="c33b2-126">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="c33b2-127">Os perfis devem ser migrados manualmente.</span><span class="sxs-lookup"><span data-stu-id="c33b2-127">Profiles must be manually migrated.</span></span> <span data-ttu-id="c33b2-128">Um perfil de utilizador contém informações como favoritos, ficheiros locais, configurações do navegador e definições de menu Iniciar.</span><span class="sxs-lookup"><span data-stu-id="c33b2-128">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="c33b2-129">A melhor abordagem é encontrar uma ferramenta de terceiros para mapear ficheiros e configurações existentes para o novo perfil.</span><span class="sxs-lookup"><span data-stu-id="c33b2-129">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="c33b2-130">Se o dispositivo estiver a utilizar objetos de política de grupo (GPO), alguns GPOs podem não ter um [Fornecedor de Serviço de Configuração](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) comparável (CSP) no Intune.</span><span class="sxs-lookup"><span data-stu-id="c33b2-130">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="c33b2-131">Executar a [ferramenta MMAT](https://www.microsoft.com/download/details.aspx?id=45520) para encontrar CSPs comparáveis para os GPOs existentes.</span><span class="sxs-lookup"><span data-stu-id="c33b2-131">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="c33b2-132">Os utilizadores não poderão autenticar aplicações que dependam da autenticação do Ative Directory.</span><span class="sxs-lookup"><span data-stu-id="c33b2-132">Users won't be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="c33b2-133">Avalie a aplicação legacy e considere atualização para uma app que usa o moderno Auth, se possível.</span><span class="sxs-lookup"><span data-stu-id="c33b2-133">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="c33b2-134">A descoberta da impressora ative do Diretório não vai funcionar.</span><span class="sxs-lookup"><span data-stu-id="c33b2-134">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="c33b2-135">Pode fornecer caminhos de impressora direta para todos os utilizadores ou utilizar [a Impressão De Nuvem Híbrida.](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)</span><span class="sxs-lookup"><span data-stu-id="c33b2-135">You can provide direct printer paths for all users or use [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
