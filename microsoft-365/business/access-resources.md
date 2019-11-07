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
description: Saiba como ter acesso a recursos locais, como aplicativos line of business, compartilhamentos de arquivos e impressoras de um diretório ativo do Azure, que se juntou ao dispositivo Windows 10.
ms.openlocfilehash: 2af5d4b4f84f39f5b157313e5b38ef030da7263d
ms.sourcegitcommit: 70e920f76526f47fc849df615de4569e0ac2f4be
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/07/2019
ms.locfileid: "38030540"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>Acesse recursos locais de um dispositivo azure ad no Microsoft 365 Business

Qualquer dispositivo Windows 10 que esteja no Diretório Ativo Do Azure, juntou-se, terá acesso a todos os recursos baseados em nuvem, como seus aplicativos do Office 365, e pode ser protegido pelo Microsoft 365 Business. Para também permitir o acesso a recursos no local, como aplicativos Line Of Business (LOB), compartilhamentos de arquivos e impressoras, você deve sincronizar seu Diretório Ativo no local com o Diretório Ativo Do Azure usando o [AZure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect). 

Veja [a introdução ao gerenciamento de dispositivos no Diretório Ativo Do Azure](https://docs.microsoft.com/azure/active-directory/device-management-introduction) para saber mais.
As etapas também são resumidas nas seguintes seções.

## <a name="run-azure-ad-connect"></a>Executar azure ad connect

Complete as seguintes etapas para permitir que o AD Azure da sua organização acesse dispositivos para acessar recursos locais.
  
1. Para sincronizar seus usuários, grupos e contatos do Diretório Ativo local no Diretório Ativo Do Azure, execute o assistente de sincronização do Diretório e o AD Connect do Azure, conforme descrito na sincronização do diretório para o [Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
2. Depois que a sincronização do diretório tiver sido concluída, certifique-se de que os dispositivos Windows 10 da sua organização estão aderidos ao AD do Azure. Esta etapa é feita individualmente em cada dispositivo Windows 10. Veja [configurar dispositivos Windows para usuários do Microsoft 365 Business](set-up-windows-devices.md) para obter detalhes. 
    
3. Uma vez que os dispositivos Windows 10 são ajuntados pelo AD Do Azure, cada usuário deve reiniciar seus dispositivos e fazer login com suas credenciais Microsoft 365 Business. Todos os dispositivos terão agora acesso a recursos no local também.
    
Não são necessárias medidas adicionais para ter acesso a recursos locais para dispositivos azure azure ajuntados a AD. Esta é a funcionalidade incorporada disponível no Windows 10. 
  
Se a sua organização não estiver pronta para ser implantada na configuração do dispositivo adjacente ao AZure Azure descrita acima, considere a configuração da configuração do [dispositivo Hybrid Azure AD Joined](manage-windows-devices.md).
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a>Considerações ao juntar seus dispositivos Windows ao AD do Azure

Se você é aD do Azure que adere a um dispositivo Windows que já foi unido ou em um grupo de trabalho, você precisa considerar as seguintes limitações:
  
- Quando um dispositivo azure AD junta, ele cria um novo usuário sem referenciar um perfil existente. Para corrigir isso, os perfis precisam ser migrados manualmente. Um perfil de usuário contém informações como favoritos, arquivos locais, configurações do navegador, configurações de menu iniciar, etc. Uma melhor abordagem é encontrar uma ferramenta de terceiros para mapear arquivos e configurações existentes para o novo perfil

- Se o dispositivo estiver usando objetos de política de grupo (GPO), alguns GPOs podem não ter um provedor de serviço de [configuração](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) comparável (CSP) em sintonia. Executar a [ferramenta MMAT](https://www.microsoft.com/download/details.aspx?id=45520) para encontrar CSPs comparáveis para GPOs existentes.

- Os usuários não poderão autenticar aplicativos que dependem da autenticação do Diretório Ativo. Para lidar com isso avaliar usando um aplicativo legado e considerar a atualização para um aplicativo que usa Auth moderno, se possível.

- A descoberta ativa da impressora do diretório não funcionará. Para corrigir isso, forneça caminhos de impressora direta para todos os usuários ou aproveite o [Hybrid Cloud Print.](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)
