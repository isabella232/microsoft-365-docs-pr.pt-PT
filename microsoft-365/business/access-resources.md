---
title: Acessar recursos locais de um dispositivo ingressado no Azure AD no Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: M365-subscription-management
localization_priority: Normal
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Saiba como obter acesso a recursos locais, como aplicativos de linha de negócios, compartilhamentos de arquivos e impressoras de um dispositivo do Windows 10 ingressado no Azure Active Directory.
ms.openlocfilehash: 26ba0ffb64ddce32369002120657456e47ac0c7f
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2019
ms.locfileid: "37287361"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>Acessar recursos locais de um dispositivo ingressado no Azure AD no Microsoft 365 Business

Qualquer dispositivo Windows 10 que é o Azure Active Directory ingressado terá acesso a todos os recursos baseados em nuvem, como seus aplicativos do Office 365 e pode ser protegido pelo Microsoft 365 Business. Para permitir também o acesso a recursos locais, como aplicativos LOB (linha de negócios), compartilhamentos de arquivos e impressoras, você deve sincronizar seu Active Directory local com o Azure Active Directory usando o [Azure ad Connect](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect). 

Consulte [introdução ao gerenciamento de dispositivos no Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) para saber mais.
As etapas também são resumidas nas seções a seguir.

## <a name="run-azure-ad-connect"></a>Executar o Azure AD Connect

Conclua as etapas a seguir para permitir que os dispositivos ingressados no Azure AD da sua organização acessem recursos locais.
  
1. Para sincronizar os utilizadores, grupos e contactos do Active Directory local para o Azure Active Directory, execute o assistente de sincronização de directórios e o Azure AD Connect conforme descrito em [Configurar a sincronização de directórios para o Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
2. Após a conclusão da sincronização de diretórios, certifique-se de que os dispositivos Windows 10 da sua organização estejam ingressados no Azure AD. Esta etapa é feita individualmente em cada dispositivo Windows 10. Consulte [configurar dispositivos Windows para usuários do Microsoft 365 Business](set-up-windows-devices.md) para obter detalhes. 
    
3. Depois que os dispositivos Windows 10 são ingressados no Azure AD, cada usuário deve reiniciar seus dispositivos e fazer logon com suas credenciais do Microsoft 365 Business. Todos os dispositivos agora terão acesso a recursos locais também.
    
Não são necessárias etapas adicionais para obter acesso a recursos locais para dispositivos ingressados no Azure AD. Esta é a funcionalidade incorporada disponível no Windows 10. 
  
Se sua organização não estiver pronta para implantar na configuração de dispositivo ingressado no Azure AD descrita acima, considere configurar a [configuração de dispositivo ingressado no Azure ad híbrida](manage-windows-devices.md).
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a>Considerações ao ingressar em seus dispositivos Windows no Azure AD

Se você estiver ingressado no Azure AD em um dispositivo Windows que tenha sido associado ao domínio anteriormente ou em um grupo de trabalho, você precisará considerar as seguintes limitações:
  
- Quando um dispositivo do Azure AD ingressa, ele cria um novo usuário sem referenciar um perfil existente. Para corrigir isso, os perfis precisam ser migrados manualmente. Um perfil de usuário contém informações como favoritos, arquivos locais, configurações do navegador, configurações do menu Iniciar, etc. A melhor abordagem é encontrar uma ferramenta de terceiros para mapear arquivos e configurações existentes para o novo perfil

- Se o dispositivo estiver usando objetos de diretiva de grupo (GPO), alguns GPOs podem não ter um [provedor de](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) serviços de configuração (CSP) comparável no Intune. Execute a [ferramenta Mmat](https://www.microsoft.com/download/details.aspx?id=45520) para localizar CSPs comparáveis para GPOs existentes.

- Os usuários não poderão se autenticar em aplicativos que dependem da autenticação do Active Directory. Para lidar com isso, avalie o uso de um aplicativo herdado e considere a atualização para um aplicativo que usa o auth moderno, se possível.

- Descoberta de impressora do Active Directory não funcionará. Para corrigir isso, forneça caminhos de impressora diretos para todos os usuários ou aproveite a [impressão de nuvem híbrida](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).
