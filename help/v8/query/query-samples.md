---
audience: end-user
title: Amostras de consulta
description: Saiba como trabalhar com o modelador de consultas.
hide: true
hidefromtoc: true
exl-id: 6f8154ea-5d64-4950-9da3-427070ec7bf0
source-git-commit: eccd1ce6f95682d3dcfc224061f747f7da0b6681
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 41%

---


# Amostras de consulta {#query-samples}

## Consultas sobre recipients {#querying-recipient-table}

* Recupere os nomes e e-mails dos recipients cujo domínio de e-mail é &quot;orange.co.uk&quot; e que não vivem em Londres.

* Destinatários não contatados nos últimos sete dias.

* Domínios de email selecionados mais de 30 vezes durante deliveries anteriores.

## Consultas sobre deliveries {#number-of-clicks-for-a-specific-delivery}

* Número de cliques de uma delivery específica.

* Recipients que não abriram um email nos últimos 7 dias.

* Perfis que abriram um delivery nas últimas 2 semanas.

* Acompanhar após um delivery anterior.

  Uma entrega &quot;Oferta esportiva de verão&quot; é enviada. Quatro dias após a entrega, duas outras entregas são enviadas. Uma delas é &quot;oferta de artigos de esportes aquáticos&quot;, a outra é uma continuidade da primeira delivery &quot;oferta esportiva de verão&quot;. A entrega &quot;oferta de artigos de esportes aquáticos&quot; é enviada aos destinatários que clicaram no link &quot;esportes aquáticos&quot; na primeira entrega. Estes cliques mostram que o destinatário está interessado no tópico. Faz sentido orientá-los para ofertas semelhantes. No entanto, os destinatários que não clicaram na &quot;oferta de esportes de verão&quot; devem receber o mesmo conteúdo novamente.
