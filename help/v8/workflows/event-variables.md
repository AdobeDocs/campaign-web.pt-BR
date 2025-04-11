---
audience: end-user
title: Variáveis de evento do fluxo de trabalho
description: Saiba como aproveitar variáveis de evento em seus workflows.
exl-id: 526dc98f-391d-4f3f-a687-c980bf60b93b
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 9%

---

# Variáveis de evento do fluxo de trabalho {#event-variables}

Algumas atividades de workflow permitem editar scripts no editor de expressão para executar ações específicas, como recuperar dados de atividades anteriores, condições de criação ou calcular nomes de arquivo com base em variáveis de evento.

## O que são variáveis de evento {#scripting}

Os scripts executados no contexto de um fluxo de trabalho acessam uma série de **objetos** globais adicionais, como o próprio fluxo de trabalho que está sendo executado (`instance`), suas várias tarefas (`task`) ou os eventos que ativaram determinada tarefa (`event`).

Cada tipo de **objeto** está associado a uma categoria de **variáveis** que podem ser usadas no editor de expressão ao editar scripts em atividades, como **[!UICONTROL código JavaScript]** ou **[!UICONTROL Teste]**.

* **As variáveis de instância** (`instance.vars.xxx`) são comparáveis às variáveis globais. Eles são compartilhados por todas as atividades.
* **As variáveis de tarefa** (`task.vars.xxx`) são comparáveis com as variáveis locais. São utilizadas somente pela tarefa atual. Essas variáveis são usadas por atividades persistentes para manter os dados e, às vezes, são usadas para trocar dados entre os diferentes scripts da mesma atividade.
* **As variáveis de evento** (`vars.xxx`) habilitam a troca de dados entre as tarefas primárias de um processo de fluxo de trabalho. Essas variáveis são passadas pela tarefa que ativou a tarefa em andamento. Eles são passados para as atividades seguintes. **As variáveis de evento** são as variáveis usadas com mais frequência e devem ser usadas em detrimento de variáveis de instância.

>[!NOTE]
>
>Informações adicionais sobre scripts e os objetos e variáveis expostos no Adobe Campaign estão disponíveis na documentação do Campaign v8 (console do cliente) em [esta seção](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-scripts-and-templates).
>
>Observe que, embora esse recurso ofereça insights valiosos, podem existir discrepâncias, pois ele se aplica especificamente ao console do cliente em vez da interface da Web do Campaign.

## Aproveitar variáveis de evento no editor de expressão {#expression-editor}

As variáveis de evento predefinidas estão disponíveis para uso no painel lateral esquerdo do editor de expressão. Você também pode criar novas variáveis inicializando uma nova variável no código.

![Captura de tela mostrando variáveis de evento predefinidas no painel do lado esquerdo do editor de expressão](assets/event-variables.png)

Além dessas variáveis de evento, você também pode usar o menu **[!UICONTROL Condições]** no painel esquerdo para criar condições e o menu **[!UICONTROL Adicionar data atual]** para aplicar funções relacionadas à formatação de data.