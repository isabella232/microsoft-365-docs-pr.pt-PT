---
title: Acesse recursos locais de um dispositivo azure ad no Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: M365-subscription-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Saiba como ter acesso a recursos locais, como linha de aplicativos de negócios, compartilhamentos de arquivos e impressoras de um diretório ativo do Azure, que se juntou ao dispositivo Windows 10.
ms.openlocfilehash: 89ac38f3da9cbdd3ff1a5eb33dc129d2e83521c7
ms.sourcegitcommit: 8c244b38c43dd00c4ef0102f8bed02ab36639a6b
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/10/2019
ms.locfileid: "39967169"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>Acesse recursos locais de um dispositivo azure ad no Microsoft 365 Business

Qualquer dispositivo Windows 10 que esteja no Diretório Ativo Do Azure, juntou-se, tem acesso a todos os recursos baseados em nuvem, como seus aplicativos do Office 365, e pode ser protegido pelo Microsoft 365 Business. Você também pode permitir o acesso a recursos no local, como aplicativos de linha de negócios (LOB), compartilhamentos de arquivos e impressoras. Para permitir o acesso, use o AD Connect do [Azure](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) para sincronizar seu Diretório Ativo no local com o Diretório Ativo Do Azure. 

Para saber mais, consulte [a introdução ao gerenciamento de dispositivos no Diretório Ativo Do Azure.](https://docs.microsoft.com/azure/active-directory/device-management-introduction)
As etapas também são resumidas nas seguintes seções.

> [!IMPORTANT]
> Este procedimento só é aplicável à OAuth e à NTLM. Kerberos não é apoiado.
 
## <a name="run-azure-ad-connect"></a>Executar azure ad connect

Complete as seguintes etapas para permitir que o AD Azure da sua organização acesse dispositivos para acessar recursos locais.
  
1. Para sincronizar seus usuários, grupos e contatos do Diretório Ativo local no Diretório Ativo Do Azure, execute o assistente de sincronização do Diretório e o AD Connect do Azure, conforme descrito na sincronização do diretório para o [Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
2. Depois que a sincronização do diretório estiver concluída, certifique-se de que os dispositivos Windows 10 da sua organização estão aderidos ao AD do Azure. Esta etapa é feita individualmente em cada dispositivo Windows 10. Veja [configurar dispositivos Windows para usuários do Microsoft 365 Business](set-up-windows-devices.md) para obter detalhes. 
    
3. Uma vez que os dispositivos Windows 10 são ajuntados pelo AD do Azure, cada usuário deve reiniciar seus dispositivos e entrar com suas credenciais microsoft 365 Business. Todos os dispositivos agora têm acesso a recursos no local também.
    
Não são necessárias medidas adicionais para ter acesso a recursos locais para dispositivos azure azure ajuntados a AD. Essa funcionalidade é incorporada ao Windows 10. 

Se você tem planos de fazer login no dispositivo AADJ além do método de senha Como PIN/Bio-metric via login de credencial WHFB e, em seguida, acessar recursos locais (compartilhamentos, impressoras.. etc), por favor, sigahttps://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Se a sua organização não estiver pronta para ser implantada na configuração do dispositivo adjacente ao AZure AD descrita acima, considere a configuração da configuração do [dispositivo Hybrid Azure AD Joined](manage-windows-devices.md).
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Considerações quando você adere dispositivos Windows a um anúncio do Azure

Se o dispositivo Windows que você azure-AD juntou foi previamente introduzido em domínio ou em um grupo de trabalho, considere as seguintes limitações:
  
- Quando um dispositivo azure AD junta, ele cria um novo usuário sem referenciar um perfil existente. Os perfis devem ser migrados manualmente. Um perfil de usuário contém informações como favoritos, arquivos locais, configurações do navegador e configurações do menu Iniciar. Uma abordagem melhor é encontrar uma ferramenta de terceiros para mapear arquivos e configurações existentes para o novo perfil.

- Se o dispositivo estiver usando objetos de política de grupo (GPO), alguns GPOs podem não ter um provedor de serviço de [configuração](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) comparável (CSP) em sintonia. Executar a [ferramenta MMAT](https://www.microsoft.com/download/details.aspx?id=45520) para encontrar CSPs comparáveis para GPOs existentes.

- Os usuários não poderão autenticar aplicativos que dependem da autenticação do Diretório Ativo. Avalie o aplicativo legado e considere atualizar para um aplicativo que usa a Auth moderna, se possível.

- A descoberta ativa da impressora do diretório não funcionará. Você pode fornecer caminhos de impressora direta para todos os usuários ou usar [o Hybrid Cloud Print.](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)
