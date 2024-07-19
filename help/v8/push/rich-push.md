---
audience: end-user
title: Criar um delivery de notificação por push avançado
description: Saiba como criar uma entrega de notificação por push avançada do Android com o Adobe Campaign Web
exl-id: a87cb933-b564-4fa4-b173-6a94d7e27da5
source-git-commit: bb61fdb34fecb4131d4069965cda8a3a5099b6bc
workflow-type: tm+mt
source-wordcount: '1420'
ht-degree: 10%

---

# Criar uma entrega de push avançada do Android {#rich-push}


>[!CONTEXTUALHELP]
>id="acw_deliveries_push_remind_later"
>title="Botão Lembrar mais tarde"
>abstract="O botão **Lembrar mais tarde** fornece a opção de agendar um lembrete. O campo Carimbo de data/hora exige um valor que represente a época em segundos."

>[!AVAILABILITY]
>
>Este recurso está em **Disponibilidade Limitada** (DL).

Com o Firebase Cloud Messaging, você pode escolher entre dois tipos de mensagens:

* A **[!UICONTROL Mensagem de dados]** é manipulada pelo aplicativo cliente. Essas mensagens são enviadas diretamente para o aplicativo móvel, que gera e exibe uma notificação do Android no dispositivo. As mensagens de dados contêm somente as variáveis personalizadas do aplicativo.

* A **[!UICONTROL Mensagem de notificação]**, manipulada automaticamente pelo SDK do FCM. O FCM exibe automaticamente a mensagem nos dispositivos dos usuários em nome do aplicativo do cliente. As mensagens de notificação contêm um conjunto predefinido de parâmetros e opções, mas ainda podem ser personalizadas com variáveis de aplicativo personalizadas.

![](assets/rich_push.png){zoomable="yes"}

## Definir o conteúdo da notificação {#push-message}

Depois que o delivery de push é criado, é possível definir seu conteúdo. Três modelos estão disponíveis:

* **Modelo padrão** permite enviar notificações com um ícone simples e uma imagem associada.

* **Modelo Básico** pode incluir texto, imagens e botões em suas notificações.

* **Modelo do Carrossel** permite enviar notificações com texto e várias imagens que os usuários podem passar.

Navegue pelas guias abaixo para saber mais sobre como personalizar esses modelos.

>[!BEGINTABS]

>[!TAB Modelo padrão]

1. No menu suspenso **[!UICONTROL Modelo]**, selecione **[!UICONTROL Padrão]**.

   ![](assets/rich_push_default.png)

1. Para redigir a mensagem, digite o texto nos campos **[!UICONTROL Título]** e **[!UICONTROL Mensagem]**.

   ![](assets/rich_push_default_2.png)

1. Use o Editor de expressão para definir o conteúdo, personalizar os dados e adicionar conteúdo dinâmico. [Saiba mais](../personalization/personalize.md)

1. Defina a **[!UICONTROL Ação de clique]** associada a um clique do usuário em sua notificação. Isso determina o comportamento quando o usuário interage com a notificação, como abrir uma tela específica ou executar uma ação específica no aplicativo.

1. Para personalizar ainda mais sua notificação por push, você pode escolher uma URL da **[!UICONTROL Imagem]** para adicionar à sua notificação por push e o **[!UICONTROL Ícone]** da notificação para exibir nos dispositivos de seus perfis.

   ![](assets/rich_push_default_3.png)

1. Defina as **[!UICONTROL Configurações avançadas]** de sua notificação por push. [Saiba mais](#push-advanced)

Depois de definir o conteúdo da mensagem, você pode usar assinantes de teste para pré-visualizar e testar a mensagem.

>[!TAB Modelo básico]

1. No menu suspenso **[!UICONTROL Modelo]**, selecione **[!UICONTROL Básico]**.

   ![](assets/rich_push_basic.png)

1. Para redigir a mensagem, digite o texto nos campos **[!UICONTROL Título]**, **[!UICONTROL Mensagem]** e **[!UICONTROL Mensagem expandida]**.

   O texto **[!UICONTROL Mensagem]** aparece no modo de exibição recolhido enquanto a **[!UICONTROL Mensagem expandida]** é exibida quando a notificação é expandida.

   ![](assets/rich_push_basic_2.png)

1. Use o Editor de expressão para definir o conteúdo, personalizar os dados e adicionar conteúdo dinâmico. [Saiba mais](../personalization/personalize.md)

1. Adicione a URL que define a **[!UICONTROL Ação de clique]** associada a um clique do usuário em sua notificação. Isso determina o comportamento quando o usuário interage com a notificação, como abrir uma tela específica ou executar uma ação específica no aplicativo.

1. Selecione o **[!UICONTROL Tipo de link]** da URL que você adicionou ao campo **[!UICONTROL Ação de clique]**:

   * **[!UICONTROL URL da Web]**: as URLs da Web direcionam os usuários para o conteúdo online. Ao clicar em, eles solicitam que o navegador da Web padrão do dispositivo abra e navegue até o URL designado.

   * **[!UICONTROL Deeplink]**: deep links são URLs que direcionam os usuários para seções específicas dentro de um aplicativo, mesmo que ele esteja fechado. Quando clicada, uma caixa de diálogo pode ser exibida, permitindo que os usuários escolham entre vários aplicativos capazes de manipular o link.

   * **[!UICONTROL Abrir aplicativo]**: as URLs de aplicativos abertos permitem que você se conecte diretamente ao conteúdo de um aplicativo. Ela permite que o aplicativo se estabeleça como o manipulador padrão para um tipo específico de link, ignorando a caixa de diálogo de desambiguação.

   Para obter mais informações sobre como lidar com Links de aplicativos da Android, consulte a [documentação de Desenvolvedores da Android](https://developer.android.com/training/app-links).

   ![](assets/rich_push_basic_3.png)

1. Para personalizar ainda mais sua notificação por push, você pode escolher uma URL da **[!UICONTROL Imagem]** para adicionar à sua notificação por push e o **[!UICONTROL Ícone]** da notificação para exibir nos dispositivos de seus perfis.

1. Clique no **[!UICONTROL Botão Adicionar]** e preencha os seguintes campos:

   * **[!UICONTROL Rótulo]**: texto exibido no botão.
   * **[!UICONTROL URI do link]**: especifique o URI a ser executado ao clicar no botão.
   * **[!UICONTROL Tipo de link]**: tipo de link **[!UICONTROL URL da Web]**, **[!UICONTROL Deeplink]** ou **[!UICONTROL Abrir Aplicativo]**.

   Você tem a opção de incluir até três botões na sua notificação por push. Se você optar pelo **[!UICONTROL botão Lembrar mais tarde]**, poderá incluir no máximo dois botões.

   ![](assets/rich_push_basic_4.png)

1. Clique no botão **[!UICONTROL Adicionar lembrete mais tarde]** para adicionar uma opção Lembrar-me mais tarde à sua notificação por push. Insira um **[!UICONTROL Rótulo]** e **[!UICONTROL Carimbo de data/hora]**.

   O campo Timestamp espera um valor que representa a época em segundos.

   ![](assets/rich_push_basic_5.png)

1. Defina as **[!UICONTROL Configurações avançadas]** de sua notificação por push. [Saiba mais](#push-advanced)

Depois de definir o conteúdo da mensagem, você pode usar assinantes de teste para pré-visualizar e testar a mensagem.

>[!TAB Modelo do carrossel]

1. No menu suspenso **[!UICONTROL Modelo]**, selecione **[!UICONTROL Carrossel]**.

   ![](assets/rich_push_carousel.png)

1. Para redigir a mensagem, digite o texto nos campos **[!UICONTROL Título]**, **[!UICONTROL Mensagem]** e **[!UICONTROL Mensagem expandida]**.

   O texto **[!UICONTROL Mensagem]** aparece no modo de exibição recolhido enquanto a **[!UICONTROL Mensagem expandida]** é exibida quando a notificação é expandida.

   ![](assets/rich_push_carousel_1.png)

1. Use o Editor de expressão para definir o conteúdo, personalizar os dados e adicionar conteúdo dinâmico. [Saiba mais](../personalization/personalize.md)

1. Adicione a URL que define a **[!UICONTROL Ação de clique]** associada a um clique do usuário em sua notificação. Isso determina o comportamento quando o usuário interage com a notificação, como abrir uma tela específica ou executar uma ação específica no aplicativo.

1. Selecione o **[!UICONTROL Tipo de link]** da URL que você adicionou ao campo **[!UICONTROL Ação de clique]**:

   * **[!UICONTROL URL da Web]**L: URLs da Web direcionam usuários para conteúdo online. Ao clicar em, eles solicitam que o navegador da Web padrão do dispositivo abra e navegue até o URL designado.

   * **[!UICONTROL Deeplink]**: deep links são URLs que direcionam os usuários para seções específicas dentro de um aplicativo, mesmo que ele esteja fechado. Quando clicada, uma caixa de diálogo pode ser exibida, permitindo que os usuários escolham entre vários aplicativos capazes de manipular o link.

   * **[!UICONTROL Abrir aplicativo]**: as URLs de aplicativos abertos permitem que você se conecte diretamente ao conteúdo de um aplicativo. Ela permite que o aplicativo se estabeleça como o manipulador padrão para um tipo específico de link, ignorando a caixa de diálogo de desambiguação.

   Para obter mais informações sobre como lidar com Links de aplicativos da Android, consulte a [documentação de Desenvolvedores da Android](https://developer.android.com/training/app-links).

   ![](assets/rich_push_carousel_2.png)

1. Para personalizar ainda mais sua notificação por push, você pode escolher o **[!UICONTROL Ícone]** da notificação para exibir nos dispositivos de seus perfis.

1. Escolha como o **[!UICONTROL carrossel]** é operado:

   * **[!UICONTROL Automático]**: percorre automaticamente imagens como slides, fazendo a transição em intervalos predefinidos.
   * **[!UICONTROL Manual]**: permite que os usuários deslizem manualmente entre slides para navegar pelas imagens.

     Habilite a opção **[!UICONTROL Filmstrip]** para incluir visualizações das imagens anteriores e seguintes ao lado do slide principal.

1. Clique em **[!UICONTROL Adicionar imagem]** e insira a URL da imagem e o texto.

   Certifique-se de incluir no mínimo três imagens e no máximo cinco imagens.

   ![](assets/rich_push_carousel_3.png)

1. Manipule a ordem das imagens com as setas para baixo e para cima.

1. Defina as **[!UICONTROL Configurações avançadas]** de sua notificação por push. [Saiba mais](#push-advanced)

Depois de definir o conteúdo da mensagem, você pode usar assinantes de teste para pré-visualizar e testar a mensagem.

>[!ENDTABS]

## Configurações avançadas de notificações por push {#push-advanced}

![](assets/push_content_5.png){zoomable="yes"}

| Parâmetro | Descrição |
|---------|---------|
| **[!UICONTROL Cor do ícone]** | Defina a cor do ícone com seus códigos de cor hexadecimal. |
| **[!UICONTROL Cor do título]** | Defina a cor do Título com os códigos de cor hexadecimal. |
| **[!UICONTROL Cor do texto da mensagem]** | Defina a cor do texto da mensagem com os códigos de cor hexadecimal. |
| **[!UICONTROL Cor de fundo da notificação]** | Defina a cor do plano de fundo da Notificação com os códigos de cor hexadecimal. |
| **[!UICONTROL Som]** | Defina o som que será reproduzido quando o dispositivo receber sua notificação. |
| **[!UICONTROL Contagem de Notificações]** | Defina o número de novas informações não lidas a serem exibidas diretamente no ícone do aplicativo. Isso permite que o usuário veja rapidamente o número de notificações pendentes. |
| **[!UICONTROL ID do canal]** | Defina a ID do canal da sua notificação. O aplicativo deve criar um canal com essa ID de canal antes que qualquer notificação com essa ID de canal seja recebida. |
| **[!UICONTROL Marca]** | Defina um identificador usado para substituir notificações existentes na gaveta de notificações. Isso ajuda a evitar o acúmulo de várias notificações e garante que somente a notificação relevante mais recente seja exibida. |
| **[!UICONTROL Priority]** | Defina o nível de prioridade da sua notificação, que pode ser padrão, mínimo, baixo ou alto. O nível de prioridade determina a importância e a urgência da notificação, influenciando como ela é exibida e se pode ignorar determinadas configurações do sistema. Para obter mais informações, consulte a [documentação do FCM](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#notificationpriority). |
| **[!UICONTROL Visibilidade]** | Defina o nível de visibilidade de sua notificação, que pode ser público, privado ou secreto. O nível de visibilidade determina quanto do conteúdo da notificação é exibido na tela de bloqueio e em outras áreas confidenciais. Para obter mais informações, consulte a [documentação do FCM](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#visibility). |
| **[!UICONTROL Notificação fixa]** | Quando ativada, a notificação permanece visível mesmo depois que o usuário clica nela. <br>Se desativada, a notificação é automaticamente descartada quando o usuário interage com ela. O comportamento fixo permite que notificações importantes persistam na tela por períodos mais longos. |
| **[!UICONTROL Variáveis de aplicativo]** | Permite definir o comportamento da notificação. Essas variáveis são totalmente personalizáveis e incluídas com parte do conteúdo da mensagem enviada para o dispositivo móvel. |
