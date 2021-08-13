---
title: Editar ou criar definições de proteção de dispositivos para Windows 10 PCs
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
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: Saiba mais sobre as definições disponíveis no Microsoft 365 para empresas para proteger os Windows 10 dispositivos.
ms.openlocfilehash: b246a0caeb34bac8b9ccbecc9e1008992a700f9e16083a78c98e780605c5af01
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53809296"
---
# <a name="edit-or-create-device-protection-settings-for-windows-10-pcs"></a>Editar ou criar definições de proteção de dispositivos para Windows 10 PCs

Este artigo aplica-se a Microsoft 365 Empresas Premium.

Após configurar as definições de proteção Windows predefinição na página Configuração, pode adicionar novas definições que se aplicam a todos os utilizadores ou a um conjunto de utilizadores. Também pode editar qualquer uma das que criou.

## <a name="create-protection-settings-for-windows-10-devices"></a>Criar definições de proteção para Windows 10 dispositivos

Veja um vídeo sobre como proteger Windows 10 dispositivos com Microsoft 365 Empresas Premium:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. Vá para o centro de administração em <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> . 
2. No navegador esquerdo, selecionar Adicionar **Políticas** \> **de** \> **Dispositivos.**
3. No painel **Adicionar política**, introduza um nome exclusivo para esta política. 
4. Em **Tipo de política**, selecione **Configuração de Dispositivos Windows 10**.
5. Expanda a janela **Proteger Dispositivos Windows 10** \> configure as definições da forma que pretende. Para obter mais informações, consulte [Definições disponíveis.](#available-settings) 
    
    Pode sempre utilizar a ligação **Repor predefinições** para regressar à predefinição. 
    
    ![Add policy pane with Windows 10 Device configuration selected](../media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. Em seguida, decida **Quem irá ver estas definições?** Se não quiser utilizar o grupo de segurança predefinido, **Todos os Utilizadores**, selecione **Alterar**, procure o grupo de segurança que irá obter essas definições \> **Selecionar**.
7. Por fim, selecione **Concluído** para guardar a política e atribuí-la aos dispositivos. 

## <a name="edit-windows-10-protection-settings"></a>Editar Windows 10 de proteção dos ficheiros
 
1. Vá para o centro de administração em <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .     
2. No navegador esquerdo, selecionar Políticas **de** \> **Dispositivos** .
1. Escolha uma política de Windows dispositivo e, em seguida, **Editar**.
1. **Selecionar Editar** junto a uma definição que pretende alterar e, em seguida, **Guardar.**

## <a name="available-settings"></a>Definições disponíveis

Por predefinição, todas as definições estão **Ativadas**. As seguintes definições estão disponíveis.
  
Para obter mais informações, consulte [Como é que as funcionalidades de proteção Microsoft 365 Premium mapeiam às definições do Intune.](map-protection-features-to-intune-settings.md) 


|Definição  <br/> |Descrição  <br/> |
|:-----|:-----|
|Ajudar a proteger os PCs contra vírus e outras ameaças com o Antivírus do Windows Defender  <br/> |Exige que o Antivírus do Windows Defender esteja ativado para proteger os PCs contra os perigos que uma ligação à Internet envolve.  <br/> |
|Ajudar a proteger os PCs contra ameaças baseadas na Web no Microsoft Edge  <br/> |Ativa as definições no Microsoft Edge que ajudam a proteger os utilizadores contra transferências e sites maliciosos.  <br/> |
|Utilize regras que reduzam a superfície de ataque dos dispositivos  <br/> |Quando ativada, a redução da superfície de ataque ajuda a bloquear ações e aplicações normalmente utilizadas por software maligno para infetar dispositivos. Esta definição só está disponível se o Antivírus do Windows Defender estiver Ativado. Consulte [Reduzir superfícies de ataque](/windows/security/threat-protection/microsoft-defender-atp/exploit-protection) para saber mais.  <br/> |
|Proteger pastas contra ameaças como o ransomware  <br/> |Esta definição utiliza o acesso controlado a pastas para proteger os dados da empresa contra modificações de aplicações suspeitas e maliciosas, como o ransomware. Estes tipos de aplicações são impedidas de fazer alterações a pastas protegidas. Esta definição só está disponível se o Antivírus do Windows Defender estiver Ativado. Consulte [Proteger pastas com acesso controlado a pastas](/mem/configmgr/protect/deploy-use/create-deploy-exploit-guard-policy#bkmk_CFA) para saber mais.  <br/> |
|Impedir o acesso da rede a conteúdo potencialmente malicioso na Internet  <br/> |Utilize esta definição para bloquear as ligações de utilizadores de saída a localizações na Internet de baixa reputação que possam aloinhar esquemas de phishing, exploits ou outros conteúdos maliciosos. Esta definição só está disponível se a Antivírus do Windows Defender estiver definida para **Ação**. Para obter mais informações, consulte [Proteger a sua rede.](/windows/security/threat-protection/windows-defender-antivirus/configure-real-time-protection-windows-defender-antivirus)  <br/> |
|Ajudar a proteger ficheiros e pastas nos PCs contra acesso não autorizado com o BitLocker  <br/> |O Bitlocker protege os dados ao encriptar os discos rígidos do computador e proteger contra exposição de dados em caso de roubo ou perda do computador. Para obter mais informações, consulte [FAQ do Bitlocker.](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions)  <br/> |
|Permitir que os utilizadores transfiram aplicações da Microsoft Store  <br/> |Permite que os utilizadores transfiram e instalem aplicações da Microsoft Store. As aplicações incluem tudo, desde jogos a ferramentas de produtividade, pelo que deixamos esta definição **Ativada**, embora a possa desativar para garantir uma segurança adicional.  <br/> |
|Permitir que os utilizadores acedam à Cortana  <br/> |A Cortana pode ser bastante útil! Cortana ative ou deslige as definições por si, forneça direções e certifique-se  de que está a horas para os compromissos, pelo que mantemos esta definição Ative por predefinição.  <br/> |
|Permitir que os utilizadores recebam sugestões e anúncios da Microsoft acerca do Windows  <br/> |As sugestões do Windows podem ser úteis e ajudar a orientar os utilizadores quando são lançadas novas versões.  <br/> |
|Manter os dispositivos Windows 10 atualizados automaticamente  <br/> |Garante que os dispositivos Windows 10 recebem automaticamente as atualizações mais recentes.  <br/> |
|Desligar o ecrã do dispositivo quando estiver inativo durante este período de tempo  <br/> |Garante que os dados da empresa são protegidos se um utilizador estiver inativo. É possível que um utilizador esteja a trabalhar num local público, como um café, e se afaste ou distraia por um momento, deixando o dispositivo vulnerável a olhares alheios. Esta definição permite-lhe controlar quanto tempo um utilizador pode estar inativo antes de o ecrã se desligar.  <br/> |