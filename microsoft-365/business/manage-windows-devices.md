---
title: Ativar a gestão, por parte do Microsoft 365 Business, de dispositivos associados ao domínio Windows 10
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
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Saiba como habilitar o Microsoft 365 para proteger dispositivos do Windows 10 ingressados no AD local.
ms.openlocfilehash: 5cce4bc53f118560e31ad7e6048e4efcb49d662e
ms.sourcegitcommit: c0f769244d05ad019ea2307c38d5543d7b1e5afd
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992235"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="ca465-103">Ativar a gestão, por parte do Microsoft 365 Business, de dispositivos associados ao domínio Windows 10</span><span class="sxs-lookup"><span data-stu-id="ca465-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="ca465-104">Se sua organização usa o Active Directory do Windows Server no local, você pode configurar o Microsoft 365 Business para proteger seus dispositivos Windows 10, enquanto ainda mantém o acesso a recursos locais que exigem autenticação local.</span><span class="sxs-lookup"><span data-stu-id="ca465-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="ca465-105">Você pode configurá-lo sincronizando primeiro o Active Directory com o Azure Active Directory, seguido de registrar os dispositivos Windows 10 com o Azure AD e inscrevendo-os para o gerenciamento de dispositivos móveis pelo Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="ca465-105">You can set this up by first synchronizing your Active Directory with Azure Active Directory, followed by registering the Windows 10 devices with Azure AD and enrolling them for mobile device management by Microsoft 365 Business.</span></span>
<span data-ttu-id="ca465-106">O vídeo a seguir detalha as etapas de como configurá-lo para o cenário mais comum.</span><span class="sxs-lookup"><span data-stu-id="ca465-106">The following video details the steps for how to set this up for the most common scenario.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="ca465-107">Configurar dispositivos ingressados no domínio a serem gerenciados pelo Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="ca465-107">Set up domain-joined devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="ca465-108">Para configurar os dispositivos ingressados no domínio da sua organização para se beneficiarem dos recursos fornecidos pelo Azure Active Directory, além do Active Directory local, você pode implementar **dispositivos ingressados no Azure ad híbridos**.</span><span class="sxs-lookup"><span data-stu-id="ca465-108">To set up your organization's domain-joined devices to benefit from the capabilities provided by Azure Active Directory in addition to on-premises Active Directory, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="ca465-109">Estes são dispositivos que estão associados ao Active Directory no local e ao Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ca465-109">These are devices that are joined both to your on-premises Active Directory and your Azure Active Directory.</span></span> <span data-ttu-id="ca465-110">Os dispositivos ingressados no Azure AD híbridos podem ser protegidos e gerenciados pelo Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="ca465-110">Hybrid Azure AD joined devices can be protected and managed by Microsoft 365 Business.</span></span> 
  
<span data-ttu-id="ca465-111">Conclua as etapas abaixo para tornar seus dispositivos Windows 10 híbridos do Azure AD ingressados e gerenciados pelo Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="ca465-111">Complete the steps below to make your Windows 10 devices Hybrid Azure AD joined and managed by Microsoft 365 Business.</span></span>
  
1. <span data-ttu-id="ca465-112">Para sincronizar seus usuários, grupos e contatos do Active Directory local no Active Directory do Azure, execute o assistente de sincronização de diretórios e o Azure Active Directory Connect, conforme descrito em [Configurar a sincronização de diretórios para o Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="ca465-112">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure Active Directory Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
    > [!NOTE]
    > <span data-ttu-id="ca465-113">As etapas são exatamente as mesmas para o Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="ca465-113">The steps are exactly the same for Microsoft 365 Business.</span></span> 
  
2. <span data-ttu-id="ca465-114">Antes de concluir a etapa 3 para permitir que os dispositivos Windows 10 sejam ingressados no Azure AD híbrido, você precisa certificar-se de que atende aos seguintes pré-requisitos:</span><span class="sxs-lookup"><span data-stu-id="ca465-114">Before you complete step 3 to enable Windows 10 devices to be Hybrid Azure AD joined, you need to make sure that you meet the following prerequisites:</span></span>

   - <span data-ttu-id="ca465-115">Você está executando a versão mais recente do Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="ca465-115">You are running the latest version of Azure AD connect.</span></span>

   - <span data-ttu-id="ca465-116">O Azure AD Connect sincronizou todos os objetos de computador dos dispositivos que você deseja que sejam ingressados no Azure AD híbrido.</span><span class="sxs-lookup"><span data-stu-id="ca465-116">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined.</span></span> <span data-ttu-id="ca465-117">Se os objetos de computador pertencerem a unidades organizacionais específicas (UO), certifique-se de que essas OUs estão definidas para sincronização no Azure AD conectar também.</span><span class="sxs-lookup"><span data-stu-id="ca465-117">If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>
    
3. <span data-ttu-id="ca465-118">Registre dispositivos existentes do Windows 10 ingressados no domínio para ser híbrido do Azure AD ingressado e inscrevê-los para gerenciamento de dispositivos móveis pelo Intune (Microsoft 365 Business):</span><span class="sxs-lookup"><span data-stu-id="ca465-118">Register existing domain-joined Windows 10 devices to be hybrid Azure AD Joined and enroll them for mobile device management by Intune (Microsoft 365 Business):</span></span>
    
4. <span data-ttu-id="ca465-119">Siga as instruções passo a passo em [como configurar os dispositivos ingressados no Azure Active Directory híbrido](https://go.microsoft.com/fwlink/p/?linkid=872870).</span><span class="sxs-lookup"><span data-stu-id="ca465-119">Follow the step by step instructions in [How to configure hybrid Azure Active Directory joined devices](https://go.microsoft.com/fwlink/p/?linkid=872870).</span></span> <span data-ttu-id="ca465-120">Isso permitirá a sincronização de seu Active Directory local ingressado em computadores com Windows 10 e disponibilizá-los na nuvem.</span><span class="sxs-lookup"><span data-stu-id="ca465-120">This will enable the synchronization of your on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
5. <span data-ttu-id="ca465-121">Para inscrever um dispositivo Windows 10 para gerenciamento de dispositivos móveis, consulte [inscrever um dispositivo Windows 10 com o Intune usando uma política de grupo](https://go.microsoft.com/fwlink/p/?linkid=872871) para obter instruções.</span><span class="sxs-lookup"><span data-stu-id="ca465-121">In order to enroll a Windows 10 device for mobile device management, see [Enroll a Windows 10 device with Intune by using a Group Policy](https://go.microsoft.com/fwlink/p/?linkid=872871) for instructions.</span></span> <span data-ttu-id="ca465-122">Você pode definir a diretiva de grupo em um nível de computador local ou para operações em massa, você pode criar essa configuração de diretiva de grupo no seu servidor de controlador de domínio.</span><span class="sxs-lookup"><span data-stu-id="ca465-122">You can set the Group Policy at a local computer level or for bulk operations, you can create this group policy setting on your domain controller server.</span></span>