---
title: Microsoft 365 Empresas Premium funcionalidades de segurança e conformidade
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: Saiba mais sobre as funcionalidades de segurança que estão Microsoft 365 Empresas Premium ajudar a proteger os seus dados em PCs, telemóveis e tablets.
ms.openlocfilehash: 974204e100d3228f78406aca4acce67a889b08c3
ms.sourcegitcommit: 05f40904f8278f53643efa76a907968b5c662d9a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/30/2021
ms.locfileid: "52113472"
---
# <a name="microsoft-365-business-premium-security-and-compliance-features"></a>Microsoft 365 Empresas Premium funcionalidades de segurança e conformidade

Microsoft 365 Empresas Premium oferece funcionalidades de segurança simplificadas para ajudar a proteger os seus dados em PCs, telemóveis e tablets.
    
## <a name="microsoft-365-admin-center-security-features"></a>Microsoft 365 funcionalidades de segurança do centro de administração

Pode gerir muitas das funcionalidades de Microsoft 365 Empresas Premium segurança do Centro de administração, o que lhe proporciona uma forma simplificada de ativo e desativo destas funcionalidades. No centro de administração, pode fazer o seguinte:
  
- [Defina as definições de gestão de aplicações para dispositivos Android ou iOS.](app-protection-settings-for-android-and-ios.md) 
    
    Estas definições incluem eliminar ficheiros de um dispositivo inativo após um período definido, encriptar ficheiros de trabalho, requerer que os utilizadores definam um PIN, entre outros.
    
- [Defina as definições de proteção de aplicações para Windows 10 dispositivos](protection-settings-for-windows-10-devices.md) . 
    
    Estas definições podem ser aplicadas a dados da empresa em dispositivos de propriedade pessoal ou de propriedade pessoal.
    
- [Defina as definições de proteção para dispositivos Windows 10 dispositivos](protection-settings-for-windows-10-pcs.md) . 
    
    Pode ativar a [BitLocker](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions) para ajudar a proteger os dados no caso de um dispositivo ser perdido ou roubado e permitir que [o Windows Exploit Guard](/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) forneça proteção avançada contra ransomware. 
    
- [Remover dados empresariais de dispositivos](remove-company-data.md)
    
    Pode eliminar remotamente os dados da empresa se um dispositivo for perdido, roubado ou se um funcionário sair da sua empresa.
    
- [Repor Windows 10 dispositivos para as definições de fábrica.](reset-devices-to-factory-settings.md) 
    
    Pode repor todos os Windows 10 que tenham definições de proteção de dispositivos aplicadas.
    
## <a name="additional-security-features"></a>Funcionalidades de segurança adicionais 

As funcionalidades avançadas do Microsoft 365 Empresas Premium estão disponíveis para o ajudar a proteger a sua empresa contra ciberameaças e proteger informações confidenciais.
  
- **[Microsoft Defender para Office 365](../security/office-365-security/defender-for-office-365.md)**
    
    O Microsoft Defender para Office 365 ajuda a proteger a sua empresa contra ataques de phishing e ransomware sofisticados concebidos para comprometer as informações dos clientes ou funcionários. As funcionalidades incluem:
    
  - Análise sofisticada de anexos e análises com tecnologia de LA para detetar e eliminar mensagens perigosas.
    
  - Verificações automáticas de ligações no e-mail para avaliar se fazem parte de um esquema de phishing. Isto impede o acesso a sites não seguros.

- **[As funcionalidades completas do Intune no portal do Azure](/mem/intune/fundamentals/what-is-intune)**
    
    Aceder ao centro de administração do Intune no portal do Azure permite-lhe configurar funcionalidades de segurança adicionais, como a gestão de dispositivos MacOS, iPhone e dispositivos Android, juntamente com a gestão de dispositivos avançada para o Windows, que não estão disponíveis através do centro de administração do Microsoft 365.
- **O [mesmo Acesso Condicional](/azure/active-directory/conditional-access/overview) que o Azure AD Premium plano P1**


    O Acesso Condicional pode ajudar a proteger a sua organização contra riscos de funcionamento, tentativas de acesso de uma rede ou local inesperada, tentativas de acesso de tipos de dispositivos arriscados, entre outros. As políticas de Acesso Condicional são impostas após a conclusão da primeira autenticação e utiliza sinais do primeiro evento de autenticação para determinar se o acesso tentado deve ser aprovado, recusado ou se é necessária mais prova (como uma segunda forma de identificação).

    As funcionalidades de acesso condicional incluídas são:

    - Acesso com base no nome de utilizador, grupo e função
    - Access [com base numa aplicação](/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Acesso com base na localização](/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  permitir apenas o acesso a partir de intervalos de IP de confiança ou de países específicos 
    - Exigir mfa para acesso
    - Bloquear o acesso a aplicações que utilizam [a autenticação legada](/azure/active-directory/conditional-access/block-legacy-authentication)
    - Exigir que as aplicações utilizem a [proteção da aplicação Intune](/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Autenticação personalizada, como MFA com fornecedores terceiros, por exemplo DUO.
   
    Outras funcionalidades:
    - [Reposição de palavra-passe self-service](/azure/active-directory/authentication/concept-sspr-customization) para o Azure AD híbrido
    
## <a name="compliance-features"></a>Funcionalidades de conformidade

A Microsoft 365 Empresas Premium subscrição inclui funcionalidades que o ajudam a manter as normas de conformidade e regulamentação.

- **[Saiba mais sobre a prevenção de perda de dados](../compliance/dlp-learn-about-dlp.md))** (DLP). 
    
    Pode configurar o DLP para detetar automaticamente informações confidenciais, como números de cartões de crédito, números de segurança social, entre outro, para impedir a partilha inadvertida dos mesmos fora da sua empresa.
    
- **[Arquivo do Exchange Online](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Arquivo de Exchange Online licença permite que as mensagens sejam facilmente arquivadas com uma cópia de segurança de dados contínua. Armazena todos os e-mails de um utilizador, incluindo itens eliminados, caso sejam necessários mais tarde para deteção ou restauro. Além disso, pode utilizar diferentes políticas de retenção para preservar os dados de e-mail para deteções de litigações, deteção de dados eletrónicos ou para cumprir os requisitos de conformidade.
    
- **[Etiquetas de confidencialidade](../compliance/sensitivity-labels.md)**

   Microsoft 365 Empresas Premium inclui todas as funcionalidades do [Plano Azure Information Protection 1.](https://go.microsoft.com/fwlink/p/?linkid=871407) Com este plano, pode criar **etiquetas** de Confidencialidade que lhe permitem controlar o acesso a informações confidenciais em e-mails e documentos, com controlos como "Não encaminhar" e "Não copiar". Também pode classificar informações confidenciais como "Confidencial" e especificar a forma como as informações classificadas podem ser partilhadas fora e dentro da empresa. A encriptação de nível empresarial é fácil de aplicar ao e-mail e aos documentos para manter as suas informações privadas. Também pode instalar o add-in do cliente do Azure Information Protection para Office aplicações. Para obter mais informações, consulte [Cliente de etiquetagem unificado do Azure Information Protection.](/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history) Para etiquetas de sensibilidade, instale **oAzInfoProtection_UL.exe**.

Pode gerir estas funcionalidades no centro de &amp; Conformidade de Segurança e no centro de administração do Intune. Ao longo do tempo, os controlos simplificados serão adicionados ao Microsoft 365 de administração.
  
    
## <a name="faq"></a>FAQ

 ### <a name="are-these-security-features-available-in-all-markets"></a>Estas funcionalidades de segurança estão disponíveis em todos os mercados?
  
Sim, estas funcionalidades estão disponíveis em todos os mercados onde o Microsoft 365 Empresas Premium é vendido.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Como posso encontrar o centro de &amp; Conformidade de Segurança?
  
1. [Inscreva-se no Microsoft 365 Empresas Premium](https://portal.microsoft.com/) com as suas credenciais de administrador. 
    
2. No navegador esquerdo, localize **Centros de administração e** expanda-os. 
    
    ![No navegador esquerdo no centro de administração do Microsoft 365, selecionar Centros de administração.](../media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. **Selecionar &amp; Conformidade de** Segurança para ir para Centro de conformidade de &amp; segurança.
