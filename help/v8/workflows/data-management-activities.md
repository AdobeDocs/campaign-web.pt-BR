---
audience: end-user
title: Trabalhar com atividades de gestão de dados de fluxos de trabalho
description: Saiba como usar atividades de gestão de dados em workflows da Web do Adobe Campaign
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 0b5bfea60b65fd52f397f276e0c31e854adddb7b
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 1%

---

# Atividades de gerenciamento de dados {#data-management}

visão geral: o que são usados para o caso de uso que você pode executar com eles

listar atividades disponíveis + descrição curta + referência para a seção

## Enriquecimento {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Enriquecimento Atividade de "
>abstract="A atividade Enrichment permite aprimorar os dados direcionados com informações adicionais do banco de dados. Normalmente é usado em um workflow após atividades de direcionamento.<br/>Depois que os dados de enriquecimento tiverem sido adicionados ao workflow, eles poderão ser usados nas atividades adicionadas após a atividade de Enriquecimento para segmentar clientes em grupos distintos com base em seus comportamentos, preferências e necessidades, ou para criar mensagens e campanhas de marketing personalizadas que tenham mais probabilidade de ressoar com seu público-alvo."

A atividade Enrichment permite aprimorar os dados direcionados com informações adicionais do banco de dados. Normalmente é usado em um workflow após atividades de direcionamento.

Os dados de enriquecimento podem vir de:

* **Da mesma tabela de trabalho** como o direcionado para o seu fluxo de trabalho:

   *Direcione um grupo de clientes e adicione o campo &quot;Data de nascimento&quot; à tabela de trabalho atual*

* **De outra tabela de trabalho**:

   *Direcione um grupo de clientes e adicione os campos &quot;Quantia&quot; e &quot;Tipo de produto&quot; da tabela &quot;Compra&quot;*.

Depois que os dados de enriquecimento tiverem sido adicionados ao workflow, eles poderão ser usados nas atividades adicionadas após a atividade de Enriquecimento para segmentar clientes em grupos distintos com base em seus comportamentos, preferências e necessidades, ou para criar mensagens de marketing personalizadas e campanhas que têm mais probabilidade de repercutir no público-alvo.

Por exemplo, você pode adicionar à tabela de trabalho do workflow informações relacionadas às compras dos clientes e usar esses dados para personalizar emails com a compra mais recente ou a quantidade gasta nessas compras.

Para adicionar uma atividade Enrichment no workflow, siga estas etapas:

1. adicionar atividade
1. selecione o atributo a ser usado como dados de enriquecimento

   botão exibir campos avançados

   observação: atributos do target dimension

1. Selecione como os dados são coletados
1. número de registros a serem recuperados se quiser recuperar uma coleção de vários registros
1. Aplicar filtros e criar regra

   selecione um filtro existente salve o filtro para reutilizar os resultados da visualização do filtro visualmente ou na visualização de código

1. classificar registros usando um atributo

utilizar dados de enriquecimento no campaign

onde podemos usar os dados de enriquecimento: personalizar email, outros casos de uso?