---
title: Configurar as definições de proteção de aplicações para dispositivos Android ou iOS
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Saiba como criar, editar ou eliminar uma política de gestão de aplicações e proteger ficheiros de trabalho em dispositivos Android ou iOS.
ms.openlocfilehash: 92dce1e8761e53b85df85f2a84f30ab307f63e6d
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/14/2021
ms.locfileid: "52925069"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Configurar as definições de proteção de aplicações para dispositivos Android ou iOS

Este artigo aplica-se a Microsoft 365 Empresas Premium.

## <a name="create-an-app-management-policy"></a>Criar uma política de gestão de aplicações

1. Vá para o centro de administração em <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> . 
    
2. No navegador esquerdo, selecionar Adicionar **Políticas** \> **de** \> **Dispositivos.**
  
3. No painel **Adicionar política**, introduza um nome exclusivo para esta política. 
    
4. Em **Tipo de política,** escolha Gestão de **Aplicações** para Android ou Gestão de Aplicações para **iOS,** consoante o conjunto de políticas que pretende criar. 
    
5. Expanda **as secções Proteger os ficheiros de trabalho se os dispositivos for** perdidos ou roubados e Gerir a forma como os **utilizadores Office ficheiros em dispositivos móveis**. Configure as definições da forma que quiser. **Faça a gestão** da forma como  os utilizadores acedem a ficheiros Office em dispositivos móveis está Desligado por predefinição, mas recomendamos que a deslige e aceite os valores predefinido.  Para obter mais informações, consulte [Definições disponíveis.](#available-settings) 
    
    Pode sempre utilizar a ligação **Repor predefinições** para regressar à predefinição. 
    
    ![Screenshot of Create a policy with Application management for Android selected](../media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. Em seguida, decida **Quem irá ver estas definições?** Se não quiser utilizar o grupo de segurança predefinido **Todos** os Utilizadores, selecione **Alterar**, selecione os grupos de segurança que têm estas definições \> **Selecione**.
    
7. Por fim, selecione **Concluído** para guardar a política e atribuí-la aos dispositivos. 
    
## <a name="edit-an-app-management-policy"></a>Editar uma política de gestão de aplicações

1. No cartão **Políticas,** selecionar **Editar política.**
    
2. No painel **Editar política**, selecione a política que pretende alterar 
    
3. Selecione **Editar** junto a cada definição para alterar os valores na política. Quando altera um valor, este é automaticamente guardado na política.
    
4. Quando terminar, feche o painel **Editar** política. 
    
## <a name="delete-an-app-management-policy"></a>Eliminar uma política de gestão de aplicações

1. Na página **Políticas,** selecionar uma política e, em **seguida, Eliminar.**
    
2. No painel **Eliminar política,** selecionar **Confirmar para** eliminar a política ou políticas que escolheu. 
    
## <a name="available-settings"></a>Definições disponíveis

As tabelas seguintes disponibilizam informações detalhadas sobre as definições disponíveis para proteger ficheiros de trabalho em dispositivos e as definições que controlam a forma como os utilizadores acedem Office dos respetivos dispositivos móveis.
  
 Para obter mais informações, consulte [Como é que as funcionalidades de proteção Microsoft 365 Empresas Premium mapeiam às definições do Intune.](map-protection-features-to-intune-settings.md) 
  
### <a name="settings-that-protect-work-files"></a>Definições que protegem os ficheiros de trabalho

As seguintes definições para proteger ficheiros de trabalho estarão disponíveis se o dispositivo de um utilizador for perdido ou roubado:


|Definição  <br/> |Descrição  <br/> |
|:-----|:-----|
|Eliminar ficheiros de trabalho de um dispositivo inativo após este número de dias  <br/> |Se um dispositivo não for utilizado durante o número de dias que especificar aqui, todos os ficheiros de trabalho armazenados no dispositivo serão eliminados automaticamente.  <br/> |
|Forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas  <br/> |Se esta definição estiver **Ação,** a única localização disponível para guardar ficheiros de trabalho é OneDrive para Empresas.  <br/> |
|Encriptar ficheiros de trabalho  <br/> |Mantenha esta definição **Ativada** para que os ficheiros de trabalho sejam protegidos por encriptação. Mesmo que o dispositivo seja perdido ou roubado, ninguém pode ler os dados da sua empresa.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Definições que controlam a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis

As seguintes definições estão disponíveis para gerir como os utilizadores acedem a ficheiros de trabalho do Office:


|Definição  <br/> |Descrição  <br/> |
|:-----|:-----|
|Exigir um PIN ou uma impressão digital para aceder às aplicações do Office  <br/> |Se esta  definição estiver Ativada, os utilizadores têm de fornecer outra forma de autenticação, para além do nome de utilizador e palavra-passe, antes de poderem utilizar aplicações Office nos respetivos dispositivos móveis.<br/> |
|Repor o PIN quando o início de sessão falha este número de vezes  <br/> |Para impedir um utilizador não autorizado de adivinhar um PIN aleatoriamente, o PIN será reposto após o número de tentativas incorretas que especificar.  <br/> |
|Exigir que o utilizador inicie a sessão novamente após as aplicações do Office estarem inativas durante  <br/> |Esta definição determina durante quanto tempo um utilizador pode estar indisque antes de lhe ser pedido para voltar a entrar.  <br/> |
|Negar o acesso a ficheiros de trabalho em dispositivos desbloqueados por jailbreak ou rooting  <br/> |Alguns utilizadores podem ter um dispositivo desbloqueado através de jailbreak ou rooting. Isto significa que o utilizador pode modificar o sistema operativo, o que pode tornar o dispositivo mais suscetível a software maligno. Estes dispositivos são bloqueados quando esta definição se encontra **Ativada**.  <br/> |
|Não permitir que os utilizadores copiem conteúdos de aplicações Office para aplicações pessoais  <br/> |Por predefinição, permitimos esta opção. No entanto, se a definição estiver **Aada,** o utilizador pode copiar informações de um ficheiro de trabalho para um ficheiro pessoal. Se a definição estiver **Des desligada,** o utilizador não poderá copiar informações de uma conta pessoal para uma aplicação ou conta pessoal.  <br/> |
