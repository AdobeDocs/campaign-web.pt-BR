---
audience: end-user
title: Listas de filtros
description: Saiba como filtrar listas da Web do Adobe Campaign usando filtros incorporados e personalizados.
exl-id: 41c3c4c3-5991-4223-ad02-e2531d76fdda
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 5%

---

# Listas de filtros {#filter-lists}

A Adobe Campaign Web fornece filtros em cada lista de objetos, permitindo filtrar informações com base em critérios contextuais específicos. Por exemplo, você pode filtrar as entregas por seu status, canal, data de contato ou pasta. Você também pode ocultar provas.

## Aplicar filtros{#apply}

Para aplicar filtros a uma lista, clique no botão **[!UICONTROL Mostrar filtros]** localizado no canto superior esquerdo da lista, ao lado da barra de pesquisa.

O painel Filtros é aberto, exibindo os filtros disponíveis para a lista selecionada. Por exemplo, você pode filtrar campanhas em seu status, datas de início e término ou pasta de armazenamento, enquanto a lista de serviços de assinatura pode ser filtrada no canal e na pasta de armazenamento.

![](assets/filters-pane.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

Para filtrar uma lista com base em seus próprios critérios, crie um filtro personalizado. Para fazer isso, navegue até a parte inferior do painel de filtros e clique no botão **Adicionar regras**. [Saiba como criar filtros personalizados](#custom)

Depois de aplicados a uma lista, os filtros ficam visíveis abaixo da barra de pesquisa. Você pode remover um filtro individual a qualquer momento ou remover todos os filtros clicando no botão **Limpar tudo**.

## Criar filtros personalizados {#custom}

Filtros personalizados permitem refinar listas com base em seus próprios critérios específicos. Eles foram projetados usando o modelador de query do Campaign. Para criar um filtro personalizado, siga estas etapas:

1. Abra o painel de filtros e clique no botão **Adicionar regras** localizado na parte inferior do painel.

1. O modelador de consultas é aberto. Defina e combine os critérios de filtro para atender às suas necessidades. Informações detalhadas sobre como usar o modelador de consultas estão disponíveis em [esta seção](../query/query-modeler-overview.md).

   O exemplo abaixo mostra um filtro personalizado projetado para exibir na lista de campanhas campanhas SMS executadas por operadores dos departamentos Running ou Yoga.

   ![](assets/filters-sample.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

1. Após configurar o filtro personalizado, clique em **[!UICONTROL Confirmar]** para aplicá-lo à lista.
