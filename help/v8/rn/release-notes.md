---
title: Notas de versão da interface do Campaign Web v8
description: Conheça os novos recursos que acompanham a versão mais recente da interface do Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2: id: a075b2c1-7748-4328-b7f6-343aa314616aid: c309ee4e-82e4-4f7e-b608-ef345678c34eid: d5ef99fa-df0c-4153-bf94-105ad0724167
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: cbecd07b053d0ceb4e9114aa3c6d37752392febc
workflow-type: ht
source-wordcount: 243
ht-degree: 100%

---

# Notas de versão {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de versão"
>abstract="As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, as notas de versão do Campaign são atualizadas várias vezes por mês, com os recursos, melhorias e correções mais recentes. Recomendamos que você as verifique regularmente."

As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, essas notas de versão são atualizadas várias vezes por mês. Verifique-as regularmente.

## Versão de junho de 2026 {#26-6-release}

_16 de junho de 2026_

### Aprimoramentos {#26-6-improvements}

<!--
* Technical administrators can now create and configure brands directly from the Campaign Web User Interface, without using the Client Console. All brand settings, including identity, subdmain and protocols, email header parameters and URL tracking parameters, are now available in the Web UI. <!-- [Learn more](../administration/branding/branding-configure.md)
-->

* Agora é possível exportar dados de qualquer tela de listas, incluindo logs de rastreamento. Encontre sua lista e simplesmente clique no botão de exportação. A exportação inclui as linhas carregadas no momento e leva em conta as colunas exibidas na tela e em quaisquer pesquisas ou filtros ativos. [Saiba mais](../get-started/list-filters.md)

* As atividades de fluxo de trabalho **Desduplicação** e **Fim** agora oferecem suporte a várias transições de entrada. Quando
mais de uma transição de entrada está disponível, use a seção **Conjuntos para unir** nas propriedades da atividade
para selecionar quais transições conectar. Saiba mais nestas páginas: [Desduplicação](../workflows/activities/deduplication.md), [Fim](../workflows/activities/end.md)

* Parâmetros avançados agora estão expostos na seção **Dados de enriquecimento** das atividades de fluxo de trabalho **Criar público-alvo** (tipo de consulta) e **Enriquecimento**. Esses parâmetros permitem ajustar com precisão como os dados de enriquecimento são criados, incluindo agrupamento, desduplicação, tratamento da chave primária e dados do evento de entrada. [Saiba mais](../workflows/activities/enrichment.md)

<!--
* Delivery templates now allow you to define a time zone in the Schedule settings.
-->
