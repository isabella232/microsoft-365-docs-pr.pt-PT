---
title: Acesso aos recursos no local a partir de um dispositivo azure ad-join no Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Saiba como aceder a recursos no local, como linha de aplicações de negócios, partilhas de ficheiros e impressoras de um dispositivo Azure Ative Directory que se juntou ao Windows 10.
ms.openlocfilehash: c1e04e5ca0d36c32a55a9819140356db5093e3a1
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/21/2020
ms.locfileid: "43627460"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Acesso aos recursos no local a partir de um dispositivo azure ad-join no Microsoft 365 Business Premium

Qualquer dispositivo Windows 10 que seja o Azure Ative Directory junto tem acesso a todos os recursos baseados na nuvem, como as suas aplicações Microsoft 365, e pode ser protegido pelo Microsoft 365 Business Premium. Também pode permitir o acesso a recursos no local, como aplicações de linha de negócios (LOB), partilhas de ficheiros e impressoras. Para permitir o acesso, utilize o [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) para sincronizar o seu Diretório Ativo no local com o Diretório Ativo Azure. 

Para saber mais, consulte Introdução à gestão de [dispositivos no Diretório Ativo Azure.](https://docs.microsoft.com/azure/active-directory/device-management-introduction)
Os passos também são resumidos nas seguintes secções.

> [!IMPORTANT]
> Este procedimento só é aplicável à OAuth e à NTLM. Kerberos não é apoiado.
 
## <a name="run-azure-ad-connect"></a>Executar Ligação AD Azure

Complete os seguintes passos para permitir que o Azure AD da sua organização tenha acesso aos recursos no local.
  
1. Para sincronizar os seus utilizadores, grupos e contactos do Diretório Ativo local para o Diretório Ativo Azure, execute o assistente de sincronização do Diretório e o Azure AD Connect, conforme descrito na sincronização do diretório para o [Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
2. Depois de concluída a sincronização do diretório, certifique-se de que os dispositivos Windows 10 da sua organização são Azure AD. Este passo é feito individualmente em cada dispositivo do Windows 10. Consulte a [configuração de dispositivos Windows para utilizadores do Microsoft 365 Business Premium](set-up-windows-devices.md) para obter mais detalhes. 
    
3. Uma vez que os dispositivos Do Windows 10 são AD Azure, cada utilizador deve reiniciar os seus dispositivos e iniciar sessão com as suas credenciais Microsoft 365 Business Premium. Todos os dispositivos têm agora acesso aos recursos no local também.
    
Não são necessárias medidas adicionais para ter acesso aos recursos no local para dispositivos ligados à AD Azure. Esta funcionalidade está incorporada no Windows 10. 

Se tiver planos para iniciar sessão no dispositivo AADJ que não seja o método de senha, como PIN/Bio-metric via login credencial WHFB e, em seguida, aceder aos recursos no local (ações,impressoras.. etc), por favor, sigahttps://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Se a sua organização não estiver pronta para ser implementada na configuração de dispositivo seletiva do Azure AD descrita acima, considere configurar a configuração do [dispositivo Hybrid Azure AD Joined](manage-windows-devices.md).
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Considerações quando se juntam a dispositivos Windows para a Azure AD

Se o dispositivo Windows a que aderiu o Azure-AD foi previamente associado ao domínio ou num grupo de trabalho, considere as seguintes limitações:
  
- Quando um dispositivo Azure AD se junta, cria um novo utilizador sem se referir a um perfil existente. Os perfis devem ser migrados manualmente. Um perfil de utilizador contém informações como favoritos, ficheiros locais, definições de navegador e definições de menu Iniciar. A melhor abordagem é encontrar uma ferramenta de terceiros para mapear ficheiros e configurações existentes para o novo perfil.

- Se o dispositivo estiver a utilizar objetos de política de grupo (GPO), alguns GPOs podem não ter um fornecedor de [serviçode configuração](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) comparável (CSP) em Intune. Executar a [ferramenta MMAT](https://www.microsoft.com/download/details.aspx?id=45520) para encontrar CSPs comparáveis para GPOs existentes.

- Os utilizadores não poderão autenticar aplicações que dependem da autenticação do Diretório Ativo. Avalie a aplicação legacy e considere a atualização para uma app que usa o moderno Auth, se possível.

- A descoberta da impressora de diretório ativo não vai funcionar. Pode fornecer caminhos de impressora direta para todos os utilizadores ou utilizar impressão [de nuvem híbrida](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).
