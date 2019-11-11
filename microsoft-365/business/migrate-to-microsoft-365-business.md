---
title: Atualização para microsoft 365 negócios do Office 365 Business Premium
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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Etapas que atualizam seus negócios do Office 365 Business Premium para o Microsoft 365 Business.
ms.openlocfilehash: f3a25746cf123fa471c29084a62a6fcfc1542a02
ms.sourcegitcommit: f0a4290793e296474ecd3c6eb0ca96eae7faa434
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/11/2019
ms.locfileid: "38231417"
---
# <a name="upgrade-to-microsoft-365-business-from-office-365-business-premium"></a>Atualização para microsoft 365 negócios do Office 365 Business Premium

Se você tiver um [Office 365 para assinatura](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2)de negócios, por exemplo, o Office 365 Business Premium, você pode facilmente atualizar para o Microsoft 365 Business. Atualização para o Microsoft 365 Business se você quiser adicionar: 
- Windows 10 Pro (para PCs rodando o Windows 8 ou mais tarde)
- Controles simples que gerenciam dados de negócios em dispositivos
- Capacidades avançadas de segurança.
Saiba mais sobre o Microsoft 365 Business na [Microsoft.com](https://www.microsoft.com/microsoft-365/business)

## <a name="whats-the-difference-between-office-365-business-premium-and-microsoft-365-business"></a>Qual é a diferença entre o Office 365 Business Premium e o Microsoft 365 Business?
Adicionamos uma comparação lado a lado desses dois planos à descrição do [serviço Microsoft 365 Business.](https://docs.microsoft.com/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description) 

## <a name="before-you-get-started"></a>Antes de começar.

- **Quando devo escolher a atualização?** A atualização é a escolha certa quando você deseja atualizar **todos os usuários** designados para um único plano. Quando você escolhe a atualização, todos os usuários do plano são transferidos para outro plano ao mesmo tempo. Se você não quiser atualizar todos os designados para um único plano, compre licenças para o novo plano (neste caso, o Microsoft 365 Business) e [atribua essas licenças individualmente](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) a cada usuário que deseja atualizar. 
- **Alguns complementos podem impedir a atualização** Se você tentar iniciar uma atualização e você tem um complemento que impede que você continue, você pode remover o complemento primeiro e, em seguida, adicioná-lo de volta mais tarde - se você ainda precisar dele. 
- **Se você pagou antecipadamente o seu plano** Não há um caminho de atualização simples para planos pré-pagos. Você saberá se você tem um plano pré-pago porque configurou seu plano usando uma identificação do produto que você pode ter comprado em uma loja. Entre em contato com um parceiro, vá à loja da Microsoft ou espere até que seu plano pré-pago expire para mudar para um novo plano.

## <a name="upgrade-to-microsoft-365-business"></a>Atualização para o Microsoft 365 Business
Compre suas licenças seguindo estas etapas no centro novo do [admin:](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)
1. Entrar no centro de <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>administração em .
2. Vá para o painel de navegação e selecione **Produtos de faturamento** \> **& Serviços**. Encontre sua assinatura do Office 365 e selecione-a para visualizar os detalhes. 

    ![Uma captura de tela mostra como encontrar e selecionar sua assinatura no centro de administração.](media/FindYourSubscription.png)

3. Na próxima página, selecione **Atualização**. 

      ![Uma captura de tela mostra onde selecionar a atualização no centro de administração.](media/SelectUpgrade.png)

  > [!NOTE]
  > Se você ver uma mensagem que diz "Atualizar sua assinatura não é suportado com licenciamento baseado em grupo no Azure Active Directory", você pode ignorar isso com segurança, a menos que você tenha uma organização muito grande. As organizações que selecionaram essa opção estarão cientes de que estão usando o licenciamento baseado em grupo.

4. Em seguida, você pode visualizar uma lista de planos do Office para os os que pode atualizar. Neste caso, encontre o plano de negócios Microsoft 365. Você pode rolar para baixo se quiser ver todos os aplicativos e serviços do Office que estão incluídos neste plano. No **Microsoft 365 Business,** selecione **Atualização** para adicionar o Microsoft 365 Business ao seu carrinho.
5. No carrinho:
    1. Incluímos automaticamente licenças para todos os usuários atuais no carrinho. Se você precisar de mais, ou menos licenças, você precisará [comprar e atribuir essas licenças individualmente.](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users)  
    2. Você pode ajustar como você gostaria de pagar - mensal ou anualmente. Selecione o menu suspenso para fazer sua escolha.
6. Selecione **Ir para checkout** onde você verá um resumo de sua compra, incluindo o método de pagamento para esta conta. Você também pode adicionar um código promocional aqui se você tiver um.
7. Selecione **a ordem de lugar** para concluir sua compra.
A Microsoft leva alguns minutos para configurar seus novos planos de serviço. Para verificar o progresso, selecione o status de **atualização de verificação.** 
1. Uma vez que seu plano esteja pronto, talvez seja necessário concluir algumas etapas adicionais de configuração no centro de administração. No painel de navegação, selecione **Home** para completar quaisquer etapas adicionais de configuração.

> [!NOTE]
> Você receberá um reembolso proporcional para as licenças Ofifce 365 que você não precisa mais. Sua conta bancária ou cartão de crédito será cobrado cerca de dois dias depois de configurar o novo plano.
  
## <a name="protect-user-devices-and-files"></a>Proteger os dispositivos e arquivos do usuário

Agora que as licenças de negócios do Microsoft 365 foram atribuídas, sejam atribuídas etapas completas para começar a proteger dispositivos e arquivos. Você estará usando algumas novas opções incluídas no painel de navegação do centro de administração.
  
1. No centro de administração, no painel de navegação, vá para as Políticas de \> **Dispositivos.** ****
    
2. Na página de **políticas** do dispositivo, **selecione Adicionar**.
    
3. No painel de **política adicionar** dar a política de um nome (por exemplo, proteger arquivos de trabalho), e, em seguida, escolher um tipo de **política** a partir do drop-down. 
    
    Você pode configurar políticas de aplicativos para proteger arquivos em dispositivos Android e iPhone, bem como o Windows 10, e você pode configurar políticas de configuração de dispositivos para dispositivos Windows 10 de propriedade da empresa. Veja os seguintes links para detalhes:
    
  - [Configurar as definições de proteção de aplicações para dispositivos Android ou iOS](app-protection-settings-for-android-and-ios.md)
    
  - [Configurar as definições de proteção de aplicações para dispositivos Windows 10](protection-settings-for-windows-10-devices.md)
    
  - [Definir configurações de proteção do dispositivo para PCs do Windows 10](protection-settings-for-windows-10-pcs.md)
    
  
4. Depois de configurar políticas, você e seus funcionários podem configurar dispositivos:
    
  - Se os dispositivos Windows ainda não estiverem usando a atualização do Windows Pro Creator, precisará [atualizá-los para o Windows Pro Creators Update.](upgrade-to-windows-pro-creators-update.md)
    
  - Veja [configurar dispositivos Windows para usuários do Microsoft 365 Business](set-up-windows-devices.md) para etapas para dispositivos Windows. 
    
  - Veja [configurar dispositivos móveis para usuários do Microsoft 365 Business](set-up-mobile-devices.md) para etapas para telefones Android e iPhones. 



