---
audience: end-user
title: Introdução ao gerenciamento de ofertas
description: Saiba como gerenciar ofertas no Adobe Campaign Web
feature: Offers
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 58c94bacd8eaf86f9f90a4c641f42bd04a442fab
workflow-type: tm+mt
source-wordcount: 763
ht-degree: 3%

---

# Introdução ao gerenciamento de ofertas {#gs-offer-management}

Esse recurso permite adicionar ofertas personalizadas aos seus deliveries e apresentar as mais relevantes para cada perfil em um determinado contexto. As ofertas podem ser uma mensagem de comunicação simples ou promoções em um ou vários produtos. Com base nas regras de elegibilidade e nos pesos de prioridade, o mecanismo de oferta seleciona a melhor proposta a ser apresentada.

A interface da Web do Campaign permite gerenciar ofertas de ponta a ponta. Você pode criar e configurar ambientes de oferta, projetar espaços de oferta, criar seu catálogo de ofertas, definir regras de elegibilidade, editar conteúdo de oferta e publicar ofertas.

As ofertas são apresentadas aos recipients por meio de entregas com base em **regras de elegibilidade** e **pesos de prioridade**, para que a melhor oferta seja selecionada para cada perfil em um determinado contexto.

>[!NOTE]
>
>A interface da Web do Campaign se concentra no uso mais comum do gerenciamento de ofertas. As configurações avançadas permanecem disponíveis no Console do cliente do Campaign. Consulte a [documentação do Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=pt-BR){target="_blank"}

<!--
and check the [Campaign Web and client console capability matrix](../get-started/capability-matrix.md#offer-capabilities) for the current scope.
-->

## Principais conceitos {#concepts}

Antes de começar a trabalhar com ofertas, familiarize-se com os principais objetos envolvidos.

* **Ambiente de oferta** — Contêiner que contém um catálogo de oferta e os espaços de oferta relacionados. Há dois tipos, o ambiente **Design**, em que você cria e configura ofertas, e o ambiente **[!UICONTROL Live]** somente leitura, que contém os objetos aprovados e implantados disponíveis para entrega. [Saiba mais](offer-environment.md)

* **Espaço de ofertas** — Define onde e como uma oferta é exposta (email, correspondência direta, SMS, Web de entrada etc.). O espaço lista os campos de conteúdo que podem ser usados na oferta, a função de renderização que cria a representação da oferta e as configurações de armazenamento que direcionam o status da proposta. [Saiba mais](offer-space.md)

* **Catálogo de ofertas e categorias** — as ofertas são organizadas em um catálogo hierárquico de **categorias** e subcategorias. Cada categoria pode compartilhar regras de qualificação, datas de validade e **temas de aplicativo**. Uma categoria padrão é fornecida no ambiente de design para que todas as ofertas sejam recebidas.

<!--
To configure categories in depth — including sub-categories, fallback categories, and theme management — refer to the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-catalog/interaction-offer-catalog.html){target="_blank"}.
-->

* **Oferta** — Uma oferta individual com seu próprio período de qualificação, filtro de direcionamento, peso e conteúdo. As ofertas são aprovadas e implantadas antes de serem apresentadas aos recipients. [Saiba mais](create-offer.md)

* **Apresentação de oferta** — Resultado da apresentação de uma oferta a um contato em um determinado espaço (um banner em um site, um email, um SMS etc.). O número de apresentações por entrega é configurado ao [configurar ofertas em uma entrega](../msg/offers.md).

* **Arbitragem** — Princípio pelo qual o mecanismo de oferta classifica as ofertas qualificadas por prioridade para selecionar quais apresentar. A arbitragem usa os critérios definidos nas categorias, nas ofertas e nas ofertas de contexto.

## Fluxo de gerenciamento de ofertas {#workflow}

O fluxo completo típico na interface do usuário da Web do Campaign é o seguinte:

1. **Revise as configurações do ambiente de oferta** — Verifique o design/mapeamento em tempo real, a qualificação e as configurações de gerenciamento de peso. [Saiba mais](offer-environment.md)

1. **Criar um espaço de ofertas** — Defina os campos de conteúdo, a função de renderização e os parâmetros avançados correspondentes ao seu canal. [Saiba mais](offer-space.md)

1. **Criar ofertas no catálogo** — Defina o período de qualificação, o filtro de direcionamento, o peso e o conteúdo para cada oferta. [Saiba mais](create-offer.md)

1. **Aprovar e implantar** — Envie a oferta para aprovação, aprove seu conteúdo e qualificação e permita que o processo de implantação a publique no ambiente ativo. [Saiba mais](create-offer.md#approve-deploy)

1. **Adicionar a oferta a uma entrega** — Faça referência ao espaço de ofertas e às propostas na entrega por email, SMS, push ou correspondência direta. [Saiba mais](../msg/offers.md)

## Acessar ofertas na interface da Web {#access}

Ofertas estão disponíveis no menu esquerdo **[!UICONTROL Ofertas]**. Lá, você pode navegar no catálogo, abrir uma oferta para edição e monitorar seu status de aprovação e implantação.

![Captura de tela mostrando o menu Oferta.](assets/offers-gs.png){zoomable="yes"}

Os ambientes de oferta e espaços de oferta são acessados por meio do **[!UICONTROL Explorer]**, navegando até a pasta correspondente.


## Complementos exclusivos de console {#console-complements}

Alguns recursos de ofertas ainda não estão expostos na interface da Web e ainda devem ser configurados no console do cliente:

* **Simulação de oferta** — O módulo **Simulação** que permite testar a distribuição de ofertas antes do envio. Consulte [Simulação de oferta](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer.html?lang=pt-BR#offer-simulation){target="_blank"}.

* Gerenciamento de **Filtros predefinidos** — Regras de filtros reutilizáveis que podem ser referenciadas a partir de qualquer oferta. Consulte [Gerenciar filtros predefinidos](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-predefined-filters.html){target="_blank"}.

* **Rastreamento de oferta** — Configuração do rastreamento para apresentações de oferta para alimentar o histórico de apresentações. Consulte [Rastrear apresentações de oferta](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-tracking.html?lang=pt-BR){target="_blank"}.

* **Funções do operador** — atribuição de direitos de Gerente de ofertas/Gerente de entregas. Consulte [Operadores do módulo de Interação](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-operators.html){target="_blank"}.

* **Práticas recomendadas de interação e regras de arbitragem**. Consulte [Práticas recomendadas de interação de campanha](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html?lang=pt-BR){target="_blank"}.

* **Relatórios** — Os relatórios de oferta e proposta dedicados ainda não estão disponíveis na interface do usuário da Web.