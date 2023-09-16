---
audience: end-user
title: Introdução aos públicos-alvo
description: Saiba como usar públicos na interface do Campaign Web
badge: label="Beta"
exl-id: 21bb5082-82ce-47d6-a4d4-becf44490f13
source-git-commit: a61eb527f22346c51b935e4170e1a56bed428f78
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 98%

---


# Introdução aos públicos-alvo {#about-audiences}

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


O público-alvo é o principal foco da sua entrega: os destinatários que receberão as mensagens O tipo de público-alvo depende do target mapping definido no modelo de entrega. Saiba o que é um modelo de entrega [nesta seção](../msg/delivery-template.md).

Para definir o público, você pode:

* Criar e combinar públicos. [Saiba mais](create-audience.md)
* Selecionar um público-alvo já existente, criado como uma lista no console do cliente. [Saiba mais](add-audience.md)
* Selecionar um público-alvo da Adobe Experience Platform. [Saiba mais](aep-audience.md)
* Criar um público-alvo novo com o criador de regras definindo e combinando critérios de filtro. [Saiba mais](segment-builder.md)
* Usar um público-alvo de um arquivo externo: esta opção está disponível apenas para entregas independentes de email e não pode ser usada em entregas de campanha. [Saiba mais](file-audience.md)

Ao enviar mensagens no contexto de um workflow de campanha, o público-alvo é definido em uma atividade de workflow **Ler público-alvo** especifica. Nesse contexto, não é possível carregar um público-alvo de um arquivo para uma entrega de email, e o público-alvo é definido somente nessa atividade dedicada. Saiba como definir o público-alvo da sua entrega em um workflow de campanha [nesta seção](../workflows/orchestrate-activities.md).

Além disso, você pode definir grupos de controle para evitar o envio de mensagens para uma parte do público e medir o impacto das campanhas. [Saiba mais](control-group.md)

![](assets/about-audience.png)

