---
audience: end-user
title: Criar uma entrega da central de atendimento
description: Saiba como criar uma entrega de call center com o Adobe Campaign Web
exl-id: fe8d4773-2271-46ec-9b2e-f50311a4ccf3
source-git-commit: 1581943b0f13cbd4296e1f42fae8560626b61bdf
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 4%

---

# Criar e enviar uma entrega da central de atendimento {#create-call-center}

Você pode criar uma entrega independente da central de atendimento ou criar uma no contexto de um fluxo de trabalho da campanha. As etapas abaixo detalham o procedimento para um delivery independente (único). Se você estiver trabalhando no contexto de um fluxo de trabalho de campanha, as etapas de criação serão detalhadas em [esta seção](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

Para criar e enviar um novo delivery independente da central de atendimento, siga estas etapas principais:

1. Crie a entrega, [leia mais](#create-delivery)
1. Defina a audiência, [leia mais](#select-audience)
1. Edite o conteúdo, [leia mais](#edit-content)
1. Pré-visualizar e enviar a entrega, [leia mais](#preview-send)

## Criar a entrega{#create-delivery}

Siga estas etapas para criar o delivery e configurar suas propriedades:

1. Selecione o menu **[!UICONTROL Deliveries]** e clique no botão **[!UICONTROL Criar delivery]**.

1. Escolha **[!UICONTROL Call center]** como canal e clique em **[!UICONTROL Criar entrega]** para confirmar.

   ![Captura de tela mostrando a criação de uma entrega da central de atendimento](assets/cc-create.png){zoomable="yes"}

   >[!NOTE]
   >
   >Para selecionar um modelo diferente, consulte esta [página](../msg/delivery-template.md).

1. Em **[!UICONTROL Propriedades]**, insira um **[!UICONTROL Rótulo]** para a entrega. Opções adicionais são detalhadas nesta [seção](../email/create-email.md#create-email).

   ![Captura de tela mostrando a configuração de propriedades para uma entrega da central de atendimento](assets/cc-properties.png){zoomable="yes"}

>[!NOTE]
>
>Você pode programar o delivery para ser enviado em uma data específica. Para obter mais informações, consulte esta [seção](../msg/gs-deliveries.md#gs-schedule).

## Definir o público-alvo{#select-audience}

Agora, é necessário definir o público-alvo que será direcionado para o arquivo de extração.

1. Na seção **[!UICONTROL Público-alvo]** da página de entrega, clique em **[!UICONTROL Selecionar público-alvo]**.

   ![Captura de tela mostrando a seleção de público para uma entrega da central de atendimento](assets/cc-audience.png){zoomable="yes"}

1. Escolha um público existente ou crie o seu próprio público.

   * [Saiba como selecionar um público existente](../audience/add-audience.md)
   * [Saiba como criar um novo público-alvo](../audience/one-time-audience.md)

   ![Captura de tela mostrando a seleção de público para uma entrega da central de atendimento](assets/cc-audience2.png){zoomable="yes"}

>[!NOTE]
>
>Os recipients da central de atendimento devem conter pelo menos seus nomes e número de telefone. Quaisquer recipients com informações incompletas serão excluídos dos deliveries da central de atendimento.
>
>Para saber como configurar grupos de controle, consulte esta [página](../audience/control-group.md).

## Editar o conteúdo{#edit-content}

Agora, vamos editar o conteúdo do arquivo de extração que será gerado pelo delivery da central de atendimento.

1. Na página de entrega, clique no botão **[!UICONTROL Editar conteúdo]**.

   ![Captura de tela mostrando a edição de conteúdo para uma entrega da central de atendimento](assets/cc-content0.png){zoomable="yes"}

1. Especifique o **[!UICONTROL Nome do arquivo]**. Para saber como personalizar o nome do arquivo, consulte esta [página](../personalization/personalize.md).

1. Selecione um **[!UICONTROL Formato de arquivo]**: **Texto**, **Texto usando colunas de largura fixa**, **CSV (Excel)** ou **XML**.

   ![Captura de tela mostrando a edição de conteúdo para uma entrega da central de atendimento](assets/cc-content.png){zoomable="yes"}

   >[!NOTE]
   >
   >As opções de formato de extração estão detalhadas nesta [página](../direct-mail/content-direct-mail.md#properties).

1. Ative a opção **[!UICONTROL Quantidade solicitada]** se não conseguir restringir o número de destinatários da sua entrega.

1. Na seção **[!UICONTROL Conteúdo]**, clique no botão **[!UICONTROL Adicionar Atributo]** para criar uma nova coluna a ser exibida no arquivo de extração.

1. Escolha o atributo a ser exibido na coluna e confirme. Para saber mais sobre como selecionar atributos e adicioná-los aos favoritos, consulte esta [página](../get-started/attributes.md).

   ![Captura de tela mostrando o botão Adicionar Atributo e as opções para adicionar atributos ao arquivo de extração.](assets/cc-add-attribute.png)

1. Repita essas etapas para adicionar quantas colunas forem necessárias para o arquivo de extração.

   Em seguida, você pode editar os atributos, classificar o arquivo de extração ou alterar a posição das colunas. Para obter mais informações, consulte esta [página](../direct-mail/content-direct-mail.md#content).

   ![Captura de tela mostrando as opções de configuração de atributos para o arquivo de extração.](assets/cc-content-attributes.png)

## Pré-visualizar e enviar o delivery{#preview-send}

Quando o conteúdo do delivery estiver pronto, você poderá pré-visualizá-lo usando perfis de teste e enviar provas. Em seguida, você pode enviar o delivery da central de atendimento para gerar o arquivo de extração.

As principais etapas para visualizar e enviar o arquivo de extração são as seguintes. Mais detalhes estão disponíveis em [esta página](../direct-mail/send-direct-mail.md).

1. Na página de conteúdo da entrega, clique no botão **[!UICONTROL Simular conteúdo]**.

   ![Captura de tela mostrando a opção de simulação de conteúdo na página de conteúdo da entrega](assets/cc-simulate0.png){zoomable="yes"}

1. Selecione um ou vários perfis de teste para visualizar o conteúdo personalizado. Você também pode enviar provas. [Leia mais](../direct-mail/send-direct-mail.md#preview-dm)

   ![Captura de tela mostrando a opção de simulação de conteúdo na página de conteúdo da entrega](assets/cc-simulate.png){zoomable="yes"}

1. Na página de entrega, clique em **[!UICONTROL Revisar e enviar]**.

   ![Captura de tela mostrando a opção de revisão e envio na página de entrega](assets/cc-review-send.png){zoomable="yes"}

1. Clique em **[!UICONTROL Preparar]**, monitore o progresso e as estatísticas fornecidas e, em seguida, confirme.

   ![Captura de tela mostrando a opção de preparação e o menu de logs](assets/cc-prepare.png){zoomable="yes"}

1. Clique em **[!UICONTROL Enviar]** para continuar com o processo de envio final e, em seguida, confirme.

Depois que a entrega é enviada, o arquivo de extração é gerado automaticamente e exportado para o local especificado na conta externa **[!UICONTROL Roteamento]** selecionada nas [configurações avançadas](../advanced-settings/delivery-settings.md) do modelo de entrega. Você também pode visualizar o arquivo clicando no botão **Visualizar arquivo**, na seção **Conteúdo** da tela.

Acompanhe seus KPIs (indicadores principais de desempenho) na página de entrega e os dados do menu **[!UICONTROL Logs]**.

Comece a medir o impacto da sua mensagem com relatórios integrados. [Saiba mais](../reporting/direct-mail.md)
