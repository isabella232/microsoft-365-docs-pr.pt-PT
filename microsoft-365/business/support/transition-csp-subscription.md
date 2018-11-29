---
title: Transição de uma subscrição do Microsoft 365 Business CSP 
description: Descubra como pode transitar uma subscrição do Microsoft 365 Business CSP de pré-visualização GA. 
author: jasongroce
ms.author: jasgro
ms.topic: article 
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business 
keywords: Microsoft 365 Business, Microsoft 365, SMB, a alternativa de subscrição de CSP
ms.date: 11/01/2017
ms.openlocfilehash: 8109c0b00f06a15c12bbccf89e7f49dc3fa4b34a
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982488"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Transição de uma subscrição do Microsoft 365 Business CSP

Se tiver uma subscrição do Microsoft 365 Business pré-visualizar CSP, siga este guia para saber como pode transitar a subscrição de pré-visualização existente para Microsoft 365 Business GA (disponibilidade geral).

**Como alternativa de uma subscrição de pré-visualizar GA**

1. Inicie sessão no <a href="https://partnercenter.microsoft.com" target="_blank">Centro de parceiros</a>.
2. Do dashboard, seleccione **os clientes**e, em seguida, localize e seleccione o nome da empresa.

    As subscrições da empresa serão listadas.

    ![Subscrições do cliente no Centro de parceiros](images/pc_customer_subscriptions_1.png)
    
3. Na página de **subscrições** da empresa, seleccione **Adicionar subscrição**.
4. Na página **nova subscrição** , seleccione a **pequenas empresas** e, em seguida, seleccione **Microsoft 365 Business** a partir da lista.
5. Adicione o número de licenças e, em seguida, seleccione **seguinte: Rever** para rever a subscrição e, em seguida, seleccionar **Submeter**.

    ![Reveja a nova subscrição para o Microsoft 365 Business](images/pc_customer_reviewnewsubscription.png)

    As **subscrições baseada na licença** apresentará **Microsoft 365 Business Preview** e **Microsoft 365 Business**. Terá de suspender a subscrição de pré-visualizar a seguinte.

6. Seleccione **pré-visualização do Microsoft 365 Business**.
7. Na página **Microsoft 365 Business Preview** , seleccione **suspenso** para suspender a subscrição de pré-visualizar.

    ![Suspender a subscrição do Microsoft 365 Business Preview](images/pc_customer_m365bpreview_suspend.png)

8. Seleccione **Submeter** para confirmar.

    Na página de **subscrições** , confirme que o estado de **Pré-visualização de negócio do Microsoft 365** mostra **suspenso**.

    ![Confirmar que o estado de subscrição de pré-visualização é suspensa](images/pc_customer_m365bpreview_suspend_confirm.png)

9. Opcionalmente, também pode validar o contrato de licença. Para tal, siga estes passos:
    1. Seleccione **os utilizadores e as licenças** da página de **subscrições** da empresa.
    2. Na página de **licenças e utilizadores** , seleccione um utilizador.
    3. Na página do utilizador, consulte a secção **atribuir licenças** e confirme que mostra **Microsoft 365 Business**.

        ![Confirmar que a licença do Microsoft 365 Business está atribuída ao utilizador](images/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Impacto a clientes e utilizadores durante e após transição

Não há qualquer impacto a clientes e utilizadores durante a transição e de transição de registar.

## <a name="impact-to-customers-who-dont-transition"></a>Impacto para os clientes que não transição

A tabela seguinte resume o impacto para os clientes que não transição de uma subscrição do Microsoft 365 Business Preview para uma subscrição do Microsoft 365 Business.

|       | T-0 T + 30.     | T + 30 a T + 60 | T + 60 a T + 120 | Para além de T + 120  |
|-------|-----------------|--------------|---------------|---------------|
| **Estado** | No período de tolerância | Expirado      | Desactivado      | Deprovisioned |
| **Impactos do serviço**                                                        |
| **Portal de administração do Microsoft 365 Business** | Sem afectar a funcionalidade | Sem afectar a funcionalidade | Pode adicionar ou eliminar utilizadores, as subscrições de compra.</br> Não é possível atribuir/revogar licenças. | Subscrição do cliente e todos os dados são eliminados. Admin pode gerir outras subscrições pagas. |
| **Aplicações do Office**                         | Nenhum impacto do utilizador final | Nenhum impacto do utilizador final | Office entra em modo de funcionalidade reduzida.</br> Os utilizadores podem visualizar apenas ficheiros. | Office entra em modo de funcionalidade reduzida.</br> Os utilizadores podem visualizar apenas ficheiros. |
| **Serviços de nuvem (SharePoint Online, Exchange Online, Skype, equipas e mais)** | Nenhum impacto do utilizador final | Nenhum impacto do utilizador final | Os utilizadores finais e administradores não têm acesso a dados na nuvem. | Subscrição do cliente e todos os dados são eliminados. |
| **Componentes EM + S** | Nenhum impacto de admin</br> Nenhum impacto do utilizador final | Nenhum impacto de admin</br> Nenhum impacto do utilizador final | Capacidade deixará de ser aplicadas.</br> Consulte o [dispositivo móvel impactos após a expiração de subscrição](#mobile-device-impacts-upon-subscription-expiration) e [impactos Windows 10 PC após a expiração de subscrição](#windows-10-pc-impacts-upon-subscription-expiration) para obter mais informações. | Capacidade deixará de ser aplicadas.</br> Consulte o [dispositivo móvel impactos após a expiração de subscrição](#mobile-device-impacts-upon-subscription-expiration) e [impactos Windows 10 PC após a expiração de subscrição](#windows-10-pc-impacts-upon-subscription-expiration) para obter mais informações. |
| **Windows 10 Business** | Nenhum impacto de admin</br> Nenhum impacto do utilizador final | Nenhum impacto de admin</br> Nenhum impacto do utilizador final | Capacidade deixará de ser aplicadas.</br> Consulte o [dispositivo móvel impactos após a expiração de subscrição](#mobile-device-impacts-upon-subscription-expiration) e [impactos Windows 10 PC após a expiração de subscrição](#windows-10-pc-impacts-upon-subscription-expiration) para obter mais informações. | Capacidade deixará de ser aplicadas.</br> Consulte o [dispositivo móvel impactos após a expiração de subscrição](#mobile-device-impacts-upon-subscription-expiration) e [impactos Windows 10 PC após a expiração de subscrição](#windows-10-pc-impacts-upon-subscription-expiration) para obter mais informações. |
| **Início de sessão de AD Azure para um computador com o Windows 10** | Nenhum impacto de admin</br> Nenhum impacto do utilizador final | Nenhum impacto de admin</br> Nenhum impacto do utilizador final | Nenhum impacto de admin</br> Nenhum impacto do utilizador final | Uma vez eliminado o inquilino, um utilizador pode iniciar sessão com credenciais locais apenas. Imagem novamente o dispositivo se existirem sem credenciais de locais. |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>Dispositivo móvel impactos após a expiração de subscrição

A tabela seguinte resume o impacto para as políticas de gestão de aplicações em dispositivos móveis.

|                            | Experiência licenciada completo                      | Expiração de post T + 60 dias          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Eliminar ficheiros de trabalho a partir de um dispositivo inactivo** | Ficheiros de trabalho são removidos depois de seleccionado de dias | Ficheiros de trabalho permanecem em dispositivos pessoais do utilizador |
| **Forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas** | Ficheiros de trabalho só podem ser guardados para OneDrive para a empresa | Ficheiros de trabalho podem ser guardados em qualquer local |
| **Encriptar ficheiros de trabalho** | Os ficheiros de trabalho são encriptados | Ficheiros de trabalho já não estão encriptados.</br> Políticas de segurança são removidas e dados de aplicações do Office são removidos. |
| **Exigir um PIN ou de impressões digitais para aceder a aplicações do Office** | Acesso restrito para aplicações | Sem restrição de acesso a nível da aplicação |
| **Repor o PIN quando falha de início de sessão** | Acesso restrito para aplicações | Sem restrição de acesso a nível da aplicação |
| **Pedir aos utilizadores iniciar sessão novamente depois de aplicações do Office tem estado inactivas** | Sinal-in necessário | Nenhum sinal-in necessário para aceder a aplicações |
| **Negar o acesso a ficheiros de trabalho em dispositivos desbloqueados por jailbreak ou rooting** | Não não possível aceder a ficheiros de trabalho em dispositivos raiz/jailbroken | Ficheiros de trabalho podem ser acedidos em dispositivos raiz/jailbroken |
| **Permitir que os utilizadores copiar conteúdo de aplicações do Office para aplicações pessoais** | Copiar/colar restringido a aplicações disponíveis como parte da subscrição do Microsoft 365 Business | Copiar/colar disponível para todas as aplicações |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>PC com Windows 10 impactos após a expiração de subscrição

A tabela seguinte resume o impacto das políticas de configuração de dispositivo do Windows 10.

|                            | Experiência licenciada completo                      | Expiração de post T + 60 dias          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Ajudar a proteger o PC contra ameaças, utilizando o Windows Defender** | Activar/desactivar está fora do controlo de utilizador | Utilizador pode activar/desactivar o Windows Defender no PC de 10 do Windows |
| **Ajudar a proteger os PCs contra ameaças baseadas na Web no Microsoft Edge** | Protecção do PC no Microsoft Edge | Utilizador pode activar/desactivar a protecção do PC no Microsoft Edge |
| **Desactivar o ecrã do dispositivo quando inactivo** | Admin define a política de intervalo de tempo limite do ecrã | Tempo limite do ecrã pode ser configurado pelo utilizador final |
| **Permitir que os utilizadores transfiram aplicações da Microsoft Store** | Admin define se um utilizador pode transferir aplicações do Microsoft Store | Utilizador pode transferir aplicações do Microsoft Store em qualquer altura |
| **Permitir que os utilizadores acedam à Cortana** | Admin define a política de acesso de utilizador para Cortana | Dispositivos de utilizador para activar/desactivar Cortana |
| **Permitir que os utilizadores receber sugestões e anúncios da Microsoft** | Admin define a política de utilizador receber sugestões e anúncios da Microsoft | Utilizador pode activar/desactivar sugestões e anúncios da Microsoft |
| **Permitir que os utilizadores copiem conteúdos das aplicações do Office para aplicações pessoais** | Admin define a política para manter o Windows 10 dispositivos actualizados | Os utilizadores podem decidir quando actualizar o Windows |




