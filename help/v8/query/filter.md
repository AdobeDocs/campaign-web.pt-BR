---
audience: end-user
title: Listas de filtros
description: Saiba como filtrar listas da Web do Adobe Campaign usando filtros incorporados e personalizados.
badge: label="Disponibilidade limitada"
source-git-commit: 7f4d8a2c2b0592515c25628f35234311dc61b4fd
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 6%

---


# Listas de filtros {#filter-lists}

A Adobe Campaign Web fornece filtros em cada lista de objetos, permitindo filtrar informações com base em critérios contextuais específicos. Por exemplo, você pode filtrar as entregas por seu status, canal, data de contato ou pasta. Também é possível ocultar testes.

## Aplicar filtros{#apply}

Para aplicar filtros a uma lista, clique no link **[!UICONTROL Mostrar filtros]** botão localizado no canto superior esquerdo da lista, ao lado da barra de pesquisa.

O painel Filtros é aberto, exibindo os filtros disponíveis para a lista selecionada. Por exemplo, você pode filtrar campanhas em seu status, datas de início e término ou pasta de armazenamento, enquanto a lista de serviços de assinatura pode ser filtrada no canal e na pasta de armazenamento.

![](assets/filters-pane.png){width="70%" align="left" zoomable="yes"}

Para filtrar uma lista com base em seus próprios critérios, crie um filtro personalizado. Para fazer isso, navegue até a parte inferior do painel de filtros e clique no **Adicionar regras** botão. [Saiba como criar filtros personalizados](#custom)

Depois de aplicados a uma lista, os filtros ficam visíveis abaixo da barra de pesquisa. Você pode remover um filtro individual a qualquer momento ou remover todos os filtros clicando no **Limpar tudo** botão.

## Criar filtros personalizados {#custom}

Filtros personalizados permitem refinar listas com base em seus próprios critérios específicos. Eles foram projetados usando o modelador de query do Campaign. Para criar um filtro personalizado, siga estas etapas:

1. Abra o painel Filtros e clique na guia **Adicionar regras** localizado na parte inferior do painel.
1. O modelador de consultas é aberto. Defina e combine os critérios de filtro para atender às suas necessidades. Informações detalhadas sobre como usar o modelador de consulta estão disponíveis em [nesta seção](../query/query-modeler-overview.md).

   O exemplo abaixo mostra um filtro personalizado projetado para exibir na lista de campanhas campanhas SMS executadas por operadores dos departamentos Running ou Yoga.

   ![](assets/filters-sample.png){width="70%" align="left" zoomable="yes"}

1. Após configurar o filtro personalizado, clique em **[!UICONTROL Confirmar o]** para aplicá-lo à lista.
