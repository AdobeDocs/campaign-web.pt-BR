---
audience: end-user
title: Usar uma atividade de workflow Delivery contínuo
description: Saiba como usar a atividade de workflow Delivery contínuo
exl-id: 659bddcb-280c-4623-8115-6f975515d1a2
TQID: https://experienceleague.adobe.com/uWGhvUmHdS0ixFI4d-uEPgpxSnZoOwNRMbn8aZfqA98
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 5a231f1dc49379d1be5d36e1732660111f851649
workflow-type: tm+mt
source-wordcount: 242
ht-degree: 24%

---

# Entrega contínua {#continuous-delivery}

A atividade de **Entrega contínua** permite adicionar novos destinatários a uma entrega existente. Esse tipo de entrega evita a necessidade de criar uma nova entrega a cada vez, tornando o processo mais eficiente para alertas ou notificações de baixo volume que são enviados conforme necessário.

Uma entrega contínua cria uma única instância de entrega. Todos os logs de entrega (broadLog) e logs de rastreamento fazem referência a esta única entrega, simplificando o monitoramento e os relatórios.

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
* [Entrega automatizada](automated-delivery.md)
* [Atividades de email, SMS, Push, Correspondência direta](channels.md)
* [Modelos de entrega](../../msg/delivery-template.md)
