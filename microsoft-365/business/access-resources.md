---
title: Acesso local recursos a partir de um dispositivo associado AD Azure no Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Obter informações sobre como obter acesso a recursos no local, tais como aplicações de linha de negócios, partilhas de ficheiros e impressoras a partir de um Azure Active Directory associado Windows 10 dispositivo.
ms.openlocfilehash: 0a5d4b0828888fcb99676223000c446479f84ddc
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982258"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a><span data-ttu-id="9272b-103">Acesso local recursos a partir de um dispositivo associado AD Azure no Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="9272b-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>

<span data-ttu-id="9272b-p101">Qualquer dispositivo Windows 10 Azure do Active Directory associado terão acesso a todos os recursos baseada na nuvem, tais como as suas aplicações do Office 365 e pode ser protegido por negócio do Microsoft 365. Para também permitir o acesso a recursos no local, como aplicações, partilhas de ficheiros e impressoras de linha de negócio (LOB), terá de sincronizar no local, Active Directory com o Active Directory de Azure utilizando [Azure AD ligar](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect). Consulte [Introdução à gestão de dispositivos no Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="9272b-p101">Any Windows 10 device that is Azure Active Directory joined will have access to all cloud-based resources such as your Office 365 apps and can be protected by Microsoft 365 Business. To also allow access to on-premises resources like Line Of Business (LOB) apps, file shares, and printers, you must synchronize your on-premises Active Directory with Azure Active Directory by using [Azure AD Connect](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect). See [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) to learn more.</span></span> 
  
## <a name="run-azure-ad-connect"></a><span data-ttu-id="9272b-107">Executar Azure AD ligar</span><span class="sxs-lookup"><span data-stu-id="9272b-107">Run Azure AD Connect</span></span>

<span data-ttu-id="9272b-108">Conclua os seguintes passos para activar dispositivos de AD Azure associado da organização aceder a recursos no local.</span><span class="sxs-lookup"><span data-stu-id="9272b-108">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="9272b-109">Para sincronizar a utilizadores, grupos e contactos a partir do Active Directory local do Active Directory Azure, execute o Assistente de sincronização de directório e Azure AD ligar, como descrito em [Configurar a sincronização de directório para o Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="9272b-109">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
2. <span data-ttu-id="9272b-p102">Depois de concluída a sincronização de directório, certifique-se Windows 10 dispositivos da sua organização são AD Azure associado. Este passo é efectuado individualmente em cada dispositivo do Windows 10. Consulte [Configurar dispositivos do Windows para utilizadores empresariais do Microsoft 365](set-up-windows-devices.md) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="9272b-p102">After the directory synchronization has completed, make sure your organization's Windows 10 devices are Azure AD joined. This step is done individually on each Windows 10 device. See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="9272b-p103">Depois dos dispositivos de 10 de Windows Azure AD associado, cada utilizador deverá reiniciar os dispositivos e o início de sessão com as respectivas credenciais de Microsoft 365 Business. Todos os dispositivos terão agora acesso aos recursos do local bem.</span><span class="sxs-lookup"><span data-stu-id="9272b-p103">Once the Windows 10 devices are Azure AD joined, each user should reboot their devices and login with their Microsoft 365 Business credentials. All devices will now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="9272b-p104">Não existem passos adicionais são necessários para aceder a recursos para Azure AD associado dispositivos no local. Esta é a funcionalidade incorporada disponível no Windows 10.</span><span class="sxs-lookup"><span data-stu-id="9272b-p104">No additional steps are required to get access to on-premise resources for Azure AD joined devices. This is built-in functionality available in Windows 10.</span></span> 
  
<span data-ttu-id="9272b-117">Se a organização não estiver preparada para implementar na Azure AD associado dispositivo configuração acima descrito, considere a definição de [configuração do dispositivo híbrido Azure AD associado](manage-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="9272b-117">If your organization is not ready to deploy in the Azure AD Joined Device Configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a><span data-ttu-id="9272b-118">Considerações sobre quando colocar os dispositivos Windows Azure AD</span><span class="sxs-lookup"><span data-stu-id="9272b-118">Considerations when joining your Windows devices to Azure AD</span></span>

<span data-ttu-id="9272b-119">Se estiver AD Azure aderir a um dispositivo do Windows que foi anteriormente associados ao domínio ou num grupo de trabalho, terá de considerar as seguintes limitações:</span><span class="sxs-lookup"><span data-stu-id="9272b-119">If you are Azure AD joining a Windows device that has previously been domain-joined or in a workgroup, you need to consider the following limitations:</span></span>
  
- <span data-ttu-id="9272b-p105">Quando adere a um dispositivo Azure AD, cria um novo utilizador sem fazer referência um perfil existente. Para corrigir este problema, perfis tem de ser migrados manualmente. Um perfil de utilizador contém informações como favoritos, ficheiros locais, as definições do browser, definições do menu Iniciar, etc. Uma abordagem melhor será localizar uma ferramenta de outros fabricantes para mapear os ficheiros existentes e as definições para o novo perfil</span><span class="sxs-lookup"><span data-stu-id="9272b-p105">When a device Azure AD joins, it creates a new user without referencing an existing profile. To fix this, profiles need to be manually migrated. A user profile contains information like favorites, local files, browser settings, Start menu settings, etc. A best approach is to find a third-party tool to map existing files and settings to the new profile</span></span>
    
- <span data-ttu-id="9272b-p106">Se o dispositivo estiver a utilizar objectos de política de grupo (GPO), alguns GPOs poderão não ter um comparáveis [Configuração Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) no Intune. Execute a [ferramenta MMAT](https://www.microsoft.com/download/details.aspx?id=45520) para localizar os CSPs comparáveis para os GPOs existentes.</span><span class="sxs-lookup"><span data-stu-id="9272b-p106">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune. Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span> 
    
- <span data-ttu-id="9272b-p107">Os utilizadores não conseguirão autenticar para aplicações que dependem de autenticação do Active Directory. Para lidar com avaliar a utilização de uma aplicação de legacy e considere a hipótese de actualizar para uma aplicação que utiliza autenticação moderna se possível.</span><span class="sxs-lookup"><span data-stu-id="9272b-p107">Users will not be able to authenticate to applications that depend on Active Directory authentication. To deal with this evaluate using a legacy app and consider updating to an app that uses modern Auth if possible.</span></span>
    
- <span data-ttu-id="9272b-p108">Detecção de impressora do Active Directory não irá funcionar. Para corrigir este problema, forneça caminhos directa de impressora para todos os utilizadores ou tirar partido de [Impressão de nuvem de híbridos](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span><span class="sxs-lookup"><span data-stu-id="9272b-p108">Active Directory printer discovery will not work. To fix this, provide direct printer paths for all users or leverage [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
    

