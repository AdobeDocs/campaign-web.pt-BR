---
audience: end-user
title: Rastrear suas mensagens
description: Saiba como adicionar links e rastrear mensagens enviadas
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 23%

---

# Adicionar links e rastrear mensagens {#tracking}

Use o Designer de email para adicionar links ao seu conteúdo e rastrear as mensagens enviadas, permitindo monitorar o comportamento dos destinatários.

## Inserir links {#insert-links}

Ao criar uma mensagem, você pode adicionar links ao seu conteúdo.

>[!NOTE]
>
>Quando o rastreamento é ativado, todos os links incluídos no conteúdo da mensagem são rastreados.

Para inserir links no seu conteúdo de email, siga estas etapas:

1. Selecione um elemento e clique em **[!UICONTROL Inserir link]** na barra de ferramentas contextual.

1. Escolha o tipo de link que deseja criar:

   ![Captura de tela mostrando a interface para inserir links na ferramenta de rastreamento de mensagens](assets/message-tracking-insert-link.png){zoomable="yes"}

   * **[!UICONTROL Link externo]**: insira um link para uma URL externa.

     >[!AVAILABILITY]
     >
     >Os seguintes recursos (link para **[!UICONTROL Página de aterrissagem]**, **[!UICONTROL Link de assinatura]** e **[!UICONTROL Link de cancelamento de assinatura]**) estão em Disponibilidade Limitada (DL). Eles estão restritos a clientes que estão migrando **do Adobe Campaign Standard para o Adobe Campaign v8** e não podem ser implantados em nenhum outro ambiente.

   * **[!UICONTROL Página de aterrissagem]**: insira um link para uma página de aterrissagem. Se você selecionar uma página de aterrissagem dinâmica (com a opção **[!UICONTROL Serviço da URL]** selecionada), será possível selecionar qualquer serviço da lista. [Saiba mais](../landing-pages/create-lp.md#define-actions-on-form-submission)

     ![Captura de tela mostrando a interface para vinculação a uma página de aterrissagem no designer de email](assets/email-link-to-landing-page.png){zoomable="yes"}

   * **[!UICONTROL Link de assinatura]**: insira um link para um serviço de assinatura. Quando os usuários clicam no link, eles são direcionados para a landing page de assinatura referenciada no serviço selecionado. [Saiba mais](../audience/manage-services.md#create-service)

     ![Captura de tela mostrando a interface para criar um link de assinatura padrão na ferramenta de serviço](assets/service-create-default-lp-link.png){zoomable="yes"}

   * **[!UICONTROL Link de cancelamento de assinatura]**: insira um link para um serviço de cancelamento de assinatura. Quando os assinantes clicam no link, eles são direcionados para a landing page de cancelamento de subscrição referenciada no serviço selecionado. [Saiba mais](../audience/manage-services.md#create-service)

   <!--* **[!UICONTROL Mirror page]**: Add a link to display the email content in a web browser. [Learn more]-->

1. Insira o URL desejado no campo correspondente ou selecione uma landing page ou um serviço e defina as configurações e os estilos do link.

1. Adicione um **[!UICONTROL Rótulo]** e um **[!UICONTROL Link]**.

1. Salve as alterações.

1. Depois de criar o link, modifique-o na guia **[!UICONTROL Configurações]**, se necessário.

   * Editar o link e alterar seu **[!UICONTROL Target]**.
   * Escolha se deseja sublinhar o link marcando a opção correspondente.

   ![Captura de tela mostrando a interface de configurações para modificar propriedades de links na ferramenta de rastreamento de mensagens](assets/message-tracking-link-settings.png){zoomable="yes"}

>[!NOTE]
>
>As mensagens de email de marketing devem incluir um link para opção de não participação, o que não é necessário para mensagens transacionais. A categoria da mensagem (**[!UICONTROL Marketing]** ou **[!UICONTROL Transacional]**) é definida no nível da superfície de canal e ao criar a mensagem.

Inclua um link específico para a mirror page em todas as suas mensagens de email. Saiba mais sobre a mirror page [nesta seção](mirror-page.md).

## Gerenciar rastreamento {#manage-tracking}

O [Designer de Email](create-email-content.md) permite gerenciar URLs rastreadas, como editar o tipo de rastreamento para cada link.

1. Clique no ícone **[!UICONTROL Links]** no painel esquerdo para exibir a lista de todas as URLs do seu conteúdo a serem rastreadas.

   Essa lista fornece uma visualização centralizada e ajuda a localizar cada URL no conteúdo do email.

1. Para editar um link, clique no ícone de lápis correspondente.

   ![Captura de tela mostrando a interface para editar links na ferramenta de rastreamento de mensagens](assets/message-tracking-edit-links.png){zoomable="yes"}

1. Modifique o **[!UICONTROL Tipo de rastreamento]** se necessário:

   ![Captura de tela mostrando a interface para editar tipos de rastreamento na ferramenta de rastreamento de mensagens](assets/message-tracking-edit-a-link.png){zoomable="yes"}

   Para cada URL rastreado, defina o modo de rastreamento para um destes valores:

   * **[!UICONTROL Rastreado]**: ativa o rastreamento para esta URL.
   * **[!UICONTROL Recusar]**: marca esta URL como uma URL de recusa ou de cancelamento de assinatura.
   * **[!UICONTROL Mirror page]**: marca esta URL como uma URL de mirror page.
   * **[!UICONTROL Nunca]**: impede o rastreamento desta URL. <!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

1. Adicione uma **[!UICONTROL Categoria]** ao seu link para agrupar links rastreados e clique em **[!UICONTROL Salvar]**.

   ![Captura de tela mostrando a interface para adicionar categorias a links rastreados na ferramenta de rastreamento de mensagens](assets/message-tracking-edit-a-link_2.png){zoomable="yes"}

1. Após enviar a entrega, acesse o relatório de entrega. Em **[!UICONTROL Rastreamento]**, o relatório **[!UICONTROL Fluxos de cliques e URL]** exibe quais são os URLs mais visitados de sua entrega. [Saiba mais](../reporting/gs-reports.md)