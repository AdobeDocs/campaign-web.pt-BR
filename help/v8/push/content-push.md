---
audience: end-user
title: Criar um delivery de notificação por push
description: Saiba como criar um delivery de notificação por push com o Adobe Campaign Web
badge: label="Alpha" type="Positive"
source-git-commit: a9c9079a64dd7113aa7da1040aa30cef2c9c0aec
workflow-type: tm+mt
source-wordcount: '1070'
ht-degree: 19%

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

* A variável **[!UICONTROL Mensagem de dados]e** é manipulada pelo aplicativo do cliente. Essas mensagens são enviadas diretamente para o aplicativo móvel, que gera e exibe uma notificação do Android no dispositivo. As mensagens de dados contêm somente as variáveis personalizadas do aplicativo.

  Para definir o conteúdo, personalizar dados e adicionar conteúdo dinâmico, clique no link **[!UICONTROL Mensagem]** e use o Editor de expressão. Você pode acessar esse editor para personalizar suas mensagens na **[!UICONTROL Variáveis do aplicativo]** , suas Variáveis de aplicativo são adicionadas automaticamente. Essas variáveis permitem definir o comportamento da notificação. Por exemplo, você pode configurar uma tela de aplicativo específica para ser exibida quando o usuário ativar a notificação.

  ![](assets/push_content_4.png)

* A variável **[!UICONTROL Mensagem de notificação]**, manipulada automaticamente pelo SDK do FCM. O FCM exibe automaticamente a mensagem nos dispositivos dos usuários em nome do aplicativo do cliente. As mensagens de notificação contêm um conjunto predefinido de parâmetros e opções, mas ainda podem ser personalizadas com variáveis de aplicativo personalizadas.

  Para redigir a mensagem, clique no link **[!UICONTROL Título]** e **[!UICONTROL Corpo]** campos. Use o Editor de expressão para definir o conteúdo, personalizar os dados e adicionar conteúdo dinâmico.

  Para personalizar ainda mais sua notificação por push, você pode escolher uma imagem para adicionar à notificação por push, o ícone da notificação a ser exibido nos dispositivos dos perfis e sua cor.

  ![](assets/push_content_3.png)

>[!TAB iOS]

Para redigir a mensagem, clique no link **[!UICONTROL Título]** e **[!UICONTROL Corpo]** campos. Use o Editor de expressão para definir o conteúdo, personalizar os dados e adicionar conteúdo dinâmico.

Você pode adicionar um **[!UICONTROL Legenda]**, valor do parâmetro de subtítulo da carga de notificação do iOS. Consulte esta seção.

O modo Push silencioso permite que uma notificação &quot;silenciosa&quot; seja enviada a um aplicativo móvel. O usuário não está ciente da chegada da notificação. Ele é transferido diretamente para o aplicativo.

![](assets/push_content_1.png)

>[!ENDTABS]

## Configurações avançadas {#push-advanced}

>[!BEGINTABS]

>[!TAB Android]

![](assets/push_content_5.png)

| Parâmetro | Descrição |
|---------|---------|
| **[!UICONTROL Som]** | Defina o som que será reproduzido quando o dispositivo receber sua notificação. |
| **[!UICONTROL Contagem de notificações]** | Defina o número de novas informações não lidas a serem exibidas diretamente no ícone do aplicativo. Isso permite que o usuário veja rapidamente o número de notificações pendentes. |
| **[!UICONTROL ID do canal]** | Defina a ID do canal da sua notificação. O aplicativo deve criar um canal com essa ID de canal antes que qualquer notificação com essa ID de canal seja recebida. |
| **[!UICONTROL Ação Clicar]** | Defina a ação associada a um clique do usuário em sua notificação. Isso determina o comportamento quando o usuário interage com a notificação, como abrir uma tela específica ou executar uma ação específica no aplicativo. |
| **[!UICONTROL Tag]** | Defina um identificador usado para substituir notificações existentes na gaveta de notificações. Isso ajuda a evitar o acúmulo de várias notificações e garante que somente a notificação relevante mais recente seja exibida. |
| **[!UICONTROL Priority]** | Defina o nível de prioridade da sua notificação, que pode ser padrão, mínimo, baixo ou alto. O nível de prioridade determina a importância e a urgência da notificação, influenciando como ela é exibida e se pode ignorar determinadas configurações do sistema. Para obter mais informações, consulte a [documentação do FCM](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#notificationpriority). |
| **[!UICONTROL Visibilidade]** | Defina o nível de visibilidade de sua notificação, que pode ser público, privado ou secreto. O nível de visibilidade determina quanto do conteúdo da notificação é exibido na tela de bloqueio e em outras áreas confidenciais. Para obter mais informações, consulte [Documentação do FCM](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#visibility). |
| **[!UICONTROL Fixo]** | Quando ativada, a notificação permanece visível mesmo depois que o usuário clica nela. <br>Se desativada, a notificação é automaticamente descartada quando o usuário interage com ela. O comportamento fixo permite que notificações importantes persistam na tela por períodos mais longos. |
| **[!UICONTROL Variáveis de aplicativo]** | Permite definir o comportamento da notificação. Essas variáveis são totalmente personalizáveis e incluídas como parte da carga da mensagem enviada ao dispositivo móvel. |

>[!TAB iOS]

![](assets/push_content_2.png)

| Parâmetro | Descrição |
|---------|---------|
| **[!UICONTROL Modo de alerta crítico]** | Ative essa opção para adicionar som à sua notificação, mesmo quando o telefone do usuário estiver configurado para o modo de foco ou se o iPhone estiver sem áudio. Isso garante que alertas importantes sejam notados pelo usuário. |
| **[!UICONTROL Limpar selo]** | Ative essa opção para atualizar o valor do selo exibido no ícone do aplicativo. Isso garante que o selo reflita com precisão o número de novas informações não lidas. |
| **[!UICONTROL Contagem de notificações]** | Defina um número que será exibido diretamente no ícone do aplicativo, indicando o número de novas informações não lidas. Isso fornece uma referência visual rápida para o usuário. |
| **[!UICONTROL Volume]** | Volume do som, de 0 a 100. |
| **[!UICONTROL Conteúdo mutável]** | Ative essa opção para permitir que o aplicativo móvel baixe conteúdo de mídia associado à notificação. Para saber mais, consulte a [documentação para desenvolvedores da Apple](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ModifyingNotifications.html). |
| **[!UICONTROL Pontuação de relevância]** | Defina uma pontuação de relevância de 0 a 100 para priorizar a ordem das notificações no resumo de notificação. Pontuações mais altas indicam notificações mais importantes. |
| **[!UICONTROL Nível de interrupção]** | <ul> <li>**[!UICONTROL Ativo]**: selecionado por padrão; o sistema apresenta a notificação imediatamente, ativa a tela e pode reproduzir um som. As notificações não interrompem os modos de foco.</li><li>**[!UICONTROL Passivo]**: o sistema adiciona a notificação à lista de notificações sem ativar a tela ou reproduzir um som. As notificações não interrompem os modos de foco.</li><li>**[!UICONTROL Sensível ao tempo]**: o sistema apresenta a notificação imediatamente, ativa a tela, pode reproduzir um som e interrompe os modos de foco. Esse nível não requer uma permissão especial da Apple.</li> <li>**[!UICONTROL Crítico]**: o sistema apresenta a notificação imediatamente, ativa a tela e ignora os modos de foco e a opção de mudo. Observe que esse nível requer uma permissão especial da Apple.</ul> |
| **[!UICONTROL Thread-id]** | Identificador usado para agrupar notificações relacionadas. As notificações com a mesma ID de thread são organizadas como uma única conversa ou thread na lista de notificações. |
| **[!UICONTROL Categoria]** | Especifique o nome da ID de categoria associada à notificação. Isso permite a exibição de botões de ação, permitindo que o usuário execute várias tarefas diretamente da notificação, sem abrir o aplicativo. |
| **[!UICONTROL ID do conteúdo do público-alvo]** | Identificador usado para definir qual janela de aplicativo será apresentada quando a notificação for aberta. |
| **[!UICONTROL Imagem de inicialização]** | Especifique o nome do arquivo de imagem a ser exibido quando o usuário optar por iniciar seu aplicativo a partir da notificação. A imagem selecionada será exibida em vez da tela de inicialização regular do aplicativo. |
| **[!UICONTROL Variáveis de aplicativo]** | Permite definir o comportamento da notificação. Essas variáveis são totalmente personalizáveis e incluídas como parte da carga da mensagem enviada ao dispositivo móvel. |

>[!ENDTABS]

<!--Sounds must be included in the application and defined when the service is created. Refer to this section.-->



