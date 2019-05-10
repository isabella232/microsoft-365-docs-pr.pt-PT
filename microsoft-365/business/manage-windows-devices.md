---
title: Ativar a gestão, por parte do Microsoft 365 Business, de dispositivos associados ao domínio Windows 10
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Obter informações sobre como activar o Microsoft 365 proteger local AD associado Windows 10 dispositivos.
ms.openlocfilehash: 661e5bf8205a661eb4382b4bdd8fcf3a54ecc12f
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660354"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="4f764-103">Ativar a gestão, por parte do Microsoft 365 Business, de dispositivos associados ao domínio Windows 10</span><span class="sxs-lookup"><span data-stu-id="4f764-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="4f764-104">Se a organização utilizar o Windows Server Active Directory no local, pode configurar o Microsoft 365 Business para proteger os dispositivos Windows 10, mantendo o acesso a recursos locais que requerem autenticação local.</span><span class="sxs-lookup"><span data-stu-id="4f764-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="4f764-105">Pode configurar esta tarefa pela primeira sincronização do Active Directory com Azure Active Directory, seguido de registar os dispositivos de 10 de Windows Azure AD e inscrição-los para gestão do dispositivo móvel pelo Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="4f764-105">You can set this up by first synchronizing your Active Directory with Azure Active Directory, followed by registering the Windows 10 devices with Azure AD and enrolling them for mobile device management by Microsoft 365 Business.</span></span>
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="4f764-106">Configurar dispositivos de domínio a ser gerido pelo Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="4f764-106">Set up domain-joined devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="4f764-107">Para configurar dispositivos de domínio da organização para beneficiar as capacidades fornecidas pelo Azure Active Directory para além do Active Directory no local, pode implementar **híbrido Azure AD associado dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="4f764-107">To set up your organization's domain-joined devices to benefit from the capabilities provided by Azure Active Directory in addition to on-premises Active Directory, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="4f764-108">Estes são dispositivos que estão associados no local, Active Directory e o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4f764-108">These are devices that are joined both to your on-premises Active Directory and your Azure Active Directory.</span></span> <span data-ttu-id="4f764-109">Híbrido AD Azure associado dispositivos que podem ser protegidos e geridos pelo Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="4f764-109">Hybrid Azure AD joined devices can be protected and managed by Microsoft 365 Business.</span></span> 
  
<span data-ttu-id="4f764-110">Conclua os passos abaixo para certificar os dispositivos Windows 10 híbrido AD Azure associado e geridos pelo Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="4f764-110">Complete the steps below to make your Windows 10 devices Hybrid Azure AD joined and managed by Microsoft 365 Business.</span></span>
  
1. <span data-ttu-id="4f764-111">Para sincronizar a utilizadores, grupos e contactos a partir do Active Directory local do Active Directory Azure, execute o Assistente de sincronização de directório e Azure Active Directory ligar conforme descrito em [Configurar a sincronização de directório para o Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="4f764-111">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure Active Directory Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
    > [!NOTE]
    > <span data-ttu-id="4f764-112">Os passos são exactamente o mesmo para o Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="4f764-112">The steps are exactly the same for Microsoft 365 Business.</span></span> 
  
2. <span data-ttu-id="4f764-113">Antes de concluir o passo 3 para permitir que dispositivos Windows 10 ser híbrido Azure AD associado, tem de certificar-se de que cumpre os seguintes pré-requisitos:</span><span class="sxs-lookup"><span data-stu-id="4f764-113">Before you complete step 3 to enable Windows 10 devices to be Hybrid Azure AD joined, you need to make sure that you meet the following prerequisites:</span></span>

   - <span data-ttu-id="4f764-114">Tem a versão mais recente do Azure AD ligar.</span><span class="sxs-lookup"><span data-stu-id="4f764-114">You are running the latest version of Azure AD connect.</span></span>

   - <span data-ttu-id="4f764-115">Ligar Azure AD sincronizou todos os objectos de computador dos dispositivos que pretende ser híbrido Azure AD associado.</span><span class="sxs-lookup"><span data-stu-id="4f764-115">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined.</span></span> <span data-ttu-id="4f764-116">Se os objectos de computador pertencem a unidades organizacionais específicas (UO), em seguida, certifique-se que estes UOs são definidos para sincronização no Azure AD ligar bem.</span><span class="sxs-lookup"><span data-stu-id="4f764-116">If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>
    
3. <span data-ttu-id="4f764-117">Registe existentes associados ao domínio Windows 10 dispositivos ser híbrido Azure AD associado e inscrevê-los para gestão do dispositivo móvel pelo Intune (Microsoft 365 Business):</span><span class="sxs-lookup"><span data-stu-id="4f764-117">Register existing domain-joined Windows 10 devices to be hybrid Azure AD Joined and enroll them for mobile device management by Intune (Microsoft 365 Business):</span></span>
    
4. <span data-ttu-id="4f764-118">Siga as instruções passo a passo de [como configurar dispositivos de Azure do Active Directory associado híbrida](https://go.microsoft.com/fwlink/p/?linkid=872870).</span><span class="sxs-lookup"><span data-stu-id="4f764-118">Follow the step by step instructions in [How to configure hybrid Azure Active Directory joined devices](https://go.microsoft.com/fwlink/p/?linkid=872870).</span></span> <span data-ttu-id="4f764-119">Isto permitirá a sincronização do Active Directory no local associado a computadores Windows 10 e torná-los cloud preparado.</span><span class="sxs-lookup"><span data-stu-id="4f764-119">This will enable the synchronization of your on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
5. <span data-ttu-id="4f764-120">Para inscrever um dispositivo Windows 10 para a gestão do dispositivo móvel, consulte a [Inscrever-se um dispositivo Windows 10 com Intune, utilizando uma política de grupo](https://go.microsoft.com/fwlink/p/?linkid=872871) para obter instruções.</span><span class="sxs-lookup"><span data-stu-id="4f764-120">In order to enroll a Windows 10 device for mobile device management, see [Enroll a Windows 10 device with Intune by using a Group Policy](https://go.microsoft.com/fwlink/p/?linkid=872871) for instructions.</span></span> <span data-ttu-id="4f764-121">Pode definir a política de grupo no computador local nível ou para operações em massa, pode criar esta definição de política de grupo no seu servidor de controlador de domínio.</span><span class="sxs-lookup"><span data-stu-id="4f764-121">You can set the Group Policy at a local computer level or for bulk operations, you can create this group policy setting on your domain controller server.</span></span>