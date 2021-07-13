---
title: Aceder a recursos no local a partir de um dispositivo associado ao Azure AD no Microsoft 365 Empresas
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
- AdminTemplateSet
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Saiba como obter acesso a recursos no local, como aplicações de linha de negócio, partilhas de ficheiros e impressoras a partir de um Azure Active Directory dispositivo Windows 10 empresa.
ms.openlocfilehash: 71d60e0187c917dffb7390afcedf22dc73f44008
ms.sourcegitcommit: 00f001019c653269d85718d410f970887d904304
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/12/2021
ms.locfileid: "53393465"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a><span data-ttu-id="519a4-103">Aceder a recursos no local a partir de um dispositivo associado ao Azure AD no Microsoft 365 Empresas Premium</span><span class="sxs-lookup"><span data-stu-id="519a4-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium</span></span>

<span data-ttu-id="519a4-104">Este artigo aplica-se a Microsoft 365 Empresas Premium.</span><span class="sxs-lookup"><span data-stu-id="519a4-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="519a4-105">Qualquer Windows 10 dispositivo que esteja Azure Active Directory associado tem acesso a todos os recursos baseados na nuvem, como as suas aplicações do Microsoft 365, e pode ser protegido pelo Microsoft 365 Empresas Premium.</span><span class="sxs-lookup"><span data-stu-id="519a4-105">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Microsoft 365 apps, and can be protected by Microsoft 365 Business Premium.</span></span> <span data-ttu-id="519a4-106">Também pode permitir o acesso a recursos no local, como aplicações de linha de negócio (LOB), partilhas de ficheiros e impressoras.</span><span class="sxs-lookup"><span data-stu-id="519a4-106">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="519a4-107">Para permitir o acesso, utilize o [Azure AD Ligação](/azure/active-directory/connect/active-directory-aadconnect) para sincronizar o seu Active Directory no local com o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="519a4-107">To allow access, use [Azure AD Connect](/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span>

<span data-ttu-id="519a4-108">Para saber mais, consulte [Introdução à gestão de dispositivos no Azure Active Directory](/azure/active-directory/device-management-introduction).</span><span class="sxs-lookup"><span data-stu-id="519a4-108">To learn more, see [Introduction to device management in Azure Active Directory](/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="519a4-109">Os passos também estão resumidos nas secções seguintes.</span><span class="sxs-lookup"><span data-stu-id="519a4-109">The steps are also summarized in the following sections.</span></span>

## <a name="run-azure-ad-connect"></a><span data-ttu-id="519a4-110">Executar o Azure AD Ligação</span><span class="sxs-lookup"><span data-stu-id="519a4-110">Run Azure AD Connect</span></span>

<span data-ttu-id="519a4-111">Conclua os seguintes passos para permitir que os dispositivos associados ao Azure AD da sua organização acedam a recursos no local.</span><span class="sxs-lookup"><span data-stu-id="519a4-111">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>

1. <span data-ttu-id="519a4-112">Para sincronizar os seus utilizadores, grupos e contactos do Active Directory local no Azure Active Directory, execute o Assistente de sincronização de diretórios e o Azure AD Ligação conforme descrito em Configurar a [sincronização](../enterprise/set-up-directory-synchronization.md)de diretórios para Office 365.</span><span class="sxs-lookup"><span data-stu-id="519a4-112">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](../enterprise/set-up-directory-synchronization.md).</span></span>

2. <span data-ttu-id="519a4-113">Após a sincronização de diretórios estar concluída, certifique-se de que os dispositivos móveis Windows 10 da sua organização estão associados ao Azure AD.</span><span class="sxs-lookup"><span data-stu-id="519a4-113">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="519a4-114">Este passo é realizado individualmente em cada Windows 10 dispositivo.</span><span class="sxs-lookup"><span data-stu-id="519a4-114">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="519a4-115">Consulte [Configurar dispositivos Windows para utilizadores Microsoft 365 Empresas Premium utilizadores para](set-up-windows-devices.md) obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="519a4-115">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for details.</span></span>

3. <span data-ttu-id="519a4-116">Assim que os Windows 10 dispositivos móveis estiverem associados ao Azure AD, cada utilizador terá de reiniciar os respetivos dispositivos e entrar com as Microsoft 365 Empresas Premium credenciais.</span><span class="sxs-lookup"><span data-stu-id="519a4-116">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business Premium credentials.</span></span> <span data-ttu-id="519a4-117">Todos os dispositivos agora também têm acesso a recursos no local.</span><span class="sxs-lookup"><span data-stu-id="519a4-117">All devices now have access to on-premises resources as well.</span></span>

<span data-ttu-id="519a4-118">Não são necessários passos adicionais para aceder aos recursos no local em dispositivos associados ao Azure AD.</span><span class="sxs-lookup"><span data-stu-id="519a4-118">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="519a4-119">Esta funcionalidade está incorporada no Windows 10.</span><span class="sxs-lookup"><span data-stu-id="519a4-119">This functionality is built into Windows 10.</span></span>

<span data-ttu-id="519a4-120">Se tiver planos de início de sessão no dispositivo AADJ sem ser através de um método de palavra-passe Como o PIN/Bio-métrica através do início de sessão de credenciais WHFB e, em seguida, aceder aos recursos no local (partilhas, impressoras, etc.), siga este [artigo.](/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)</span><span class="sxs-lookup"><span data-stu-id="519a4-120">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares, printers, etc.), please follow [this article](/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="519a4-121">Se a sua organização não estiver pronta para implementar na configuração de dispositivos associados ao Azure AD acima, considere configurar a configuração de dispositivos associados ao [Azure AD Híbrido.](manage-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="519a4-121">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>

### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="519a4-122">Considerações a ter ao aderir Windows dispositivos ao Azure AD</span><span class="sxs-lookup"><span data-stu-id="519a4-122">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="519a4-123">Se o Windows dispositivo a que aderiu ao Azure-AD tiver aderido anteriormente a um domínio ou num grupo de trabalho, tenha em consideração as seguintes limitações:</span><span class="sxs-lookup"><span data-stu-id="519a4-123">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>

- <span data-ttu-id="519a4-124">Quando um dispositivo Azure AD adere, cria um novo utilizador sem referenciar um perfil existente.</span><span class="sxs-lookup"><span data-stu-id="519a4-124">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="519a4-125">Os perfis têm de ser migrados manualmente.</span><span class="sxs-lookup"><span data-stu-id="519a4-125">Profiles must be manually migrated.</span></span> <span data-ttu-id="519a4-126">Um perfil de utilizador contém informações como favoritos, ficheiros locais, definições do browser e menu Iniciar definições de utilizador.</span><span class="sxs-lookup"><span data-stu-id="519a4-126">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="519a4-127">A melhor abordagem é encontrar uma ferramenta de terceiros para mapear ficheiros e definições existentes para o novo perfil.</span><span class="sxs-lookup"><span data-stu-id="519a4-127">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="519a4-128">Se o dispositivo estiver a utilizar Objetos da Política de Grupo (GPO), alguns GPOs poderão não ter um Fornecedor de Serviços de [Configuração](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) comparável no Intune.</span><span class="sxs-lookup"><span data-stu-id="519a4-128">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="519a4-129">Execute [a ferramenta MMAT](https://www.microsoft.com/download/details.aspx?id=45520) para encontrar CSPs comparáveis para GPOs existentes.</span><span class="sxs-lookup"><span data-stu-id="519a4-129">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="519a4-130">Os utilizadores poderão não conseguir autenticar as aplicações que dependem da autenticação do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="519a4-130">Users might not be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="519a4-131">Avalie a aplicação legada e considere atualizar para uma aplicação que utilize a Auth moderna, se possível.</span><span class="sxs-lookup"><span data-stu-id="519a4-131">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="519a4-132">A deteção de impressoras do Active Directory não irá funcionar.</span><span class="sxs-lookup"><span data-stu-id="519a4-132">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="519a4-133">Pode fornecer caminhos diretos para a impressora a todos os utilizadores ou utilizar a [impressão universal.](/universal-print/)</span><span class="sxs-lookup"><span data-stu-id="519a4-133">You can provide direct printer paths for all users or use [Universal Print](/universal-print/).</span></span>

### <a name="related-articles"></a><span data-ttu-id="519a4-134">Artigos relacionados</span><span class="sxs-lookup"><span data-stu-id="519a4-134">Related Articles</span></span>

[<span data-ttu-id="519a4-135">Pré-requisitos para o Azure AD Ligação</span><span class="sxs-lookup"><span data-stu-id="519a4-135">Prerequisites for Azure AD Connect</span></span>](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)
