---
product: campaign
title: Trabalho com entregas
description: Saiba como criar sua primeira entrega no Campaign Web
feature: Email, Push, SMS, Cross Channel Orchestration
role: User
level: Beginner
badge: label="Disponibilidade limitada"
exl-id: 3afff35c-c15f-46f8-b791-9bad5e38ea44
source-git-commit: 74048d2e6001d2d9b4813a78096a481374233ea6
workflow-type: tm+mt
source-wordcount: '1203'
ht-degree: 100%

---

# Trabalho com entregas {#work-with-deliveries}

>[!CONTEXTUALHELP]
>id="acw_deliveries_list"
>title="Entregas"
>abstract="Uma entrega é uma comunicação enviada para um público-alvo em um canal específico: email, SMS ou notificação por push. Nesta tela, você pode editar, duplicar e excluir as entregas existentes. Também é possível exibir relatórios de entregas concluídas. Clique no botão **Criar entrega** para adicionar uma nova entrega."

## Criação de uma entrega {#create-delivery}

Você pode criar entregas independentes a partir do menu **[!UICONTROL Entregas]** à esquerda ou criar entregas no contexto de um fluxo de trabalho, incluído ou não em uma campanha.

Navegue pelas guias abaixo para saber como criar uma entrega:

>[!BEGINTABS]

>[!TAB Criação de uma entrega independente]

Para criar uma entrega independente, siga estas etapas:

1. Navegue até o menu **[!UICONTROL Entregas]** no painel de navegação esquerdo e clique no botão **[!UICONTROL Criar entrega]**.

   ![](assets/create-a-delivery.png)

1. Escolha um canal para a entrega. 
1. Defina o público da entrega, para o público-alvo principal e o grupo de controle. Saiba mais sobre públicos-alvo [nesta seção](../audience/about-recipients.md).

   ![](assets/select-audience.png){width="70%" align="left"}

1. Defina o conteúdo da mensagem. Saiba mais sobre canais de entrega e como definir um conteúdo de entrega nestas seções:

   * [Canal de email](../email/create-email.md)
   * [Canal de notificação por push](../push/gs-push.md)
   * [Canal de SMS](../sms/create-sms.md)

1. (opcional) Defina a [programação](#gs-schedule) da entrega. Se nenhuma programação for definida, as mensagens serão enviadas imediatamente após clicar no botão **[!UICONTROL Enviar]**.
1. Clique no botão  **[!UICONTROL Revisar e enviar]** para verificar suas configurações.
1. Use o botão **[!UICONTROL Simular conteúdo]** para testar a entrega e as configurações de personalização. Saiba mais simulação de mensagens [nesta seção](../preview-test/preview-test.md).
1. Clique no botão **[!UICONTROL Preparar]** para calcular o público-alvo e gerar as mensagens. A etapa de preparação pode levar alguns minutos. Quando a preparação estiver concluída, as mensagens estarão prontas para envio. Em caso de erro, navegue até os **Logs** para verificar os alertas e avisos.
1. Verifique os resultados e clique no botão **[!UICONTROL Enviar]** para iniciar o envio das mensagens.
1. Depois que as mensagens forem enviadas, navegue até a seção **Relatórios** para acessar as métricas principais. Saiba mais sobre relatórios de entrega [nesta seção](../reporting/delivery-reports.md).

>[!TAB Criação de uma entrega em um fluxo de trabalho]

Para criar uma entrega em um fluxo de trabalho, siga estas etapas:

1. Crie um fluxo de trabalho ou abra um já existente. Saiba mais sobre fluxos de trabalho [nesta página](../workflows/gs-workflow-creation.md#gs-workflow-steps)
1. Adicione e configure uma atividade **[!UICONTROL Criar público-alvo]**. Saiba mais sobre a atividade **[!UICONTROL Construir público-alvo]**[nesta seção](../workflows/activities/build-audience.md).
1. Clique no ícone `+` e selecione uma atividade de entrega: **[!UICONTROL Email]**, **[!UICONTROL SMS]**, **[!UICONTROL Notificação por push (Android)]** ou **[!UICONTROL Notificação por push (iOS)]**. Saiba mais sobre as atividades do canal de entrega em um workflow e como definir um conteúdo de entrega nesta [seção](../workflows/activities/channels.md).

   ![](assets/add-delivery-in-wf.png)

1. Inicie o workflow e verifique os logs.

Também é possível adicionar entregas em uma campanha sem criar um workflow. Para fazer isso, navegue até a guia **[!UICONTROL Entregas]** da campanha e clique no botão **[!UICONTROL Criar entrega]**.

![](assets/new-campaign-delivery.png)

As etapas de configuração são semelhantes às das entregas independentes.

Para obter mais informações sobre como configurar uma campanha e gerenciar entregas que pertencem a uma campanha, consulte [esta seção](../campaigns/gs-campaigns.md).

>[!ENDTABS]


## Adicionar personalização {#personalization}

As mensagens entregues pelo Adobe Campaign podem ser personalizadas de várias maneiras. [Saiba mais sobre os recursos de personalização](../personalization/gs-personalization.md).

Use o Campaign para criar conteúdo dinâmico e enviar mensagens personalizadas. Os recursos de personalização podem ser combinados para melhorar suas mensagens e criar uma experiência do usuário personalizada.

Você pode personalizar o conteúdo da mensagem ao:

* Inserir **campos de personalização** dinâmicos

  Os campos de personalização são usados na personalização de primeiro nível das mensagens. Você pode selecionar qualquer campo disponível no banco de dados no editor de personalização. Para uma entrega, é possível selecionar qualquer campo relacionado ao recipient, à mensagem ou à entrega. Esses atributos de personalização podem ser inseridos na linha de assunto ou no corpo das mensagens. [Saiba mais](../personalization/personalize.md)

* Inserção de **blocos de conteúdo** predefinidos

  O Campaign vem com um conjunto de blocos de personalização contendo uma renderização específica que você pode inserir nas entregas. Por exemplo, você pode adicionar um logotipo, uma mensagem de saudação ou um link para a mirror page da mensagem. Os blocos de conteúdo estão disponíveis em uma entrada dedicada no editor de personalização. [Saiba mais](../personalization/personalize.md#ootb-content-blocks)

* Criação de **conteúdo condicional**

  Configure o conteúdo condicional para adicionar personalização dinâmica com base no perfil do destinatário, por exemplo. Blocos de texto e/ou imagens são inseridos quando uma determinada condição for satisfeita. [Saiba mais](../personalization/conditions.md)

* Adição de **ofertas personalizadas**

  Insira ofertas personalizadas no conteúdo da mensagem, dependendo do local do destinatário, do clima atual ou da última compra. [Saiba mais](../msg/offers.md)

## Visualização e teste de suas entregas

Depois que o conteúdo da mensagem for definido, você poderá visualizá-lo para controlar a renderização das mensagens e verificar as configurações de personalização com perfis de teste. [Saiba mais](../preview-test/preview-test.md)

## Agendar o envio da entrega {#gs-schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="Definir uma data e hora de contato"
>abstract="Defina a data e a hora exata do envio da sua entrega. Ao escolher o horário mais apropriado para sua mensagem de marketing, você pode maximizar as taxas de abertura."

Você pode definir a data e a hora exata para enviar suas mensagens. Ao escolher o horário mais apropriado para sua mensagem de marketing, você pode maximizar as taxas de abertura.

Para agendar o envio de uma entrega, abra a entrega e navegue até a seção **[!UICONTROL Agendar]**. Use o botão de alternância **[!UICONTROL Habilitar agendamento]** para ativá-lo e defina a data e a hora desejada para o envio. Após enviar a entrega, o envio só será realizado na data de contato definida.

![](assets/schedule.png)

Por padrão, a opção **[!UICONTROL Ativar confirmação antes de enviar]** está habilitada. Essa opção exige que você confirme o envio antes que a entrega seja enviada na data e hora programadas. Se precisar enviar a entrega automaticamente na data e hora programadas, desabilite essa opção.

Saiba mais sobre as etapas para enviar uma entrega programada [nesta seção](../monitor/prepare-send.md#schedule-the-send).

## Logs de rastreamento e monitoramento {#gs-tracking-logs}

O monitoramento de entregas após o envio é uma etapa essencial para garantir que as campanhas de marketing sejam eficientes e atinjam os clientes.

Você pode monitorar após enviar uma entrega, bem como entender como as falhas de entrega e as quarentenas são gerenciadas.

Saiba mais sobre os recursos de rastreamento e monitoramento [nesta seção](../reporting/gs-reports.md).

## Duplicação de uma entrega {#delivery-duplicate}

É possível criar uma cópia de uma entrega existente, ou na lista de entregas ou no painel de entregas.

Para duplicar uma entrega da lista de entregas, siga estas etapas:

1. Clique no botão de três pontos à direita, ao lado do nome da entrega a ser duplicada.
1. Selecione  **[!UICONTROL Duplicar]**.
1. Confirme a duplicação: o novo painel de entrega será aberto na tela central.

Para duplicar uma entrega do painel, siga estas etapas:

1. Abra a entrega e clique no botão **[!UICONTROL ...Mais]** na seção superior da tela.
1. Selecione **[!UICONTROL Duplicar]**.
1. Confirme a duplicação: a nova entrega substituirá a entrega atual na tela central.

## Excluir uma entrega {#delivery-delete}

As entregas são excluídas na lista de entregas - seja da entrada da entrega principal no painel esquerdo ou da lista de entregas de uma campanha.

Para excluir uma entrega da lista de entregas, siga estas etapas:

1. Clique no botão de três pontos à direita, ao lado do nome da entrega a ser duplicada.
1. Selecione **[!UICONTROL Excluir]**.
1. Confirmar exclusão.

![Excluir uma entrega da lista de entregas](assets/delete-delivery-from-list.png)

Todas as entregas estão disponíveis nessas listas, mas as entregas criadas em um workflow não podem ser excluídas nelas. Para excluir uma entrega criada no contexto de um workflow, será necessário excluir a atividade de entrega do workflow.

Para excluir uma entrega de um workflow, siga estas etapas:

1. Selecionar a atividade de entrega.
1. Clique no ícone de **[!UICONTROL Excluir]** no painel direito.
1. Confirmar exclusão. Se a entrega tiver nós derivados, você poderá optar por excluí-los também ou mantê-los.

![Excluir uma entrega em um workflow](assets/delete-delivery-from-wf.png)
