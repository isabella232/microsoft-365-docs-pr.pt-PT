---
title: Microsoft 365 Business Premium funcionalidades de segurança e conformidade
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-security-compliance
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Conheça as funcionalidades de segurança que vêm com o Microsoft 365 Business Premium para ajudar a salvaguardar os seus dados em Computadores, telefones e tablets.
ms.openlocfilehash: f04a998c74128edac306167617e073c412fce2ea
ms.sourcegitcommit: dcb97fbfdae52960ae62b6faa707a05358193ed5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/25/2021
ms.locfileid: "51198417"
---
# <a name="microsoft-365-business-premium-security-and-compliance-features"></a>Microsoft 365 Business Premium funcionalidades de segurança e conformidade

O Microsoft 365 Business Premium oferece funcionalidades de segurança simplificadas para ajudar a salvaguardar os seus dados em Computadores, telefones e tablets.
    
## <a name="microsoft-365-admin-center-security-features"></a>Microsoft 365 admin center funcionalidades de segurança

Pode gerir muitas das funcionalidades de segurança Do Microsoft 365 Business Premium no centro de administração, o que lhe dá uma forma simplificada de ligar ou desligar estas funcionalidades. No centro de administração, pode fazer o seguinte:
  
- [Definir definições de gestão de aplicações para dispositivos Android ou iOS](app-protection-settings-for-android-and-ios.md) . 
    
    Estas definições incluem a eliminação de ficheiros de um dispositivo inativo após um período de definição, encriptando ficheiros de trabalho, exigindo que os utilizadores estabeleçam um PIN, e assim por diante.
    
- [Definir definições de proteção de aplicações para dispositivos Windows 10](protection-settings-for-windows-10-devices.md) . 
    
    Estas definições podem ser aplicadas aos dados da empresa em dispositivos pertencentes à empresa ou pessoalmente.
    
- [Definir as definições de proteção do dispositivo para dispositivos Windows 10](protection-settings-for-windows-10-pcs.md) . 
    
    Pode ativar a encriptação [BitLocker](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions) para ajudar a proteger os dados no caso de um dispositivo ser perdido ou roubado, e permitir que o [Windows Exploit Guard](/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) forneça proteção avançada contra ransomware. 
    
- [Remover dados empresariais de dispositivos](remove-company-data.md)
    
    Pode limpar remotamente os dados da empresa se um dispositivo for perdido, roubado ou se um empregado deixar a sua empresa.
    
- [Redefinir os dispositivos do Windows 10 para as suas definições de fábrica](reset-devices-to-factory-settings.md) . 
    
    Pode redefinir todos os dispositivos do Windows 10 que tenham as definições de proteção do dispositivo aplicadas aos mesmos.
    
## <a name="additional-security-features"></a>Funcionalidades de segurança adicionais 

Funcionalidades avançadas no Microsoft 365 Business Premium estão disponíveis para ajudá-lo a proteger o seu negócio contra ameaças cibernéticas e salvaguardar informações sensíveis.
  
- **[Microsoft Defender para o Office 365](../security/office-365-security/defender-for-office-365.md)**
    
    O Microsoft Defender para o Office 365 ajuda a proteger o seu negócio contra ataques sofisticados de phishing e ransomware concebidos para comprometer a informação dos funcionários ou do cliente. As funcionalidades incluem:
    
  - Digitalização sofisticada de anexos e análise alimentada por IA para detetar e descartar mensagens perigosas.
    
  - Verificações automáticas de links por e-mail para avaliar se fazem parte de um esquema de phishing. Isto o impede de aceder a sites inseguros.

- **[As capacidades completas do Intune no portal Azure](/mem/intune/fundamentals/what-is-intune)**
    
    O acesso ao centro de administração Intune no portal Azure permite-lhe configurar funcionalidades de segurança adicionais, como a gestão de dispositivos MacOS, iPhone e Android, juntamente com a gestão avançada de dispositivos para windows, que não estão disponíveis através do centro de administração microsoft 365.
- **Mesmo [acesso condicional](/azure/active-directory/conditional-access/overview) como plano Azure AD Premium P1**


    O Acesso Condicional pode ajudar a proteger a sua organização do risco de inscrição, tentativas de acesso a partir de uma rede inesperada ou local, tentativas de acesso de tipos de dispositivos de risco, e assim por diante. As políticas de acesso condicional são aplicadas após a conclusão da primeira autenticação, e utiliza sinais do primeiro evento de autenticação para determinar se a tentativa de acesso deve ser aprovada, negada ou se é necessária mais provas (como uma segunda forma de identificação).

    As funcionalidades de acesso condicional incluídas são:

    - Acesso com base no nome de utilizador, grupo e papel
    - Acesso [com base numa aplicação](/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Acesso com base na localização;](/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration)  apenas permitir o acesso a partir de gamas IP fidedignas ou países específicos 
    - Exigir MFA para acesso
    - Bloquear acesso a apps que usam [autenticação de legado](/azure/active-directory/conditional-access/block-legacy-authentication)
    - Exigir que as aplicações utilizem a [proteção de aplicações Intune](/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Autenticação personalizada, como MFA com fornecedores de terceiros, por exemplo DUO.
   
    Outras características:
    - [Autosserviço de senha reset](/azure/active-directory/authentication/concept-sspr-customization) para híbrido Azure AD
    
## <a name="compliance-features"></a>Funcionalidades de conformidade

A sua subscrição Microsoft 365 Business Premium inclui funcionalidades que o ajudam a manter a conformidade e os padrões regulamentares.

- **[Visão geral das políticas de prevenção de perdas de dados](../compliance/data-loss-prevention-policies.md)** (DLP). 
    
    Pode configurar o DLP para detetar automaticamente informações sensíveis, como números de cartões de crédito, números de segurança social, e assim por diante, para evitar a sua partilha inadvertida fora da sua empresa.
    
- **[Arquivo do Exchange Online](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    A licença de Arquivamento Online de Intercâmbio permite que as mensagens sejam facilmente arquivadas com cópia de segurança contínua de dados. Armazena todos os e-mails de um utilizador, incluindo itens eliminados, caso sejam necessários mais tarde para serem descobertos ou restaurados. Além disso, pode usar diferentes políticas de retenção para preservar dados de e-mail para contenção de litígios, eDiscovery ou para cumprir os requisitos de conformidade.
    
- **[Etiquetas de confidencialidade](../compliance/sensitivity-labels.md)**

   O Microsoft 365 Business Premium inclui todas as funcionalidades do Plano de [Proteção de Informação Azure 1](https://go.microsoft.com/fwlink/p/?linkid=871407). Com este plano, pode criar **etiquetas de sensibilidade** que lhe permitam controlar o acesso a informações sensíveis em e-mails e documentos, com controlos como "Não encaminhar" e "Não copiar". Também pode classificar informações confidenciais como "Confidenciais" e especificar como as informações classificadas podem ser partilhadas fora e dentro do negócio. A encriptação de nível empresarial é fácil de aplicar a e-mails e documentos para manter a sua informação privada. Também pode instalar o complemento do cliente Azure Information Protection para aplicações do Office. Para mais informações, consulte o cliente unificado de [rotulagem Azure Information Protection](/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history). Para etiquetas de sensibilidade, instale o **AzInfoProtection_UL.exe**.

Pode gerir estas funcionalidades no Centro de Conformidade de Segurança &amp; e no centro de administração Intune. Com o tempo, os controlos simplificados serão adicionados ao centro de administração microsoft 365.
  
    
## <a name="faq"></a>FAQ

 ### <a name="are-these-security-features-available-in-all-markets"></a>Estas funcionalidades de segurança estão disponíveis em todos os mercados?
  
Sim, estas funcionalidades estão disponíveis em todos os mercados onde o Microsoft 365 Business Premium é vendido.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Como encontro o &amp; Centro de Conformidade de Segurança?
  
1. [Inscreva-se no Microsoft 365 Business Premium](https://portal.microsoft.com/) utilizando as suas credenciais de administração. 
    
2. Na navegação esquerda, localiza os **centros de administração** e expande-o. 
    
    ![No navegador esquerdo no centro de administração microsoft 365, escolha centros de administração.](../media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Escolha **&amp; a Conformidade de Segurança** para ir ao Centro de Conformidade de &amp; Segurança.
