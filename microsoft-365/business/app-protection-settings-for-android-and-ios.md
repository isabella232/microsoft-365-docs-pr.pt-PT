---
title: Configurar as definições de proteção de aplicações para dispositivos Android ou iOS
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
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Saiba como criar, editar ou excluir uma política de gerenciamento de aplicativos e proteger arquivos de trabalho em dispositivos Android ou iOS.
ms.openlocfilehash: 2eebe5b603837d7e4125ab7e88b61792ca3a1e5d
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/14/2019
ms.locfileid: "38321851"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Configurar as definições de proteção de aplicações para dispositivos Android ou iOS

![Banner que https://aka.ms/aboutM365previewapontam para .](media/m365admincenterchanging.png)

## <a name="create-an-app-management-policy"></a>Criar uma política de gestão de aplicações

1. Vá para o centro <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>de administração em . 
    
2. No nav esquerdo, escolha **políticas** \> dos **dispositivos** \> **adicione.**
  
3. No painel **Adicionar política**, introduza um nome exclusivo para esta política. 
    
4. De acordo com o **tipo de política,** escolha gerenciamento de **aplicativos para Android** ou gerenciamento de **aplicativos para iOS,** dependendo de qual conjunto de políticas você deseja criar. 
    
5. Expanda os arquivos de **trabalho protect quando os dispositivos são perdidos ou roubados** e **gerencie como os usuários acessam os arquivos do Office em dispositivos móveis.** Configure as configurações como você gostaria. **Gerenciar como os usuários acessam os arquivos do Office em dispositivos móveis** está **desligado** por padrão, mas recomendamos que você **os** desligue e aceite os valores padrão. Para mais informações, consulte [as configurações disponíveis.](#available-settings) 
    
    Pode sempre utilizar a ligação **Repor predefinições** para regressar à predefinição. 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. Em seguida, decida **Quem irá ver estas definições?** Se você não quiser usar o grupo de segurança padrão **de todos os usuários,** escolha **o Change,** escolha os \> **grupos**de segurança que selecionem essas configurações.
    
7. Por fim, selecione **Concluído** para guardar a política e atribuí-la aos dispositivos. 
    
## <a name="edit-an-app-management-policy"></a>Editar uma política de gestão de aplicações

1. No cartão **de Políticas,** escolha **a política de eitar**.
    
2. No painel **Editar política**, selecione a política que pretende alterar 
    
3. Selecione **Editar** junto a cada definição para alterar os valores na política. Quando você muda um valor, ele é automaticamente salvo na política.
    
4. Quando terminar, feche o painel de políticas de **eite.** 
    
## <a name="delete-an-app-management-policy"></a>Eliminar uma política de gestão de aplicações

1. Na página **de Políticas,** escolha uma política e, em seguida, **excluir**.
    
2. No painel de **política supressão,** escolha **confirmar** para excluir a política ou as políticas que você escolheu. 
    
## <a name="available-settings"></a>Definições disponíveis

As tabelas a seguir dão informações detalhadas sobre as configurações disponíveis para proteger os arquivos de trabalho em dispositivos e as configurações que controlam como os usuários acessam os arquivos do Office de seus dispositivos móveis.
  
 Para obter mais informações, consulte [Como é que as funcionalidades de proteção no Microsoft 365 Empresas são mapeadas para as definições do Intune](map-protection-features-to-intune-settings.md). 
  
### <a name="settings-that-protect-work-files"></a>Definições que protegem os ficheiros de trabalho

As seguintes definições para proteger ficheiros de trabalho estarão disponíveis se o dispositivo de um utilizador for perdido ou roubado:
  
|||
|:-----|:-----|
|Definição  <br/> |Descrição  <br/> |
|Eliminar ficheiros de trabalho de um dispositivo inativo após este número de dias  <br/> |Se um dispositivo não for usado para o número de dias que você especifica aqui, quaisquer arquivos de trabalho armazenados no dispositivo serão excluídos automaticamente.  <br/> |
|Forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas  <br/> |Se esta configuração estiver **em ação,** o único local disponível para salvar arquivos de trabalho é o OneDrive for Business.  <br/> |
|Encriptar ficheiros de trabalho  <br/> |Mantenha esta definição **Ativada** para que os ficheiros de trabalho sejam protegidos por encriptação. Mesmo que o dispositivo esteja perdido ou roubado, ninguém pode ler os dados da empresa.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Definições que controlam a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis

As seguintes definições estão disponíveis para gerir como os utilizadores acedem a ficheiros de trabalho do Office:
  
|||
|:-----|:-----|
|Definição  <br/> |Descrição  <br/> |
|Exigir um PIN ou uma impressão digital para aceder às aplicações do Office  <br/> |Se essa **** configuração estiver on,00, os usuários devem fornecer outra forma de autenticação, além de seu nome de usuário e senha, antes que eles possam usar aplicativos do Office em seus dispositivos móveis.<br/> |
|Repor o PIN quando o início de sessão falha este número de vezes  <br/> |Para impedir um utilizador não autorizado de adivinhar um PIN aleatoriamente, o PIN será reposto após o número de tentativas incorretas que especificar.  <br/> |
|Exigir que o utilizador inicie a sessão novamente após as aplicações do Office estarem inativas durante  <br/> |Essa configuração determina quanto tempo um usuário pode ficar ocioso antes de ser solicitado a entrar novamente.  <br/> |
|Negar o acesso a ficheiros de trabalho em dispositivos desbloqueados por jailbreak ou rooting  <br/> |Alguns utilizadores podem ter um dispositivo desbloqueado através de jailbreak ou rooting. Isto significa que o utilizador pode modificar o sistema operativo, o que pode tornar o dispositivo mais suscetível a software maligno. Estes dispositivos são bloqueados quando esta definição se encontra **Ativada**.  <br/> |
|Permitir que os utilizadores copiem conteúdos das aplicações do Office para aplicações pessoais  <br/> |Nós permitimos isso por padrão, mas se a configuração estiver **on,** o usuário poderá copiar informações em um arquivo de trabalho para um arquivo pessoal. Se a configuração estiver **desligada,** o usuário não poderá copiar informações de uma conta de trabalho em um aplicativo pessoal ou conta pessoal.  <br/> |
