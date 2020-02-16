---
title: Upgrade para Microsoft 365 Business a partir do Office 365 Business Premium
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
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Passos que atualizam o seu negócio do Office 365 Business Premium para o Microsoft 365 Business.
ms.openlocfilehash: e17ac2658c7276ba4a77de371847343866815c42
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/15/2020
ms.locfileid: "42065297"
---
# <a name="upgrade-to-microsoft-365-business-from-office-365-business-premium"></a>Upgrade para Microsoft 365 Business a partir do Office 365 Business Premium

Se tiver um [Office 365 para subscrição](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2)de negócios , por exemplo, Office 365 Business Premium, pode facilmente fazer upgrade para o Microsoft 365 Business. Upgrade para Microsoft 365 Business se quiser adicionar: 
- Windows 10 Pro (para PCs que executam o Windows 8 ou mais tarde)
- Controlos simples que gerem dados empresariais em dispositivos
- Capacidades de segurança avançadas.
Saiba mais sobre o Microsoft 365 Business em [Microsoft.com](https://www.microsoft.com/microsoft-365/business)

## <a name="whats-the-difference-between-office-365-business-premium-and-microsoft-365-business"></a>Qual é a diferença entre o Office 365 Business Premium e o Microsoft 365 Business?
Adicionámos uma comparação lado a lado destes dois planos à Descrição do [Serviço Empresarial Microsoft 365.](https://docs.microsoft.com/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description) 

## <a name="before-you-get-started"></a>Antes de começar.

- **Quando devo escolher fazer upgrade?** O upgrade é a escolha certa quando pretende atualizar **todos os utilizadores atribuídos** a um único plano. Ao optar pela atualização, todos os utilizadores do plano são transferidos para outro plano ao mesmo tempo. Se não quiser atualizar todos os designados para um único plano, compre licenças para o novo plano (neste caso Microsoft 365 Business), e [atribua essas licenças individualmente](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) a cada utilizador que pretenda fazer upgrade. 
- **Alguns addons podem impedir a atualização** Se tentar iniciar uma atualização e tiver um addon que o impeça de continuar, pode remover primeiro o addon e, em seguida, adicioná-lo de volta mais tarde se ainda precisar. 
- **Se pagou o seu plano de pré-pagamento** Não há um caminho simples de atualização para planos pré-pagos. Saberá se tem um plano pré-pago porque configura o seu plano usando uma identificação de produto que pode ter comprado numa loja. Contacte um parceiro, vá à Microsoft Store ou espere até que o seu plano pré-pago expire para mudar para um novo plano.

## <a name="upgrade-to-microsoft-365-business"></a>Upgrade para Microsoft 365 Business
Compre as suas licenças seguindo estes passos no [novo centro de administração:](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)
1. Assine no centro de <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>administração em .
2. Vá ao painel de navegação e selecione **Produtos de Faturação** \> **& Serviços**. Encontre a subscrição do Office 365 e selecione-a para ver os detalhes. 

    ![Uma imagem mostra como encontrar e selecionar a sua subscrição no centro de administração.](../media/FindYourSubscription.png)

3. Na página seguinte, selecione **Upgrade**. 

      ![Uma imagem mostra onde selecionar Upgrade no centro de administração.](../media/SelectUpgrade.png)

  > [!NOTE]
  > Se vir uma mensagem que diga que atualizar a **sua subscrição não é suportado com licenciamento baseado em grupo no Azure Ative Directory,** pode ignorá-lo com segurança a menos que tenha uma organização muito grande. As organizações que escolheram esta opção estarão cientes de que estão a usar o licenciamento baseado em grupo.

4. Em seguida, pode ver uma lista de planos do Office para os dois. Neste caso, encontre o plano de negócios da Microsoft 365. Você pode rolar para baixo se você quiser ver todas as aplicações e serviços do Office que estão incluídos com este plano. No **Microsoft 365 Business,** selecione **Upgrade** para adicionar o Microsoft 365 Business ao seu carrinho.
5. No carrinho:
    1. Vamos automaticamente incluir licenças para todos os seus utilizadores atuais. Se precisar de mais ou menos licenças, tem de [comprar e atribuir essas licenças individualmente](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users).  
    2. Pode ajustar a forma como gostaria de pagar: mensal ou anualmente. Selecione o menu suspenso para fazer a sua escolha.
6. Selecione **Ir ao Checkout** onde verá um resumo da sua compra, incluindo o método de pagamento desta conta. Também pode adicionar um código promocional aqui se tiver um.
7. Selecione **O pedido de lugar** para completar a sua compra.
A Microsoft leva alguns minutos para configurar os seus novos planos de serviço. Para verificar o progresso, selecione Verifique o estado da **atualização**. 
1. Uma vez que o seu plano esteja pronto, você pode precisar completar alguns passos adicionais de configuração no centro de administração. No painel de navegação, selecione **Casa** para completar quaisquer passos adicionais de configuração.

> [!NOTE]
> Receberá um reembolso prostrado pelas 365 licenças do Office que já não precisa. A sua conta bancária ou cartão de crédito será cobrada cerca de dois dias após a configuração do novo plano.
  
## <a name="protect-user-devices-and-files"></a>Proteja os dispositivos e ficheiros do utilizador

Agora que foram atribuídas licenças empresariais da Microsoft 365, completam as etapas para começar a proteger dispositivos e ficheiros. Você usará algumas novas opções incluídas no painel de navegação do centro de administração.
  
1. No centro de administração, no painel de navegação, vá para as **Políticas**de **Dispositivos** \> .
    
2. Na página de políticas do **Dispositivo,** selecione **Adicionar**.
    
3. No painel de **política Add** dá à política um nome (por exemplo, Proteja os ficheiros de trabalho) e, em seguida, escolha um tipo **de Política** a partir da lista de drop-down. 
    
    Pode configurar políticas de aplicação para proteger ficheiros em dispositivos Android e iPhone, bem como windows 10, e pode configurar políticas de configuração de dispositivos de configuração de dispositivos Windows 10 da empresa. Consulte os seguintes links para mais detalhes:
    
  - [Configurar as definições de proteção de aplicações para dispositivos Android ou iOS](app-protection-settings-for-android-and-ios.md)
    
  - [Configurar as definições de proteção de aplicações para dispositivos Windows 10](protection-settings-for-windows-10-devices.md)
    
  - [Definir definições de proteção do dispositivo para PCs windows 10](protection-settings-for-windows-10-pcs.md)
    
  
4. Depois de configurar políticas, você e os seus colaboradores podem configurar dispositivos:
    
  - Se os dispositivos Windows ainda não estiverem a utilizar a atualização do Windows Pro Creator, terá de os atualizar para a Atualização dos [Criadores do Windows Pro](upgrade-to-windows-pro-creators-update.md).
    
  - Consulte [a configuração de dispositivos Windows para utilizadores do Microsoft 365 Business](set-up-windows-devices.md) para obter medidas para dispositivos Windows. 
    
  - Consulte a [Configuração de dispositivos móveis para os utilizadores do Microsoft 365 Business](set-up-mobile-devices.md) para passos para telemóveis e iPhones Android. 
