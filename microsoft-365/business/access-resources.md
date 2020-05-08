---
title: Acesso aos recursos no local a partir de um dispositivo azure ad-join no Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Saiba como aceder a recursos no local, como linha de aplicações de negócios, partilhas de ficheiros e impressoras de um dispositivo Azure Ative Directory que se juntou ao Windows 10.
ms.openlocfilehash: 980efbf09349cc0203ac50ae5e028c008d5694ca
ms.sourcegitcommit: 46644f9778bc70ab6d62783e0a1e60ba2eccc27f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/08/2020
ms.locfileid: "44165907"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a><span data-ttu-id="09b13-103">Acesso aos recursos no local a partir de um dispositivo azure ad-join no Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="09b13-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium</span></span>

<span data-ttu-id="09b13-104">Qualquer dispositivo Windows 10 que seja o Azure Ative Directory junto tem acesso a todos os recursos baseados na nuvem, como as suas aplicações Microsoft 365, e pode ser protegido pelo Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="09b13-104">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Microsoft 365 apps, and can be protected by Microsoft 365 Business Premium.</span></span> <span data-ttu-id="09b13-105">Também pode permitir o acesso a recursos no local, como aplicações de linha de negócios (LOB), partilhas de ficheiros e impressoras.</span><span class="sxs-lookup"><span data-stu-id="09b13-105">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="09b13-106">Para permitir o acesso, utilize o [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) para sincronizar o seu Diretório Ativo no local com o Diretório Ativo Azure.</span><span class="sxs-lookup"><span data-stu-id="09b13-106">To allow access, use [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="09b13-107">Para saber mais, consulte Introdução à gestão de [dispositivos no Diretório Ativo Azure.](https://docs.microsoft.com/azure/active-directory/device-management-introduction)</span><span class="sxs-lookup"><span data-stu-id="09b13-107">To learn more, see [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="09b13-108">Os passos também são resumidos nas seguintes secções.</span><span class="sxs-lookup"><span data-stu-id="09b13-108">The steps are also summarized in the following sections.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="09b13-109">Este procedimento só é aplicável à OAuth e à NTLM.</span><span class="sxs-lookup"><span data-stu-id="09b13-109">This procedure is only applicable to OAuth and NTLM.</span></span> <span data-ttu-id="09b13-110">Kerberos não é apoiado.</span><span class="sxs-lookup"><span data-stu-id="09b13-110">Kerberos is not supported.</span></span>
 
## <a name="run-azure-ad-connect"></a><span data-ttu-id="09b13-111">Executar Ligação AD Azure</span><span class="sxs-lookup"><span data-stu-id="09b13-111">Run Azure AD Connect</span></span>

<span data-ttu-id="09b13-112">Complete os seguintes passos para permitir que o Azure AD da sua organização tenha acesso aos recursos no local.</span><span class="sxs-lookup"><span data-stu-id="09b13-112">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="09b13-113">Para sincronizar os seus utilizadores, grupos e contactos do Diretório Ativo local para o Diretório Ativo Azure, execute o assistente de sincronização do Diretório e o Azure AD Connect, conforme descrito na sincronização do diretório para o [Office 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="09b13-113">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization).</span></span>
    
2. <span data-ttu-id="09b13-114">Depois de concluída a sincronização do diretório, certifique-se de que os dispositivos Windows 10 da sua organização são Azure AD.</span><span class="sxs-lookup"><span data-stu-id="09b13-114">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="09b13-115">Este passo é feito individualmente em cada dispositivo do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="09b13-115">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="09b13-116">Consulte a [configuração de dispositivos Windows para utilizadores do Microsoft 365 Business Premium](set-up-windows-devices.md) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="09b13-116">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="09b13-117">Uma vez que os dispositivos Do Windows 10 são AD Azure, cada utilizador deve reiniciar os seus dispositivos e iniciar sessão com as suas credenciais Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="09b13-117">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business Premium credentials.</span></span> <span data-ttu-id="09b13-118">Todos os dispositivos têm agora acesso aos recursos no local também.</span><span class="sxs-lookup"><span data-stu-id="09b13-118">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="09b13-119">Não são necessárias medidas adicionais para ter acesso aos recursos no local para dispositivos ligados à AD Azure.</span><span class="sxs-lookup"><span data-stu-id="09b13-119">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="09b13-120">Esta funcionalidade está incorporada no Windows 10.</span><span class="sxs-lookup"><span data-stu-id="09b13-120">This functionality is built into Windows 10.</span></span> 

<span data-ttu-id="09b13-121">Se tiver planos para iniciar sessão no dispositivo AADJ que não seja o método de senha, como PIN/Bio-metric via login credencial WHFB e, em seguida, aceder aos recursos no local (ações,impressoras.. etc), por favor, sigahttps://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span><span class="sxs-lookup"><span data-stu-id="09b13-121">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares,printers..etc), please follow https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span></span>
  
<span data-ttu-id="09b13-122">Se a sua organização não estiver pronta para ser implementada na configuração de dispositivo seletiva do Azure AD descrita acima, considere configurar a configuração do [dispositivo Hybrid Azure AD Joined](manage-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="09b13-122">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="09b13-123">Considerações quando se juntam a dispositivos Windows para a Azure AD</span><span class="sxs-lookup"><span data-stu-id="09b13-123">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="09b13-124">Se o dispositivo Windows a que aderiu o Azure-AD foi previamente associado ao domínio ou num grupo de trabalho, considere as seguintes limitações:</span><span class="sxs-lookup"><span data-stu-id="09b13-124">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="09b13-125">Quando um dispositivo Azure AD se junta, cria um novo utilizador sem se referir a um perfil existente.</span><span class="sxs-lookup"><span data-stu-id="09b13-125">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="09b13-126">Os perfis devem ser migrados manualmente.</span><span class="sxs-lookup"><span data-stu-id="09b13-126">Profiles must be manually migrated.</span></span> <span data-ttu-id="09b13-127">Um perfil de utilizador contém informações como favoritos, ficheiros locais, definições de navegador e definições de menu Iniciar.</span><span class="sxs-lookup"><span data-stu-id="09b13-127">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="09b13-128">A melhor abordagem é encontrar uma ferramenta de terceiros para mapear ficheiros e configurações existentes para o novo perfil.</span><span class="sxs-lookup"><span data-stu-id="09b13-128">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="09b13-129">Se o dispositivo estiver a utilizar objetos de política de grupo (GPO), alguns GPOs podem não ter um fornecedor de [serviçode configuração](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) comparável (CSP) em Intune.</span><span class="sxs-lookup"><span data-stu-id="09b13-129">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="09b13-130">Executar a [ferramenta MMAT](https://www.microsoft.com/download/details.aspx?id=45520) para encontrar CSPs comparáveis para GPOs existentes.</span><span class="sxs-lookup"><span data-stu-id="09b13-130">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="09b13-131">Os utilizadores não poderão autenticar aplicações que dependem da autenticação do Diretório Ativo.</span><span class="sxs-lookup"><span data-stu-id="09b13-131">Users won't be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="09b13-132">Avalie a aplicação legacy e considere a atualização para uma app que usa o moderno Auth, se possível.</span><span class="sxs-lookup"><span data-stu-id="09b13-132">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="09b13-133">A descoberta da impressora de diretório ativo não vai funcionar.</span><span class="sxs-lookup"><span data-stu-id="09b13-133">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="09b13-134">Pode fornecer caminhos de impressora direta para todos os utilizadores ou utilizar impressão [de nuvem híbrida](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span><span class="sxs-lookup"><span data-stu-id="09b13-134">You can provide direct printer paths for all users or use [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
