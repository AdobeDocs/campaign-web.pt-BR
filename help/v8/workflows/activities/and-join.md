---
audience: end-user
title: Usar a atividade de fluxo de trabalho AND-join
description: Saiba como usar a atividade de fluxo de trabalho AND-join
exl-id: 2470e5fa-5596-4441-b9b9-7e8b5d1d53aa
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 50%

---

# AND-join {#join}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="Atividade AND-join"
>abstract="A atividade **AND-join** permite sincronizar várias ramificações de execução de um fluxo de trabalho. Ela é acionada quando todas as atividades anteriores forem concluídas. Isso garante que determinadas atividades sejam concluídas antes de continuar a executar o fluxo de trabalho."

A atividade **AND-join** é uma atividade de **Controle de fluxo**. Ele sincroniza várias ramificações de execução de um fluxo de trabalho.

Essa atividade aciona a transição de saída somente após todas as transições de entrada serem ativadas. Em outras palavras, é ativado depois que todas as atividades anteriores são concluídas. Isso garante que determinadas atividades sejam concluídas antes de continuar a executar o workflow.

## Configurar a atividade AND-join {#and-join-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="Opções de mesclagem"
>abstract="Selecione de quais atividades deseja juntar. No menu suspenso **Conjunto principal**, escolha a população de transição de entrada que deseja manter."

Siga estas etapas para configurar a atividade **AND-join**:

![Captura de tela mostrando a interface de configuração para a atividade AND-join.](../assets/workflow-andjoin.png)

1. Adicione várias atividades, como atividades de canal, para formar pelo menos duas ramificações de execução diferentes.
1. Adicione uma atividade **AND-join** a qualquer uma das ramificações.
1. Na seção **Opções de mesclagem**, marque todas as atividades anteriores nas quais deseja ingressar.
1. No menu suspenso **Conjunto principal**, escolha a população de transição de entrada a ser mantida. A transição de saída só pode conter uma das populações de transição de entrada.

## Exemplo {#and-join-example}

O exemplo a seguir mostra duas ramificações de fluxo de trabalho com uma entrega de SMS e email. O AND-join é acionado quando ambas as transições de entrada são ativadas. As notificações por push são enviadas somente após a conclusão de ambos os deliveries.

![Exemplo de fluxo de trabalho com duas ramificações, mostrando a entrega de emails e SMS seguida de notificações por push.](../assets/workflow-andjoin-example.png){zoomable="yes"}