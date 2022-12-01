---
audience: end-user
title: Rastrear suas mensagens
description: Saiba como adicionar links e rastrear mensagens enviadas
source-git-commit: 9def5ea791e4ef42968cd34536f3ddeac7fc238c
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 3%

---


# Adicionar links e rastrear mensagens {#tracking}

>[!NOTE]
>
>Esta documentação está em construção e é atualizada com frequência. A versão final desse conteúdo estará pronta em janeiro de 2023.

Use [!DNL Journey Optimizer] para adicionar links ao seu conteúdo e rastrear as mensagens enviadas para monitorar o comportamento dos recipients.

## Ativar rastreamento {#enable-tracking}

Você pode ativar o rastreamento no nível da mensagem de email marcando a variável **[!UICONTROL Aberturas de email]** e/ou **[!UICONTROL Clique no email]** ao criar a mensagem.

![](assets/message-tracking.png)

>[!NOTE]
>
>Ambas as opções são ativadas por padrão.

Isso permitirá rastrear o comportamento dos recipients por meio de:

* **[!UICONTROL Aberturas de email]**: Mensagens que foram abertas.
* **[!UICONTROL Clique no email]**: Cliques em links em um email.

## Inserir links {#insert-links}

Ao criar uma mensagem, você pode adicionar links ao seu conteúdo.

>[!NOTE]
>
>When [o rastreamento está ativado](#enable-tracking), todos os links incluídos no conteúdo da mensagem são rastreados.

Para inserir links no seu conteúdo de email, siga as etapas abaixo:

1. Selecione um elemento e clique em **[!UICONTROL Inserir link]** na barra de ferramentas contextual.

   ![](assets/message-tracking-insert-link.png)

1. Escolha o tipo de link que deseja criar:

   * **[!UICONTROL Link externo]**: Insira um link para um URL externo.

   * **[!UICONTROL Página de aterrissagem]**: Insira um link para uma landing page.

   * **[!UICONTROL Um clique para recusar]**: Insira um link para permitir que os usuários cancelem rapidamente a assinatura de suas comunicações, sem a necessidade de confirmar a recusa.

   * **[!UICONTROL Aceitação/assinatura externa]**: Insira um link para aceitar as comunicações de recebimento da sua marca.

   * **[!UICONTROL Cancelamento/cancelamento de subscrição externo]**: Insira um link para cancelar a assinatura do recebimento de comunicações da sua marca.

   * **[!UICONTROL Mirror page]**: Insira um link para exibir o conteúdo do email em um navegador da Web. Saiba mais [nesta seção](#mirror-page).

   ![](assets/message-tracking-links.png)

1. Você pode personalizar seus links.

1. Salve as alterações.

1. Depois que o link for criado, você ainda poderá modificá-lo da variável **[!UICONTROL Configurações do componente]** painel à direita.

   * Você pode editar o link e alterar seu tipo.
   * Você pode optar por sublinhar o link ou não, marcando a opção correspondente.

   ![](assets/message-tracking-link-settings.png)

>[!NOTE]
>
>As mensagens de email de tipo de marketing devem incluir um link para opção de não participação, que não é necessário para mensagens transacionais. A categoria da mensagem (**[!UICONTROL Marketing]** ou **[!UICONTROL Transacional]**) é definida no nível da superfície do canal (ou seja, predefinição de mensagem) e ao criar a mensagem.

## Link para uma mirror page {#mirror-page}

A mirror page é uma página HTML acessível online através de um navegador da Web. Seu conteúdo é idêntico ao conteúdo do email.

Para adicionar um link a uma mirror page no seu email, [inserir um link](#insert-links) e selecione **[!UICONTROL Mirror page]** como o tipo de link.

![](assets/message-tracking-mirror-page.png)

A mirror page é criada automaticamente.

>[!IMPORTANT]
>
>Os links de mirror pages são gerados automaticamente e não podem ser editados. Eles contêm todos os dados personalizados criptografados necessários para renderizar o email original. Como resultado, o uso de atributos personalizados com valores grandes pode gerar URLs de mirror pages longas, o que pode impedir que o link funcione em navegadores da Web com tamanho máximo de URLs.

Depois que o email for enviado, quando os recipients clicarem no link da mirror page, o conteúdo do email será exibido no navegador padrão.

>[!NOTE]
>
>Na prova enviada aos perfis de teste, o link para a mirror page não está ativo. Ela só é ativada nas mensagens finais.

O período de retenção de uma mirror page é de 60 dias. Após esse atraso, a mirror page não estará mais disponível.

## Gerenciar rastreamento {#manage-tracking}

O [Email Designer](create-email-content.md) permite gerenciar os URLs rastreados, como editar o tipo de rastreamento para cada link.

1. Clique no botão **[!UICONTROL Links]** ícone do painel esquerdo para exibir a lista de todos os URLs do seu conteúdo que serão rastreados.

   Essa lista permite que você tenha uma visualização centralizada e localize cada URL no conteúdo do email.

1. Para editar um link, clique no ícone de lápis correspondente.

   ![](assets/message-tracking-edit-links.png)

1. Você pode modificar o **[!UICONTROL Tipo de rastreamento]** se necessário:

   ![](assets/message-tracking-edit-a-link.png)

   Para cada URL rastreado, é possível definir o modo de rastreamento para um destes valores:

   * **[!UICONTROL Rastreado]**: Ativa o rastreamento nesse URL.
   * **[!UICONTROL Recusar]**: Considera esse URL como recusa ou cancelamento de subscrição.
   * **[!UICONTROL Mirror page]**: Considera esse URL como sendo de mirror page.
   * **[!UICONTROL Nunca]**: Nunca ativa o rastreamento desse URL. <!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

Os relatórios sobre aberturas e cliques estão disponíveis no relatório Ao vivo e no relatório Global .
