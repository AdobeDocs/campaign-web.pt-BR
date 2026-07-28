---
audience: end-user
title: Criar e publicar uma oferta
description: Saiba como criar, configurar, aprovar e implantar uma oferta no Campaign Web
feature: Offers
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 7bd09b83112efb99c90884b7da21a5e9a5c76b6c
workflow-type: tm+mt
source-wordcount: 1057
ht-degree: 2%

---

# Criar e publicar uma oferta {#create-offer}

Uma **oferta** é uma proposta individual com seu próprio período de qualificação, filtro de direcionamento, peso e conteúdo. As ofertas são organizadas no catálogo de ofertas por meio de **categorias** e são apresentadas aos recipients por meio de um **espaço de ofertas**.

Antes de criar uma oferta, verifique se o ambiente de oferta está configurado e se pelo menos um espaço de oferta está publicado. Saiba mais em [Configurar um ambiente de oferta](offer-environment.md) e [Criar e gerenciar espaços de oferta](offer-space.md).

## Acessar o catálogo de ofertas {#access}

Para procurar e criar ofertas, selecione **[!UICONTROL Ofertas]** no painel de navegação esquerdo. A lista exibe as ofertas existentes. Use o campo de pesquisa, o seletor de pastas ou o [modelador de consultas](../query/query-modeler-overview.md) para filtrar a lista.

![Captura de tela mostrando o catálogo de ofertas.](assets/offers-offer.png){zoomable="yes"}

Clique no nome de uma oferta para abri-la para edição ou use os três pontos ao lado dela para **[!UICONTROL Duplicar]** ou **[!UICONTROL Excluir]**.

## Criar uma oferta {#create}

Para criar uma nova oferta:

1. Na lista de ofertas, clique em **[!UICONTROL Criar oferta]**.

1. Selecione o **[!UICONTROL Modelo]** a partir do qual criar a oferta (por exemplo, uma oferta em branco ou um modelo de oferta anônimo).

   ![Captura de tela mostrando a criação da oferta.](assets/offers-offer-1.png){zoomable="yes"}

1. Insira um **[!UICONTROL Rótulo]** e, opcionalmente, atribua a oferta a um operador usando **[!UICONTROL Atribuído a]** e/ou insira um **[!UICONTROL Código da oferta]**.

1. Expanda **[!UICONTROL Opções adicionais]** para editar o **[!UICONTROL Nome interno]** gerado automaticamente, selecione a **[!UICONTROL Categoria]** em que a oferta está armazenada ou adicione uma descrição. Esta etapa é opcional.

1. Expanda **[!UICONTROL Aprovações]** para atribuir aprovadores aos grupos **[!UICONTROL Aprovação de qualificação]** e **[!UICONTROL Aprovação de conteúdo]**. Esta etapa é opcional.

1. Expanda as **[!UICONTROL Opções personalizadas]** para preencher quaisquer campos adicionais que sua organização tenha adicionado ao esquema de oferta. Os campos mostrados nesta seção variam de uma instância do Campaign para outra. Esta etapa é opcional.

1. Clique em **[!UICONTROL Create]**. A tela de configurações cheia é exibida.

   ![Captura de tela mostrando a tela de configurações da oferta.](assets/offers-offer-2.png){zoomable="yes"}

### Definir a qualificação {#eligibility}

Esta seção permite controlar quando e para quem a oferta pode ser apresentada. As seguintes opções estão disponíveis:

* **[!UICONTROL Agendar]** — Defina as datas de início e término entre as quais a oferta pode ser apresentada.

  >[!NOTE]
  >
  >As interseções do período de qualificação com a categoria principal são consideradas: mesmo que o agendamento da própria oferta seja mais amplo, a oferta só será apresentada, enquanto a categoria principal também será elegível.

* **[!UICONTROL Filtros no destino]** — Clique em **[!UICONTROL Criar filtro]** para abrir o construtor de regras e restringir a oferta a um público específico. Deixe o filtro em branco para tornar a oferta elegível para todo o público-alvo do ambiente. Para reutilizar um **filtro predefinido** declarado no nível da plataforma, consulte a [documentação do Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-predefined-filters.html){target="_blank"}. Filtros predefinidos são criados no console do cliente.

* **[!UICONTROL Gerenciamento do peso da oferta]** — Clique em **[!UICONTROL Exibir peso da oferta]** e em **[!UICONTROL Adicionar peso]** para influenciar a prioridade da oferta quando várias ofertas estiverem qualificadas ao mesmo tempo. Cada peso tem uma data de início, uma data de término e um filtro opcional.

>[!NOTE]
>
>O mecanismo de Oferta classifica as ofertas elegíveis diminuindo o peso e retorna as propostas com maior peso primeiro. A lógica de seleção — chamada de **arbitragem** — também leva em conta as regras de qualificação e os pesos configurados na categoria principal e no ambiente. Saiba mais sobre o princípio de arbitragem na [documentação do Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html){target="_blank"}.

### Definição do conteúdo {#content}

Na oferta, selecione a guia **[!UICONTROL Conteúdo]**. Essa guia define os valores que serão expostos pela função de renderização.

1. Preencha os atributos prontos para uso — **[!UICONTROL Título]**, **[!UICONTROL URL de destino]**, **[!UICONTROL URL da imagem]** e qualquer atributo personalizado declarado no esquema de oferta.

1. Use o [editor de expressão](../query/expression-editor.md) para personalizar os valores com dados de perfil, atributos de oferta ou campos de proposta.

1. Para as cargas de texto e HTML, clique em **[!UICONTROL Editar conteúdo]** para abrir o editor de conteúdo. Você pode criar o conteúdo do zero, codificar seu próprio HTML ou importar HTML existente, opcionalmente, a partir de um modelo de amostra.

>[!IMPORTANT]
>
>Os atributos disponíveis na seção **[!UICONTROL Conteúdo]** dependem do esquema [!DNL nms:offer]. Para expor atributos personalizados, estenda o esquema e selecione-os na seção **[!UICONTROL Conteúdo da oferta]**. Saiba mais em [Trabalhar com esquemas](../administration/schemas.md).

## Pré-visualizar a oferta {#preview}

Você pode visualizar a oferta antes de enviá-la.

1. Na oferta, selecione a guia **[!UICONTROL Visualização]**, ao lado de **[!UICONTROL Visão geral]**.

   ![Captura de tela mostrando a visualização da oferta.](assets/offers-offer-3.png){zoomable="yes"}

1. Selecione um perfil de público alvo e, se relevante, o espaço de ofertas no qual a visualização deve ser executada.

   A função de renderização definida no espaço de ofertas é aplicada ao conteúdo da oferta e a representação resultante é exibida.

>[!NOTE]
>
>Se a visualização retornar um erro ou nenhum conteúdo, verifique a função de renderização do espaço de oferta, as regras de elegibilidade da oferta e se todos os campos de conteúdo necessários estão preenchidos.

## Aprovar e implantar a oferta {#approve-deploy}

As ofertas não estão imediatamente disponíveis nos deliveries: elas passam por um ciclo de aprovação e implantação.

1. Na visão geral da oferta, clique em **[!UICONTROL Aprovação]**.

   ![Captura de tela mostrando a aprovação da oferta.](assets/offers-offer-4.png){zoomable="yes"}

1. Aprove a **[!UICONTROL Qualificação]** e o **[!UICONTROL Conteúdo]**. O conteúdo pode ser aprovado por espaço de oferta, para que você possa aprová-lo para um espaço de oferta enquanto deixa outros pendentes.

1. Depois que ambas as aprovações forem concedidas, clique em **[!UICONTROL Implantar]** para publicar a oferta no ambiente live.

1. Atualize a exibição de oferta para confirmar se a representação **[!UICONTROL Em tempo real]** está atualizada.

<!--
>[!NOTE]
>
>Once deployed, the design offer's status resets to **[!UICONTROL Being edited]** — its normal draft status, not a sign that someone is actively editing it. This just means the design offer is ready to accept further changes, which would then need to go through a new approval and deployment cycle. The live representation itself remains untouched until that happens.
-->

>[!CAUTION]
>
>A aprovação da qualificação e do conteúdo de uma oferta são duas ações distintas. Uma oferta pode ser parcialmente aprovada (somente conteúdo, por exemplo) e permanecer indisponível para entrega até que a aprovação de qualificação também seja concedida.

## Monitorar o painel de ofertas {#dashboard}

A guia de oferta **[!UICONTROL Visão geral]** resume o status da oferta em **[!UICONTROL Propriedades]**, **[!UICONTROL Conteúdo]** e **[!UICONTROL Qualificação]** cartões, com um ícone de lápis em cada um para voltar à edição. Um cartão **[!UICONTROL Representation]** lista todos os espaços de oferta aos quais a oferta está vinculada, juntamente com seu status de design atual.

![Captura de tela mostrando o painel Oferta.](assets/offers-offer-5.png){zoomable="yes"}

Clique em **[!UICONTROL Logs]** para acessar os logs de implantação ou no menu **····** (**[!UICONTROL Mais]**) para **[!UICONTROL Duplicar]** ou **[!UICONTROL Excluir]** a oferta.

Quando uma oferta está ativa, a modificação de qualquer configuração altera a oferta de design de volta para um estado editável. A representação em tempo real permanece inalterada até o próximo ciclo de aprovação e implantação.

## Usar a oferta em um delivery {#use-in-delivery}

Quando a oferta estiver ativa, ela poderá ser selecionada em qualquer delivery direcionado ao espaço de ofertas correspondente. Saiba como configurar ofertas em uma entrega no [Adicionar ofertas às suas mensagens](../msg/offers.md).

Para obter a integração completa de entrega de saída, incluindo como a chamada do mecanismo é criada e como o rastreamento é aplicado aos links de oferta, consulte as [ofertas de documentação do Campaign v8 em entregas de saída](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-send-offers.html){target="_blank"}.

