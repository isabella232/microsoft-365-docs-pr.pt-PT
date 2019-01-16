---
title: Acesso local recursos a partir de um dispositivo associado AD Azure no Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Obter informações sobre como obter acesso a recursos no local, tais como aplicações de linha de negócios, partilhas de ficheiros e impressoras a partir de um Azure Active Directory associado Windows 10 dispositivo.
ms.openlocfilehash: 0a5d4b0828888fcb99676223000c446479f84ddc
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982258"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>Acesso local recursos a partir de um dispositivo associado AD Azure no Microsoft 365 Business

Qualquer dispositivo Windows 10 Azure do Active Directory associado terão acesso a todos os recursos baseada na nuvem, tais como as suas aplicações do Office 365 e pode ser protegido por negócio do Microsoft 365. Para também permitir o acesso a recursos no local, como aplicações, partilhas de ficheiros e impressoras de linha de negócio (LOB), terá de sincronizar no local, Active Directory com o Active Directory de Azure utilizando [Azure AD ligar](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect). Consulte [Introdução à gestão de dispositivos no Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) para obter mais informações. 
  
## <a name="run-azure-ad-connect"></a>Executar Azure AD ligar

Conclua os seguintes passos para activar dispositivos de AD Azure associado da organização aceder a recursos no local.
  
1. Para sincronizar a utilizadores, grupos e contactos a partir do Active Directory local do Active Directory Azure, execute o Assistente de sincronização de directório e Azure AD ligar, como descrito em [Configurar a sincronização de directório para o Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
2. Depois de concluída a sincronização de directório, certifique-se Windows 10 dispositivos da sua organização são AD Azure associado. Este passo é efectuado individualmente em cada dispositivo do Windows 10. Consulte [Configurar dispositivos do Windows para utilizadores empresariais do Microsoft 365](set-up-windows-devices.md) para obter detalhes. 
    
3. Depois dos dispositivos de 10 de Windows Azure AD associado, cada utilizador deverá reiniciar os dispositivos e o início de sessão com as respectivas credenciais de Microsoft 365 Business. Todos os dispositivos terão agora acesso aos recursos do local bem.
    
Não existem passos adicionais são necessários para aceder a recursos para Azure AD associado dispositivos no local. Esta é a funcionalidade incorporada disponível no Windows 10. 
  
Se a organização não estiver preparada para implementar na Azure AD associado dispositivo configuração acima descrito, considere a definição de [configuração do dispositivo híbrido Azure AD associado](manage-windows-devices.md).
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a>Considerações sobre quando colocar os dispositivos Windows Azure AD

Se estiver AD Azure aderir a um dispositivo do Windows que foi anteriormente associados ao domínio ou num grupo de trabalho, terá de considerar as seguintes limitações:
  
- Quando adere a um dispositivo Azure AD, cria um novo utilizador sem fazer referência um perfil existente. Para corrigir este problema, perfis tem de ser migrados manualmente. Um perfil de utilizador contém informações como favoritos, ficheiros locais, as definições do browser, definições do menu Iniciar, etc. Uma abordagem melhor será localizar uma ferramenta de outros fabricantes para mapear os ficheiros existentes e as definições para o novo perfil
    
- Se o dispositivo estiver a utilizar objectos de política de grupo (GPO), alguns GPOs poderão não ter um comparáveis [Configuração Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) no Intune. Execute a [ferramenta MMAT](https://www.microsoft.com/download/details.aspx?id=45520) para localizar os CSPs comparáveis para os GPOs existentes. 
    
- Os utilizadores não conseguirão autenticar para aplicações que dependem de autenticação do Active Directory. Para lidar com avaliar a utilização de uma aplicação de legacy e considere a hipótese de actualizar para uma aplicação que utiliza autenticação moderna se possível.
    
- Detecção de impressora do Active Directory não irá funcionar. Para corrigir este problema, forneça caminhos directa de impressora para todos os utilizadores ou tirar partido de [Impressão de nuvem de híbridos](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).
    

