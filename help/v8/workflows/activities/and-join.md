---
audience: end-user
title: Usar a atividade de workflow AND-join
description: Saiba como usar a atividade de workflow AND-join
badge: label="Alpha" type="Positive"
source-git-commit: 12d87baff81298583fac12fdf04d39997e875954
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 4%

---


# AND-join {#join}

A variável **Associação AND** A atividade permite sincronizar várias ramificações de execução de um fluxo de trabalho.

A atividade AND-join só acionará a transição de saída depois que todas as transições de entrada forem ativadas, ou seja, depois que todas as atividades anteriores forem concluídas.

Siga estas etapas para configurar o **AND-join** atividade:

1. Adicione várias atividades, como **Combinar** para formar pelo menos duas ramificações de execução diferentes.
1. Adicionar um **AND-join** atividade a qualquer uma das ramificações.
1. No **Opções de mesclagem** marque todas as atividades anteriores nas quais deseja participar.
1. Selecione o **Conjunto principal** a ser mantido na transição de saída.
