---
title: Como é que as funcionalidades de proteção Microsoft 365 Empresas Premium mapeiam para as definições do Intune
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
manager: scotv
ms.date: 8/13/2018
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
ms.assetid: aad21b1a-c775-469a-b89c-c5d1d59d27db
description: Saiba como as funcionalidades de proteção Microsoft 365 Empresas Premium mapeiam às definições do Intune. A subscrição fornece-lhe uma licença para modificar as definições do Intune.
ms.openlocfilehash: 844b83bca9483f72fd322d666803c42b90fee41d3e0047ea93b4b6b07717b0dd
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53852737"
---
# <a name="how-do-protection-features-in-microsoft-365-business-premium-map-to-intune-settings"></a>Como é que as funcionalidades de proteção Microsoft 365 Empresas Premium mapeiam para as definições do Intune

## <a name="android-and-ios-application-protection-settings"></a>Definições de proteção de aplicações para Android e iOS

A seguinte tabela mostra como as definições de política de aplicação para Android e iOS são mapeadas às definições do Intune.
  
Para encontrar a definição do Intune, indique-a com as Microsoft 365 Empresas Premium de administrador da conta, vá para **Centros** de administração e, em seguida, **Intune.**
  
 > [!IMPORTANT]
 > 
 > Uma Microsoft 365 Empresas Premium subscrição fornece-lhe uma licença para modificar todas as definições do Intune. Consulte [Introdução ao Intune para começar.](/intune/introduction-intune)
  
Selecione o nome da Política que &mdash; pretende, por exemplo, Política de aplicação para Android &mdash; e, em seguida, **selecione Definições de política.**
  
Em **Proteger os ficheiros de trabalho se os dispositivos forem perdidos ou roubados**
  
|**Definição de política de aplicação para Android e iOS**|**Definições do Intune**|
|:-----|:-----|
|Eliminar ficheiros de trabalho de um dispositivo inativo após  <br/> |Intervalo offline (dias) antes do apagamento dos dados da aplicação  <br/> |
|Forçar os utilizadores a guardar os ficheiros de trabalho no OneDrive para Empresas  <br/> Tenha em atenção que apenas o OneDrive para Empresas é permitido  <br/> |Selecione em que serviços de armazenamento os dados empresariais podem ser guardados  <br/> |
|||
   
Em **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis**
  
|**Definição de política de aplicação para Android e iOS**|**Definições do Intune**|
|:-----|:-----|
|Eliminar ficheiros de trabalho de um dispositivo inativo após  <br/> |Intervalo offline (dias) antes do apagamento dos dados da aplicação  <br/> |
|Forçar os utilizadores a guardar os ficheiros de trabalho no OneDrive para Empresas  <br/> Tenha em atenção que apenas o OneDrive para Empresas é permitido  <br/> |Selecione em que serviços de armazenamento os dados empresariais podem ser guardados  <br/> |
|Encriptar ficheiros de trabalho  <br/> |Encriptar dados da aplicação  <br/> |
|Em **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis** <br/> ||
|Exigir um PIN ou uma impressão digital para aceder às aplicações do Office  <br/> | Exigir um PIN para aceder  <br/>  Também define:  <br/> **Permitir PIN simples** para **Sim** <br/> **Comprimento do Pin** para 4  <br/> **Permitir impressão digital em vez do PIN** para **Sim** <br/> **Desativar PIN de aplicação quando o PIN de dispositivo é gerido** para **Não** <br/> |
|Repor o PIN quando o início de sessão falha este número de vezes (esta ação é desativada se o PIN não for obrigatório)  <br/> |Número de tentativas antes da reposição do PIN  <br/> |
|Exigir que os utilizadores indiquem novamente a Office que as aplicações tenham estado inativas durante (esta ação é desativada se o PIN não for necessário)  <br/> | Reverificar os requisitos de acesso após (minutos)  <br/>  Também define:  <br/> O **Tempo limite** é definido para minutos  <br/>  É o mesmo número de minutos que definiu no Microsoft 365 Business.  <br/> O **Período de tolerância offline** está definido para 720 minutos por predefinição  <br/> |
|Negar o acesso a ficheiros de trabalho em dispositivos desbloqueados por jailbreak ou rooting  <br/> |Bloquear execução de aplicações geridas em dispositivos desbloqueados por jailbreak ou rooting  <br/> |
|Permitir que os utilizadores copiem conteúdos das aplicações do Office para aplicações pessoais  <br/> | Restringir cortar, copiar e colar com outras aplicações  <br/>  Se a Microsoft 365 Empresas Premium de Configuração estiver definida para Ativado, estas três opções também estão definidas para Todas as **Aplicações** no Intune:  <br/> **Permitir que a aplicação transfira dados para outras aplicações** <br/> **Permitir que a aplicação receba dados de outras aplicações** <br/> **Restringir operações cortar, copiar e colar com outras aplicações** <br/>  Se a opção do Microsoft 365 Business estiver definida para **Ativado**, todas as opções do Intune estarão definidas para:  <br/> **Permitir que a aplicação transfira dados para outras aplicações** está definido para **Aplicações geridas por políticas** <br/> **Permitir que a aplicação receba dados de outras aplicações** está definido para **Todas as Aplicações** <br/> **Restringir operações cortar, copiar e colar com outras aplicações** está definido para **Aplicações geridas por políticas com colar em** <br/> |
|||
   
## <a name="windows-10-app-protection-settings"></a>Definições de proteção de aplicações para Windows 10

A seguinte tabela mostra como as definições de política de aplicação para Windows 10 são mapeadas às definições do Intune.
  
Para encontrar a definição do Intune, instale-se com as Microsoft 365 Empresas Premium de administrador da empresa e vá para o [portal do Azure](https://portal.azure.com). **Selecione Mais** serviços e escreva Intune no **Filtro.** **Selecione Política da Aplicação Intune App Protection** \> .
  
 > [!IMPORTANT]
 >
 >Uma Microsoft 365 Empresas Premium subscrição fornece-lhe uma licença para modificar apenas as definições do Intune que mapeiam para as definições disponíveis no Microsoft 365 Empresas Premium. 
  
Para explorar as definições disponíveis, selecione o nome da política que pretende e, em **seguida,** selecione Geral, Atribuições **,** Aplicações permitidas , Aplicações isentas **,** Definições necessárias ou Definições  **avançadas** no painel de navegação à esquerda. 
  
|**Definição de política de aplicação para Windows 10**|**Definições do Intune**|
|:-----|:-----|
|Encriptar ficheiros de trabalho  <br/> |**Definições avançadas** \> **Proteção de dados**. **Revogar as chaves de encriptação ao anular a inscrição** e **Revogar o acesso a dados protegidos quando o dispositivo se inscreve para MDM** estão definidas para **Ativado**.      <br/> |
|Impeça os utilizadores de copiarem dados empresariais para ficheiros pessoais.  <br/> |**Definições necessárias** \> **Modo Windows Information Protection**. **Ativos** na Microsoft 365 Empresas Premium mapeia a: Ocultar **Substituições,**  Desativo no Microsoft 365 Empresas Premium mapeia a: Desativo.   <br/> |
|Controlo do acesso a documentos do Office  <br/> | Se esta ação estiver definida para **A Microsoft 365 Empresas Premium,**  <br/> **Definições avançadas** \> **Acesso**, **Utilizar o Windows Hello para Empresas como método para iniciar sessão no Windows** está definido para **Ativado**, com as seguintes definições adicionais:  <br/> **Definir o número mínimo de carateres necessários para o PIN** está definido para **4**.  <br/> **Configurar a utilização de letras em maiúsculas no PIN do Windows Hello para Empresas** está definido para **Não permitir a utilização de letras maiúsculas no PIN**.  <br/> **Configurar a utilização de letras em minúsculas no PIN do Windows Hello para Empresas** está definido para **Não permitir a utilização de letras minúsculas no PIN**.  <br/> **Configurar a utilização de carateres especiais no PIN do Windows Hello para Empresas** está definido para **Não permitir a utilização de carateres especiais no PIN**.  <br/> **Especifique o período de tempo (em dias)** em que um PIN pode ser utilizado antes de o sistema exigir que o utilizador altere esteja definido para **0.**  <br/> **Especificar o número de PINs anteriores que podem ser associados a uma conta de utilizador que não pode ser reutilizada** está definido para **0**.  <br/> **Número de falhas de autenticação permitidas antes de o dispositivo ser eliminado** está definido para Microsoft 365 Business 5 (por predefinição).  <br/> **Período de inatividade máximo (em minutos) permitido no dispositivo após o qual ficará bloqueado por PIN ou palavra-passe** está definido tal como no Microsoft 365 Business.  <br/> |
|Ativar a recuperação de dados protegidos  <br/> |**Definições avançadas** \> **Proteção de dados**. **Mostrar o ícone de proteção de dados empresariais** e **Utilizar o Azure RMS para WIP** estão definidos para **Ativado**.      <br/> |
|Proteger localizações na nuvem da empresa adicionais  <br/> |**Definições avançadas** \> **Domínios protegidos** e **Recursos da nuvem** mostram sites do SharePoint e domínios.  <br/> |
|Os ficheiros utilizados por estas aplicações estão protegidos  <br/> |A lista de aplicações protegidas é indicada em **Aplicações permitidas**.  <br/> |
|||
   
## <a name="windows-10-device-protection-settings"></a>Definições de proteção para dispositivos Windows 10

A tabela seguinte mostra como as definições de configuração para dispositivos Windows 10 são mapeadas às definições do Intune.
  
Para encontrar a definição do Intune, inicie a ação com as suas credenciais de administrador do Microsoft 365 Empresas Premium, vá para o portal do [Azure](https://portal.azure.com)e, em seguida, selecione Mais serviços e escreva Intune no Filtro **,** selecione Perfis de configuração de **Dispositivos Intune** \>  \> . Then select **Device policy for Windows 10** \> **Properties** \> **Settings**.
  
|**Definição de política para dispositivos Windows 10**|**Definições do Intune**|
|:-----|:-----|
|Ajudar a proteger os PCs contra vírus e outras ameaças com o Antivírus do Windows Defender  <br/> |Permitir Monitorização em Tempo Real = Ativado  <br/> Permitir Proteção da Nuvem = Ativado  <br/> Pedir aos Utilizadores Submissões de Exemplo = Enviar exemplos seguros automaticamente (submissão automática predefinida de dados que não sejam PII)  <br/> |
|Ajudar a proteger os PCs contra ameaças baseadas na Web no Microsoft Edge  <br/> |**SmartScreen** nas **definições do browser Microsoft Edge** está definido para **Obrigatório**.  <br/> |
|Desligar o ecrã do dispositivo quando estiver inativo durante (minutos)  <br/> |Máximo de minutos de inatividade até o ecrã ser bloqueado (minutos)  <br/> |
|Permitir que os utilizadores transfiram aplicações da Microsoft Store  <br/> |Política de URI Personalizada  <br/> |
|Permitir que os utilizadores acedam à Cortana  <br/> |**Geral** \> **Cortana está** definido para **bloquear** no Intune quando estiver definido como **desativado** no Microsoft 365 Empresas Premium.  <br/> |
|Permitir que os utilizadores recebam sugestões e anúncios da Microsoft acerca do Windows  <br/> |**Windows destaque**, está tudo bloqueado se estiver definido para **desajustado** no Microsoft 365 Empresas Premium.  <br/> |
|Manter os dispositivos Windows 10 atualizados automaticamente  <br/> | Esta definição está no **Microsoft Intune** atualizações do serviço - Windows 10 Atualizar Anéis , selecionar Atualizar política para \> **dispositivos** **Windows 10** e, em seguida,  \> **Propriedades Definições**.  <br/>  Quando a Microsoft 365 Empresas Premium de definições está definida para **Ativos,** todas as seguintes definições estão definidas:  <br/> **Ramo de** serviço está definido como **CB** (CBB quando este está desligado no Microsoft 365 Empresas Premium).  <br/> **Atualizações de produtos da Microsoft** está definido para **Permitir**.  <br/> **Controladores do Windows** está definido para **Permitir**.  <br/> **Comportamento de atualização automática** está definido para **Instalar automaticamente no período de manutenção** com:  <br/> **Início das horas extraordinárias** está definido para **06:00**.  <br/> **Fim das horas ativas** está definido para **22:00**.  <br/> **Período de deferimento da atualização de qualidade (dias)** está definido para **0**.  <br/> **Período de deferimento da atualização de funcionalidades (dias)** está definido para **0**.  <br/> **Modo de transferência de otimização de entrega** está definido para **HTTP aliado a peering atrás da mesma NAT**.  <br/> |
|||
