---
title: Verificar definições de proteção de aplicações em PCs Windows 10
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Saiba como verificar se o Microsoft 365 para definições de proteção de aplicações empresariais entrou em vigor nos dispositivos Windows 10 dos seus utilizadores.
ms.openlocfilehash: 39aee3bc811cb0090d58f9a282de7a8162c097b3
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403596"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="f0061-103">Valide as definições de proteção do dispositivo em PCs do Windows 10</span><span class="sxs-lookup"><span data-stu-id="f0061-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="f0061-104">Verifique se as políticas do dispositivo Windows 10 estão definidas</span><span class="sxs-lookup"><span data-stu-id="f0061-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="f0061-105">Depois de configurar as políticas dos [dispositivos,](protection-settings-for-windows-10-pcs.md)pode demorar até algumas horas para que a política entre em vigor nos dispositivos dos utilizadores.</span><span class="sxs-lookup"><span data-stu-id="f0061-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="f0061-106">Pode confirmar que as políticas produziram efeito ao analisar vários ecrãs de Definições do Windows nos dispositivos dos utilizadores.</span><span class="sxs-lookup"><span data-stu-id="f0061-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="f0061-107">Uma vez que os utilizadores não conseguirão modificar as definições de Windows Update e Windows Defender Antivirus nos seus dispositivos Windows 10, muitas opções serão acinzentadas.</span><span class="sxs-lookup"><span data-stu-id="f0061-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="f0061-108">Vá às **opções** de reinício do Windows Update \> \*\* &amp; e\*\* \> **Windows Update** \> **Restart options** confirme que todas as definições estão acinzentadas.</span><span class="sxs-lookup"><span data-stu-id="f0061-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![Todas as opções de Reinício estão cinzentas.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="f0061-110">Vá a **Definições** \> **De &amp; segurança** \> As opções avançadas **do Windows Update** e \> **Advanced options** confirme que todas as definições estão acinzentadas.</span><span class="sxs-lookup"><span data-stu-id="f0061-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![As opções de atualizações do Windows Advanced estão todas cinzentas.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="f0061-112">Vá a **Definições** De atualização De \> \*\* &amp; atualização\*\* \> **As** \> **opções avançadas** do Windows \> **Escolha como as atualizações são entregues**.</span><span class="sxs-lookup"><span data-stu-id="f0061-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="f0061-113">Confirme que pode ver a mensagem (em vermelho) de que algumas configurações são ocultadas ou geridas pela sua organização, e todas as opções estão cinzentas.</span><span class="sxs-lookup"><span data-stu-id="f0061-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![Escolha como as atualizações são entregues a página indica que as definições são ocultadas ou geridas pela sua organização.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="f0061-115">Para abrir o Centro de Segurança do Windows Defender, vá a **Definições** \> **de &amp; segurança O** Windows \> **Defender** clique \> em **definições de** \> \*\* &amp; \*\* \> \*\* &amp; proteção\*\*contra vírus do Centro de Segurança do Windows Defender .</span><span class="sxs-lookup"><span data-stu-id="f0061-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="f0061-116">Verifique se todas as opções estão cinzentas.</span><span class="sxs-lookup"><span data-stu-id="f0061-116">Verify that all options are grayed out.</span></span> 
    
    ![As definições de proteção contra vírus e ameaças estão acinzentadas.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="f0061-118">Tópicos Relacionados</span><span class="sxs-lookup"><span data-stu-id="f0061-118">Related Topics</span></span>

[<span data-ttu-id="f0061-119">Microsoft 365 para documentação e recursos empresariais</span><span class="sxs-lookup"><span data-stu-id="f0061-119">Microsoft 365 for business documentation and resources</span></span>](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[<span data-ttu-id="f0061-120">Começar com a Microsoft 365 para negócios</span><span class="sxs-lookup"><span data-stu-id="f0061-120">Get started with Microsoft 365 for business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="f0061-121">Gerir o Microsoft 365 para negócios</span><span class="sxs-lookup"><span data-stu-id="f0061-121">Manage Microsoft 365 for business</span></span>](manage.md)
  
[<span data-ttu-id="f0061-122">Definir as configurações de dispositivos para PCs Windows 10</span><span class="sxs-lookup"><span data-stu-id="f0061-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  

