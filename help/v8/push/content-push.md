---
audience: end-user
title: Criar um delivery de notificação por push
description: Saiba como criar um delivery de notificação por push com o Adobe Campaign Web
badge: label="Alpha" type="Positive"
source-git-commit: 7fa6a5adb22b4fc4569b93383a8e269703944582
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 29%

---

# Criar uma entrega por push {#content-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_android_content"
>title="Conteúdo de push para Android"
>abstract="Defina o conteúdo de push para Android."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_content"
>title="Conteúdo de push para iOS"
>abstract="Defina o conteúdo de push para iOS."

## Mensagem {#push-message}

>[!BEGINTABS]

>[!TAB Android]

Com o Firebase Cloud Messaging, você pode escolher entre dois tipos de mensagens:

* A variável **Mensagem de dados**, manipulada pelo aplicativo do cliente. As mensagens são enviadas diretamente para o aplicativo móvel que gerará e exibirá a notificação do Android para o dispositivo. As mensagens de dados contêm somente as variáveis personalizadas do aplicativo.

   Clique em **[!UICONTROL Mensagem]** e use o Editor de expressão para definir o conteúdo, personalizar os dados e adicionar conteúdo dinâmico.

* A mensagem de Notificação, manipulada automaticamente pelo SDK do FCM. O FCM exibe automaticamente a mensagem nos dispositivos dos usuários em nome do aplicativo do cliente. As mensagens de notificação contêm um conjunto predefinido de parâmetros e opções, mas ainda podem ser personalizadas com variáveis de aplicativo personalizadas.

   Para redigir a mensagem, clique no link **[!UICONTROL Título]** e **[!UICONTROL Corpo]** campos. Use o Editor de expressão para definir o conteúdo, personalizar os dados e adicionar conteúdo dinâmico.

   Para personalizar ainda mais sua notificação por push, você pode escolher uma imagem para adicionar à notificação por push, o ícone da notificação a ser exibido nos dispositivos dos perfis e sua cor.

>[!TAB iOS]

Para redigir a mensagem, clique no link **[!UICONTROL Título]** e **[!UICONTROL Corpo]** campos. Use o Editor de expressão para definir o conteúdo, personalizar os dados e adicionar conteúdo dinâmico.

Você pode adicionar um **[!UICONTROL Legenda]**, valor do parâmetro de subtítulo da carga de notificação do iOS. Consulte esta seção.

O modo Push silencioso permite que uma notificação &quot;silenciosa&quot; seja enviada a um aplicativo móvel. O usuário não está ciente da chegada da notificação. Ele é transferido diretamente para o aplicativo.

>[!ENDTABS]

## Configurações avançadas {#push-advanced}

>[!BEGINTABS]

>[!TAB Android]

* **[!UICONTROL Som]**: Defina o som que será reproduzido quando o dispositivo receber sua notificação.

* **[!UICONTROL Contagem de notificações]**: Defina o número de novas informações não lidas para serem exibidas diretamente no ícone do aplicativo.

* **[!UICONTROL ID do canal]**: Defina a ID do canal da sua notificação. O aplicativo deve criar um canal com essa ID de canal antes que qualquer notificação com essa ID de canal seja recebida.

* **[!UICONTROL Ação Clicar]**: Defina a ação associada a um clique do usuário em sua notificação.

* **[!UICONTROL Tag]**: Defina o identificador usado para substituir notificações existentes na gaveta de notificações.

* **[!UICONTROL Prioridade]**: Defina os níveis de prioridade da sua notificação como padrão, mínimo, baixo ou alto. Para obter mais informações, consulte a documentação do FCM.

* **[!UICONTROL Visibilidade]**: Defina os níveis de visibilidade de sua notificação como público, privado ou secreto. Para obter mais informações, consulte a documentação do FCM.

* **[!UICONTROL Fixo]**: se desativada, a notificação é automaticamente descartada quando o usuário clica nela. Se ativada, a notificação ainda será exibida mesmo quando o usuário clicar nela.

>[!TAB iOS]

* **[!UICONTROL Modo de alerta crítico]**: ative essa opção para adicionar som à sua notificação, mesmo que o telefone do usuário esteja configurado no modo de foco ou se o iPhone estiver sem áudio.

* **[!UICONTROL Limpar selo]**: ative essas opções para atualizar o valor do selo.

* **[!UICONTROL Contagem de notificações]**: defina um número que será usado para exibir o número de novas informações não lidas diretamente no ícone do aplicativo.

* **[!UICONTROL Volume]**: volume do som, de 0 a 100.

* **[!UICONTROL Conteúdo mutável]** (Somente no iOS): envia o sinalizador de conteúdo mutável no payload por push e permitirá que o conteúdo da notificação por push seja modificado por uma extensão de aplicativo de serviço de notificação fornecida no SDK do iOS. Para saber mais, consulte a [documentação para desenvolvedores da Apple](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ModifyingNotifications.html). habilite essa opção para permitir que o aplicativo móvel baixe conteúdo de mídia.

* **[!UICONTROL Pontuação de relevância]**: defina uma pontuação de relevância de 0 a 100. O sistema usa essa opção para classificar as notificações no resumo de notificações.

* **[!UICONTROL Nível de interrupção]**:

   * **[!UICONTROL Ativo]**: selecionado por padrão; o sistema apresenta a notificação imediatamente, ativa a tela e pode reproduzir um som. As notificações não interrompem os modos de foco.

   * **[!UICONTROL Passivo]**: o sistema adiciona a notificação à lista de notificações sem ativar a tela ou reproduzir um som. As notificações não interrompem os modos de foco.

   * **[!UICONTROL Sensível ao tempo]**: o sistema apresenta a notificação imediatamente, ativa a tela, pode reproduzir um som e interrompe os modos de foco. Esse nível não requer uma permissão especial da Apple.

   * **[!UICONTROL Crítico]**: o sistema apresenta a notificação imediatamente, ativa a tela e ignora os modos de foco e a opção de mudo. Observe que esse nível requer uma permissão especial da Apple.

* **[!UICONTROL Thread-id]**: identificador usado para agrupar notificações relacionadas.

* **[!UICONTROL Categoria]**: nome da ID da categoria que exibirá botões de ação. Essas notificações fornecem ao usuário uma maneira mais rápida de realizar tarefas diferentes em resposta a uma notificação sem abrir o aplicativo ou navegar até ele.

* **[!UICONTROL ID do conteúdo do Target]**: identificador usado para definir qual janela de aplicativo será apresentada quando a notificação for aberta.

* **[!UICONTROL Imagem de inicialização]**: nome do arquivo de imagem que será exibido na inicialização. Se o usuário optar por iniciar seu aplicativo, a imagem selecionada será exibida em vez da tela de inicialização do aplicativo.

>[!ENDTABS]

<!--Sounds must be included in the application and defined when the service is created. Refer to this section.-->



