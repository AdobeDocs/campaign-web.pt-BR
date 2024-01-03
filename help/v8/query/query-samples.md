---
audience: end-user
title: Amostras de consulta
description: Saiba como trabalhar com o construtor de regras.
badge: label="Disponibilidade limitada"
source-git-commit: a53f33360f0dc7ca80b235bd5814fd3ccc0ff698
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 43%

---

# Amostras de consulta {#query-samples}

## Consultas sobre recipients {#querying-recipient-table}

* recupere os nomes e e-mails dos recipients cujo domínio de e-mail é &quot;orange.co.uk&quot; e que não vivem em Londres.

* destinatários não contatados nos últimos sete dias.

* domínios de email selecionados mais de 30 vezes durante deliveries anteriores.

## Consultas sobre deliveries {#number-of-clicks-for-a-specific-delivery}

* número de cliques de uma delivery específica.

* destinatários que não abriram um email nos últimos 7 dias.

* perfis que abriram um delivery nas últimas 2 semanas:

* Acompanhar após um delivery anterior.

  Uma entrega &quot;Oferta esportiva de verão&quot; é enviada. Quatro dias após a entrega, duas outras entregas são enviadas. Uma delas é &quot;oferta de artigos de esportes aquáticos&quot;, a outra é uma continuidade da primeira delivery &quot;oferta esportiva de verão&quot;. A entrega &quot;oferta de artigos de esportes aquáticos&quot; é enviada aos recipients que clicaram no link &quot;esportes aquáticos&quot; na primeira entrega. Estes cliques mostram que o recipient está interessado no tópico. Faz sentido orientá-los para ofertas semelhantes. No entanto, os recipients que não clicaram na &quot;oferta de esportes de verão&quot; devem receber o mesmo conteúdo novamente.
