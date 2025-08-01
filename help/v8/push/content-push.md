---
audience: end-user
title: Criar um delivery de notificação por push
description: Saiba como criar um delivery de notificação por push com o Adobe Campaign Web
exl-id: 031bc38a-2435-4468-8ee6-3bcf1132da55
source-git-commit: 53f4662e9497c8614036f9f89c1ea2b1233756f0
workflow-type: tm+mt
source-wordcount: '1632'
ht-degree: 42%

---


# Criar uma entrega por push {#content-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_android_content"
>title="Conteúdo de push para Android"
>abstract="Defina o conteúdo da sua notificação por push para dispositivos Android. Para começar a redigir a mensagem, clique em **Editar conteúdo**."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_content"
>title="Conteúdo de push para iOS"
>abstract="Defina o conteúdo da sua notificação por push para dispositivos iOS. Para começar a redigir a mensagem, clique em **Editar conteúdo**."

## Definir o conteúdo da notificação {#push-message}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_msg"
>title="Mensagem por push para iOS"
>abstract="Defina o conteúdo da sua notificação por push para dispositivos iOS. Para redigir a mensagem, clique nos campos **Título** e **Mensagem**. Use o Editor de expressão para personalizar dados e adicionar conteúdo dinâmico. Para mais configurações personalizadas, navegue até a seção **Configurações avançadas**."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_android_msg"
>title="Mensagem por push para Android"
>abstract="Defina o conteúdo da sua notificação por push para dispositivos Android. Para redigir a mensagem, clique nos campos **Título** e **Mensagem**. Use o Editor de expressão para personalizar dados e adicionar conteúdo dinâmico. Para personalizar ainda mais a notificação por push, você pode escolher uma imagem para adicionar à notificação por push, o ícone de notificação a ser exibido nos dispositivos dos perfis e sua cor. Para mais configurações personalizadas, navegue até a seção **Configurações avançadas**."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_silent"
>title="Notificação silenciosa para iOS"
>abstract="O modo Push silencioso permite que uma notificação “silenciosa” seja enviada a um aplicativo móvel. O usuário não está ciente da chegada da notificação. Ele é transferido diretamente para o aplicativo."

Depois que o delivery por push for criado, defina o conteúdo. Os parâmetros e as configurações dependem do sistema operacional móvel: Android ou iOS. Navegue pelas guias abaixo para saber como compor sua mensagem para cada sistema operacional.

>[!BEGINTABS]

>[!TAB Android]

Com o Firebase Cloud Messaging, escolha entre dois tipos de mensagens:

* A **[!UICONTROL Mensagem de dados]** é manipulada pelo aplicativo cliente. Essas mensagens são enviadas diretamente para o aplicativo móvel, que gera e exibe uma notificação do Android no dispositivo. As mensagens de dados contêm somente as variáveis personalizadas do aplicativo.

  Para definir o conteúdo, personalizar dados e adicionar conteúdo dinâmico, clique no campo **[!UICONTROL Mensagem]** e use o editor de expressão. Acesse este editor para personalizar suas mensagens.
No menu **[!UICONTROL Variáveis de aplicativo]**, suas variáveis de aplicativo são adicionadas automaticamente. Essas variáveis permitem definir o comportamento da notificação. Por exemplo, configure uma tela de aplicativo específica para ser exibida quando o usuário ativar a notificação.

  ![Descrição: Exemplo de definição de conteúdo para uma mensagem de dados em notificações do Android](assets/push_content_4.png){zoomable="yes"}

* A **[!UICONTROL Mensagem de notificação]**, manipulada automaticamente pelo FCM SDK. O FCM exibe automaticamente a mensagem nos dispositivos dos usuários em nome do aplicativo do cliente. As mensagens de notificação contêm um conjunto predefinido de parâmetros e opções, mas ainda podem ser personalizadas com variáveis de aplicativo personalizadas.

  Para redigir a mensagem, clique nos campos **[!UICONTROL Título]** e **[!UICONTROL Mensagem]**. Use o Editor de expressão para definir o conteúdo, personalizar dados e adicionar conteúdo dinâmico.

  Para personalizar ainda mais sua notificação por push, escolha uma imagem para adicionar a ela, o ícone da notificação a ser exibido nos dispositivos de seus perfis e a cor.

  ![Descrição: Exemplo de definição de conteúdo para uma mensagem de notificação em notificações do Android](assets/push_content_3.png){zoomable="yes"}

>[!TAB iOS]

Para redigir a mensagem, clique nos campos **[!UICONTROL Título]** e **[!UICONTROL Mensagem]**. Use o Editor de expressão para definir o conteúdo, personalizar dados e adicionar conteúdo dinâmico.

Você pode adicionar um **[!UICONTROL Subtítulo]**, que é o valor do parâmetro de subtítulo da carga de notificação do iOS. Consulte esta seção.

O modo Push silencioso permite que uma notificação “silenciosa” seja enviada a um aplicativo móvel. O usuário não está ciente da chegada da notificação. Ele é transferido diretamente para o aplicativo.

![Descrição: Exemplo de definição de conteúdo para notificações do iOS](assets/push_content_1.png){zoomable="yes"}

>[!ENDTABS]

## Configurações avançadas de notificações por push {#push-advanced}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings"
>title="Configurações avançadas para notificações por push"
>abstract="Defina configurações avançadas para sua notificação por push, como prioridade, contagem de notificações associadas, variáveis do aplicativo e muito mais."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_critical"
>title="Modo de alerta crítico"
>abstract="Habilite essa opção para adicionar som à sua notificação, mesmo que o telefone do usuário esteja configurado no modo Foco ou se estiver no modo silencioso. Isso garante que os usuários sejam notificados de alertas importantes em qualquer caso."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_count"
>title="Contagem de notificações"
>abstract="Use esta opção para exibir o número de notificações não lidas diretamente no ícone do aplicativo. Isso permite que o usuário veja rapidamente o número de notificações pendentes."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_mutable"
>title="Conteúdo mutável"
>abstract="Use essa opção para permitir que o aplicativo para dispositivos móveis baixe o conteúdo de mídia associado à notificação."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_score"
>title="Pontuação de relevância"
>abstract="Defina uma pontuação de relevância de 0 a 100 para priorizar a ordem das notificações no resumo de notificações. Pontuações mais altas indicam notificações mais importantes."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_app_variables"
>title="Variáveis de aplicativo"
>abstract="Use as variáveis do aplicativo para definir o comportamento das notificações. Essas variáveis são totalmente personalizáveis e incluídas com parte do conteúdo da mensagem enviada para o dispositivo móvel."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_category"
>title="ID da categoria"
>abstract="Especifique o nome da ID da categoria associada à notificação. Isso habilita a exibição de botões de ação, permitindo que o usuário execute várias tarefas diretamente da notificação, sem abrir o aplicativo."

As opções avançadas dependem do sistema operacional móvel: Android ou iOS. Navegue pelas guias abaixo para saber como definir opções para sua mensagem para cada sistema operacional.

>[!BEGINTABS]

>[!TAB Android]

![Descrição: Exemplo de configurações avançadas para notificações do Android](assets/push_content_5.png){zoomable="yes"}

| Parâmetro | Descrição |
|---------|---------|
| **[!UICONTROL Som]** | Defina o som que será reproduzido quando o dispositivo receber sua notificação. |
| **[!UICONTROL Contagem de Notificações]** | Defina o número de novas informações não lidas a serem exibidas diretamente no ícone do aplicativo. Isso permite que o usuário veja rapidamente o número de notificações pendentes. |
| **[!UICONTROL ID do canal]** | Defina a ID do canal da sua notificação. O aplicativo deve criar um canal com essa ID de canal antes que qualquer notificação com essa ID de canal seja recebida. |
| **[!UICONTROL Ação de clique]** | Defina a ação associada a um clique do usuário em sua notificação. Isso determina o comportamento quando o usuário interage com a notificação, como abrir uma tela específica ou executar uma ação específica no aplicativo. |
| **[!UICONTROL Marca]** | Defina um identificador usado para substituir notificações existentes na gaveta de notificações. Isso ajuda a evitar o acúmulo de várias notificações e garante que somente a notificação relevante mais recente seja exibida. |
| **[!UICONTROL Priority]** | Defina o nível de prioridade da sua notificação, que pode ser padrão, mínimo, baixo ou alto. O nível de prioridade determina a importância e a urgência da notificação, influenciando como ela é exibida e se pode ignorar determinadas configurações do sistema. Para obter mais informações, consulte a [documentação do FCM](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#notificationpriority). |
| **[!UICONTROL Visibilidade]** | Defina o nível de visibilidade de sua notificação, que pode ser público, privado ou secreto. O nível de visibilidade determina quanto do conteúdo da notificação é exibido na tela de bloqueio e em outras áreas confidenciais. Para obter mais informações, consulte a [documentação do FCM](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#visibility). |
| **[!UICONTROL Fixo]** | Quando ativada, a notificação permanece visível mesmo depois que o usuário clica nela. <br>Se desativada, a notificação é automaticamente descartada quando o usuário interage com ela. O comportamento fixo permite que notificações importantes persistam na tela por períodos mais longos. |
| **[!UICONTROL Variáveis de aplicativo]** | Permite definir o comportamento da notificação. Essas variáveis são totalmente personalizáveis e incluídas com parte do conteúdo da mensagem enviada para o dispositivo móvel. |

>[!TAB iOS]

![Descrição: Exemplo de configurações avançadas para notificações do iOS](assets/push_content_2.png){zoomable="yes"}

| Parâmetro | Descrição |
|---------|---------|
| **[!UICONTROL Modo de alerta crítico]** | Habilite essa opção para adicionar som à sua notificação, mesmo que o telefone do usuário esteja configurado no modo Foco ou se estiver no modo silencioso. Isso garante que alertas importantes sejam notados pelo usuário. Quando essa opção estiver selecionada, você poderá ajustar o volume da notificação usando a barra Volume level. Um número entre 0 e 100 acima da barra reflete suas configurações. |
| **[!UICONTROL Limpar medalha]** | Ative essa opção para atualizar o valor do selo exibido no ícone do aplicativo. Isso garante que o selo reflita com precisão o número de novas informações não lidas. |
| **[!UICONTROL Contagem de notificações]** | Defina um número que será exibido diretamente no ícone do aplicativo, indicando o número de novas informações não lidas. Isso fornece uma referência visual rápida para o usuário. |
| **[!UICONTROL Volume]** | Volume do som, de 0 a 100. |
| **[!UICONTROL Conteúdo mutável]** | Ative essa opção para permitir que o aplicativo móvel baixe conteúdo de mídia associado à notificação. Para saber mais, consulte a [documentação para desenvolvedores da Apple](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ModifyingNotifications.html). |
| **[!UICONTROL Conteúdo disponível]** | Ative essa opção para permitir que sua notificação acione atualizações em segundo plano em dispositivos iOS, mesmo quando o aplicativo não estiver aberto ativamente. Isso garante que conteúdo como mensagens ou atualizações de dados possam ser processados e armazenados na caixa de entrada do aplicativo, sem exigir interação do usuário. Quando selecionado, o sinalizador `content-available: 1` é adicionado à carga `aps` em conformidade com os padrões do Serviço de Notificação por Push (APNS) da Apple. |
| **[!UICONTROL Pontuação de relevância]** | Defina uma pontuação de relevância de 0 a 100 para priorizar a ordem das notificações no resumo de notificações. Pontuações mais altas indicam notificações mais importantes. |
| **[!UICONTROL Nível de interrupção]** | <ul> <li>**[!UICONTROL Ativo]**: definido por padrão, o sistema apresenta a notificação imediatamente, ativa a tela e pode reproduzir um som. As notificações não interrompem os modos de foco.</li><li>**[!UICONTROL Passivo]**: o sistema adiciona a notificação à lista de notificações sem ativar a tela ou reproduzir um som. As notificações não interrompem os modos de foco.</li><li>**[!UICONTROL Sensível ao tempo]**: o sistema apresenta a notificação imediatamente, ativa a tela, pode reproduzir um som e interrompe os modos de foco. Esse nível não requer permissão especial da Apple.</li> <li>**[!UICONTROL Crítico]**: o sistema apresenta a notificação imediatamente, ativa a tela e ignora os modos de foco e a opção de mudo. Observe que esse nível requer permissão especial da Apple.</ul> |
| **[!UICONTROL Thread-id]** | Identificador usado para agrupar notificações relacionadas. As notificações com a mesma ID de thread são organizadas como uma única conversa ou thread na lista de notificações. |
| **[!UICONTROL Categoria]** | Especifique o nome da ID da categoria associada à notificação. Isso habilita a exibição de botões de ação, permitindo que o usuário execute várias tarefas diretamente da notificação, sem abrir o aplicativo. |
| **[!UICONTROL ID do conteúdo do Target]** | Identificador usado para definir qual janela de aplicativo será apresentada quando a notificação for aberta. |
| **[!UICONTROL Imagem de inicialização]** | Especifique o nome do arquivo de imagem a ser exibido quando o usuário optar por iniciar seu aplicativo a partir da notificação. A imagem selecionada será exibida em vez da tela de inicialização regular do aplicativo. |
| **[!UICONTROL Variáveis de aplicativo]** | Permite definir o comportamento da notificação. Essas variáveis são totalmente personalizáveis e incluídas com parte do conteúdo da mensagem enviada para o dispositivo móvel. |

>[!ENDTABS]

<!--Sounds must be included in the application and defined when the service is created. Refer to this section.-->
