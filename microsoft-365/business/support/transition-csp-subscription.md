---
title: Transição de uma subscrição de CSP empresarial da Microsoft 365
description: Descubra como pode transitar uma subscrição de CSP empresarial Microsoft 365 da pré-visualização para a disponibilidade geral (GA).
author: jasongroce
f1.keywords:
- NOCSH
ms.custom:
- seo-marvel-mar
ms.author: jasgro
ms.topic: article 
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business 
keywords: Microsoft 365 Business, Microsoft 365, SMB, assinatura CSP de transição
ms.date: 11/01/2017
ms.openlocfilehash: da56ce5bc70dfed5a3e86c739ef3c940b4ac1511
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/21/2020
ms.locfileid: "43635070"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Transição de uma subscrição de CSP empresarial da Microsoft 365

Se tiver uma subscrição cSP de Pré-visualização de Empresas Microsoft 365, siga este guia para saber como pode transitar a sua subscrição de pré-visualização existente para o Microsoft 365 Business GA (disponibilidade geral).

**Como transitar uma subscrição de pré-visualização para ga**

1. Inscreva-se no <a href="https://partnercenter.microsoft.com" target="_blank">Partner Center</a>.
2. A partir do painel de instrumentos, selecione **Clientes,** e depois encontre e selecione o nome da empresa.

    As subscrições da empresa serão listadas.

    ![Assinaturas do cliente no Partner Center](../../media/pc_customer_subscriptions_1.png)
    
3. Na página de **Subscrições** da empresa, selecione **Adicionar subscrição**.
4. Na nova página de **subscrição,** selecione **Small business** e, em seguida, selecione **Microsoft 365 Business** da lista.
5. Adicione o número de licenças e, em seguida, selecione **Seguinte: Reveja** para rever a subscrição e, em seguida, selecione **Enviar**.

    ![Reveja a nova subscrição do Microsoft 365 Business](../../media/pc_customer_reviewnewsubscription.png)

    As **subscrições baseadas em Licença** mostrarão o Microsoft **365 Business Preview** e o Microsoft **365 Business**. Suspenderá a subscrição de Pré-visualização em seguida.

6. Selecione **Microsoft 365 Business Preview**.
7. Na página **de Pré-visualização do Microsoft 365,** selecione **Suspended** para suspender a subscrição de Pré-visualização.

    ![Suspenda a subscrição de Pré-visualização de negócios da Microsoft 365](../../media/pc_customer_m365bpreview_suspend.png)

8. Selecione **Submeter** para confirmar.

    Na página **De Assinaturas,** confirme que o estado de **pré-visualização do Microsoft 365** mostra **suspenso**.

    ![Confirme que o estado de subscrição de Pré-visualização está suspenso](../../media/pc_customer_m365bpreview_suspend_confirm.png)

9. Opcionalmente, também pode validar o contrato de licença. To do this, follow these steps:
    1. Selecione **Utilizadores e licenças** na página de **Subscrições** da empresa.
    2. Na página **Utilizadores e licenças,** selecione um utilizador.
    3. Na página do utilizador, consulte a secção **de licenças de Atribuição** e confirme que mostra o Microsoft **365 Business**.

        ![Confirme que a licença de negócio si da Microsoft 365 é atribuída ao utilizador](../../media/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Impacto para clientes e utilizadores durante e após a transição

Não há impacto para clientes e utilizadores durante a transição e pós-transição.

## <a name="impact-to-customers-who-dont-transition"></a>Impacto para clientes que não fazem a transição

A tabela seguinte resume o impacto para os clientes que não fazem a transição de uma subscrição de Pré-visualização de negócios da Microsoft 365 para uma subscrição do Microsoft 365 Business.

|       | T-0 a T+30     | T+30 para T+60 | T+60 para T+120 | Além do T+120  |
|-------|-----------------|--------------|---------------|---------------|
| **Estado** | No período de graça | Expirado      | Deficientes      | Deprovisionado |
| **Impactos do serviço**                                                        |
| **Portal de administração de negócios microsoft 365** | Sem impacto na funcionalidade | Sem impacto na funcionalidade | Pode adicionar/excluir utilizadores, comprar subscrições.</br> Não posso atribuir/revogar licenças. | A subscrição do cliente e todos os dados são eliminados. A Administração pode gerir outras subscrições pagas. |
| **Aplicativos de escritório**                         | Sem impacto final do utilizador | Sem impacto final do utilizador | O Office entra no modo de funcionalidade reduzida.</br> Os utilizadores podem ver apenas ficheiros. | O Office entra no modo de funcionalidade reduzida.</br> Os utilizadores podem ver apenas ficheiros. |
| **Serviços em nuvem (SharePoint Online, Exchange Online, Skype, Equipas e muito mais)** | Sem impacto final do utilizador | Sem impacto final do utilizador | Os utilizadores finais e os administradores não têm acesso a dados na nuvem. | A subscrição do cliente e todos os dados são eliminados. |
| **Componentes EM+S** | Sem impacto administrativo</br> Sem impacto final do utilizador | Sem impacto administrativo</br> Sem impacto final do utilizador | A capacidade já não é aplicada.</br> Veja os impactos do [dispositivo Mobile na expiração da subscrição](#mobile-device-impacts-upon-subscription-expiration) e os impactos do [PC do Windows 10 na expiração da subscrição](#windows-10-pc-impacts-upon-subscription-expiration) para mais informações. | A capacidade já não é aplicada.</br> Veja os impactos do [dispositivo Mobile na expiração da subscrição](#mobile-device-impacts-upon-subscription-expiration) e os impactos do [PC do Windows 10 na expiração da subscrição](#windows-10-pc-impacts-upon-subscription-expiration) para mais informações. |
| **Negócio supor 10 Windows** | Sem impacto administrativo</br> Sem impacto final do utilizador | Sem impacto administrativo</br> Sem impacto final do utilizador | A capacidade já não é aplicada.</br> Veja os impactos do [dispositivo Mobile na expiração da subscrição](#mobile-device-impacts-upon-subscription-expiration) e os impactos do [PC do Windows 10 na expiração da subscrição](#windows-10-pc-impacts-upon-subscription-expiration) para mais informações. | A capacidade já não é aplicada.</br> Veja os impactos do [dispositivo Mobile na expiração da subscrição](#mobile-device-impacts-upon-subscription-expiration) e os impactos do [PC do Windows 10 na expiração da subscrição](#windows-10-pc-impacts-upon-subscription-expiration) para mais informações. |
| **Acesso à AD Azure num PC do Windows 10** | Sem impacto administrativo</br> Sem impacto final do utilizador | Sem impacto administrativo</br> Sem impacto final do utilizador | Sem impacto administrativo</br> Sem impacto final do utilizador | Uma vez que o inquilino é eliminado, um utilizador pode iniciar sessão apenas com credenciais locais. Re-imagem do dispositivo se não houver credenciais locais. |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>Dispositivo móvel impacta na expiração da subscrição

A tabela que se segue resume o impacto nas políticas de gestão de aplicações em dispositivos móveis.

|                            | Experiência totalmente licenciada                      | T+60 dias após a expiração          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Eliminar ficheiros de trabalho de um dispositivo inativo** | Os ficheiros de trabalho são removidos após dias selecionados | Os ficheiros de trabalho permanecem nos dispositivos pessoais do utilizador |
| **Forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas** | Os ficheiros de trabalho só podem ser guardados para o OneDrive para o Negócios | Ficheiros de trabalho podem ser guardados em qualquer lugar |
| **Encriptar ficheiros de trabalho** | Os ficheiros de trabalho são encriptados | Os ficheiros de trabalho já não estão encriptados.</br> As políticas de segurança são removidas e os dados do Office sobre aplicações são removidos. |
| **Requerer PIN ou impressão digital para aceder a aplicações do Office** | Acesso restrito a apps | Sem restrição de acesso ao nível de aplicações |
| **Redefinir PIN quando o login falhar** | Acesso restrito a apps | Sem restrição de acesso ao nível de aplicações |
| **Exigir que os utilizadores voltem a fazer o insessão depois de as aplicações do Office terem ficado inativas** | Inscrição necessária | Não é necessário iniciar sessão |
| **Negar o acesso a ficheiros de trabalho em dispositivos desbloqueados por jailbreak ou rooting** | Os ficheiros de trabalho não podem ser acedidos em dispositivos encadeçados/enraizados | Os ficheiros de trabalho podem ser acedidos em dispositivos encadeçados/enraizados |
| **Permitir que os utilizadores copiem conteúdo de aplicações do Office para aplicações pessoais** | Cópia/pasta restrita a aplicações disponíveis como parte da subscrição do Microsoft 365 | Cópia/pasta disponível para todas as aplicações |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>Windows 10 PC impacta na expiração da subscrição

A tabela que se segue resume o impacto nas políticas de configuração do dispositivo Windows 10.

|                            | Experiência totalmente licenciada                      | T+60 dias após a expiração          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Ajude a proteger os Computadores de ameaças usando o Windows Defender** | Ligar/desligar está fora do controlo do utilizador | O utilizador pode ligar/desligar o Windows Defender no PC windows 10 |
| **Ajudar a proteger os PCs contra ameaças baseadas na Web no Microsoft Edge** | Proteção para PC no Microsoft Edge | O utilizador pode ligar/desligar a proteção do PC no Microsoft Edge |
| **Desligue o ecrã do dispositivo quando estiver inativo** | Admin define política de intervalo de intervalo de intervalo de ecrã | O tempo de paragem do ecrã pode ser configurado pelo utilizador final |
| **Permitir que os utilizadores transfiram aplicações da Microsoft Store** | Admin define se um utilizador pode descarregar aplicações da Microsoft Store | O utilizador pode descarregar aplicações da Microsoft Store a qualquer momento |
| **Permitir que os utilizadores acedam à Cortana** | Administrador define política de acesso ao utilizador à Cortana | Dispositivos de utilizador para ligar/desligar cortana |
| **Permitir que os utilizadores recebam dicas e anúncios da Microsoft** | Admin define política sobre utilizadores que recebem dicas e anúncios da Microsoft | O utilizador pode ligar/desligar dicas e anúncios da Microsoft |
| **Permitir que os utilizadores copiem conteúdos das aplicações do Office para aplicações pessoais** | Admin define política para manter dispositivos Windows 10 atualizados | Os utilizadores podem decidir quando atualizar o Windows |
