---
title: Microsoft 365 Recursos de segurança e conformidade de negócios
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
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Saiba mais sobre os recursos de segurança que vêm com o Microsoft 365 Business.
ms.openlocfilehash: 98eb0c2015ed6088b2d5e8621c8e72a5b63f2a17
ms.sourcegitcommit: 58a7bd70a4bcf52530baf5f82507fd5dc4455fd9
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/03/2019
ms.locfileid: "39668854"
---
# <a name="microsoft-365-business-security-and-compliance-features"></a>Microsoft 365 Recursos de segurança e conformidade de negócios

O Microsoft 365 Business oferece recursos de segurança simplificados para ajudar a proteger seus dados em PCs, telefones e tablets.
    
## <a name="microsoft-365-business-admin-center-security-features"></a>Microsoft 365 Características de segurança do centro de administração de negócios

[![Etiqueta que informa que o centro de administração está a mudar e que pode encontrar mais detalhes em aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Você pode gerenciar muitos dos recursos de segurança do Microsoft 365 Business no centro de administração, o que lhe dá uma maneira simplificada de ativar ou desligar esses recursos. No centro de administração, você pode fazer o seguinte:
  
- Definir configurações de gerenciamento de [aplicativos para dispositivos Android ou iOS.](app-protection-settings-for-android-and-ios.md) 
    
    Essas configurações incluem a exclusão de arquivos de um dispositivo inativo após um período definido, criptografação de arquivos de trabalho, exigindo que os usuários definam um PIN e assim por diante.
    
- [Definir configurações de proteção de aplicativos para dispositivos Windows 10.](protection-settings-for-windows-10-devices.md) 
    
    Essas configurações podem ser aplicadas aos dados da empresa em dispositivos de propriedade da empresa ou de propriedade pessoal.
    
- [Ajuste as configurações de proteção do dispositivo para dispositivos Windows 10.](protection-settings-for-windows-10-pcs.md) 
    
    Você pode habilitar a criptografia [do BitLocker](https://go.microsoft.com/fwlink/p/?linkid=871405) para ajudar a proteger os dados caso um dispositivo seja perdido ou roubado e permita que o [Windows Exploit Guard](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) forneça proteção avançada contra ransomware. 
    
- [Remover dados empresariais de dispositivos](remove-company-data.md)
    
    Você pode limpar remotamente os dados da empresa se um dispositivo for perdido, roubado ou um funcionário deixar sua empresa.
    
- [Redefinir os dispositivos Windows 10 em suas configurações de fábrica.](reset-devices-to-factory-settings.md) 
    
    Você pode redefinir todos os dispositivos Windows 10 que tenham configurações de proteção do dispositivo aplicadas a eles.
    
## <a name="additional-security-features"></a>Funcionalidades de segurança adicionais 

Recursos avançados no Microsoft 365 Business estão disponíveis para ajudá-lo a proteger seus negócios contra ameaças cibernéticas e proteger informações confidenciais.
  
- **[Office 365 Advanced Threat Protection](https://support.office.com/article/e100fe7c-f2a1-4b7d-9e08-622330b83653)**
    
    A Proteção avançada de ameaças (ATP) ajuda a proteger seus negócios contra ataques sofisticados de phishing e ransomware projetados para comprometer as informações dos funcionários ou clientes. Os recursos incluem:
    
  - Digitalização sofisticada de anexos e análises alimentadas por IA para detectar e descartar mensagens perigosas.
    
  - Verificações automáticas de links no e-mail para avaliar se eles fazem parte de um esquema de phishing. Isso o mantém a salvo de acessar sites inseguros.

- **[As capacidades completas de Sintonia no portal Azure](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Acessar o centro de administração Intune no portal Azure permite configurar recursos de segurança adicionais, como gerenciamento de dispositivos MacOS, iPhone e dispositivos Android, juntamente com gerenciamento avançado de dispositivos para Windows, que não estão disponíveis através da Microsoft Centro de administração de negócios 365.
- **Mesmo [acesso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) do plano Azure AD P1**


    O Acesso Condicional pode ajudar a proteger sua organização contra riscos de login, tentativas de acesso de uma rede ou local inesperado, tentativas de acesso de tipos de dispositivos de risco e assim por diante. As políticas de acesso condicional são aplicadas após a primeira autenticação ser concluída e usam sinais do primeiro evento de autenticação para determinar se a tentativa de acesso deve ser aprovada, negada ou se mais provas (como uma segunda forma de identificação) é necessário.

    Os recursos de acesso condicional incluídos são:

    - Acesso com base no nome de usuário, grupo e função
    - Acesso [com base em um aplicativo](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Acesso com base na localização;](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration)  apenas permitir o acesso de faixas de IP confiáveis ou países específicos 
    - Exigir MFA para acesso
    - Bloquear o acesso a aplicativos que usam [autenticação herdada](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication)
    - Exigir aplicativos tp usar [proteção de aplicativos Intune](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Autenticação personalizada, como mfa com provedores de terceiros, por exemplo DUO.
   
    Outras características:
    - [Redefinição de senha de autoatendimento](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization) para anúncio híbrido do Azure
    
## <a name="compliance-features"></a>Recursos de conformidade

Sua assinatura Microsoft 365 Business inclui recursos que ajudam a manter padrões regulatórios e de conformidade.

- **[Visão geral das políticas de prevenção de perdas de dados](https://support.office.com/article/1966b2a7-d1e2-4d92-ab61-42efbb137f5e)** (DLP). 
    
    Você pode configurar o DLP para detectar automaticamente informações confidenciais, como números de cartão de crédito, números de segurança social e assim por diante, para evitar seu compartilhamento inadvertido fora de sua empresa.
    
- **[Arquivo do Exchange Online](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    A licença de arquivamento on-line de intercâmbio permite que as mensagens sejam facilmente arquivadas com backup contínuo de dados. Ele armazena todos os e-mails de um usuário, incluindo itens excluídos, caso sejam necessários mais tarde para descoberta ou restauração. Além disso, você pode usar diferentes políticas de retenção para preservar dados de e-mail para litígios, eDiscovery ou para atender aos requisitos de conformidade.
    
- **[Etiquetas de confidencialidade](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)**

   Microsoft 365 Business inclui todos os recursos do [Plano de Proteção de Informações Azure 1](https://go.microsoft.com/fwlink/p/?linkid=871407). Com esse plano, você pode criar **rótulos** de sensibilidade que permitem controlar o acesso a informações confidenciais em e-mail e documentos, com controles como "Não encaminhada" e "Não copie". Você também pode classificar informações confidenciais como "confidenciais" e especificar como informações classificadas podem ser compartilhadas fora e dentro da empresa. A criptografia de nível corporativo é fácil de aplicar a e-mails e documentos para manter suas informações privadas. Você também pode instalar o complemento do cliente de Proteção de Informações do Azure para aplicativos do Office. Para mais informações, consulte o cliente unificado de rotulagem da [Azure Information Protection.](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history) Para rótulos de sensibilidade, instale o **AzInfoProtection_UL.exe**.

Você pode gerenciar esses &amp; recursos no centro de conformidade de segurança e no centro de administração Intune. Com o tempo, os controles simplificados serão adicionados ao centro de administração microsoft 365 business.
  
    
## <a name="faq"></a>FAQ

 ### <a name="are-these-security-features-available-in-all-markets"></a>Esses recursos de segurança estão disponíveis em todos os mercados?
  
Sim, esses recursos estão disponíveis em todos os mercados onde o Microsoft 365 Business é vendido.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Como encontro o &amp; centro de conformidade de segurança?
  
1. [Entre no Microsoft 365 Business](https://portal.microsoft.com/) usando suas credenciais de administrador. 
    
2. Na navegação esquerda, localizar **centros de administração** e expandi-lo. 
    
    ![Na navegação esquerda no centro de administração microsoft 365, escolha os centros de administração.](media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Escolha a conformidade de &amp; **segurança &amp; ** para ir ao centro de conformidade de segurança.
