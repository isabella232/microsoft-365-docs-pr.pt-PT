---
title: Faça a transição de uma assinatura CSP de negócios da Microsoft 365 
description: Descubra como você pode fazer a transição de uma assinatura CSP de negócios do Microsoft 365 da visualização para a GA. 
author: jasongroce
ms.author: jasgro
ms.topic: article 
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business 
keywords: Microsoft 365 Business, Microsoft 365, SMB, assinatura CSP de transição
ms.date: 11/01/2017
ms.openlocfilehash: 72e620df69a425ca7e5c41c5a6651bc0f7f533de
ms.sourcegitcommit: b535fe233234fd25146cfe15478e20d954f71e03
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/20/2019
ms.locfileid: "38748347"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Faça a transição de uma assinatura CSP de negócios da Microsoft 365

Se você tiver uma assinatura CSP de visualização de negócios do Microsoft 365, siga este guia para descobrir como você pode fazer a transição de sua assinatura de visualização existente para o Microsoft 365 Business GA (disponibilidade geral).

**Como fazer a transição de uma assinatura de visualização para GA**

1. Entre no <a href="https://partnercenter.microsoft.com" target="_blank">Centro de Parceiros.</a>
2. A partir do painel, selecione **clientes**e, em seguida, encontre e selecione o nome da empresa.

    As assinaturas da empresa serão listadas.

    ![Assinaturas do cliente no Partner Center](images/pc_customer_subscriptions_1.png)
    
3. Na página de **assinaturas** da empresa, selecione **adicionar assinatura**.
4. Na nova página de **assinatura,** selecione **pequenas empresas** e, em seguida, **selecione o Microsoft 365 Business** da lista.
5. Adicione o número de licenças e, em seguida, selecione **Em seguida: Revisão** para revisar a assinatura e, em seguida, **selecione Enviar**.

    ![Analise a nova assinatura do Microsoft 365 Business](images/pc_customer_reviewnewsubscription.png)

    As **assinaturas baseadas em licença** mostrarão a Microsoft **365 Business Preview** e a Microsoft **365 Business**. Você suspenderá a assinatura de visualização em seguida.

6. Selecione **a visualização de negócios da Microsoft 365.**
7. Na página de visualização de **negócios do Microsoft 365,** selecione **suspenso** para suspender a assinatura de visualização.

    ![Suspender a assinatura de visualização de negócios do Microsoft 365](images/pc_customer_m365bpreview_suspend.png)

8. Selecione **enviar** para confirmar.

    Na página **de assinaturas,** confirme que o status de visualização de **negócios da Microsoft 365** mostra **suspenso.**

    ![Confirme que o status da assinatura de visualização está suspenso](images/pc_customer_m365bpreview_suspend_confirm.png)

9. Opcionalmente, você também pode validar o contrato de licença. To do this, follow these steps:
    1. Selecione **usuários e licenças** da página de **assinaturas** da empresa.
    2. Na página **de usuários e licenças,** selecione um usuário.
    3. Na página do usuário, verifique a seção de **licenças de design** e confirme que ele mostra o Microsoft **365 Business**.

        ![Confirme que a licença de negócios da Microsoft 365 é atribuída ao usuário](images/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Impacto para clientes e usuários durante e após a transição

Não há impacto para clientes e usuários durante a transição e pós-transição.

## <a name="impact-to-customers-who-dont-transition"></a>Impacto para os clientes que não transitam

A tabela a seguir resume o impacto para os clientes que não transitam de uma assinatura microsoft 365 Business Preview para uma assinatura Microsoft 365 Business.

|       | T-0 a T+30     | T+30 a T+60 | T+60 a T+120 | Além do T+120  |
|-------|-----------------|--------------|---------------|---------------|
| **Estado** | No período de carência | Expirado      | Desativado      | Desprovisionado |
| **Impactos do serviço**                                                        |
| **Microsoft 365 Portal de administração de negócios** | Sem impacto na funcionalidade | Sem impacto na funcionalidade | Pode adicionar/ excluir usuários, comprar assinaturas.</br> Não é possível atribuir/ revogar licenças. | A assinatura do cliente e todos os dados são excluídos. O administrador pode gerenciar outras assinaturas pagas. |
| **Aplicativos do office**                         | Sem impacto final do usuário | Sem impacto final do usuário | O Office entra no modo de funcionalidade reduzida.</br> Os usuários podem visualizar arquivos apenas. | O Office entra no modo de funcionalidade reduzida.</br> Os usuários podem visualizar arquivos apenas. |
| **Serviços de nuvem (SharePoint Online, Exchange Online, Skype, Equipes e muito mais)** | Sem impacto final do usuário | Sem impacto final do usuário | Usuários finais e administradores não têm acesso aos dados na nuvem. | A assinatura do cliente e todos os dados são excluídos. |
| **Componentes EM+S** | Sem impacto administrativo</br> Sem impacto final do usuário | Sem impacto administrativo</br> Sem impacto final do usuário | A capacidade não é mais aplicada.</br> Veja [os impactos do dispositivo móvel na expiração da assinatura](#mobile-device-impacts-upon-subscription-expiration) e os [impactos do PC do Windows 10 na expiração](#windows-10-pc-impacts-upon-subscription-expiration) da assinatura para obter mais informações. | A capacidade não é mais aplicada.</br> Veja [os impactos do dispositivo móvel na expiração da assinatura](#mobile-device-impacts-upon-subscription-expiration) e os [impactos do PC do Windows 10 na expiração](#windows-10-pc-impacts-upon-subscription-expiration) da assinatura para obter mais informações. |
| **Windows 10 Negócios** | Sem impacto administrativo</br> Sem impacto final do usuário | Sem impacto administrativo</br> Sem impacto final do usuário | A capacidade não é mais aplicada.</br> Veja [os impactos do dispositivo móvel na expiração da assinatura](#mobile-device-impacts-upon-subscription-expiration) e os [impactos do PC do Windows 10 na expiração](#windows-10-pc-impacts-upon-subscription-expiration) da assinatura para obter mais informações. | A capacidade não é mais aplicada.</br> Veja [os impactos do dispositivo móvel na expiração da assinatura](#mobile-device-impacts-upon-subscription-expiration) e os [impactos do PC do Windows 10 na expiração](#windows-10-pc-impacts-upon-subscription-expiration) da assinatura para obter mais informações. |
| **Login em anúncio szure em um PC do Windows 10** | Sem impacto administrativo</br> Sem impacto final do usuário | Sem impacto administrativo</br> Sem impacto final do usuário | Sem impacto administrativo</br> Sem impacto final do usuário | Uma vez que o inquilino é excluído, um usuário pode entrar com credenciais locais apenas. Re-imagem do dispositivo se não houver credenciais locais. |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>Impactos de dispositivos móveis na expiração da assinatura

A tabela a seguir resume o impacto nas políticas de gerenciamento de aplicativos em dispositivos móveis.

|                            | Experiência totalmente licenciada                      | T+60 dias após a expiração          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Excluir arquivos de trabalho de um dispositivo inativo** | Os arquivos de trabalho são removidos após dias selecionados | Os arquivos de trabalho permanecem nos dispositivos pessoais do usuário |
| **Forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas** | Arquivos de trabalho só podem ser salvos no OneDrive for Business | Arquivos de trabalho podem ser salvos em qualquer lugar |
| **Encriptar ficheiros de trabalho** | Arquivos de trabalho são criptografados | Os arquivos de trabalho não são mais criptografados.</br> As políticas de segurança são removidas e os dados do Office sobre aplicativos são removidos. |
| **Exigir PIN ou impressão digital para acessar aplicativos do Office** | Acesso restrito a aplicativos | Sem restrição de acesso ao nível de aplicativo |
| **Pin de redefinição quando o login falha** | Acesso restrito a aplicativos | Sem restrição de acesso ao nível de aplicativo |
| **Exigir que os usuários entrem novamente depois que os aplicativos do Office estiverem ociosos** | A inscrição necessária | Não é necessário entrar |
| **Negar o acesso a ficheiros de trabalho em dispositivos desbloqueados por jailbreak ou rooting** | Arquivos de trabalho não podem ser acessados em dispositivos presos/enraizados | Arquivos de trabalho podem ser acessados em dispositivos presos/enraizados |
| **Permitir que os usuários copiem conteúdo de aplicativos do Office para aplicativos pessoais** | Cópia/pasta restrita a aplicativos disponíveis como parte da assinatura microsoft 365 business | Cópia/pasta disponível para todos os aplicativos |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>O PC do Windows 10 afeta a expiração da assinatura

A tabela a seguir resume o impacto nas políticas de configuração do dispositivo Windows 10.

|                            | Experiência totalmente licenciada                      | T+60 dias após a expiração          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Ajude a proteger os PCs de ameaças usando o Windows Defender** | Ligar/desligar está fora do controle do usuário | O usuário pode ativar/desligar o Windows Defender no PC do Windows 10 |
| **Ajudar a proteger os PCs contra ameaças baseadas na Web no Microsoft Edge** | Proteção de PC no Microsoft Edge | O usuário pode ativar/desligar a proteção do PC no Microsoft Edge |
| **Desligue a tela do dispositivo quando ocioso** | Admin define política de intervalo de intervalo de tempo de tempo de tela | O intervalo de tempo da tela pode ser configurado pelo usuário final |
| **Permitir que os utilizadores transfiram aplicações da Microsoft Store** | Admin define se um usuário pode baixar aplicativos da Microsoft Store | O usuário pode baixar aplicativos da Microsoft Store a qualquer momento |
| **Permitir que os utilizadores acedam à Cortana** | Administrador define política de acesso do usuário à Cortana | Dispositivos de usuário para ligar/desligar cortana |
| **Permitir que os usuários recebam dicas e anúncios da Microsoft** | Admin define política sobre usuário receber dicas e anúncios da Microsoft | O usuário pode ativar/desligar dicas e anúncios da Microsoft |
| **Permitir que os utilizadores copiem conteúdos das aplicações do Office para aplicações pessoais** | Admin define política para manter os dispositivos Windows 10 atualizados | Os usuários podem decidir quando atualizar o Windows |
