---
audience: end-user
title: Usar uma atividade de workflow Delivery contínuo
description: Saiba como usar a atividade de workflow Delivery contínuo
source-git-commit: f238fde4a79d3303f2b5c9a2d26b11ffad8ac54e
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 3%

---

# Entrega contínua {#continuous-delivery}

A atividade de **Entrega contínua** permite adicionar novos destinatários a uma entrega existente. Esse tipo de delivery evita a necessidade de criar um novo delivery a cada vez, tornando-o mais eficiente para alertas de baixo volume ou notificações enviadas conforme necessário.

Uma entrega contínua cria uma única instância de entrega. Todos os logs do delivery (broadLog) e logs de rastreamento fazem referência a esse delivery, simplificando o monitoramento e os relatórios.

## Configurar a atividade de entrega contínua {#configure}

1. Adicione uma atividade **Entrega contínua** à tela do fluxo de trabalho.

   ![Captura de tela mostrando a atividade de entrega contínua](../assets/continuous-delivery.png){zoomable="yes"}

1. Insira um **[!UICONTROL Rótulo]** personalizado para a atividade (opcional). Por padrão, é rotulado como &quot;Delivery contínuo&quot;.

1. Ao lado do campo **[!UICONTROL Modelo]**, clique no ícone de pesquisa para selecionar um modelo de entrega. Somente templates (não deliveries padrão) estão disponíveis para seleção. O template define o canal, o conteúdo e a configuração do delivery.

1. Nas **[!UICONTROL Opções de direcionamento]**, escolha como a população do público alvo será definida:

   * **[!UICONTROL Especificado pelos eventos de entrada]**: o destino vem da transição de entrada (de atividades upstream, como Compilar público ou Consulta incremental). Essa é a opção mais comum.

   * **[!UICONTROL Especificado no modelo de entrega]**: o destino é definido no próprio modelo.

   * **[!UICONTROL Arquivo especificado no evento de entrada]**: o destino é fornecido por meio de um arquivo passado pelo fluxo de trabalho.

A atividade de delivery contínuo gera automaticamente uma transição de saída para continuar seu workflow.

## Tópicos relacionados {#related}

* [Sobre atividades de fluxo de trabalho](about-activities.md)
* [Atividades de email, SMS, Push, Correspondência direta](channels.md)
* [Modelos de entrega](../../msg/delivery-template.md)
