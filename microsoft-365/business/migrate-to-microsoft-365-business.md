---
title: Migrar para o Microsoft 365 Business do Office 365 Business Premium
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
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Saiba como mover sua empresa para o Microsoft 365 Business.
ms.openlocfilehash: a3f77bd18b9b900151c50f923b705e4ff0150519
ms.sourcegitcommit: 91ff1d4339f0f043c2b43997d87d84677c79e279
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2019
ms.locfileid: "36982447"
---
# <a name="migrate-to-microsoft-365-business-from-office-365-business-premium"></a>Migrar para o Microsoft 365 Business do Office 365 Business Premium

Se já tiver uma subscrição do Office 365 para empresas, por exemplo, Office 365 Business Premium, pode adicionar facilmente licenças ao Microsoft 365 Business e atribuí-las a algumas ou a todos os utilizadores.
  
> [!NOTE]
> Você não pode usar o botão de [planos de switch](https://support.office.com/article/73318661-8f33-478b-bcc7-fb8d69dbb22a?.aspx#switchbutton) para atualizar para o Microsoft 365 Business ainda. 
  
## <a name="add-microsoft-365-business-licenses"></a>Adicionar licenças do Microsoft 365 Business

Você tem duas maneiras de obter o Microsoft 365 Business. Um parceiro pode comprar o Microsoft 365 Business para você no [Microsoft Partner Center](get-microsoft-365-business.md). Seu parceiro também pode ajudá-lo a fazer a transição para o Microsoft 365 Business.
  
Se você gerenciar sua própria assinatura, poderá [entrar em contato com as vendas](https://www.microsoft.com/microsoft-365/business) para adquirir as licenças do Microsoft 365 Business. 
  
Consulte [Adicionar, alterar ou excluir um parceiro de conselheiro de assinatura](https://support.office.com/article/f86e8177-936e-491e-9024-44dea2b296ff) para descobrir como você pode começar a trabalhar com um parceiro. 
  
Se você for dado um link para comprar suas licenças, você vai percorrer um assistente como o abaixo. Escolha **Sim, adicioná-lo à minha conta**. Você também pode escolher o número de licenças e o método de pagamento.
  
![No link de compra direta do Microsoft 365 Business, opte por adicionar à sua conta atual ou Inscreva-se em uma nova conta.](media/8bc54fd1-9cab-44d5-af91-c471e89aea46.png)
  
## <a name="assign-microsoft-365-licenses"></a>Atribuir licenças do Microsoft 365

1. Depois de ter comprado novas licenças, e esta é a primeira vez que você fez, o banner de configuração para o Microsoft 365 Business será exibido na parte superior do centro de administração.
    
    > [!NOTE]
    > O banner de configuração é uma oportunidade para adicionar novos usuários, um novo domínio e migrar emails para novos usuários. Se você não planeja fazer qualquer, você ainda deve percorrer o assistente e escolher as opções padrão para fazê-lo desaparecer da home page do administrador. 
  
   ![Escolha Iniciar configuração no Microsoft 365 Business está pronto para configurar banner.](media/8d3b0d97-7cca-497f-9364-4b00ad670209.png)
  
    Selecione **Iniciar configuração**.
    
2. Na página **personalizar sua inscrição e email** , você pode adicionar um domínio escolhendo **conectar um domínio que você já possui** se quiser usar essa oportunidade para adicionar outro domínio à sua assinatura. 
    
    Se você já configurou um domínio, o segundo campo indicará que e dirá **continuar usando** \< _seu nome_ \> **de domínio para email e entrando**.   Se você não configurou um domínio com sua assinatura, ele dirá **continuar usando** \< _sua empresa Name.onmicrosoft.com_ \> **para e-mail e entrando**.  
    
    Selecione **Seguinte**.
    
    ![Na página personalizar sua inscrição e email, escolha Adicionar um domínio ou use o que você está usando.](media/c3f5cfb2-1189-4d2f-803b-c9feb008a7a3.png)
  
3. Na página **Adicionar novos usuários** , você pode adicionar novos usuários, se você tiver novos funcionários aos quais deseja atribuir as licenças do Microsoft 365 Business. 
    
    Se não tiver novos funcionários para adicionar e pretender atribuir licenças a utilizadores existentes, escolha **seguinte**.
    
4. Na página * * migrar mensagens de email * *, você pode optar por migrar emails para qualquer um dos novos usuários adicionados na etapa 3. Você pode pular esta etapa também. Selecione **Seguinte**.
    
5. Na última página, escolha **ir para o centro de administração**e continuar a configuração lá.
    
6. No centro de administração, **aceda a** \> utilizadores **activos**.
    
7. Selecione o usuário para o qual você deseja atribuir a licença de **negócios do Microsoft 365** e, em seguida, escolha **Editar** próximo a **licenças de produto**.
    
    ![No cartão de usuário, escolha Editar ao lado de licenças de produto.](media/be0fe2d8-7ff8-447c-88f6-d212ed78451c.png)
  
8. Em **licenças de produto** deslize **Microsoft 365 Business** **para** \> **salvar**e, em seguida, **feche**.
    
Depois de adquirir a licença inicial para o Microsoft 365 Business, agora você também pode adicionar mais em **** \> **serviços de compra**de faturamento. Na página de **serviços de compra** , você pode clicar nas reticências no cartão de visita do **Microsoft 365** e escolher **alterar a quantidade de licença** para comprar mais. 
  
## <a name="protect-user-devices-and-files"></a>Proteja os dispositivos e arquivos do usuário

Depois de atribuir licenças ao Microsoft 365 Business, você pode começar a proteger os dispositivos e arquivos dos usuários.
  
1. No centro de administração, no NAV esquerdo, vá para **políticas**de **dispositivos** \> .
    
2. Na página **diretivas de dispositivo** , escolha **Adicionar**.
    
3. No painel **Adicionar política** , dê um nome à política e escolha um tipo de **política** no menu suspenso. 
    
    Você pode configurar políticas de aplicativo para proteger arquivos em dispositivos Android e iPhone, bem como o Windows 10, e você pode configurar políticas de configuração de dispositivo para dispositivos Windows 10 de propriedade da empresa. Consulte os seguintes links para obter detalhes:
    
  - [Configurar as definições de proteção de aplicações para dispositivos Android ou iOS](app-protection-settings-for-android-and-ios.md)
    
  - [Configurar as definições de proteção de aplicações para dispositivos Windows 10](protection-settings-for-windows-10-devices.md)
    
  - [Definir configurações de proteção do dispositivo para PCs com Windows 10](protection-settings-for-windows-10-pcs.md)
    
   ![No painel Adicionar política, insira um nome para ele e escolha o tipo de política no menu suspenso.](media/76ef37e4-1d18-4f34-8a0f-391ab1d0ae2b.png)
  
4. Depois de configurar políticas, você e seus funcionários podem configurar dispositivos:
    
  - Se o Windows ainda não estiver na atualização do Windows pro Creator, será necessário [atualizá-los para a atualização do Windows pro Creators](upgrade-to-windows-pro-creators-update.md).
    
  - Consulte [configurar dispositivos Windows para usuários do Microsoft 365 Business](set-up-windows-devices.md) para obter as etapas para dispositivos Windows. 
    
  - Consulte [configurar dispositivos móveis para usuários do Microsoft 365 Business](set-up-mobile-devices.md) para obter as etapas para telefones e iPhones Android. 
    
5. Para instalar automaticamente aplicativos cliente do Office, consulte [preparar para implantação de cliente do Office pelo Microsoft 365 Business](prepare-for-office-client-deployment.md) e [instalar ou desinstalar automaticamente o Office em dispositivos Windows 10](auto-install-or-uninstall-office.md).
    


