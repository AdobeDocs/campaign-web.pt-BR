---
audience: end-user
title: Criar um delivery de notificação por push
description: Saiba como criar um delivery de notificação por push com o Adobe Campaign Web
badge: label="Beta"
exl-id: 031bc38a-2435-4468-8ee6-3bcf1132da55
source-git-commit: 54f91769daff0a6043a345ee44ccd84229336c36
workflow-type: tm+mt
source-wordcount: '1484'
ht-degree: 38%

---

# Criar uma entrega de mensagem por push {#content-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_android_content"
>title="Conteúdo de push para Android"
>abstract="Defina o conteúdo da sua notificação por push para dispositivos Android. Para redigir a mensagem, clique no link **Título** e **Mensagem** campos. Use o Editor de expressão para personalizar dados e adicionar conteúdo dinâmico. Para personalizar ainda mais sua notificação por push, você pode escolher uma imagem para adicionar à notificação por push, o ícone da notificação a ser exibido nos dispositivos dos perfis e sua cor. Para obter mais configurações personalizadas, navegue até a **Configurações avançadas** seção."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_content"
>title="Conteúdo de push para iOS"
>abstract="Defina o conteúdo da sua notificação por push para dispositivos iOS. Para redigir a mensagem, clique no link **Título** e **Mensagem** campos. Use o Editor de expressão para personalizar dados e adicionar conteúdo dinâmico. Para obter mais configurações personalizadas, navegue até a **Configurações avançadas** seção."

## Definir o conteúdo da notificação {#push-message}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_msg"
>title="Mensagem por push para iOS"
>abstract="Defina o título e o conteúdo da mensagem por push para iOS. Use a caixa de diálogo de personalização para personalizar o conteúdo e adicionar condições."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_silent"
>title="Notificação silenciosa para iOS"
>abstract="O modo Push silencioso permite que uma notificação “silenciosa” seja enviada a um aplicativo móvel. O usuário não está ciente da chegada da notificação. Ele é transferido diretamente para o aplicativo."

Depois que o delivery de push é criado, é possível definir seu conteúdo. Os parâmetros e as configurações dependem do sistema operacional móvel: Android ou iOS. Navegue pelas guias abaixo para saber como compor sua mensagem para cada sistema operacional.

>[!BEGINTABS]

>[!TAB Android]

Com o Firebase Cloud Messaging, você pode escolher entre dois tipos de mensagens:

* A variável **[!UICONTROL Mensagem de dados]** é manipulada pelo aplicativo do cliente. Essas mensagens são enviadas diretamente para o aplicativo móvel, que gera e exibe uma notificação do Android no dispositivo. As mensagens de dados contêm somente as variáveis personalizadas do aplicativo.

  Para definir o conteúdo, personalizar dados e adicionar conteúdo dinâmico, clique no link **[!UICONTROL Mensagem]** e use o Editor de expressão. Você pode acessar esse editor para personalizar suas mensagens.
No **[!UICONTROL Variáveis do aplicativo]** , suas Variáveis de aplicativo são adicionadas automaticamente. Essas variáveis permitem definir o comportamento da notificação. Por exemplo, você pode configurar uma tela de aplicativo específica para ser exibida quando o usuário ativar a notificação.

  ![](assets/push_content_4.png)

* A variável **[!UICONTROL Mensagem de notificação]**, manipulada automaticamente pelo SDK do FCM. O FCM exibe automaticamente a mensagem nos dispositivos dos usuários em nome do aplicativo do cliente. As mensagens de notificação contêm um conjunto predefinido de parâmetros e opções, mas ainda podem ser personalizadas com variáveis de aplicativo personalizadas.

  Para redigir a mensagem, clique no link **[!UICONTROL Título]** e **[!UICONTROL Mensagem]** campos. Use o Editor de expressão para definir o conteúdo, personalizar os dados e adicionar conteúdo dinâmico.

  Para personalizar ainda mais sua notificação por push, você pode escolher uma imagem para adicionar à notificação por push, o ícone da notificação a ser exibido nos dispositivos dos perfis e sua cor.

  ![](assets/push_content_3.png)

>[!TAB iOS]

Para redigir a mensagem, clique no link **[!UICONTROL Título]** e **[!UICONTROL Mensagem]** campos. Use o Editor de expressão para definir o conteúdo, personalizar os dados e adicionar conteúdo dinâmico.

Você pode adicionar um **[!UICONTROL Legenda]**, valor do parâmetro de subtítulo da carga de notificação do iOS. Consulte esta seção.

O modo Push silencioso permite que uma notificação “silenciosa” seja enviada a um aplicativo móvel. O usuário não está ciente da chegada da notificação. Ele é transferido diretamente para o aplicativo.

![](assets/push_content_1.png)

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
>title="Número da medalha"
>abstract="Use esta opção para definir o número de novas informações não lidas a serem exibidas diretamente no ícone do aplicativo. Isso permite que o usuário veja rapidamente o número de notificações pendentes."


>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_mutable"
>title="Conteúdo mutável"
>abstract="Use essa opção para permitir que o aplicativo para dispositivos móveis baixe conteúdo de mídia associado à notificação."

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
| **[!UICONTROL Variáveis do aplicativo]** | Permite definir o comportamento da notificação. Essas variáveis são totalmente personalizáveis e incluídas com parte do conteúdo da mensagem enviada para o dispositivo móvel. |

>[!TAB iOS]

![](assets/push_content_2.png)

| Parâmetro | Descrição |
|---------|---------|
| **[!UICONTROL Modo de alerta crítico]** | Habilite essa opção para adicionar som à sua notificação, mesmo que o telefone do usuário esteja configurado no modo Foco ou se estiver no modo silencioso. Isso garante que alertas importantes sejam notados pelo usuário. |
| **[!UICONTROL Limpar selo]** | Ative essa opção para atualizar o valor do selo exibido no ícone do aplicativo. Isso garante que o selo reflita com precisão o número de novas informações não lidas. |
| **[!UICONTROL Contagem de notificações]** | Defina um número que será exibido diretamente no ícone do aplicativo, indicando o número de novas informações não lidas. Isso fornece uma referência visual rápida para o usuário. |
| **[!UICONTROL Volume]** | Volume do som, de 0 a 100. |
| **[!UICONTROL Conteúdo mutável]** | Ative essa opção para permitir que o aplicativo móvel baixe conteúdo de mídia associado à notificação. Para saber mais, consulte a [documentação para desenvolvedores da Apple](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ModifyingNotifications.html). |
| **[!UICONTROL Pontuação de relevância]** | Defina uma pontuação de relevância de 0 a 100 para priorizar a ordem das notificações no resumo de notificações. Pontuações mais altas indicam notificações mais importantes. |
| **[!UICONTROL Nível de interrupção]** | <ul> <li>**[!UICONTROL Ativo]**: selecionado por padrão; o sistema apresenta a notificação imediatamente, ativa a tela e pode reproduzir um som. As notificações não interrompem os modos de foco.</li><li>**[!UICONTROL Passivo]**: o sistema adiciona a notificação à lista de notificações sem ativar a tela ou reproduzir um som. As notificações não interrompem os modos de foco.</li><li>**[!UICONTROL Sensível ao tempo]**: o sistema apresenta a notificação imediatamente, ativa a tela, pode reproduzir um som e interrompe os modos de foco. Esse nível não requer uma permissão especial da Apple.</li> <li>**[!UICONTROL Crítico]**: o sistema apresenta a notificação imediatamente, ativa a tela e ignora os modos de foco e a opção de mudo. Observe que esse nível requer uma permissão especial da Apple.</ul> |
| **[!UICONTROL Thread-id]** | Identificador usado para agrupar notificações relacionadas. As notificações com a mesma ID de thread são organizadas como uma única conversa ou thread na lista de notificações. |
| **[!UICONTROL Categoria]** | Especifique o nome da ID da categoria associada à notificação. Isso habilita a exibição de botões de ação, permitindo que o usuário execute várias tarefas diretamente da notificação, sem abrir o aplicativo. |
| **[!UICONTROL ID do conteúdo do Target]** | Identificador usado para definir qual janela de aplicativo será apresentada quando a notificação for aberta. |
| **[!UICONTROL Imagem de inicialização]** | Especifique o nome do arquivo de imagem a ser exibido quando o usuário optar por iniciar seu aplicativo a partir da notificação. A imagem selecionada será exibida em vez da tela de inicialização regular do aplicativo. |
| **[!UICONTROL Variáveis do aplicativo]** | Permite definir o comportamento da notificação. Essas variáveis são totalmente personalizáveis e incluídas com parte do conteúdo da mensagem enviada para o dispositivo móvel. |

>[!ENDTABS]

<!--Sounds must be included in the application and defined when the service is created. Refer to this section.-->
