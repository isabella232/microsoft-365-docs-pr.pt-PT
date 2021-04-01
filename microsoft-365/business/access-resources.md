---
title: Aceder aos recursos no local a partir de um dispositivo AD AZure ligado ao Microsoft 365 Business
f1.keywords:
- NOCSH
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Saiba como obter acesso a recursos no local, como linha de aplicações empresariais, partilhas de ficheiros e impressoras de um Azure Ative Directory que aderiu ao dispositivo Windows 10.
ms.openlocfilehash: 1bca0beb3ccc78e670ad33ce446b9b3f7c372ba7
ms.sourcegitcommit: 39609c4d8c432c8e7d7a31cb35c8020e5207385b
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/30/2021
ms.locfileid: "51445354"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Aceder aos recursos no local a partir de um dispositivo AD AD Azure no Microsoft 365 Business Premium

Este artigo aplica-se ao Microsoft 365 Business Premium.

Qualquer dispositivo do Windows 10 que seja a aderido ao Azure Ative Directory tem acesso a todos os recursos baseados na nuvem, como as suas aplicações Microsoft 365, e pode ser protegido pelo Microsoft 365 Business Premium. Também pode permitir o acesso a recursos no local, como aplicações de linha de negócios (LOB), partilhas de ficheiros e impressoras. Para permitir o acesso, utilize [o Azure AD Connect](/azure/active-directory/connect/active-directory-aadconnect) para sincronizar o seu Ative Directory no local com o Azure Ative Directory. 

Para saber mais, consulte [Introdução à gestão de dispositivos no Azure Ative Directory](/azure/active-directory/device-management-introduction).
Os passos são também resumidos nas seguintes secções.
 
## <a name="run-azure-ad-connect"></a>Executar Azure AD Connect

Complete os seguintes passos para permitir que os dispositivos Azure AD da sua organização tenham acesso aos recursos no local.
  
1. Para sincronizar os seus utilizadores, grupos e contactos do Diretório Ativo local para o Azure Ative Directory, executar o assistente de sincronização do Diretório e a Azure AD Connect, conforme descrito na [sincronização do diretório configurado para o Office 365](../enterprise/set-up-directory-synchronization.md).
    
2. Depois de concluída a sincronização do diretório, certifique-se de que os dispositivos windows 10 da sua organização estão unidos a Azure AD. Este passo é feito individualmente em cada dispositivo Windows 10. Consulte [os dispositivos Windows para os utilizadores Do Microsoft 365 Business Premium](set-up-windows-devices.md) para obter mais detalhes. 
    
3. Uma vez que os dispositivos Windows 10 estejam ligados ao Azure AD, cada utilizador deve reiniciar os seus dispositivos e iniciar sôs com as suas credenciais Microsoft 365 Business Premium. Todos os dispositivos têm agora acesso a recursos no local também.
    
Não são necessárias medidas adicionais para ter acesso aos recursos no local para dispositivos aderidos a Azure AD. Esta funcionalidade encontra-se integrada no Windows 10. 

Se tiver planos para iniciar sessão no dispositivo AADJ que não seja o método de senha Como PIN/Bio-métrica via login credencial WHFB e, em seguida, aceder a recursos no local (partilhas,impressoras.. etc), por favor, siga https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Se a sua organização não estiver pronta para implantar na configuração do dispositivo azure AD descrita acima, considere configurar a [configuração do dispositivo AD AD Ad Hybrid Azure](manage-windows-devices.md).
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Considerações quando se junta dispositivos Windows ao Azure AD

Se o dispositivo Windows a que aD Azure-AD aderiu foi previamente agrupado por domínio ou num grupo de trabalho, considere as seguintes limitações:
  
- Quando um dispositivo Azure AD se junta, cria um novo utilizador sem se referir a um perfil existente. Os perfis devem ser migrados manualmente. Um perfil de utilizador contém informações como favoritos, ficheiros locais, configurações do navegador e definições de menu Iniciar. A melhor abordagem é encontrar uma ferramenta de terceiros para mapear ficheiros e configurações existentes para o novo perfil.

- Se o dispositivo estiver a utilizar objetos de política de grupo (GPO), alguns GPOs podem não ter um [Fornecedor de Serviço de Configuração](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) comparável (CSP) no Intune. Executar a [ferramenta MMAT](https://www.microsoft.com/download/details.aspx?id=45520) para encontrar CSPs comparáveis para os GPOs existentes.

- Os utilizadores podem não conseguir autenticar aplicações que dependam da autenticação do Ative Directory. Avalie a aplicação legacy e considere atualização para uma app que usa o moderno Auth, se possível.

- A descoberta da impressora ative do Diretório não vai funcionar. Pode fornecer caminhos de impressora direta para todos os utilizadores ou utilizar [a Impressão Universal.](/universal-print/)

### <a name="related-articles"></a>Artigos Relacionados

[Pré-requisitos para Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)
