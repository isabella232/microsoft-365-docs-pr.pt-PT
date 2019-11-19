---
title: Configurar as definições de proteção de dispositivos para PCs Windows 10
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
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: Saiba mais sobre o padrão e outras configurações disponíveis no Microsoft 365 Business para proteger os dispositivos Windows 10.
ms.openlocfilehash: 1846ee7ae09db94575ef27dcf4f5721661f7666d
ms.sourcegitcommit: 5d11f516e78ea4a74145e19ba2300f0792c8bac1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/19/2019
ms.locfileid: "38715208"
---
# <a name="set-device-protection-settings-for-windows-10-pcs"></a>Configurar as definições de proteção de dispositivos para PCs Windows 10

## <a name="secure-windows-10-devices"></a>Proteger dispositivos Windows 10

Veja um vídeo sobre como proteger os dispositivos com Windows 10 com Microsoft 365 Business:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. Vá para o centro <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>de administração em . 
    
2. No nav esquerdo, escolha **políticas** \> dos **dispositivos** \> **adicione.**
  
3. No painel **Adicionar política**, introduza um nome exclusivo para esta política. 
    
4. Em **Tipo de política**, selecione **Configuração de Dispositivos Windows 10**.
    
5. Expanda a janela **Proteger Dispositivos Windows 10** \> configure as definições da forma que pretende. Para mais informações, consulte [as configurações disponíveis.](#available-settings) 
    
    Pode sempre utilizar a ligação **Repor predefinições** para regressar à predefinição. 
    
    ![Add policy pane with Windows 10 Device configuration selected](media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. Em seguida, decida **Quem irá ver estas definições?** Se não quiser utilizar o grupo de segurança predefinido, **Todos os Utilizadores**, selecione **Alterar**, procure o grupo de segurança que irá obter essas definições \> **Selecionar**.
    
7. Por fim, selecione **Concluído** para guardar a política e atribuí-la aos dispositivos. 
    
## <a name="available-settings"></a>Definições disponíveis

Por predefinição, todas as definições estão **Ativadas**. As seguintes definições estão disponíveis.
  
Para obter mais informações, consulte [Como é que as funcionalidades de proteção no Microsoft 365 Empresas são mapeadas para as definições do Intune](map-protection-features-to-intune-settings.md). 
  
|||
|:-----|:-----|
|Definição  <br/> |Descrição  <br/> |
|Ajudar a proteger os PCs contra vírus e outras ameaças com o Antivírus do Windows Defender  <br/> |Exige que o Antivírus do Windows Defender esteja ativado para proteger os PCs contra os perigos que uma ligação à Internet envolve.  <br/> |
|Ajudar a proteger os PCs contra ameaças baseadas na Web no Microsoft Edge  <br/> |Ativa as definições no Microsoft Edge que ajudam a proteger os utilizadores contra transferências e sites maliciosos.  <br/> |
|Utilize regras que reduzam a superfície de ataque dos dispositivos  <br/> |Quando ativada, a redução da superfície de ataque ajuda a bloquear ações e aplicações normalmente utilizadas por software maligno para infetar dispositivos. Esta definição só está disponível se o Antivírus do Windows Defender estiver Ativado. Consulte [Reduzir superfícies de ataque](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/exploit-protection) para saber mais.  <br/> |
|Proteger pastas contra ameaças como o ransomware  <br/> |Esta definição utiliza o acesso controlado a pastas para proteger os dados da empresa contra modificações de aplicações suspeitas e maliciosas, como o ransomware. Estes tipos de aplicações são impedidas de fazer alterações a pastas protegidas. Esta definição só está disponível se o Antivírus do Windows Defender estiver Ativado. Veja [as pastas Protect com acesso](https://docs.microsoft.com/configmgr/protect/deploy-use/create-deploy-exploit-guard-policy#bkmk_CFA) de pasta controlada para saber mais.  <br/> |
|Impedir o acesso da rede a conteúdo potencialmente malicioso na Internet  <br/> |Use essa configuração para bloquear conexões de ida de usuário s locais de Internet de baixa reputação que podem hospedar golpes de phishing, explorações ou outros conteúdos maliciosos. Esta configuração só está disponível se o Antivírus Defensor do Windows estiver definido para **on.** Para mais informações, [consulte proteger sua rede](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/configure-real-time-protection-windows-defender-antivirus).  <br/> |
|Ajudar a proteger ficheiros e pastas nos PCs contra acesso não autorizado com o BitLocker  <br/> |O Bitlocker protege os dados ao encriptar os discos rígidos do computador e proteger contra exposição de dados em caso de roubo ou perda do computador. Para mais informações, consulte [bitlocker FAQ](https://go.microsoft.com/fwlink/?linkid=871000).  <br/> |
|Permitir que os utilizadores transfiram aplicações da Microsoft Store  <br/> |Permite que os utilizadores transfiram e instalem aplicações da Microsoft Store. As aplicações incluem tudo, desde jogos a ferramentas de produtividade, pelo que deixamos esta definição **Ativada**, embora a possa desativar para garantir uma segurança adicional.  <br/> |
|Permitir que os utilizadores acedam à Cortana  <br/> |A Cortana pode ser bastante útil! Cortana pode ativar ou desligar as configurações para você, dar instruções e certificar-se de que você está na hora de compromissos, por isso mantemos essa **configuração** por padrão.  <br/> |
|Permitir que os utilizadores recebam sugestões e anúncios da Microsoft acerca do Windows  <br/> |As sugestões do Windows podem ser úteis e ajudar a orientar os utilizadores quando são lançadas novas versões.  <br/> |
|Manter os dispositivos Windows 10 atualizados automaticamente  <br/> |Garante que os dispositivos Windows 10 recebem automaticamente as atualizações mais recentes.  <br/> |
|Desligar o ecrã do dispositivo quando estiver inativo durante este período de tempo  <br/> |Garante que os dados da empresa são protegidos se um utilizador estiver inativo. É possível que um utilizador esteja a trabalhar num local público, como um café, e se afaste ou distraia por um momento, deixando o dispositivo vulnerável a olhares alheios. Esta definição permite-lhe controlar quanto tempo um utilizador pode estar inativo antes de o ecrã se desligar.  <br/> |
