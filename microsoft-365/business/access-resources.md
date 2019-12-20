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
description: Saiba como ter acesso a recursos locais, como linha de aplicativos de negócios, compartilhamentos de arquivos e impressoras de um diretório ativo do Azure, que se juntou ao dispositivo Windows 10.
ms.openlocfilehash: 89ac38f3da9cbdd3ff1a5eb33dc129d2e83521c7
ms.sourcegitcommit: 8c244b38c43dd00c4ef0102f8bed02ab36639a6b
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/10/2019
ms.locfileid: "39967169"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a><span data-ttu-id="cb9cb-103">Acesse recursos locais de um dispositivo azure ad no Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="cb9cb-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>

<span data-ttu-id="cb9cb-104">Qualquer dispositivo Windows 10 que esteja no Diretório Ativo Do Azure, juntou-se, tem acesso a todos os recursos baseados em nuvem, como seus aplicativos do Office 365, e pode ser protegido pelo Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="cb9cb-104">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Office 365 apps, and can be protected by Microsoft 365 Business.</span></span> <span data-ttu-id="cb9cb-105">Você também pode permitir o acesso a recursos no local, como aplicativos de linha de negócios (LOB), compartilhamentos de arquivos e impressoras.</span><span class="sxs-lookup"><span data-stu-id="cb9cb-105">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="cb9cb-106">Para permitir o acesso, use o AD Connect do [Azure](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) para sincronizar seu Diretório Ativo no local com o Diretório Ativo Do Azure.</span><span class="sxs-lookup"><span data-stu-id="cb9cb-106">To allow access, use [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="cb9cb-107">Para saber mais, consulte [a introdução ao gerenciamento de dispositivos no Diretório Ativo Do Azure.](https://docs.microsoft.com/azure/active-directory/device-management-introduction)</span><span class="sxs-lookup"><span data-stu-id="cb9cb-107">To learn more, see [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="cb9cb-108">As etapas também são resumidas nas seguintes seções.</span><span class="sxs-lookup"><span data-stu-id="cb9cb-108">The steps are also summarized in the following sections.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="cb9cb-109">Este procedimento só é aplicável à OAuth e à NTLM.</span><span class="sxs-lookup"><span data-stu-id="cb9cb-109">This procedure is only applicable to OAuth and NTLM.</span></span> <span data-ttu-id="cb9cb-110">Kerberos não é apoiado.</span><span class="sxs-lookup"><span data-stu-id="cb9cb-110">Kerberos is not supported.</span></span>
 
## <a name="run-azure-ad-connect"></a><span data-ttu-id="cb9cb-111">Executar azure ad connect</span><span class="sxs-lookup"><span data-stu-id="cb9cb-111">Run Azure AD Connect</span></span>

<span data-ttu-id="cb9cb-112">Complete as seguintes etapas para permitir que o AD Azure da sua organização acesse dispositivos para acessar recursos locais.</span><span class="sxs-lookup"><span data-stu-id="cb9cb-112">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="cb9cb-113">Para sincronizar seus usuários, grupos e contatos do Diretório Ativo local no Diretório Ativo Do Azure, execute o assistente de sincronização do Diretório e o AD Connect do Azure, conforme descrito na sincronização do diretório para o [Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="cb9cb-113">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
2. <span data-ttu-id="cb9cb-114">Depois que a sincronização do diretório estiver concluída, certifique-se de que os dispositivos Windows 10 da sua organização estão aderidos ao AD do Azure.</span><span class="sxs-lookup"><span data-stu-id="cb9cb-114">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="cb9cb-115">Esta etapa é feita individualmente em cada dispositivo Windows 10.</span><span class="sxs-lookup"><span data-stu-id="cb9cb-115">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="cb9cb-116">Veja [configurar dispositivos Windows para usuários do Microsoft 365 Business](set-up-windows-devices.md) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="cb9cb-116">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="cb9cb-117">Uma vez que os dispositivos Windows 10 são ajuntados pelo AD do Azure, cada usuário deve reiniciar seus dispositivos e entrar com suas credenciais microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="cb9cb-117">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business credentials.</span></span> <span data-ttu-id="cb9cb-118">Todos os dispositivos agora têm acesso a recursos no local também.</span><span class="sxs-lookup"><span data-stu-id="cb9cb-118">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="cb9cb-119">Não são necessárias medidas adicionais para ter acesso a recursos locais para dispositivos azure azure ajuntados a AD.</span><span class="sxs-lookup"><span data-stu-id="cb9cb-119">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="cb9cb-120">Essa funcionalidade é incorporada ao Windows 10.</span><span class="sxs-lookup"><span data-stu-id="cb9cb-120">This functionality is built into Windows 10.</span></span> 

<span data-ttu-id="cb9cb-121">Se você tem planos de fazer login no dispositivo AADJ além do método de senha Como PIN/Bio-metric via login de credencial WHFB e, em seguida, acessar recursos locais (compartilhamentos, impressoras.. etc), por favor, sigahttps://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span><span class="sxs-lookup"><span data-stu-id="cb9cb-121">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares,printers..etc), please follow https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span></span>
  
<span data-ttu-id="cb9cb-122">Se a sua organização não estiver pronta para ser implantada na configuração do dispositivo adjacente ao AZure AD descrita acima, considere a configuração da configuração do [dispositivo Hybrid Azure AD Joined](manage-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="cb9cb-122">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="cb9cb-123">Considerações quando você adere dispositivos Windows a um anúncio do Azure</span><span class="sxs-lookup"><span data-stu-id="cb9cb-123">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="cb9cb-124">Se o dispositivo Windows que você azure-AD juntou foi previamente introduzido em domínio ou em um grupo de trabalho, considere as seguintes limitações:</span><span class="sxs-lookup"><span data-stu-id="cb9cb-124">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="cb9cb-125">Quando um dispositivo azure AD junta, ele cria um novo usuário sem referenciar um perfil existente.</span><span class="sxs-lookup"><span data-stu-id="cb9cb-125">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="cb9cb-126">Os perfis devem ser migrados manualmente.</span><span class="sxs-lookup"><span data-stu-id="cb9cb-126">Profiles must be manually migrated.</span></span> <span data-ttu-id="cb9cb-127">Um perfil de usuário contém informações como favoritos, arquivos locais, configurações do navegador e configurações do menu Iniciar.</span><span class="sxs-lookup"><span data-stu-id="cb9cb-127">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="cb9cb-128">Uma abordagem melhor é encontrar uma ferramenta de terceiros para mapear arquivos e configurações existentes para o novo perfil.</span><span class="sxs-lookup"><span data-stu-id="cb9cb-128">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="cb9cb-129">Se o dispositivo estiver usando objetos de política de grupo (GPO), alguns GPOs podem não ter um provedor de serviço de [configuração](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) comparável (CSP) em sintonia.</span><span class="sxs-lookup"><span data-stu-id="cb9cb-129">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="cb9cb-130">Executar a [ferramenta MMAT](https://www.microsoft.com/download/details.aspx?id=45520) para encontrar CSPs comparáveis para GPOs existentes.</span><span class="sxs-lookup"><span data-stu-id="cb9cb-130">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="cb9cb-131">Os usuários não poderão autenticar aplicativos que dependem da autenticação do Diretório Ativo.</span><span class="sxs-lookup"><span data-stu-id="cb9cb-131">Users won't be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="cb9cb-132">Avalie o aplicativo legado e considere atualizar para um aplicativo que usa a Auth moderna, se possível.</span><span class="sxs-lookup"><span data-stu-id="cb9cb-132">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="cb9cb-133">A descoberta ativa da impressora do diretório não funcionará.</span><span class="sxs-lookup"><span data-stu-id="cb9cb-133">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="cb9cb-134">Você pode fornecer caminhos de impressora direta para todos os usuários ou usar [o Hybrid Cloud Print.](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)</span><span class="sxs-lookup"><span data-stu-id="cb9cb-134">You can provide direct printer paths for all users or use [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
