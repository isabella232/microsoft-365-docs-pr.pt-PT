---
title: Aceder a recursos no local a partir de um dispositivo associado ao Azure AD no Microsoft 365 Empresas
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Saiba como obter acesso a recursos no local, como aplicações de linha de negócio, partilhas de ficheiros e impressoras a partir de um Azure Active Directory dispositivo Windows 10 empresa.
ms.openlocfilehash: 72b3c5ae538cad24fc12e25717dedccb2fdc9017
ms.sourcegitcommit: 4fb1226d5875bf5b9b29252596855a6562cea9ae
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/08/2021
ms.locfileid: "52843328"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Aceder a recursos no local a partir de um dispositivo associado ao Azure AD no Microsoft 365 Empresas Premium

Este artigo aplica-se a Microsoft 365 Empresas Premium.

Qualquer Windows 10 dispositivo que esteja Azure Active Directory associado tem acesso a todos os recursos baseados na nuvem, como as suas aplicações do Microsoft 365, e pode ser protegido pelo Microsoft 365 Empresas Premium. Também pode permitir o acesso a recursos no local, como aplicações de linha de negócio (LOB), partilhas de ficheiros e impressoras. Para permitir o acesso, utilize o [Azure AD Ligação](/azure/active-directory/connect/active-directory-aadconnect) para sincronizar o seu Active Directory no local com o Azure Active Directory.

Para saber mais, consulte [Introdução à gestão de dispositivos no Azure Active Directory](/azure/active-directory/device-management-introduction).
Os passos também estão resumidos nas secções seguintes.

## <a name="run-azure-ad-connect"></a>Executar o Azure AD Ligação

Conclua os seguintes passos para permitir que os dispositivos associados ao Azure AD da sua organização acedam a recursos no local.

1. Para sincronizar os seus utilizadores, grupos e contactos do Active Directory local no Azure Active Directory, execute o Assistente de sincronização de diretórios e o Azure AD Ligação conforme descrito em Configurar a [sincronização](../enterprise/set-up-directory-synchronization.md)de diretórios para Office 365.

2. Após a sincronização de diretórios estar concluída, certifique-se de que os dispositivos móveis Windows 10 da sua organização estão associados ao Azure AD. Este passo é realizado individualmente em cada Windows 10 dispositivo. Consulte [Configurar dispositivos Windows para utilizadores Microsoft 365 Empresas Premium utilizadores para](set-up-windows-devices.md) obter mais detalhes.

3. Assim que os Windows 10 dispositivos móveis estiverem associados ao Azure AD, cada utilizador terá de reiniciar os respetivos dispositivos e entrar com as Microsoft 365 Empresas Premium credenciais. Todos os dispositivos agora também têm acesso a recursos no local.

Não são necessários passos adicionais para aceder aos recursos no local em dispositivos associados ao Azure AD. Esta funcionalidade está incorporada no Windows 10.

Se tiver planos de início de sessão no dispositivo AADJ sem ser através de um método de palavra-passe Como o PIN/Bio-métrica através do início de sessão de credenciais WHFB e, em seguida, aceder aos recursos no local (partilhas, impressoras, etc.), siga este [artigo.](/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

Se a sua organização não estiver pronta para implementar na configuração de dispositivos associados ao Azure AD acima, considere configurar a configuração de dispositivos associados ao [Azure AD Híbrido.](manage-windows-devices.md)

### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Considerações a ter ao aderir Windows dispositivos ao Azure AD

Se o Windows dispositivo a que aderiu ao Azure-AD tiver aderido anteriormente a um domínio ou num grupo de trabalho, tenha em consideração as seguintes limitações:

- Quando um dispositivo Azure AD adere, cria um novo utilizador sem referenciar um perfil existente. Os perfis têm de ser migrados manualmente. Um perfil de utilizador contém informações como favoritos, ficheiros locais, definições do browser e definições do menu Iniciar. A melhor abordagem é encontrar uma ferramenta de terceiros para mapear ficheiros e definições existentes para o novo perfil.

- Se o dispositivo estiver a utilizar Objetos da Política de Grupo (GPO), alguns GPOs poderão não ter um Fornecedor de Serviços de [Configuração](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) comparável no Intune. Execute [a ferramenta MMAT](https://www.microsoft.com/download/details.aspx?id=45520) para encontrar CSPs comparáveis para GPOs existentes.

- Os utilizadores poderão não conseguir autenticar as aplicações que dependem da autenticação do Active Directory. Avalie a aplicação legada e considere atualizar para uma aplicação que utilize a Auth moderna, se possível.

- A deteção de impressoras do Active Directory não irá funcionar. Pode fornecer caminhos diretos para a impressora a todos os utilizadores ou utilizar a [impressão universal.](/universal-print/)

### <a name="related-articles"></a>Artigos relacionados

[Pré-requisitos para o Azure AD Ligação](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)
