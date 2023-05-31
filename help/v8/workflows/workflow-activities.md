---
audience: end-user
title: Trabalhar com atividades de fluxos de trabalho
description: Saiba como executar atividades de workflow
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 92444d4ee324f64a35f4cca0b40907bdf453732c
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 98%

---


# Atividades de fluxos de trabalho {#workflow-activities}

## Atividades de direcionamento {#targeting}

Conteúdo a ser definido

<!--à reformuler-->Essas atividades permitem construir um ou mais públicos alvos definindo conjuntos e dividindo ou combinando esses conjuntos usando operações de intersecção, união ou exclusão.


## Atividades de controle de fluxo {#flow-control}

Conteúdo a ser definido

<!--à reformuler-->Essas atividades permitem construir um ou mais públicos alvos definindo conjuntos e dividindo ou combinando esses conjuntos usando operações de intersecção, união ou exclusão.

As atividades de controle de fluxo são usadas para coordenar as atividades do fluxo de trabalho.

## Atividades de gerenciamento de dados {#data-management}

visão geral: para que são usados
que caso de uso você pode executar com eles

listar atividades disponíveis + descrição curta + referência para a seção

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
