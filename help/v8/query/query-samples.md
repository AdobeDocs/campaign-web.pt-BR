---
audience: end-user
title: Amostras de consulta
description: Saiba como trabalhar com o modelador de consultas.
hide: true
hidefromtoc: true
exl-id: 6f8154ea-5d64-4950-9da3-427070ec7bf0
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 42%

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

  Uma entrega &quot;Oferta esportiva de verão&quot; é enviada. Quatro dias após a entrega, duas outras entregas são enviadas. Uma delas é &quot;oferta de artigos de esportes aquáticos&quot;, a outra é uma continuidade da primeira delivery &quot;oferta esportiva de verão&quot;. A entrega &quot;oferta de artigos de esportes aquáticos&quot; é enviada aos destinatários que clicaram no link &quot;esportes aquáticos&quot; na primeira entrega. Estes cliques mostram que o destinatário está interessado no tópico. Faz sentido orientá-los para ofertas semelhantes. No entanto, os destinatários que não clicaram na &quot;oferta de esportes de verão&quot; devem receber o mesmo conteúdo novamente.
