---
title: Recursos de conformidade e segurança do Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Saiba mais sobre os recursos de segurança que vêm com o Microsoft 365 Business.
ms.openlocfilehash: 6b8fc215b95913e1beef3a3715119b947a7af406
ms.sourcegitcommit: 7690c8bfdea6e6d245cfa7c5b09b913b092cde0a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/23/2019
ms.locfileid: "37121164"
---
# <a name="microsoft-365-business-security-and-compliance-features"></a>Recursos de conformidade e segurança do Microsoft 365 Business

O Microsoft 365 Business oferece recursos de segurança simplificados para ajudar a proteger seus dados em PCs, telefones e tablets.
    
## <a name="microsoft-365-business-admin-center-security-features"></a>Microsoft 365 Business Admin Center recursos de segurança

[![Label para que você saiba que o centro de administração está mudando e você pode encontrar mais detalhes em aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Você pode gerenciar muitos dos recursos de segurança do Microsoft 365 Business no centro de administração, o que oferece uma maneira simplificada de ativar ou desativar esses recursos. No centro de administração, você pode fazer o seguinte:
  
  
- [Defina as configurações de gerenciamento de aplicativos para dispositivos Android ou Ios](app-protection-settings-for-android-and-ios.md) . 
    
    Essas configurações incluem a exclusão de arquivos de um dispositivo inativo após um período definido, criptografando arquivos de trabalho, exigindo que os usuários definam um PIN, etc.
    
- [Defina as configurações de proteção de aplicativos para dispositivos Windows 10](protection-settings-for-windows-10-devices.md) . 
    
    Essas configurações podem ser aplicadas aos dados da empresa em ambos os dispositivos pertencentes à empresa ou de propriedade pessoal.
    
- [Defina as configurações de proteção do dispositivo para dispositivos Windows 10](protection-settings-for-windows-10-pcs.md) . 
    
    Você pode habilitar a criptografia [BitLocker](https://go.microsoft.com/fwlink/p/?linkid=871405) para ajudar a proteger os dados caso um dispositivo seja perdido ou roubado e habilitar o [Windows Exploit Guard](https://go.microsoft.com/fwlink/p/?linkid=871404) para fornecer proteção avançada contra ransomware. 
    
- [Remover dados empresariais de dispositivos](remove-company-data.md)
    
    Você pode limpar remotamente os dados da empresa se um dispositivo for perdido, roubado ou um funcionário deixar sua empresa.
    
- [Redefinir dispositivos Windows 10 para suas configurações de fábrica](reset-devices-to-factory-settings.md) . 
    
    Você pode redefinir todos os dispositivos Windows 10 que tenham as configurações de proteção do dispositivo aplicadas a eles.
    
## <a name="additional-security-features"></a>Funcionalidades de segurança adicionais 

Os recursos avançados do Microsoft 365 Business estão disponíveis para ajudá-lo a proteger seus negócios contra ameaças cibernéticas e proteger informações confidenciais.
  
- **[Proteção avançada contra ameaças do Office 365](https://support.office.com/article/e100fe7c-f2a1-4b7d-9e08-622330b83653)**
    
    A proteção avançada contra ameaças (ATP) ajuda a proteger sua empresa contra ataques sofisticados de phishing e ransomware projetados para comprometer informações de funcionários ou clientes. As características incluem:
    
  - Análise sofisticada de anexos e análises com tecnologia de ia para detectar e descartar mensagens perigosas.
    
  - Verificações automáticas de links no e-mail para avaliar se eles fazem parte de um esquema de phishing. Isso mantém você seguro de acessar sites não seguros.

- **[Os recursos completos do Intune no portal do Azure](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Acessar o centro de administração do Intune no portal do Azure permite que você configure recursos de segurança adicionais, como o gerenciamento de dispositivos MacOS, iPhone e dispositivos Android, juntamente com o gerenciamento avançado de dispositivo para Windows, que não estão disponíveis por meio da Microsoft 365 centro de administração de negócios.
- **Mesmo [acesso condicional](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/overview) como plano do Azure ad P1**

    O acesso condicional pode ajudar a proteger sua organização contra o risco de login, as tentativas de acesso de uma rede ou localidade inesperada, tentativas de acesso formam tipos de dispositivos arriscados e assim por diante. As diretivas de acesso condicional são impostas após a conclusão da primeira autenticação, e ele usa sinais do primeiro evento de autenticação para determinar se o acesso tentado deve ser aprovado, nega ou f mais prova (como a segunda forma de identificação) é Necessário.

    Os recursos de acesso condicional incluídos são:

    - Acesso baseado em nome de usuário, grupo e função
    - Acesso [baseado em um aplicativo](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Acesso com base no local](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  apenas permitir o acesso a partir de intervalos de IP confiáveis ou países específicos 
    - Exigir MFA para acesso
    - Bloquear o acesso a aplicativos que usam a [autenticação herdada](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication)
    - Exigir aplicativos TP usar [proteção de aplicativo do Intune](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Autenticação personalizada, como MFA com provedores terceirizados, por exemplo, DUO.
   
    Outras características:
    - [Redefinição de senha de autoatendimento](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization) para o Azure ad híbrido
    
## <a name="compliance-features"></a>Recursos de conformidade

Sua assinatura do Microsoft 365 Business inclui recursos que ajudam a manter padrões de conformidade e regulatórios.

- **[Visão geral das políticas de prevenção de perda de dados](https://support.office.com/article/1966b2a7-d1e2-4d92-ab61-42efbb137f5e)** (DLP). 
    
    Você pode configurar o DLP para detectar automaticamente informações confidenciais, como números de cartão de crédito, números de segurança social, etc. para evitar sua partilha inadvertida fora de sua empresa.
    
- **[Arquivo do Exchange Online](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    A licença de arquivamento do Exchange Online permite que as mensagens sejam facilmente arquivadas com backup contínuo de dados. Ele armazena todos os emails de um usuário, incluindo itens excluídos, caso eles sejam necessários posteriormente para descoberta ou restauração. Além disso, você pode usar políticas de retenção diferentes para preservar dados de email para retenções de litígio, eDiscovery ou para atender aos requisitos de conformidade.
    
- **[Proteção de informações do Azure](https://go.microsoft.com/fwlink/p/?linkid=871406)**
    
    A proteção de informações ajuda você a controlar o acesso a informações confidenciais em emails e documentos com controles como "não encaminhar" e "não copiar". Você também pode classificar informações confidenciais como "confidenciais" e especificar como as informações classificadas podem ser compartilhadas fora e dentro da empresa. A criptografia de nível corporativo é fácil de aplicar a emails e documentos para manter suas informações privadas. O Microsoft 365 Business inclui todos os recursos do [plano de proteção de informações do Azure 1](https://go.microsoft.com/fwlink/p/?linkid=871407). Você também pode instalar o suplemento do cliente do Azure Information Protection para aplicativos do Office. Para obter mais detalhes, consulte [Guia do administrador do cliente do Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide).

Você pode gerenciar esses recursos no centro de &amp; conformidade de segurança e no centro de administração do Intune. Ao longo do tempo, os controles simplificados serão adicionados ao centro de administração do Microsoft 365 Business.
  
    
## <a name="faq"></a>FAQ

 ### <a name="are-these-security-features-available-in-all-markets"></a>Estes recursos de segurança estão disponíveis em todos os mercados?
  
Sim, esses recursos estão disponíveis em todos os mercados onde o Microsoft 365 Business é vendido.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Como encontro o centro de conformidade &amp; de segurança?
  
1. [Entre no Microsoft 365 Business](https://portal.microsoft.com/) usando suas credenciais de administrador. 
    
2. No NAV esquerdo, localize **centros de administração** e expandi-lo. 
    
    ![No NAV esquerdo no centro de administração do Microsoft 365, escolha centros de administração.](media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Escolha **conformidade &amp; de segurança** para ir para &amp; o centro de conformidade de segurança.