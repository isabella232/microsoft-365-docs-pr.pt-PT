---
title: Validar as definições de proteção de aplicações Windows 10 PCs
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: Saiba como verificar se as Microsoft 365 de proteção de aplicações empresariais tomaram efeito nos dispositivos Windows 10 utilizadores.
ms.openlocfilehash: 464a246a0da65dcffeb70946287ce4fa0e67ae7c
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/14/2021
ms.locfileid: "52925265"
---
# <a name="validate-device-protection-settings-for-windows-10-pcs"></a><span data-ttu-id="65c8c-103">Validar as definições de proteção de dispositivos Windows 10 PCs</span><span class="sxs-lookup"><span data-stu-id="65c8c-103">Validate device protection settings for Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="65c8c-104">Verificar se as Windows 10 dispositivos estão definidas</span><span class="sxs-lookup"><span data-stu-id="65c8c-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="65c8c-105">Após [configurar as políticas de dispositivos,](protection-settings-for-windows-10-pcs.md)poderá demorar até algumas horas para que a política entre em vigor nos dispositivos dos utilizadores.</span><span class="sxs-lookup"><span data-stu-id="65c8c-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="65c8c-106">Pode confirmar que as políticas foram em vigor ao ver vários ecrãs Windows Definições ecrãs nos dispositivos dos utilizadores.</span><span class="sxs-lookup"><span data-stu-id="65c8c-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="65c8c-107">Uma vez que os utilizadores não poderão modificar as definições Windows Atualização Antivírus do Windows Defender dos respetivos dispositivos de Windows 10, muitas opções estarão a cinzento.</span><span class="sxs-lookup"><span data-stu-id="65c8c-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="65c8c-108">Vá para a **Definições** Opções de \> **&amp; Windows** Atualizar \>  \> **Reinício** e confirme que todas as definições estão a cinzento.</span><span class="sxs-lookup"><span data-stu-id="65c8c-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![Todas as opções de Reinício estão a cinzento.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="65c8c-110">Vá para o **Definições** \> **&amp; Atualizar segurança** Windows Atualizar opções Avançadas e confirme que todas as \>  \>  definições estão a cinzento.</span><span class="sxs-lookup"><span data-stu-id="65c8c-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![Windows As opções de atualizações avançadas estão todas a cinzento.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="65c8c-112">Vá para o **Definições** \> **Atualizar &amp; segurança Windows** Opções \> **de** \> **Atualização Avançadas** \> **Selecionar a forma como as atualizações são entregues**.</span><span class="sxs-lookup"><span data-stu-id="65c8c-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="65c8c-113">Confirme que consegue ver a mensagem (a vermelho) de que algumas definições estão ocultas ou geridas pela sua organização e de que todas as opções estão desa cinzento.</span><span class="sxs-lookup"><span data-stu-id="65c8c-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![Selecionar a forma como as atualizações são entregues indica que as definições estão ocultas ou geridas pela sua organização.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="65c8c-115">Para abrir o Centro de Windows Defender  de Segurança do Definições atualizar a segurança Windows Defender clique em Abrir Windows Defender definições de proteção contra vírus contra \> **&amp;** \>  \>  \> **&amp;** \> **&amp; ameaças** por thread do Centro de Segurança do Windows Defender .</span><span class="sxs-lookup"><span data-stu-id="65c8c-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="65c8c-116">Verifique se todas as opções estão a cinzento.</span><span class="sxs-lookup"><span data-stu-id="65c8c-116">Verify that all options are grayed out.</span></span> 
    
    ![As definições de proteção contra vírus e ameaças estão desa cinzento.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="65c8c-118">Tópicos Relacionados</span><span class="sxs-lookup"><span data-stu-id="65c8c-118">Related Topics</span></span>

[<span data-ttu-id="65c8c-119">Microsoft 365 para recursos e documentação empresarial</span><span class="sxs-lookup"><span data-stu-id="65c8c-119">Microsoft 365 for business documentation and resources</span></span>](./index.yml)
  
[<span data-ttu-id="65c8c-120">Começar a trabalhar com o Microsoft 365 para empresas</span><span class="sxs-lookup"><span data-stu-id="65c8c-120">Get started with Microsoft 365 for business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="65c8c-121">Gerir Microsoft 365 para empresas</span><span class="sxs-lookup"><span data-stu-id="65c8c-121">Manage Microsoft 365 for business</span></span>](manage.md)
  
[<span data-ttu-id="65c8c-122">Definir as configurações de dispositivos para PCs Windows 10</span><span class="sxs-lookup"><span data-stu-id="65c8c-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
