---
title: Como é que as funcionalidades de proteção no Microsoft 365 Business são mapeadas para as definições do Intune
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
ms.assetid: aad21b1a-c775-469a-b89c-c5d1d59d27db
description: Saiba como os recursos de proteção no mapa microsoft 365 business para configurações intune. A assinatura oferece uma licença para modificar as configurações do Intune.
ms.openlocfilehash: b7d87e9a174e942a6533ae034b4f4a551ae2159f
ms.sourcegitcommit: 9a057e70637dcfe06d4f729a96c02be989cf9e25
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/14/2019
ms.locfileid: "38633295"
---
# <a name="how-do-protection-features-in-microsoft-365-business-map-to-intune-settings"></a>Como é que as funcionalidades de proteção no Microsoft 365 Business são mapeadas para as definições do Intune

## <a name="android-and-ios-application-protection-settings"></a>Definições de proteção de aplicações para Android e iOS

A seguinte tabela mostra como as definições de política de aplicação para Android e iOS são mapeadas às definições do Intune.
  
Para encontrar a configuração Intune, inscreva-se com suas credenciais de administrador do Microsoft 365 Business e acesse **os centros de Administração**e, em **seguida, intune.**
  
 > [!IMPORTANT]
 > 
 > Uma assinatura Microsoft 365 Business oferece uma licença para modificar todas as configurações do Intune. Veja [a introdução a intune para começar.](https://docs.microsoft.com/intune/introduction-intune)
  
Selecione o nome &mdash; de política que &mdash; você deseja, por exemplo, a política de aplicativos para Android e, em seguida, escolha **as configurações**de política.
  
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
|Redefinir PIN quando o login falha isso muitas vezes (isso é desativado se pin não for necessário)  <br/> |Número de tentativas antes da reposição do PIN  <br/> |
|Exigir que os usuários entrem novamente depois que os aplicativos do Office estiverem ociosos (isso é desativado se o PIN não for necessário)  <br/> | Reverificar os requisitos de acesso após (minutos)  <br/>  Também define:  <br/> O **Tempo limite** é definido para minutos  <br/>  É o mesmo número de minutos que definiu no Microsoft 365 Business.  <br/> O **Período de tolerância offline** está definido para 720 minutos por predefinição  <br/> |
|Negar o acesso a ficheiros de trabalho em dispositivos desbloqueados por jailbreak ou rooting  <br/> |Bloquear execução de aplicações geridas em dispositivos desbloqueados por jailbreak ou rooting  <br/> |
|Permitir que os utilizadores copiem conteúdos das aplicações do Office para aplicações pessoais  <br/> | Restringir corte, cópia e colar com outros aplicativos  <br/>  Se a opção do Microsoft 365 Business estiver definida para **Ativado**, estas três opções também estarão definidas para **Todas as Aplicações** no Intune:  <br/> **Permitir que a aplicação transfira dados para outras aplicações** <br/> **Permitir que a aplicação receba dados de outras aplicações** <br/> **Restringir operações cortar, copiar e colar com outras aplicações** <br/>  Se a opção do Microsoft 365 Business estiver definida para **Ativado**, todas as opções do Intune estarão definidas para:  <br/> **Permitir que a aplicação transfira dados para outras aplicações** está definido para **Aplicações geridas por políticas** <br/> **Permitir que a aplicação receba dados de outras aplicações** está definido para **Todas as Aplicações** <br/> **Restringir operações cortar, copiar e colar com outras aplicações** está definido para **Aplicações geridas por políticas com colar em** <br/> |
|||
   
## <a name="windows-10-app-protection-settings"></a>Definições de proteção de aplicações para Windows 10

A seguinte tabela mostra como as definições de política de aplicação para Windows 10 são mapeadas às definições do Intune.
  
Para encontrar a configuração Intune, inscreva-se com suas credenciais de administrador do Microsoft 365 Business e acesse o [portal Azure.](https://portal.azure.com) Selecione **mais serviços**e digite intune no **filtro.** Selecione a política de aplicativos de \> proteção de **aplicativos** **intune.**
  
 > [!IMPORTANT]
 >
 >Uma assinatura Microsoft 365 Business oferece uma licença para modificar apenas as configurações intune que mapeiam as configurações disponíveis no Microsoft 365 Business. 
  
Para explorar as configurações disponíveis, selecione o nome da política que deseja e, em seguida, escolha **Geral, Atribuições, aplicativos** **permitidos,** **aplicativos isentos,** **configurações necessárias**ou **configurações avançadas** do painel de navegação esquerdo. 
  
|**Definição de política de aplicação para Windows 10**|**Definições do Intune**|
|:-----|:-----|
|Encriptar ficheiros de trabalho  <br/> |**Definições avançadas** \> **Proteção de dados**. **Revogar as chaves de encriptação ao anular a inscrição** e **Revogar o acesso a dados protegidos quando o dispositivo se inscreve para MDM** estão definidas para **Ativado**.      <br/> |
|Impeça os utilizadores de copiarem dados empresariais para ficheiros pessoais.  <br/> |**Definições necessárias** \> **Modo Windows Information Protection**. **Em** Microsoft 365 Mapas de negócios para: **Ocultar substitui,** **Off** in Microsoft 365 Mapas de negócios para: **Off**.  <br/> |
|Controlo do acesso a documentos do Office  <br/> | Se estiver definido para **Ativado** no Microsoft 365 Business,  <br/> **Definições avançadas** \> **Acesso**, **Utilizar o Windows Hello para Empresas como método para iniciar sessão no Windows** está definido para **Ativado**, com as seguintes definições adicionais:  <br/> **Definir o número mínimo de carateres necessários para o PIN** está definido para **4**.  <br/> **Configurar a utilização de letras em maiúsculas no PIN do Windows Hello para Empresas** está definido para **Não permitir a utilização de letras maiúsculas no PIN**.  <br/> **Configurar a utilização de letras em minúsculas no PIN do Windows Hello para Empresas** está definido para **Não permitir a utilização de letras minúsculas no PIN**.  <br/> **Configurar a utilização de carateres especiais no PIN do Windows Hello para Empresas** está definido para **Não permitir a utilização de carateres especiais no PIN**.  <br/> **Especificar o período de tempo (em dias) que um PIN pode ser usado antes que o sistema exija que o usuário altere** é ajustado a **0.**  <br/> **Especificar o número de PINs anteriores que podem ser associados a uma conta de utilizador que não pode ser reutilizada** está definido para **0**.  <br/> **Número de falhas de autenticação permitidas antes de o dispositivo ser eliminado** está definido para Microsoft 365 Business 5 (por predefinição).  <br/> **Período de inatividade máximo (em minutos) permitido no dispositivo após o qual ficará bloqueado por PIN ou palavra-passe** está definido tal como no Microsoft 365 Business.  <br/> |
|Ativar a recuperação de dados protegidos  <br/> |**Definições avançadas** \> **Proteção de dados**. **Mostrar o ícone de proteção de dados empresariais** e **Utilizar o Azure RMS para WIP** estão definidos para **Ativado**.      <br/> |
|Proteger localizações na nuvem da empresa adicionais  <br/> |**Definições avançadas** \> **Domínios protegidos** e **Recursos da nuvem** mostram sites do SharePoint e domínios.  <br/> |
|Os ficheiros utilizados por estas aplicações estão protegidos  <br/> |A lista de aplicações protegidas é indicada em **Aplicações permitidas**.  <br/> |
|||
   
## <a name="windows-10-device-protection-settings"></a>Definições de proteção para dispositivos Windows 10

A tabela seguinte mostra como as definições de configuração para dispositivos Windows 10 são mapeadas às definições do Intune.
  
Para encontrar a configuração Intune, inscreva-se com suas credenciais de administrador do Microsoft 365 Business e acesse o [portal Azure,](https://portal.azure.com)selecione **mais serviços**e digite intune no **Filtro,** selecione perfis de configuração de dispositivo **sinuoso.** \> **** \> **** Then select **Device policy for Windows 10** \> **Properties** \> **Settings**.
  
|**Definição de política para dispositivos Windows 10**|**Definições do Intune**|
|:-----|:-----|
|Ajudar a proteger os PCs contra vírus e outras ameaças com o Antivírus do Windows Defender  <br/> |Permitir Monitorização em Tempo Real = Ativado  <br/> Permitir Proteção da Nuvem = Ativado  <br/> Pedir aos Utilizadores Submissões de Exemplo = Enviar exemplos seguros automaticamente (submissão automática predefinida de dados que não sejam PII)  <br/> |
|Ajudar a proteger os PCs contra ameaças baseadas na Web no Microsoft Edge  <br/> |**SmartScreen** nas **definições do browser Microsoft Edge** está definido para **Obrigatório**.  <br/> |
|Desligar o ecrã do dispositivo quando estiver inativo durante (minutos)  <br/> |Máximo de minutos de inatividade até o ecrã ser bloqueado (minutos)  <br/> |
|Permitir que os utilizadores transfiram aplicações da Microsoft Store  <br/> |Política de URI Personalizada  <br/> |
|Permitir que os utilizadores acedam à Cortana  <br/> |**Geral** \> **Cortana** está definido para **bloquear** no Intune quando está definido para **desativado** no Microsoft 365 Business.  <br/> |
|Permitir que os utilizadores recebam sugestões e anúncios da Microsoft acerca do Windows  <br/> |**Destaque do Windows**, está tudo bloqueado se estiver definido para **desativado** no Microsoft 365 Business.  <br/> |
|Manter os dispositivos Windows 10 atualizados automaticamente  <br/> | Essa configuração está nas atualizações do **Microsoft Intune** \> **Service - Anéis de atualização do Windows 10,** escolha a política de **atualização para dispositivos Windows 10**e, em seguida, configurações \> de **propriedades.** ****  <br/>  Quando a configuração de negócios do Microsoft 365 estiver definida para **on,** todas as seguintes configurações são definidas:  <br/> **Ramo de serviço** está definido para **CB** (CBB quando está desativado no Microsoft 365 Business).  <br/> **Atualizações de produtos da Microsoft** está definido para **Permitir**.  <br/> **Controladores do Windows** está definido para **Permitir**.  <br/> **Comportamento de atualização automática** está definido para **Instalar automaticamente no período de manutenção** com:  <br/> **Início das horas extraordinárias** está definido para **06:00**.  <br/> **Fim das horas ativas** está definido para **22:00**.  <br/> **Período de deferimento da atualização de qualidade (dias)** está definido para **0**.  <br/> **Período de deferimento da atualização de funcionalidades (dias)** está definido para **0**.  <br/> **Modo de transferência de otimização de entrega** está definido para **HTTP aliado a peering atrás da mesma NAT**.  <br/> |
|||
   

