---
audience: end-user
title: Rastrear suas mensagens
description: Saiba como adicionar links e rastrear mensagens enviadas
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
badge: label="Alpha" type="Positive"
source-git-commit: 05d87fc9ff8f5e2038eba4cc9438e058566e04c8
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 96%

---

# Adicionar links e rastrear mensagens {#tracking}

Use o Designer de email para adicionar links ao seu conteúdo e rastrear as mensagens enviadas, a fim de monitorar o comportamento dos recipients.

## Inserir links {#insert-links}

Ao criar uma mensagem, você pode adicionar links ao seu conteúdo.

>[!NOTE]
>
>Quando o rastreamento é ativado, todos os links incluídos no conteúdo da mensagem são rastreados.

Para inserir links no conteúdo do email, siga as etapas abaixo:

1. Selecione um elemento e clique em **[!UICONTROL Inserir link]** na barra de ferramentas contextual.

   ![](assets/message-tracking-insert-link.png)

1. Adicione um **[!UICONTROL Rótulo]** e um **[!UICONTROL Link]**.

1. Salve as alterações.

1. Depois que o link for criado, você ainda poderá modificá-lo no **[!UICONTROL Configurações]** guia.

   * Você pode editar o link e alterar seu **[!UICONTROL Público-alvo]**.
   * Você pode optar por sublinhar o link ou não, marcando a opção correspondente.

   ![](assets/message-tracking-link-settings.png)

>[!NOTE]
>
>As mensagens de email de marketing devem incluir um link para opção de não participação, o que não é necessário para mensagens transacionais. A categoria da mensagem (**[!UICONTROL Marketing]** ou **[!UICONTROL Transacional]**) é definida no nível da superfície de canal (ou seja, predefinição de mensagem) e ao criar a mensagem.

Um link específico para a mirror page deve ser adicionado em todas as suas mensagens de email. Saiba mais sobre a mirror page [nesta seção](mirror-page.md).

## Gerenciar rastreamento {#manage-tracking}

O [Designer de email](create-email-content.md) permite gerenciar os URLs rastreados, como editar o tipo de rastreamento de cada link.

1. Clique no ícone **[!UICONTROL Links]** no painel esquerdo para exibir a lista de todos os URLs do conteúdo a ser rastreado.

   Essa lista oferece uma visualização centralizada, permitindo localizar cada URL no conteúdo do email.

1. Para editar um link, clique no ícone de lápis correspondente.

   ![](assets/message-tracking-edit-links.png)

1. Você pode modificar o **[!UICONTROL Tipo de rastreamento]**, se necessário:

   ![](assets/message-tracking-edit-a-link.png)

   Para cada URL rastreado é possível definir o modo de rastreamento utilizando um destes valores:

   * **[!UICONTROL Rastrear]**: ativa o rastreamento nesse URL.
   * **[!UICONTROL Opt out]**: considera-o como um URL de recusa ou cancelamento de assinatura.
   * **[!UICONTROL Mirror page]**: considera-o como um URL de mirror page.
   * **[!UICONTROL Nunca]**: nunca ativa o rastreamento desse URL.<!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

1. Adicione uma **[!UICONTROL Categoria]** ao seu link para agrupar links rastreados e clique em **[!UICONTROL Salvar]**.

   ![](assets/message-tracking-edit-a-link_2.png)

1. Após enviar a entrega, acesse o relatório de entrega. Em **[!UICONTROL Rastreamento]**, o relatório **[!UICONTROL Fluxos de cliques e URL]** exibe quais são os URLs mais visitados de sua entrega. [Saiba mais](../reporting/reports.md)
