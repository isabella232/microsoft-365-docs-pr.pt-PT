---
title: Verificar definições de proteção de aplicações em PCs Windows 10
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
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Obter informações sobre como validar as definições de protecção de aplicações Microsoft 365 Business Windows 10 dispositivos.
ms.openlocfilehash: 15c2d54c6281369875d15985c9d4ed16f0114176
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/15/2019
ms.locfileid: "34072243"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="bfa1e-103">Validar as definições de protecção do dispositivo no Windows 10 PCs</span><span class="sxs-lookup"><span data-stu-id="bfa1e-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="bfa1e-104">Certifique-se de que estão definidas políticas de dispositivo do Windows 10</span><span class="sxs-lookup"><span data-stu-id="bfa1e-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="bfa1e-105">Depois de [configurar as políticas de dispositivos](protection-settings-for-windows-10-pcs.md), poderá demorar até algumas horas para a política em vigor em dispositivos de utilizadores.</span><span class="sxs-lookup"><span data-stu-id="bfa1e-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="bfa1e-106">Pode confirmar que as políticas de entrada em vigor, observando vários ecrãs de definições do Windows em dispositivos dos utilizadores.</span><span class="sxs-lookup"><span data-stu-id="bfa1e-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="bfa1e-107">Uma vez que os utilizadores não será possível modificar as definições do Windows Update e Windows Defender Antivirus nos respectivos dispositivos Windows 10, muitas dessas opções serão cinzento.</span><span class="sxs-lookup"><span data-stu-id="bfa1e-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, a lot of those options will be greyed out.</span></span>
  
1. <span data-ttu-id="bfa1e-108">Vá para **Definições** \> **Update &amp; segurança** \> **Windows Update** \> **Opções de reinício** e confirmar que todas as definições são cinzento.</span><span class="sxs-lookup"><span data-stu-id="bfa1e-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are greyed out.</span></span> 
    
    ![Todas as opções de reinício estão a cinzento.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="bfa1e-110">Vá para **Definições** \> **Update &amp; segurança** \> **Windows Update** \> **Opções avançadas** e confirme que todas as definições são cinzento.</span><span class="sxs-lookup"><span data-stu-id="bfa1e-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are greyed out.</span></span> 
    
    ![Opções das actualizações do Windows Advanced são todos cinzento.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="bfa1e-112">Vá para **Definições** \> **Update &amp; segurança** \> **Windows Update** \> **Opções avançadas de** \> **Escolher a forma como as actualizações são fornecidas**.</span><span class="sxs-lookup"><span data-stu-id="bfa1e-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="bfa1e-113">Confirme que pode vir a mensagem (em vermelho) que algumas definições estiverem ocultas ou geridas pela sua organização e todas as opções são cinzento.</span><span class="sxs-lookup"><span data-stu-id="bfa1e-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are greyed out.</span></span>
    
    ![Escolher a forma como as actualizações são fornecidas página indica as definições estiverem ocultas ou geridas pela sua organização.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="bfa1e-115">Para abrir o Centro de segurança do Windows Defender, vá para **Definições** \> **Update &amp; segurança** \> **O Windows Defender** \> clique em **Abrir o Centro de segurança Windows Defender** \> **Virus &amp; thread protecção** \> **Virus &amp; as definições de protecção de ameaças**.</span><span class="sxs-lookup"><span data-stu-id="bfa1e-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="bfa1e-116">Certifique-se de que todas as opções são cinzento.</span><span class="sxs-lookup"><span data-stu-id="bfa1e-116">Verify that all options are greyed out.</span></span> 
    
    ![As definições de protecção contra vírus e ameaças estão a cinzento.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="bfa1e-118">Tópicos relacionados</span><span class="sxs-lookup"><span data-stu-id="bfa1e-118">Related Topics</span></span>

[<span data-ttu-id="bfa1e-119">Recursos e documentação do Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="bfa1e-119">Microsoft 365 Business documentation and resources</span></span>](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[<span data-ttu-id="bfa1e-120">Introdução ao Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="bfa1e-120">Get started with Microsoft 365 Business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="bfa1e-121">Gerir o Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="bfa1e-121">Manage Microsoft 365 Business</span></span>](manage.md)
  
[<span data-ttu-id="bfa1e-122">Definir as configurações de dispositivos para PCs Windows 10</span><span class="sxs-lookup"><span data-stu-id="bfa1e-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  

