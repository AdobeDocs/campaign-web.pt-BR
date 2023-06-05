---
audience: end-user
title: Introdução aos públicos
description: Saiba como usar públicos na interface do Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 21bb5082-82ce-47d6-a4d4-becf44490f13
source-git-commit: 3ebe92659916cf2fa4cacb8d28b79d7b6d5359f3
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 31%

---


# Introdução aos públicos {#about-audiences}

<!--
Audience only created for the delivery, not available later-->


<!--
Three ways:
* existing audience

Campaign or AEP Audiences

* create new on the fly

query like AEP segment builder (same component with campaign data)

* import from file

show use case with a new audience creation (or import from file?)

control groups like acc: exract, random, based on attribute
-->


O público-alvo é o principal alvo do delivery: os recipients que recebem as mensagens. O tipo de público depende do target mapping definido no template de entrega. Saiba o que é um modelo de entrega [nesta seção](../msg/delivery-template.md).

Para definir a população do público-alvo, é possível:

* Selecione um público existente, criado como uma lista no Console do cliente. [Saiba mais](add-audience.md)
* Selecione um público-alvo do Adobe Experience Platform. [Saiba mais](aep-audience.md)
* Crie um novo público-alvo com o construtor de regras definindo e combinando critérios de filtragem. [Saiba mais](segment-builder.md)
* Use an audience from an external file: esta opção está disponível apenas para deliveries de email independentes e não pode ser usada em deliveries de campanha. [Saiba mais](file-audience.md)

Ao enviar mensagens no contexto de um workflow de campanha, o público-alvo é definido em um **Ler público** atividade de workflow. Nesse contexto, não é possível carregar um público-alvo de um arquivo para um delivery de email, e o público-alvo é definido somente nessa atividade dedicada. Saiba como definir o público-alvo do seu delivery em um fluxo de trabalho de campanha [nesta seção](../workflows/orchestrate-activities.md).

Além disso, você pode definir grupos de controle para evitar o envio de mensagens para uma parte do público e medir o impacto das campanhas. [Saiba mais](control-group.md)

![](assets/about-audience.png)

