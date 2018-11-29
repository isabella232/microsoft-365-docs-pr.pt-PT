---
title: Configurar as definições de proteção de aplicações para dispositivos Android ou iOS
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Obter informações sobre como criar, editar ou eliminar uma política de gestão de aplicações e proteger ficheiros de trabalho em dispositivos Android ou iOS.
ms.openlocfilehash: ed03227496120369b94bf2396974eebfd7798678
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983668"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Configurar as definições de proteção de aplicações para dispositivos Android ou iOS

## <a name="create-an-app-management-policy"></a>Criar uma política de gestão de aplicações

1. Inicie sessão no [Microsoft 365 Business](https://portal.office.com) com as suas credenciais de administrador global. 
    
2. No centro de administração, no cartão **Políticas de dispositivos**, selecione **Adicionar política**.
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. No painel **Adicionar política**, introduza um nome exclusivo para esta política. 
    
4. Em **Tipo de política**, selecione **Gestão de Aplicações para Android** ou **Gestão de Aplicações para iOS** consoante o conjunto de políticas que pretende criar. 
    
5. Expanda as opções **Proteger os ficheiros de trabalho se os dispositivos forem perdidos ou roubados** e **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis** \> configure as definições como pretende. A opção **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis** está **Desativada** por predefinição, mas recomenda-se que a defina como **Ativada** e aceite os valores predefinidos. Consulte as [Definições disponíveis](app-protection-settings-for-android-and-ios.md#bkmk_availablesettings) para obter mais informações. 
    
    Pode sempre utilizar a ligação **Repor predefinições** para regressar à predefinição. 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. Em seguida, decida **Quem irá ver estas definições?** Se não quiser utilizar o grupo de segurança predefinido, **Todos os Utilizadores**, selecione **Alterar**, selecione os grupos de segurança que irão receber estas definições \> **Selecionar**.
    
7. Por fim, selecione **Concluído** para guardar a política e atribuí-la aos dispositivos. 
    
## <a name="edit-an-app-management-policy"></a>Editar uma política de gestão de aplicações

1. Na ficha de **políticas** , escolha **Editar política**.
    
2. No painel **Editar política**, selecione a política que pretende alterar 
    
3. Selecione **Editar** junto a cada definição para alterar os valores na política. Ao alterar um valor, este é guardado automaticamente na política 
    
4. Quando tiver terminado, feche o painel **Editar política**. 
    
## <a name="delete-an-app-management-policy"></a>Eliminar uma política de gestão de aplicações

1. No cartão **Políticas**, selecione **Eliminar política**.
    
2. No painel **Eliminar política**, selecione as políticas que pretende eliminar \> **Selecionar** e, em seguida, **Confirmar** para eliminar as políticas selecionadas. 
    
## <a name="available-settings"></a>Definições disponíveis

As tabelas seguintes fornecem informações detalhadas sobre as definições disponíveis para proteger ficheiros de trabalho em dispositivos e as definições que controlam a forma como os utilizadores acedem a ficheiros do Office a partir dos respetivos dispositivos móveis.
  
 Consulte o artigo [Como é que as funcionalidades de proteção no Microsoft 365 Business são mapeadas às definições do Intune](map-protection-features-to-intune-settings.md) para obter mais informações. 
  
### <a name="settings-that-protect-work-files"></a>Definições que protegem os ficheiros de trabalho

As seguintes definições para proteger ficheiros de trabalho estarão disponíveis se o dispositivo de um utilizador for perdido ou roubado:
  
|||
|:-----|:-----|
|Definição  <br/> |Descrição  <br/> |
|Eliminar ficheiros de trabalho de um dispositivo inativo após este número de dias  <br/> |Se determinado dispositivo não for utilizado durante o número de dias que especificar aqui, todos os ficheiros de trabalho armazenados no dispositivo serão eliminados automaticamente.  <br/> |
|Forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas  <br/> |Se esta definição estiver **Ativada**, a única localização disponível para guardar ficheiros de trabalho será o OneDrive para Empresas.  <br/> |
|Encriptar ficheiros de trabalho  <br/> |Mantenha esta definição **Ativada** para que os ficheiros de trabalho sejam protegidos por encriptação. Mesmo que o dispositivo seja perdido ou roubado, os dados da sua empresa não poderão ser lidos por outras pessoas.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Definições que controlam a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis

As seguintes definições estão disponíveis para gerir como os utilizadores acedem a ficheiros de trabalho do Office:
  
|||
|:-----|:-----|
|Definição  <br/> |Descrição  <br/> |
|Exigir um PIN ou uma impressão digital para aceder às aplicações do Office  <br/> |Se esta definição estiver **Ativada**, os utilizadores terão de fornecer outro meio de autenticação, além do nome de utilizador e da palavra-passe, antes de poderem utilizar aplicações do Office nos respetivos dispositivos móveis.  <br/> |
|Repor o PIN quando o início de sessão falha este número de vezes  <br/> |Para impedir um utilizador não autorizado de adivinhar um PIN aleatoriamente, o PIN será reposto após o número de tentativas incorretas que especificar.  <br/> |
|Exigir que o utilizador inicie a sessão novamente após as aplicações do Office estarem inativas durante  <br/> |Esta definição determina durante quanto tempo um utilizador pode estar inativo antes de ter de voltar a iniciar sessão.  <br/> |
|Negar o acesso a ficheiros de trabalho em dispositivos desbloqueados por jailbreak ou rooting  <br/> |Alguns utilizadores podem ter um dispositivo desbloqueado através de jailbreak ou rooting. Isto significa que o utilizador pode modificar o sistema operativo, o que pode tornar o dispositivo mais suscetível a software maligno. Estes dispositivos são bloqueados quando esta definição se encontra **Ativada**.  <br/> |
|Permitir que os utilizadores copiem conteúdos das aplicações do Office para aplicações pessoais  <br/> |Vamos permitir isto por predefinição, mas se a definição estiver **activa**, o utilizador pode copiar informações num ficheiro de trabalho para um ficheiro pessoal. Se a definição estiver **desactivada**, o utilizador será não é possível copiar informações de uma conta de trabalho para uma conta pessoal ou app pessoal.<br/> |
   

  

