---
audience: end-user
title: Usar a atividade de fluxo de trabalho AND-join
description: Saiba como usar a atividade de fluxo de trabalho AND-join
badge: label="Beta"
exl-id: 2470e5fa-5596-4441-b9b9-7e8b5d1d53aa
source-git-commit: f4ffb1e033dae3d631772ef602e48e336c8c0f16
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 100%

---

# AND-join {#join}


>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="Atividade AND-join"
>abstract="A atividade **AND-join** permite sincronizar várias ramificações de execução de um fluxo de trabalho. Ela é acionada quando todas as atividades anteriores forem concluídas. Isso permite verificar se determinadas atividades foram concluídas antes de continuar a execução do fluxo de trabalho."

A atividade **AND-join** é uma atividade de **Controle de fluxo**. Ela permite sincronizar várias ramificações de execução de um fluxo de trabalho.

Essa atividade só acionará a transição de saída depois que todas as transições de entrada estiverem ativadas, ou seja, depois que todas as atividades anteriores estiverem concluídas. Isso permite verificar se determinadas atividades foram concluídas antes de continuar a executar o fluxo de trabalho.

## Configurar a atividade AND-join{#and-join-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="Configure a atividade AND-join"
>abstract="Selecione de quais atividades deseja juntar. No menu suspenso **Conjunto principal**, escolha a população de transição de entrada que deseja manter."

Siga estas etapas para configurar a atividade **AND-join**:

![](../assets/workflow-andjoin.png)

1. Adicione várias atividades, como atividades de canal, para formar pelo menos duas ramificações de execução diferentes.
1. Adicione uma atividade **AND-join** a qualquer uma das ramificações.
1. Na seção **Opções de mesclagem**, marque todas as atividades anteriores que você deseja mesclar.
1. No menu suspenso **Conjunto principal**, escolha a população de transição de entrada que deseja manter. A transição de saída só pode conter uma das populações de transição de entrada.

## Exemplo{#and-join-example}

O exemplo a seguir mostra duas ramificações de fluxo de trabalho com uma entrega de SMS e email. A AND-join será acionada quando ambas as transições de entrada estiverem habilitadas. As notificações por push serão enviadas somente após a conclusão de ambas as entregas.

![](../assets/workflow-andjoin-example.png)
