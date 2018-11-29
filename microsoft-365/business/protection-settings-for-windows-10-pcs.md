---
title: Configurar as definições de proteção de dispositivos para PCs Windows 10
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
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: Obter informações sobre a predefinição e outras definições disponíveis no Microsoft Business de 365 para proteger o Windows 10 dispositivos.
ms.openlocfilehash: ebfe5f59e544b67e5a4f2ecd990031e9221ff8e5
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982148"
---
# <a name="set-device-protection-settings-for-windows-10-pcs"></a>Configurar as definições de proteção de dispositivos para PCs Windows 10

## <a name="secure-windows-10-devices"></a>Proteger dispositivos Windows 10

Veja um vídeo sobre como proteger os dispositivos com Windows 10 com Microsoft 365 Business:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. Inicie sessão no [Microsoft 365 Business](https://portal.office.com) com as suas credenciais de administrador global. 
    
2. No centro de administração, no cartão **Políticas de dispositivos**, selecione **Adicionar política**.
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. No painel **Adicionar política**, introduza um nome exclusivo para esta política. 
    
4. Em **Tipo de política**, selecione **Configuração de Dispositivos Windows 10**.
    
5. Expanda a janela **Proteger Dispositivos Windows 10** \> configure as definições da forma que pretende. Consulte [Definições disponíveis](protection-settings-for-windows-10-pcs.md#bkmk_availablesettings) para obter mais informações. 
    
    Pode sempre utilizar a ligação **Repor predefinições** para regressar à predefinição. 
    
    ![Add policy pane with Windows 10 Device configuration selected](media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. Em seguida, decida **Quem irá ver estas definições?** Se não quiser utilizar o grupo de segurança predefinido, **Todos os Utilizadores**, selecione **Alterar**, procure o grupo de segurança que irá obter essas definições \> **Selecionar**.
    
7. Por fim, selecione **Concluído** para guardar a política e atribuí-la aos dispositivos. 
    
## <a name="available-settings"></a>Definições disponíveis

Por predefinição, todas as definições estão **Ativadas**. As seguintes definições estão disponíveis.
  
Consulte o artigo [Como é que as funcionalidades de proteção no Microsoft 365 Business são mapeadas às definições do Intune](map-protection-features-to-intune-settings.md) para obter mais informações. 
  
|||
|:-----|:-----|
|Definição  <br/> |Descrição  <br/> |
|Ajudar a proteger os PCs contra vírus e outras ameaças com o Antivírus do Windows Defender  <br/> |Exige que o Antivírus do Windows Defender esteja ativado para proteger os PCs contra os perigos que uma ligação à Internet envolve.  <br/> |
|Ajudar a proteger os PCs contra ameaças baseadas na Web no Microsoft Edge  <br/> |Ativa as definições no Microsoft Edge que ajudam a proteger os utilizadores contra transferências e sites maliciosos.  <br/> |
|Utilize regras que reduzam a superfície de ataque dos dispositivos  <br/> |Quando ativada, a redução da superfície de ataque ajuda a bloquear ações e aplicações normalmente utilizadas por software maligno para infetar dispositivos. Esta definição só está disponível se o Antivírus do Windows Defender estiver Ativado. Consulte [Reduzir superfícies de ataque](https://go.microsoft.com/fwlink/?linkid=870417) para saber mais.  <br/> |
|Proteger pastas contra ameaças como o ransomware  <br/> |Esta definição utiliza o acesso controlado a pastas para proteger os dados da empresa contra modificações de aplicações suspeitas e maliciosas, como o ransomware. Estes tipos de aplicações são impedidas de fazer alterações a pastas protegidas. Esta definição só está disponível se o Antivírus do Windows Defender estiver Ativado. Consulte [Proteger pastas com acesso controlado a pastas](https://go.microsoft.com/fwlink/?linkid=870418) para saber mais.  <br/> |
|Impedir o acesso da rede a conteúdo potencialmente malicioso na Internet  <br/> |Utilize esta definição para bloquear as ligações de utilizadores de saída a localizações na Internet de baixa reputação que possam alojar esquemas de phishing, exploits ou outros conteúdos maliciosos. Esta definição só está disponível se o Antivírus do Windows Defender estiver Ativado. Consulte [Proteger a sua rede](https://go.microsoft.com/fwlink/?linkid=870419) para obter mais informações.  <br/> |
|Ajudar a proteger ficheiros e pastas nos PCs contra acesso não autorizado com o BitLocker  <br/> |O Bitlocker protege os dados ao encriptar os discos rígidos do computador e proteger contra exposição de dados em caso de roubo ou perda do computador. Consulte as [FAQs do Bitlocker](https://go.microsoft.com/fwlink/?linkid=871000) para mais informações.  <br/> |
|Permitir que os utilizadores transfiram aplicações da Microsoft Store  <br/> |Permite que os utilizadores transfiram e instalem aplicações da Microsoft Store. As aplicações incluem tudo, desde jogos a ferramentas de produtividade, pelo que deixamos esta definição **Ativada**, embora a possa desativar para garantir uma segurança adicional.  <br/> |
|Permitir que os utilizadores acedam à Cortana  <br/> |A Cortana pode ser bastante útil! Ela pode ativar ou desativar definições automaticamente, dar indicações e certificar-se de que chega a tempo aos seus compromissos, pelo que esta opção é mantida **Ativada** por predefinição.  <br/> |
|Permitir que os utilizadores recebam sugestões e anúncios da Microsoft acerca do Windows  <br/> |As sugestões do Windows podem ser úteis e ajudar a orientar os utilizadores quando são lançadas novas versões.  <br/> |
|Manter os dispositivos Windows 10 atualizados automaticamente  <br/> |Garante que os dispositivos Windows 10 recebem automaticamente as atualizações mais recentes.  <br/> |
|Desligar o ecrã do dispositivo quando estiver inativo durante este período de tempo  <br/> |Garante que os dados da empresa são protegidos se um utilizador estiver inativo. É possível que um utilizador esteja a trabalhar num local público, como um café, e se afaste ou distraia por um momento, deixando o dispositivo vulnerável a olhares alheios. Esta definição permite-lhe controlar quanto tempo um utilizador pode estar inativo antes de o ecrã se desligar.  <br/> |
   
  

