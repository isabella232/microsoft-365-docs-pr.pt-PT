---
title: Aumentar a proteção contra ameaças para o Microsoft 365 Business
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
description: Configurar as funcionalidades de conformidade para evitar a perda de dados e os dados sensíveis à etiqueta.
ms.openlocfilehash: 09619de03aafde37106fb3942890b457c488ad43
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593411"
---
# <a name="set-up-compliance-features"></a>Configurar funcionalidades de conformidade

O Seu Microsoft 365 Business vem com funcionalidades para proteger os seus dados e dispositivos e ajudá-lo a manter as informações sensíveis dos seus e dos seus clientes seguras.

## <a name="set-up-dlp-features"></a>Configurar as funcionalidades dLP

Consulte [Criar uma política de DLP](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) a partir de um modelo para um exemplo sobre como criar uma política de proteção contra informações pessoalmente identificáveis (PII). 
  
DLP vem com muitos modelos de política prontos a usar para muitos locais diferentes. Por exemplo, Australia Financial Data, Canada Personal Information Act, Dados Financeiros dos EUA, e assim por diante. Veja [o que os modelos de política do DLP incluem](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) para uma lista completa. Todos estes modelos podem ser ativados semelhantes ao exemplo do modelo PII. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Configurar a retenção de e-mails com o Arquivo Online de Troca

 **As** funcionalidades de licença de arquivo online exchange ajudam a manter a conformidade e os padrões regulamentares preservando o conteúdo de e-mail para eDiscovery. Também ajuda a reduzir o seu risco se houver um processo judicial, e fornece uma maneira de recuperar dados após uma violação de segurança ou quando precisa de recuperar itens apagados. Pode utilizar litígios para preservar todo o conteúdo do utilizador ou utilizar políticas de retenção para personalizar o que pretende preservar.
  
**Detenção de litígios:** Pode preservar todos os conteúdos da caixa de correio, incluindo itens eliminados, colocando toda a caixa de correio de um utilizador em espera de litígios. 
    
Para colocar uma caixa de correio em espera de litígios, no centro de Administração:
    
1. Na navegação à esquerda, vá aos **utilizadores** \> **ativos.**
    
2. Selecione um utilizador cuja caixa de correio pretende colocar em espera de litígios. No painel do utilizador, expandir **as definições de Correio**, e ao lado de mais **configurações,** escolha **propriedades de Edição Exchange**.
    
3. Na página da caixa de correio para o utilizador, escolha as funcionalidades da caixa de correio ** no v ' à esquerda e, em seguida, escolha o link **Enable** sob **a porção de Litígios**.
    
4. Na **** caixa de diálogo, pode especificar a duração do processo no campo de duração do **processo.** Deixe o campo vazio se quiser colocar um porão infinito. Também pode adicionar notas e direcionar o proprietário da caixa de correio para um site que poderá ter de explicar mais sobre o processo. \>**Salvar.**
    
**Retenção:** Pode permitir que políticas de retenção personalizadas, por exemplo, preservem por um período de tempo específico ou apaguem conteúdos permanentemente no final do período de retenção. Para saber mais, consulte [a visão geral das políticas de retenção.](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423)

## <a name="set-up-sensitivity-labels"></a>Configurar rótulos de sensibilidade

As etiquetas de sensibilidade vêm com o Plano 1 de Proteção de Informação Azure (AIP) e ajudam-no a classificar e a proteger opcionalmente os seus documentos e e-mails, aplicando etiquetas. As etiquetas podem ser aplicadas automaticamente por administradores que definem regras e condições, manualmente pelos utilizadores, ou utilizando uma combinação em que os utilizadores recebem recomendações.

Para configurar etiquetas de sensibilidade, veja criar e gerir o vídeo das etiquetas de [sensibilidade.](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)



### <a name="install-the-azure-information-protection-client-manually"></a>Instale manualmente o cliente de Proteção de Informação Do Azure

Para instalar manualmente o cliente AIP:

1. Baixe **AzinfoProtection_UL.exe** do centro de [descarregamento](https://www.microsoft.com/download/details.aspx?id=53018)da Microsoft .
 
2. Pode verificar se a instalação funcionou visualizando um documento Word e certificando-se de que a opção **Sensibilidade** está disponível no separador **Home.**
<br/>![A questão da proteção cai num documento word.](media/word-sensitivity.png)

Para mais informações, consulte [Instalar o cliente.](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3)
