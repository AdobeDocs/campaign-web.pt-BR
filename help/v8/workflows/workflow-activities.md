---
audience: end-user
title: Trabalhar com atividades de fluxos de trabalho
description: Saiba como executar atividades de workflow
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: ec569f7d5acc06a027416794c056328d5fce1567
workflow-type: tm+mt
source-wordcount: '853'
ht-degree: 60%

---


# Atividades de fluxos de trabalho {#workflow-activities}

## Atividades de direcionamento {#targeting}

Essas atividades permitem construir um ou mais públicos alvos definindo conjuntos e dividindo ou combinando esses conjuntos usando operações de intersecção, união ou exclusão.

### Criar público-alvo {#build-audience}

Esta atividade permite definir um público-alvo. Você pode selecionar um público existente do Campaign ou usar o construtor de regras para definir sua própria consulta.

A variável **Criar público-alvo** A atividade pode ser colocada no início do workflow ou após qualquer outra atividade. Qualquer atividade pode ser colocada após a variável **Criar público-alvo**.

Para criar sua própria consulta:

1. Selecionar **Crie o seu próprio (consulta)**.
1. Escolha o **Dimensão de direcionamento**. O targeting dimension permite definir o público alvo da operação: recipients, beneficiários de contrato, operadores, assinantes etc. Por padrão, o target é selecionado dos recipients. Consulte a [Documentação do v8](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#targeting-and-filtering-dimensions){target="_blank"}.
1. Clique em **Continue**.
1. Use o construtor de regras para definir seu query, da mesma forma que você cria um público-alvo ao criar um novo email. Consulte esta [seção](../audience/segment-builder.md).

Para selecionar um público existente,

1. Selecionar **Ler público**.
1. Clique em **Continue**.
1. Selecione seu público, da mesma forma que você usa um público ao criar um novo email. Consulte esta [seção](../audience/add-audience.md).

### Combinar {#combine}

A variável **Combinar** A atividade pode ser colocada após qualquer outra atividade, mas não no início do workflow. Qualquer atividade pode ser colocada após a variável **Combinar**.

### Enriquecimento {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Enriquecimento atividade"
>abstract="A atividade Enriquecimento permite aprimorar os dados direcionados com informações adicionais do banco de dados. Normalmente é usado em um fluxo de trabalho após atividades de direcionamento.<br/>Depois que os dados de enriquecimento tiverem sido adicionados ao fluxo de trabalho, eles poderão ser usados nas atividades adicionadas após a atividade de Enriquecimento para segmentar clientes em grupos distintos com base em seus comportamentos, preferências e necessidades, ou para criar mensagens e campanhas de marketing personalizadas que tenham mais probabilidade de ressoar com seu público-alvo."

A atividade Enriquecimento permite aprimorar os dados direcionados com informações adicionais do banco de dados. Normalmente é usado em um fluxo de trabalho após atividades de direcionamento.

Os dados de Enriquecimento podem vir de:

* **Da mesma tabela de trabalho** como o direcionado para o seu fluxo de trabalho:

   *Direcione um grupo de clientes e adicione o campo &quot;Data de nascimento&quot; à tabela de trabalho atual*

* **De outra tabela de trabalho**:

   *Direcione um grupo de clientes e adicione os campos &quot;Quantidade&quot; e &quot;Tipo de produto&quot; da tabela &quot;Compra&quot;*.

Depois que os dados de enriquecimento tiverem sido adicionados ao fluxo de trabalho, eles poderão ser usados nas atividades adicionadas após a atividade de Enriquecimento para segmentar clientes em grupos distintos com base em seus comportamentos, preferências e necessidades, ou para criar mensagens de marketing personalizadas e campanhas que tenham mais probabilidade de repercutir junto ao público-alvo.

Por exemplo, você pode adicionar à tabela de trabalho do fluxo de trabalho as informações relacionadas às compras dos clientes e usar esses dados para personalizar emails com a compra mais recente ou a quantidade gasta nessas compras.

Para adicionar uma atividade de Enriquecimento no fluxo de trabalho, siga estas etapas:

1. adicionar atividade
1. selecione o atributo a ser usado como dados de enriquecimento

   botão de opção
exibir campos avançados

   observação: atributos da dimensão do público-alvo

1. Selecione como os dados são coletados
1. número de registros a serem recuperados se quiser recuperar uma coleção de vários registros
1. Aplicar filtros e criar regra

   selecione um filtro existente
salve o filtro para reutilizar
exiba os resultados do filtro visualmente ou na visualização de código

1. classificar registros usando um atributo

usar os dados de enriquecimento na campanha

onde podemos usar os dados de enriquecimento: personalizar email, outros casos de uso?


## Atividades de canal {#channel}

A Adobe Campaign Web permite automatizar e executar campanhas de marketing em vários canais, como email, SMS ou push. Com workflows do Adobe Campaign, você pode combinar atividades de canal na tela para criar workflows entre canais que podem acionar ações com base no comportamento do cliente.

Por exemplo, você pode criar uma campanha de email de boas-vindas que inclui uma série de mensagens em diferentes canais, como email, SMS e push. Você também pode enviar um email de acompanhamento depois que um cliente concluir uma compra ou enviar uma mensagem de aniversário personalizada para um cliente por SMS.

Usando atividades de canal, você pode criar campanhas abrangentes e personalizadas que envolvem clientes em vários pontos de contato e geram conversões.

As atividades de canal estão disponíveis na paleta, no lado esquerdo da tela, na seção Canais.

### Email {#email}

descrição, que caso de uso você pode executar (comum a outras atividades que você pode vincular antes ou depois da atividade)

como adicionar e configurar a atividade

exemplo de uma atividade configurada em um fluxo de trabalho


A atividade Email delivery permite configurar o envio de um email em um workflow.

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

Os destinatários de email são definidos no sentido upstream da atividade, no mesmo fluxo de trabalho, por meio de uma atividade de direcionamento de Público-alvo.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->


### SMS {#sms}

### Notificação por push (Android) {#push-android}

### Notificação por push (iOS) {#push-ios}

## Atividades de controle de fluxo {#flow-control}

Conteúdo a ser definido

<!--à reformuler-->Essas atividades permitem construir um ou mais públicos alvos definindo conjuntos e dividindo ou combinando esses conjuntos usando operações de intersecção, união ou exclusão.

As atividades de controle de fluxo são usadas para coordenar as atividades do fluxo de trabalho.

### Bifurcação {#fork}

### AND-join {#join}


### Aguardar {#wait}

### End {#end}

## Atividades de gerenciamento de dados {#data-management}

visão geral: para que são usados
que caso de uso você pode executar com eles

listar atividades disponíveis + descrição curta + referência para a seção

