---
audience: end-user
title: Trabalhar com atividades de gestão de dados de fluxos de trabalho
description: Saiba como usar atividades de gestão de dados em workflows da Web do Adobe Campaign
badge: label="Alpha" type="Positive"
source-git-commit: ee418ea42bc4568f2ff1f0fe9080825764fee65d
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 2%

---

# Atividades de gerenciamento de dados {#data-management}

visão geral: o que são usados para o caso de uso que você pode executar com eles

listar atividades disponíveis + descrição curta + referência para a seção

## Enriquecimento {#enrichment}

descrição: adicione um ou vários dados de enriquecimento, o pode aproveitar para personalizar o caso de uso de deliveries: recupere a compra ou a última assinatura digital mais recente e o valor total de uma compra e personalize um email com ela

exemplo de uso do processo: recupere 4 compras mais recentes com menos de 100$ e personalize um email com ele
1. adicionar atividade
1. selecione o atributo a ser usado como dados de enriquecimento

   + opção exibir campos avançados
   + botão i

   observação: atributos do target dimension

1. Selecione como os dados são coletados
1. número de registros a serem recuperados se quiser recuperar uma coleção de vários registros
1. Aplicar filtros e criar regra

   + selecionar um filtro existente
   + salvar o filtro para reutilização
   + exibir resultados do filtro visualmente ou na visualização de código

1. classificar registros usando um atributo

utilizar dados de enriquecimento no campaign

onde podemos usar os dados de enriquecimento: personalizar email, outros casos de uso?
