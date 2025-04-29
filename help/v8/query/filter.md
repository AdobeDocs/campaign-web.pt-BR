---
audience: end-user
title: Listas de filtros
description: Saiba como filtrar listas da Web do Adobe Campaign usando filtros incorporados e personalizados.
exl-id: 41c3c4c3-5991-4223-ad02-e2531d76fdda
source-git-commit: 485d8b4b715192cc5edb6442df0fa958e29d15ff
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# Listas de filtros {#filter-lists}

A Adobe Campaign Web fornece filtros em cada lista de objetos, permitindo filtrar informações com base em critérios contextuais específicos. Por exemplo, você pode filtrar deliveries com base no status, canal, data de contato ou pasta. Você também pode ocultar provas.

>[!IMPORTANT]
>
>Uma interface totalmente nova para o modelador de Consulta está disponível. O novo construtor de regras permite criar a consulta com mais facilidade graças à interface simplificada. Para alternar para essa experiência, pressione o botão de alternância no canto superior direito. Você pode voltar para o modelador de Query clássico a qualquer momento que desejar simplesmente pressionando o botão de alternância de volta para desativar a nova interface. Você pode aplicar os mesmos princípios que o modelador de consultas nessa nova interface.
>![Imagem mostrando a alternância para a nova interface do construtor de regras](assets/query-modeler-toggle.png){zoomable="yes"}

## Aplicar filtros {#apply}

Para aplicar filtros a uma lista, clique no botão **[!UICONTROL Mostrar filtros]** localizado no canto superior esquerdo da lista, ao lado da barra de pesquisa.

O painel Filtros é aberto, exibindo os filtros disponíveis para a lista selecionada. Por exemplo, você pode filtrar campanhas com base no status, datas de início e término ou pasta de armazenamento, enquanto a lista de serviços de assinatura pode ser filtrada com base no canal e na pasta de armazenamento.

![Painel de filtros mostrando os filtros disponíveis para listas](assets/filters-pane.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

Para filtrar uma lista com base em seus próprios critérios, crie um filtro personalizado. Para fazer isso, navegue até a parte inferior do painel de filtros e clique no botão **Adicionar regras**. [Saiba como criar filtros personalizados](#custom).

Depois de aplicados a uma lista, os filtros ficam visíveis abaixo da barra de pesquisa. Você pode remover um filtro individual a qualquer momento ou remover todos os filtros clicando no botão **Limpar tudo**.

## Criar filtros personalizados {#custom}

Filtros personalizados permitem refinar listas com base em seus próprios critérios específicos. Eles foram projetados usando o modelador de query do Campaign. Para criar um filtro personalizado, siga estas etapas:

1. Abra o painel de filtros e clique no botão **Adicionar regras** localizado na parte inferior do painel.

1. O modelador de consultas é aberto. Defina e combine os critérios de filtro para atender às suas necessidades. Informações detalhadas sobre como usar o modelador de consultas estão disponíveis em [esta seção](../query/query-modeler-overview.md).

   O exemplo abaixo mostra um filtro personalizado projetado para exibir na lista de campanhas campanhas SMS executadas por operadores dos departamentos Running ou Yoga.

   ![Exemplo de filtro personalizado mostrando campanhas de SMS filtradas por departamento](assets/filters-sample.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

1. Após configurar o filtro personalizado, clique em **[!UICONTROL Confirmar]** para aplicá-lo à lista.