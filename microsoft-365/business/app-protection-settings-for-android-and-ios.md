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
ms.openlocfilehash: 2e157737990c7aca6e87a676e90f62f0d40ad372
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580300"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Configurar as definições de proteção de aplicações para dispositivos Android ou iOS

Este artigo aplica-se ao Microsoft 365 Business Premium.

## <a name="create-an-app-management-policy"></a>Criar uma política de gestão de aplicações

1. Vá ao centro de administração em <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> . 
    
2. No navegador esquerdo, escolha **Políticas de Dispositivos** \>  \> **Adicionar**.
  
3. No painel **Adicionar política**, introduza um nome exclusivo para esta política. 
    
4. Sob **o tipo de Política**, escolha **Gestão de Aplicações para Android** ou **Gestão de Aplicações para iOS,** dependendo do conjunto de políticas que pretende criar. 
    
5. Expandir **Ficheiros de trabalho quando os dispositivos são perdidos ou roubados** e **Gerir como os utilizadores acedem aos ficheiros do Office em dispositivos móveis**. Configure as definições como gostaria. **Gerencie a forma como os utilizadores acedem aos ficheiros do Office em dispositivos móveis** **por** padrão, mas recomendamos que o ligue **e** aceite os valores predefinidos. Para mais informações, consulte [as definições disponíveis.](#available-settings) 
    
    Pode sempre utilizar a ligação **Repor predefinições** para regressar à predefinição. 
    
    ![Screenshot of Create a policy with Application management for Android selected](../media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. Em seguida, decida **Quem irá ver estas definições?** Se não quiser utilizar o grupo de segurança predefinido **Todos os Utilizadores,** escolha **Alterar**, escolha os grupos de segurança que obtêm estas definições \> **Selecione**.
    
7. Por fim, selecione **Concluído** para guardar a política e atribuí-la aos dispositivos. 
    
## <a name="edit-an-app-management-policy"></a>Editar uma política de gestão de aplicações

1. No cartão **Políticas,** escolha **a política de Edição.**
    
2. No painel **Editar política**, selecione a política que pretende alterar 
    
3. Selecione **Editar** junto a cada definição para alterar os valores na política. Quando se muda um valor, é automaticamente guardado na apólice.
    
4. Quando terminar, feche o painel de política de **edição.** 
    
## <a name="delete-an-app-management-policy"></a>Eliminar uma política de gestão de aplicações

1. Na página **Políticas,** escolha uma política e, em seguida, **apague**.
    
2. No painel **de política eliminar,** escolha **Confirmar** para eliminar a política ou as políticas que escolheu. 
    
## <a name="available-settings"></a>Definições disponíveis

As seguintes tabelas dão informações detalhadas sobre as definições disponíveis para proteger ficheiros de trabalho em dispositivos e as definições que controlam a forma como os utilizadores acedem aos ficheiros do Office a partir dos seus dispositivos móveis.
  
 Para obter mais informações, consulte [como as funcionalidades de proteção no mapa do Microsoft 365 Business Premium para as definições do Intune.](map-protection-features-to-intune-settings.md) 
  
### <a name="settings-that-protect-work-files"></a>Definições que protegem os ficheiros de trabalho

As seguintes definições para proteger ficheiros de trabalho estarão disponíveis se o dispositivo de um utilizador for perdido ou roubado:
  
|||
|:-----|:-----|
|Definição  <br/> |Descrição  <br/> |
|Eliminar ficheiros de trabalho de um dispositivo inativo após este número de dias  <br/> |Se um dispositivo não for utilizado durante o número de dias que especifica aqui, quaisquer ficheiros de trabalho armazenados no dispositivo serão automaticamente eliminados.  <br/> |
|Forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas  <br/> |Se esta definição estiver **on,** a única localização de poupança disponível para ficheiros de trabalho é o OneDrive for Business.  <br/> |
|Encriptar ficheiros de trabalho  <br/> |Mantenha esta definição **Ativada** para que os ficheiros de trabalho sejam protegidos por encriptação. Mesmo que o dispositivo seja perdido ou roubado, ninguém pode ler os dados da sua empresa.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Definições que controlam a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis

As seguintes definições estão disponíveis para gerir como os utilizadores acedem a ficheiros de trabalho do Office:
  
|||
|:-----|:-----|
|Definição  <br/> |Descrição  <br/> |
|Exigir um PIN ou uma impressão digital para aceder às aplicações do Office  <br/> |Se esta definição for **No que** os utilizadores devem fornecer outra forma de autenticação, além do seu nome de utilizador e palavra-passe, antes de poderem utilizar aplicações do Office nos seus dispositivos móveis.<br/> |
|Repor o PIN quando o início de sessão falha este número de vezes  <br/> |Para impedir um utilizador não autorizado de adivinhar um PIN aleatoriamente, o PIN será reposto após o número de tentativas incorretas que especificar.  <br/> |
|Exigir que o utilizador inicie a sessão novamente após as aplicações do Office estarem inativas durante  <br/> |Esta definição determina quanto tempo um utilizador pode ficar inativo antes de ser solicitado a iniciar novamente o seu sposição.  <br/> |
|Negar o acesso a ficheiros de trabalho em dispositivos desbloqueados por jailbreak ou rooting  <br/> |Alguns utilizadores podem ter um dispositivo desbloqueado através de jailbreak ou rooting. Isto significa que o utilizador pode modificar o sistema operativo, o que pode tornar o dispositivo mais suscetível a software maligno. Estes dispositivos são bloqueados quando esta definição se encontra **Ativada**.  <br/> |
|Não permita que os utilizadores copiem conteúdo de apps do Office em aplicações pessoais  <br/> |Permitimos isso por predefinição, mas se a definição estiver **em Funcionamento,** o utilizador poderá copiar informações num ficheiro de trabalho para um ficheiro pessoal. Se a definição estiver **desligada,** o utilizador não poderá copiar informação de uma conta de trabalho numa aplicação pessoal ou numa conta pessoal.  <br/> |
