---
title: Validar as definições de proteção de aplicações em dispositivos Android ou iOS
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: f3433b6b-02f7-447f-9d62-306bf03638b0
description: Saiba como validar as definições de proteção de aplicações Microsoft 365 Business Premium nos seus dispositivos Android ou iOS.
ms.openlocfilehash: a0a4a6e6cff59f66a506929e97c99d361472a68b
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578073"
---
# <a name="validate-app-protection-settings-on-android-or-ios-devices"></a>Validar as definições de proteção de aplicações em dispositivos Android ou iOS

Siga as instruções nas seguintes secções para validar as definições de proteção de aplicações em dispositivos Android ou iOS.
  
## <a name="android"></a>Android
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a>Verifique se as definições de proteção da aplicação estão a funcionar em dispositivos do utilizador

Depois de [definir as configurações das aplicações para dispositivos Android](app-protection-settings-for-android-and-ios.md) para proteger as aplicações, pode seguir estes passos para verificar se as definições que escolheu estão a funcionar. 
  
Em primeiro lugar, certifique-se de que a política se aplica à app na qual a vai validar.
  
1. No [centro de administração](https://portal.office.com)Microsoft 365 Business Premium, vá para a política **de** \> **Edição de** Políticas .
    
2. Escolha a **política de aplicação para Android** para as definições que criou na configuração, ou outra política que criou, e verifique se é aplicada ao Outlook, por exemplo. 
    
    ![Shows all the apps for which this policy protects files.](../media/b3be3ddd-f683-4073-8d7a-9c639a636a2c.png)
  
### <a name="validate-require-a-pin-or-a-fingerprint-to-access-office-apps"></a>Verificar a opção para exigir um PIN ou uma impressão digital para aceder às aplicações do Office

No painel **Editar política**, selecione **Editar** junto a **Controlo do acesso a documentos do Office**. Expanda a secção **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis** e certifique-se de que a opção **Exigir um PIN ou impressão digital para aceder às aplicações do Office** está definida como **Ativada**.
  
![Certifique-se de que o Requerer um PIN ou uma impressão digital para aceder a aplicações do Office está definido para On.](../media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. No dispositivo Android do utilizador, abra o Outlook e inscreva-se com as credenciais Microsoft 365 Business Premium do utilizador.
    
2. Também será solicitado a introduzir um PIN ou usar uma impressão digital.
    
    ![Enter a PIN on your Android device to access Office apps.](../media/9e8ecfee-8122-4a3a-8918-eece80344310.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a>Verificar a opção para repor o PIN após um número de tentativas falhadas

No painel **de política de edição,** escolha **Editar** ao lado do controlo de acesso de **documentos do Office,** **expanda a forma como os utilizadores acedem aos ficheiros do Office em dispositivos móveis**, e certifique-se de que **o RESET PIN após o número de tentativas falhadas** está definido para algum número. Este é 5 por defeito. 
  
1. No dispositivo Android do utilizador, abra o Outlook e inscreva-se com as credenciais Microsoft 365 Business Premium do utilizador.
    
2. Introduza um PIN incorreto tantas vezes quanto for especificado pela política. Verá uma solicitação que diz que **o limite de tentativa pin alcançado** para redefinir o PIN. 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](../media/fca6fcb4-bb5c-477f-af5e-5dc937e8b835.png)
  
3. Prima **Repor PIN**. Será solicitado que faça seduca com as credenciais Microsoft 365 Business Premium do utilizador e, em seguida, necessário para definir um novo PIN.
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a>Verificar a opção para forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas

No painel **Editar política**, selecione **Editar** junto a **Proteção contra dispositivos perdidos ou roubados**. Expanda a secção **Proteger os ficheiros de trabalho se os dispositivos forem perdidos ou roubados** e certifique-se de que a opção **Forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas** está definida como **Ativada**.
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](../media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. No dispositivo Android do utilizador, abra o Outlook e inscreva-se com as credenciais Microsoft 365 Business Premium do utilizador e introduza um PIN se solicitado.
    
2. Abra um e-mail que contenha um anexo e toque no ícone de seta para baixo junto às informações do anexo.
    
    ![Tap the down arrow next to an attachment to try to save it.](../media/b22573bb-91ce-455f-84fa-8feb2846b117.png)
  
    Verá Não **é possível guardar para** o dispositivo na parte inferior do ecrã. 
    
    ![Warning text that indicates cannot save a file locally to an Android.](../media/52ca3f3d-7ed0-4a52-9621-4872da6ea9c5.png)
  
    > [!NOTE]
    > A opção Guardar no OneDrive para Empresas não se encontra disponível para Android neste momento, por isso, só verá a opção para guardar localmente bloqueada. 
  
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a>Verificar a opção para exigir que o utilizador inicie sessão novamente caso as aplicações do Office estejam inativas durante um período de tempo específico

No painel **de política de edição,** escolha **Editar** ao lado do controlo de acesso a **documentos do Office**, **expanda a forma como os utilizadores acedem aos ficheiros do Office em dispositivos móveis**– e certifique-se de que **os utilizadores exigem que os utilizadores voltem a entrar depois de as aplicações do Office terem estado inativas** para alguns minutos. São 30 minutos por defeito. 
  
1. No dispositivo Android do utilizador, abra o Outlook e inscreva-se com as credenciais Microsoft 365 Business Premium do utilizador e introduza um PIN se solicitado.
    
2. Já deverá ver a caixa de entrada do Outlook. Não faça alterações ao dispositivo Android inativo durante, pelo menos, 30 minutos (ou outro período de tempo superior ao especificado na política). Provavelmente, o ecrã do dispositivo ficará mais escuro.
    
3. Access Outlook no dispositivo Android novamente.
    
4. Será solicitado que introduza o seu PIN antes de poder aceder ao Outlook novamente.
    
### <a name="validate-protect-work-files-with-encryption"></a>Verificar a opção para proteger ficheiros de trabalho com encriptação

No painel **Editar política**, selecione **Editar** junto a **Proteção contra dispositivos perdidos ou roubados**. Expanda a janela **Proteger os ficheiros de trabalho se os dispositivos forem perdidos ou roubados** e certifique-se de que a opção **Proteger ficheiros de trabalho com encriptação** está definida como **Ativada** e a opção **Forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas** está definida como **Desativada**.
  
1. No dispositivo Android do utilizador, abra o Outlook e inscreva-se com as credenciais Microsoft 365 Business Premium do utilizador e introduza um PIN se solicitado.
    
2. Abra um e-mail que contenha alguns anexos de ficheiros de imagem.
    
3. Toque no ícone de seta para baixo junto às informações do anexo para guardá-lo.
    
    ![Tap the down arrow to save the figure file to the Android device.](../media/08a9e21e-4022-45d5-acff-59cface651e7.png)
  
4. Poderá ser-lhe pedido para permitir que o Outlook aceda às fotografias, multimédia e ficheiros no seu dispositivo. Toque em **Permitir**.
    
5. Na parte inferior do ecrã, selecione **Guardar no Dispositivo** e, em seguida, abra a aplicação **Galeria**. 
    
6. Deverá ver uma fotografia encriptada (ou mais, caso tenha guardado múltiplos anexos de ficheiros de imagem) na lista. A fotografia poderá ser apresentada na Lista de imagens como um quadrado cinzento com um ponto de exclamação branco dentro de um círculo branco no centro do quadrado cinzento.
    
    ![An encrypted image file in the Gallery app.](../media/25936414-bd7e-421d-824e-6e59b877722d.png)
  
## <a name="ios"></a>iOS
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a>Verificar se as definições de proteção de aplicações estão a funcionar nos dispositivos dos utilizadores

Depois de [definir as configurações das aplicações para dispositivos iOS](app-protection-settings-for-android-and-ios.md) para proteger as aplicações, pode seguir estes passos para verificar se as definições que escolheu estão a funcionar. 
  
Em primeiro lugar, certifique-se de que a política se aplica à app na qual a vai validar.
  
1. No [centro de administração](https://portal.office.com)Microsoft 365 Business Premium, vá para a política **de** \> **Edição de** Políticas .
    
2. Escolha a **política de aplicação para iOS** para as definições que criou na configuração, ou outra política que criou, e verifique se é aplicada ao Outlook, por exemplo. 
    
    ![Shows all the apps for which this policy protects files.](../media/842441b8-e7b1-4b86-9edd-d94d1f77b6f4.png)
  
### <a name="validate-require-a-pin-to-access-office-apps"></a>Verificar a opção para exigir um PIN para aceder às aplicações do Office

No painel **Editar política**, selecione **Editar** junto a **Controlo do acesso a documentos do Office**. Expanda a secção **Gerir a forma como os utilizadores acedem a ficheiros do Office em dispositivos móveis** e certifique-se de que a opção **Exigir um PIN ou impressão digital para aceder às aplicações do Office** está definida como **Ativada**.
  
![Certifique-se de que o Requerer um PIN ou uma impressão digital para aceder a aplicações do Office está definido para On.](../media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. No dispositivo iOS do utilizador, abra o Outlook e inscreva-se com as credenciais Microsoft 365 Business Premium do utilizador.
    
2. Também será solicitado a introduzir um PIN ou usar uma impressão digital.
    
    ![Enter a PIN on your IOS device to access Office apps.](../media/06fc5cf3-9f19-4090-b23c-14bb59805b7a.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a>Verificar a opção para repor o PIN após um número de tentativas falhadas

No painel **de política de edição,** escolha **Editar** ao lado do controlo de acesso de **documentos do Office,** **expanda a forma como os utilizadores acedem aos ficheiros do Office em dispositivos móveis**, e certifique-se de que **o RESET PIN após o número de tentativas falhadas** está definido para algum número. Este é 5 por defeito. 
  
1. No dispositivo iOS do utilizador, abra o Outlook e inscreva-se com as credenciais Microsoft 365 Business Premium do utilizador.
    
2. Introduza um PIN incorreto tantas vezes quanto for especificado pela política. Verá uma solicitação que diz que **o limite de tentativa pin alcançado** para redefinir o PIN. 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](../media/fab5c089-a4a5-4e8d-8c95-b8eed1dfa262.png)
  
3. Prima **OK**. Será solicitado que faça seduca com as credenciais Microsoft 365 Business Premium do utilizador e, em seguida, necessário para definir um novo PIN.
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a>Verificar a opção para forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas

No painel **Editar política**, selecione **Editar** junto a **Proteção contra dispositivos perdidos ou roubados**. Expanda a secção **Proteger os ficheiros de trabalho se os dispositivos forem perdidos ou roubados** e certifique-se de que a opção **Forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas** está definida como **Ativada**.
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](../media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. No dispositivo iOS do utilizador, abra o Outlook e inscreva-se com as credenciais Microsoft 365 Business Premium do utilizador e introduza um PIN se solicitado.
    
2. Abra um e-mail que contenha um anexo, abra o anexo e selecione **Guardar** na parte inferior do ecrã. 
    
    ![Tap the Save option after you open an attachment to try to save it.](../media/b419b070-1530-4f14-86a8-8d89933a2b25.png)
  
3. Deverá ver apenas uma opção para o OneDrive para Empresas. Caso contrário, toque em **Adicionar Conta** e selecione **OneDrive para negócios** a partir do ecrã **da Conta de Armazenamento De Adicionar.** Forneça o Microsoft 365 Business Premium do utilizador final para iniciar sedutar quando solicitado. 
    
    Toque em **Guardar** e selecione **OneDrive para Empresas**.
    
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a>Verificar a opção para exigir que o utilizador inicie sessão novamente caso as aplicações do Office estejam inativas durante um período de tempo específico

No painel **de política de edição,** escolha **Editar** ao lado do controlo de acesso a **documentos do Office**, **expanda a forma como os utilizadores acedem aos ficheiros do Office em dispositivos móveis**– e certifique-se de que **os utilizadores exigem que os utilizadores voltem a entrar depois de as aplicações do Office terem estado inativas** para alguns minutos. São 30 minutos por defeito. 
  
1. No dispositivo iOS do utilizador, abra o Outlook e inscreva-se com as credenciais Microsoft 365 Business Premium do utilizador e introduza um PIN se solicitado.
    
2. Já deverá ver a caixa de entrada do Outlook. Não faça alterações ao dispositivo iOS durante, pelo menos, 30 minutos (ou outro período de tempo superior ao especificado na política). Provavelmente, o ecrã do dispositivo ficará mais escuro.
    
3. Aceder ao Outlook no dispositivo iOS novamente.
    
4. Será solicitado que introduza o seu PIN antes de poder aceder ao Outlook novamente.
    
### <a name="validate-protect-work-files-with-encryption"></a>Verificar a opção para proteger ficheiros de trabalho com encriptação

No painel **Editar política**, selecione **Editar** junto a **Proteção contra dispositivos perdidos ou roubados**. Expanda a janela **Proteger os ficheiros de trabalho se os dispositivos forem perdidos ou roubados** e certifique-se de que a opção **Proteger ficheiros de trabalho com encriptação** está definida como **Ativada** e a opção **Forçar os utilizadores a guardar todos os ficheiros de trabalho no OneDrive para Empresas** está definida como **Desativada**.
  
1. No dispositivo iOS do utilizador, abra o Outlook e inscreva-se com as credenciais Microsoft 365 Business Premium do utilizador e introduza um PIN se solicitado.
    
2. Abra um e-mail que contenha alguns anexos de ficheiros de imagem.
    
3. Toque no anexo e, em seguida, toque na opção **Guardar** por baixo do mesmo. 
    
4. Abra a aplicação **Fotografias** no ecrã principal. Deverá ver uma fotografia (ou mais, se tiver guardado múltiplos anexos de ficheiros de imagem) guardada, embora esteja encriptada. 
    
---

