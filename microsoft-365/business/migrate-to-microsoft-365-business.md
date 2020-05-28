---
title: Upgrade para Microsoft 365 Business Premium da Microsoft 365 Business Standard
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
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Saiba a diferença entre o Microsoft 365 Business Standard e o Microsoft 365 Business Premium e como pode fazer upgrade para o Microsoft 365 Business Premium.
ms.openlocfilehash: bdab8165623170926b17efa4cae9408b78a2f5f5
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/27/2020
ms.locfileid: "44401388"
---
# <a name="upgrade-to-microsoft-365-business-premium-from-microsoft-365-business-standard"></a>Upgrade para Microsoft 365 Business Premium da Microsoft 365 Business Standard

Se tiver um [Microsoft 365 para subscrição](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2)de negócios , por exemplo, o Microsoft 365 Business Standard, pode facilmente fazer o upgrade para o Microsoft 365 Business Premium. Upgrade para Microsoft 365 Business Premium se quiser adicionar:

- Windows 10 Pro (para PCs que executam o Windows 8 ou mais tarde)

- Controlos simples que gerem dados empresariais em dispositivos

- Capacidades de segurança avançadas.
Saiba mais sobre o Microsoft 365 Business Premium em [Microsoft.com](https://www.microsoft.com/microsoft-365/business)

## <a name="whats-the-difference-between-microsoft-365-business-standard-and-microsoft-365-business-premium"></a>Qual é a diferença entre o Microsoft 365 Business Standard e o Microsoft 365 Business Premium?

Adicionámos uma comparação lado a lado destes dois planos à Descrição do [Serviço Premium Empresarial Microsoft 365.](https://docs.microsoft.com/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description) 

## <a name="before-you-get-started"></a>Antes de começar.

- **Quando devo escolher fazer upgrade?** O upgrade é a escolha certa quando pretende atualizar **todos os utilizadores atribuídos** a um único plano. Ao optar pela atualização, todos os utilizadores do plano são transferidos para outro plano ao mesmo tempo. Se não quiser atualizar todos os atribuídos a um único plano, compre licenças para o novo plano (neste caso, microsoft 365 Business Premium), e [atribua essas licenças individualmente](../admin/manage/assign-licenses-to-users.md) a cada utilizador que pretenda fazer upgrade.

- **Alguns addons podem impedir a atualização** Se tentar iniciar uma atualização e tiver um addon que o impeça de continuar, pode remover primeiro o addon e, em seguida, adicioná-lo de volta mais tarde se ainda precisar.

- **Se pagou o seu plano de pré-pagamento** Não há um caminho simples de atualização para planos pré-pagos. Saberá se tem um plano pré-pago porque configura o seu plano usando uma identificação de produto que pode ter comprado numa loja. Contacte um parceiro, vá à Microsoft Store ou espere até que o seu plano pré-pago expire para mudar para um novo plano.

## <a name="upgrade-to-microsoft-365-business-premium"></a>Upgrade para Microsoft 365 Business Premium

1. Assine no centro de administração em <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .

2. Vá ao painel de navegação e selecione **Billing** \> **Os seus produtos**. Encontre a subscrição atual e selecione-a para ver os detalhes.

3. Na página seguinte, selecione **Upgrade**.

  > [!NOTE]
  > Se vir uma mensagem que diga que atualizar a **sua subscrição não é suportado com licenciamento baseado em grupo no Azure Ative Directory,** pode ignorá-lo com segurança a menos que tenha uma organização muito grande. As organizações que escolheram esta opção estarão cientes de que estão a usar o licenciamento baseado em grupo.

4. Em seguida, pode ver uma lista de planos para os seus planos. Neste caso, encontre o plano Microsoft 365 Business Premium. Pode deslocar-se para baixo se quiser ver todas as aplicações e serviços que estão incluídos neste plano. No **Microsoft 365 Business Premium,** selecione **Upgrade** para adicionar o Microsoft 365 Business Premium ao seu carrinho.

5. No carrinho:

    1. Vamos automaticamente incluir licenças para todos os seus utilizadores atuais. Se precisar de mais ou menos licenças, tem de [comprar e atribuir essas licenças individualmente](../admin/manage/assign-licenses-to-users.md).  
    2. Pode ajustar a forma como gostaria de pagar: mensal ou anualmente. Selecione o menu suspenso para fazer a sua escolha.

6. Selecione **Ir ao Checkout** onde verá um resumo da sua compra, incluindo o método de pagamento desta conta. Também pode adicionar um código promocional aqui se tiver um.

7. Selecione **O pedido de lugar** para completar a sua compra.\
A Microsoft leva alguns minutos para configurar os seus novos planos de serviço. Para verificar o progresso, selecione Verifique o estado da **atualização**.

8. Quando o seu plano estiver pronto, poderá ter de completar alguns passos adicionais de configuração no centro de administração. No painel de navegação, selecione **Casa** para completar quaisquer passos adicionais de configuração.

> [!NOTE]
> Receberá um reembolso prostrado pelas licenças microsoft 365 de que já não precisa. A sua conta bancária ou cartão de crédito será cobrada cerca de dois dias após a configuração do novo plano.
  
## <a name="protect-user-devices-and-files"></a>Proteja os dispositivos e ficheiros do utilizador

Agora que foram atribuídas licenças Microsoft 365 Business Premium, completam as etapas para começar a proteger dispositivos e ficheiros. Você usará algumas novas opções incluídas no painel de navegação do centro de administração.
  
1. No centro de administração, no painel de navegação, vá para as Políticas de **Dispositivos** \> **Policies**.

2. Na página de políticas do **Dispositivo,** selecione **Adicionar**.

3. No painel de **política Add** dá à política um nome (por exemplo, Proteja os ficheiros de trabalho) e, em seguida, escolha um tipo **de Política** a partir da lista de drop-down.

    Pode configurar políticas de aplicação para proteger ficheiros em dispositivos Android e iPhone, bem como windows 10, e pode configurar políticas de configuração de dispositivos de configuração de dispositivos Windows 10 da empresa. Consulte os seguintes links para mais detalhes:

    - [Configurar as definições de proteção de aplicações para dispositivos Android ou iOS](app-protection-settings-for-android-and-ios.md)

    - [Configurar as definições de proteção de aplicações para dispositivos Windows 10](protection-settings-for-windows-10-devices.md)

    - [Definir definições de proteção do dispositivo para PCs windows 10](protection-settings-for-windows-10-pcs.md)

4. Depois de configurar políticas, você e os seus colaboradores podem configurar dispositivos:

    - Se os dispositivos Windows ainda não estiverem a utilizar a atualização do Windows Pro Creator, terá de os atualizar para a Atualização dos [Criadores do Windows Pro](upgrade-to-windows-pro-creators-update.md).

    - Consulte a [configuração de dispositivos Windows para utilizadores do Microsoft 365 Business Premium](set-up-windows-devices.md) para obter passos para dispositivos Windows.

    - Consulte a [Configuração de dispositivos móveis para utilizadores do Microsoft 365 Business Premium](set-up-mobile-devices.md) para passos para telemóveis e iPhones Android.