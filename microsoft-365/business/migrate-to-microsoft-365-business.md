---
title: Migrar para o Microsoft 365 Business do prémio de negócio do Office 365
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
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Obter informações sobre como mover o seu negócio para Microsoft 365 Business.
ms.openlocfilehash: fd6f18c02453e6751d6163ab79e726eae9c951a9
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983498"
---
# <a name="migrate-to-microsoft-365-business-from-office-365-business-premium"></a>Migrar para o Microsoft 365 Business do prémio de negócio do Office 365

Se já tiver o Office 365 para a subscrição de negócio, por exemplo, Office 365 Business Premium, pode facilmente adicionar licenças à Microsoft 365 Business e atribui-los a alguns ou todos os utilizadores.
  
> [!NOTE]
> Não é possível utilizar o botão de [planos de parâmetro](https://support.office.com/article/73318661-8f33-478b-bcc7-fb8d69dbb22a?.aspx#switchbutton) para actualizar para o Microsoft 365 Business ainda. 
  
## <a name="add-microsoft-365-business-licenses"></a>Adicionar licenças Microsoft 365 Business

Tem duas formas de obter o Microsoft 365 Business. Se tiver um cônjuge, ele ou ela pode adquirir Microsoft 365 Business para lhe do [Centro de parceiros da Microsoft](get-microsoft-365-business.md). O parceiro também pode ajudar a transição para o Microsoft 365 Business.
  
Se gerir a sua subscrição, pode [contactar a vendas](https://www.microsoft.com/microsoft-365/business) para adquirir licenças Microsoft 365 Business. 
  
Consulte para [Adicionar, alterar ou eliminar um parceiro de classificação de subscrição](https://support.office.com/article/f86e8177-936e-491e-9024-44dea2b296ff) para saber como pode começar a trabalhar com um parceiro. 
  
Se for dada uma hiperligação para adquirir as licenças, irá percorrer um assistente semelhante ao abaixo apresentado. Escolha **Sim, adicioná-lo para a minha conta**. Também pode escolher o número de licenças e o método de pagamento.
  
![A actividade de 365 Microsoft direct comprar hiperligação, optar por adicionar a sua conta actual ou inscrever-se para uma nova conta.](media/8bc54fd1-9cab-44d5-af91-c471e89aea46.png)
  
## <a name="assign-microsoft-365-licenses"></a>Atribuir licenças Microsoft 365

1. Quando tiver adquirido licenças de novas e esta é a primeira vez que fez, a faixa do programa de configuração para Microsoft 365 Business será apresentado na parte superior do Centro de administração.
    
    > [!NOTE]
    > A faixa do programa de configuração é uma oportunidade para adicionar novos utilizadores, um novo domínio e migrar o correio electrónico para novos utilizadores. Se não tenciona efectuar um, deve ainda avança no assistente e escolha as opções predefinidas para o tornar desaparecem da home page da administração. 
  
   ![Escolha a configuração de início da actividade de 365 Microsoft está pronta para definir a faixa.](media/8d3b0d97-7cca-497f-9364-4b00ad670209.png)
  
    Selecione **Iniciar configuração**.
    
2. Na página **Personalizar o início de sessão no e correio electrónico** , pode adicionar um domínio seleccionando **ligar um domínio é já proprietário** se pretender utilizar esta oportunidade para adicionar outro domínio à sua subscrição. 
    
    Se já tiver configurado um domínio, o segundo campo indicará que e indicará a **continuar a utilizar** \< _o nome de domínio_ \> **para correio electrónico e o início de sessão**. Se não tiver configurado um domínio com a subscrição, vai indicar **continuar a utilizar** \< _name.onmicrosoft.com a empresa_ \> **para correio electrónico e o início de sessão**.    
    
    Selecione **Seguinte**.
    
    ![Na página correio electrónico e personalizar o início de sessão no, optar por adicionar um domínio ou utilize o que estiver a utilizar.](media/c3f5cfb2-1189-4d2f-803b-c9feb008a7a3.png)
  
3. Na página **Adicionar novos utilizadores** , pode adicionar novos utilizadores, se tiver novos empregados que pretende atribuir as licenças Microsoft 365 Business ao. 
    
    Se não tiver novos empregados para adicionar e atribuir licenças a utilizadores existentes, seleccione **seguinte**.
    
4. Sobre o * * migrar mensagens de correio electrónico * * página, pode optar por migrar de correio electrónico para qualquer um dos novos utilizadores que adicionou no passo 3. Também pode ignorar este passo. Seleccione **seguinte**.
    
5. Na última página, escolha a **Ir para o Centro admin**e continuar a configuração não existe.
    
6. No Centro de administração, vá para **utilizadores** \> **os utilizadores activos**.
    
7. Seleccione o utilizador a quem pretende atribuir a licença do **Microsoft 365 Business** para e, em seguida, escolha **Editar** junto de **Licenças de produto**.
    
    ![Na ficha de utilizador, escolha Editar junto de licenças de produto.](media/be0fe2d8-7ff8-447c-88f6-d212ed78451c.png)
  
8. Em **licenças de produto** do diapositivo **Microsoft 365 Business** **nas** \> **Guardar**e, em seguida, **Fechar**.
    
Assim que adquiriu a licença inicial para o Microsoft 365 Business, agora também pode adicionar mais em de **Facturação** \> **Serviços de compra**. Na página de **Serviços de compra** pode clique nas reticências no cartão de **Visita de 365 da Microsoft** e seleccione **Alterar quantidade de licenças** a adquirir mais. 
  
## <a name="protect-user-devices-and-files"></a>Proteger ficheiros e dispositivos de utilizador

Depois de atribuir licenças para o Microsoft 365 Business, pode começar a proteger dispositivos e ficheiros dos utilizadores.
  
1. No Centro de administração, em nav esquerda, vá para **dispositivos de** \> **políticas**.
    
2. Na página **políticas de dispositivo** , seleccione **Adicionar**.
    
3. No painel **Adicionar política** atribua a política de um nome e, em seguida, escolha um **tipo de política** da lista pendente. 
    
    Pode configurar políticas de aplicação para proteger ficheiros no Android e iPhone dispositivos, bem como o Windows 10 e pode configurar políticas de configuração do dispositivo para a empresa propriedade Windows 10 dispositivos. Consulte as hiperligações seguintes para obter detalhes:
    
  - [Configurar as definições de proteção de aplicações para dispositivos Android ou iOS](app-protection-settings-for-android-and-ios.md)
    
  - [Configurar as definições de proteção de aplicações para dispositivos Windows 10](protection-settings-for-windows-10-devices.md)
    
  - [Configurar as definições de proteção de dispositivos para PCs Windows 10](protection-settings-for-windows-10-pcs.md)
    
   ![No painel de política de adicionar, introduza um nome para o mesmo e seleccione o tipo de política a partir do menu pendente.](media/76ef37e4-1d18-4f34-8a0f-391ab1d0ae2b.png)
  
4. Depois de configurar políticas, e os seus funcionários podem configurar dispositivos:
    
  - Se o Windows ainda não estão na actualização do Windows Pro criador, terá de [actualizar para Pro criadores de actualização do Windows](upgrade-to-windows-pro-creators-update.md).
    
  - Consulte [Configurar dispositivos do Windows para utilizadores empresariais do Microsoft 365](set-up-windows-devices.md) para obter os passos para dispositivos do Windows. 
    
  - Consulte [Configurar dispositivos móveis para utilizadores empresariais do Microsoft 365](set-up-mobile-devices.md) para obter os passos para telefones Android e iPhones. 
    
5. Para instalar automaticamente as aplicações de cliente do Office, consulte [preparar a implementação de cliente do Office por negócio do Microsoft 365](prepare-for-office-client-deployment.md) e [automaticamente instalar ou desinstalar o Office no Windows 10 dispositivos](auto-install-or-uninstall-office.md).
    


