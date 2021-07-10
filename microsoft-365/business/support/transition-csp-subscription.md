---
title: Transição de uma subscrição do Microsoft 365 Empresas CSP
description: Saiba como fazer a transição de uma subscrição CSP Microsoft 365 Empresas da pré-visualização para a disponibilidade geral (AG).
author: jasongroce
f1.keywords:
- NOCSH
ms.custom:
- seo-marvel-mar
- AdminSurgePortfolio
ms.author: jasongroce
ms.topic: article
manager: jasonh
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business
keywords: Microsoft 365 Subscrição CSP de Microsoft 365, SMB, transição
ms.date: 11/01/2017
ms.openlocfilehash: 47b65b2de9db0fd27e29272937bab2041eb67300
ms.sourcegitcommit: 7dc3b4dec05299abb4290a6e3d1ebe0fdc622ed7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/10/2021
ms.locfileid: "53363825"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Transição de uma subscrição do Microsoft 365 Empresas CSP

Se tiver uma subscrição do Microsoft 365 Business Preview CSP, siga este guia para saber como pode fazer a transição da sua subscrição de pré-visualização existente para a Microsoft 365 Empresas (disponibilidade geral).

**Como transição de uma subscrição de pré-visualização para AG**

1. Inscreva-se <a href="https://partnercenter.microsoft.com" target="_blank">no Centro de Parceiros.</a>
2. No dashboard, selecione **Clientes e,** em seguida, locale e selecione o nome da empresa.

    As subscrições para a empresa serão listadas.

    ![Subscrições de clientes no Centro de Parceiros](../../media/pc_customer_subscriptions_1.png)
    
3. Na página Subscrições **da empresa,** **selecione Adicionar subscrição.**
4. Na página **Nova subscrição, selecione** Pequenas **empresas e,** em seguida, **selecione Microsoft 365 Empresas** na lista.
5. Adicione o número de licenças e, em seguida, **selecione Seguinte: Rever** para rever a subscrição e, em seguida, selecione **Submeter**.

    ![Rever a nova subscrição do Microsoft 365 Empresas](../../media/pc_customer_reviewnewsubscription.png)

    As **subscrições baseadas em Licenças** serão Microsoft 365 **Para Empresas e Microsoft 365** **Empresas.** Irá suspender a subscrição de Pré-visualização a seguir.

6. **Selecione Microsoft 365 Pré-visualização Empresarial**.
7. Na página **Microsoft 365 Business Preview,** selecione **Suspenso** para suspender a subscrição de Pré-visualização.

    ![Suspender a subscrição Microsoft 365 Pré-visualização Empresarial](../../media/pc_customer_m365bpreview_suspend.png)

8. **Selecione Submeter** para confirmar.

    Na página **Subscrições, confirme** que o estado da **Pré-visualização Microsoft 365 Empresas** é **Suspenso.**

    ![Confirmar que o estado da subscrição de Pré-visualização está suspenso](../../media/pc_customer_m365bpreview_suspend_confirm.png)

9. Opcionalmente, também pode validar o contrato de licença. Para tal, siga estes passos:
    1. **Selecione Utilizadores e licenças** na **página Subscrições da** empresa.
    2. Na página **Utilizadores e licenças,** selecione um utilizador.
    3. Na página do utilizador, verifique a **secção Atribuir licenças** e confirme se a mesma Microsoft 365 **Empresas.**

        ![Confirme que Microsoft 365 licença Empresas está atribuída ao utilizador](../../media/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Impacto nos clientes e utilizadores durante e após a transição

Os clientes e os utilizadores não serão afetados durante a transição e após a transição.

## <a name="impact-to-customers-who-dont-transition"></a>Impacto para clientes que não se transim

A seguinte tabela resume o impacto para os clientes que não transitam de uma subscrição de Pré-visualização Microsoft 365 Empresas para uma subscrição do Microsoft 365 Empresas.

|       | T-0 a T+30     | T+30 para T+60 | T+60 para T+120 | Além de T+120  |
|-------|-----------------|--------------|---------------|---------------|
| **Estado** | No período de gradação | Expirou      | Desativado      | Desaprovisionado |
| **Impactos do serviço**                                                        |
| **centro de administração do Microsoft 365** | Sem impacto na funcionalidade | Sem impacto na funcionalidade | Pode adicionar/eliminar utilizadores, comprar subscrições.</br> Não é possível atribuir/revogar licenças. | A subscrição do cliente e todos os dados são eliminados. O administrador pode gerir outras subscrições pagas. |
| **Office aplicações**                         | Sem impacto nos utilizadores finais | Sem impacto nos utilizadores finais | Office entrar no modo de funcionalidade reduzida.</br> Os utilizadores só podem ver ficheiros. | Office entrar no modo de funcionalidade reduzida.</br> Os utilizadores só podem ver ficheiros. |
| **Serviços em nuvem (SharePoint Online, Exchange Online, Skype, Teams e muito mais)** | Sem impacto nos utilizadores finais | Sem impacto nos utilizadores finais | Os utilizadores finais e os administradores não têm acesso aos dados na nuvem. | A subscrição do cliente e todos os dados são eliminados. |
| **Componentes EM+S** | Sem impacto para administradores</br> Sem impacto nos utilizadores finais | Sem impacto para administradores</br> Sem impacto nos utilizadores finais | A capacidade já não é impoda.</br> Consulte [Impactos no dispositivo móvel após](#mobile-device-impacts-upon-subscription-expiration) a expiração da subscrição Windows 10 pc afetados na expiração da [subscrição](#windows-10-pc-impacts-upon-subscription-expiration) para mais informações. | A capacidade já não é impoda.</br> Consulte [Impactos no dispositivo móvel após](#mobile-device-impacts-upon-subscription-expiration) a expiração da subscrição Windows 10 pc afetados na expiração da [subscrição](#windows-10-pc-impacts-upon-subscription-expiration) para mais informações. |
| **Windows 10 Business** | Sem impacto para administradores</br> Sem impacto nos utilizadores finais | Sem impacto para administradores</br> Sem impacto nos utilizadores finais | A capacidade já não é impoda.</br> Consulte [Impactos no dispositivo móvel após](#mobile-device-impacts-upon-subscription-expiration) a expiração da subscrição Windows 10 pc afetados na expiração da [subscrição](#windows-10-pc-impacts-upon-subscription-expiration) para mais informações. | A capacidade já não é impoda.</br> Consulte [Impactos no dispositivo móvel após](#mobile-device-impacts-upon-subscription-expiration) a expiração da subscrição Windows 10 pc afetados na expiração da [subscrição](#windows-10-pc-impacts-upon-subscription-expiration) para mais informações. |
| **Início de sessão do Azure AD num PC Windows 10 PC** | Sem impacto para administradores</br> Sem impacto nos utilizadores finais | Sem impacto para administradores</br> Sem impacto nos utilizadores finais | Sem impacto para administradores</br> Sem impacto nos utilizadores finais | Assim que o inquilino for eliminado, um utilizador só pode fazê-lo com as credenciais locais. Se não houver credenciais locais, ermae o dispositivo. |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>O impacto no dispositivo móvel após a expiração da subscrição

A seguinte tabela resume o impacto nas políticas de gestão de aplicações em dispositivos móveis.

|                            | Experiência totalmente licenciada                      | T+60 dias após a expiração          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Eliminar ficheiros de trabalho de um dispositivo inativo** | Os ficheiros de trabalho são removidos após dias selecionados | Os ficheiros de trabalho permanecem nos dispositivos pessoais do utilizador |
| **Forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas** | Os ficheiros de trabalho só podem ser guardados na OneDrive para Empresas | Os ficheiros de trabalho podem ser guardados em qualquer lugar |
| **Encriptar ficheiros de trabalho** | Os ficheiros de trabalho são encriptados | Os ficheiros de trabalho já não são encriptados.</br> As políticas de segurança são removidas e Office dados nas aplicações são removidos. |
| **Exigir PIN ou impressão digital para aceder a Office aplicações** | Acesso restrito a aplicações | Sem restrições de acesso ao nível da aplicação |
| **Repor PIN quando o início de sessão falha** | Acesso restrito a aplicações | Sem restrições de acesso ao nível da aplicação |
| **Exigir que os utilizadores indiquem novamente a Office que as aplicações tenham sido inaciosas** | Sign-in required | Não é necessário um sinal de que não é necessário |
| **Negar o acesso a ficheiros de trabalho em dispositivos desbloqueados por jailbreak ou rooting** | Não é possível aceder a ficheiros de trabalho em dispositivos desbrupados por jailbro/rooted | Pode aceder a ficheiros de trabalho em dispositivos desbrupados por jailbro/rooted |
| **Permitir que os utilizadores copiem conteúdos Office aplicações pessoais** | Copiar/colar restrito a aplicações disponíveis como parte Microsoft 365 subscrição | Copiar/colar disponível para todas as aplicações |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>Windows 10 Impactos no PC após a expiração da subscrição

A seguinte tabela resume o impacto para as políticas de configuração Windows 10 dispositivos.

|                            | Experiência totalmente licenciada                      | T+60 dias após a expiração          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Ajudar a proteger os PCs contra ameaças através de Windows Defender** | A ação/desligá-lo está fora do controlo do utilizador | O utilizador pode ligar/desligar Windows Defender no Windows 10 PC |
| **Ajudar a proteger os PCs contra ameaças baseadas na Web no Microsoft Edge** | Proteção de PC Microsoft Edge | O utilizador pode ligar/desligar a proteção de PC no Microsoft Edge |
| **Desligar o ecrã do dispositivo quando estiver inctilizado** | O administrador define a política de intervalo de tempo de tempo de ecrã | O tempo de tempo de ecrã pode ser configurado pelo utilizador final |
| **Permitir que os utilizadores transfiram aplicações da Microsoft Store** | O administrador define se um utilizador pode transferir aplicações a partir do Microsoft Store | O utilizador pode transferir aplicações a partir Microsoft Store qualquer altura |
| **Permitir que os utilizadores acedam à Cortana** | O administrador define uma política de acesso de utilizador às Cortana | Dispositivos de utilizador para a Cortana |
| **Permitir que os utilizadores recebam sugestões e anúncios da Microsoft** | O administrador define uma política para o utilizador receber sugestões e anúncios da Microsoft | O utilizador pode ativos/desligados sugestões e anúncios da Microsoft |
| **Permitir que os utilizadores copiem conteúdos das aplicações do Office para aplicações pessoais** | O Administrador define uma política para manter Windows 10 dispositivos sempre actualizados | Os utilizadores podem decidir quando atualizar a Windows |
