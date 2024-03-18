---
audience: end-user
title: Criar fluxos de trabalho com o Adobe Campaign Web
description: Saiba como criar fluxos de trabalho com o Adobe Campaign Web
exl-id: 0c8e2158-518c-4620-9971-00ed2eccdd4f
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 6%

---

# Orquestrar atividades {#orchestrate}

Depois que você tiver [criou um workflow](create-workflow.md), seja no menu de workflow ou em uma campanha, você pode começar a orquestrar as diferentes tarefas que ele executará. Para fazer isso, uma tela visual é fornecida, permitindo que você crie um diagrama de workflow. Neste diagrama, é possível adicionar várias atividades e conectá-las em ordem sequencial.

## Adicionar atividades {#add}

Nessa etapa da configuração, o diagrama é exibido com um ícone de início, representando o início do workflow. Para adicionar sua primeira atividade, clique no link **+** botão conectado ao ícone iniciar.

Uma lista de atividades que podem ser adicionadas ao diagrama é exibida. As atividades disponíveis dependem da sua posição no diagrama de workflow. Por exemplo, ao adicionar sua primeira atividade, você pode iniciar seu fluxo de trabalho direcionando um público-alvo, dividindo o caminho do fluxo de trabalho ou definindo um **Aguardar** atividade para atrasar a execução do workflow. Por outro lado, depois de uma **Criar público-alvo** você pode refinar seu público-alvo com atividades de direcionamento, enviar um delivery para o público-alvo com atividades de canal ou organizar o processo de fluxo de trabalho com atividades de controle de fluxo.

![](assets/workflow-start.png){zoomable=&quot;yes&quot;}

Depois que uma atividade é adicionada ao diagrama, um painel direito é exibido, permitindo configurar a atividade recém-adicionada com configurações específicas. Informações detalhadas sobre como configurar cada atividade estão disponíveis em [nesta seção](activities/about-activities.md).

![](assets/workflow-configure-activities.png){zoomable=&quot;yes&quot;}

Repita esse processo para adicionar quantas atividades desejar, dependendo das tarefas que deseja que seu fluxo de trabalho execute. Observe que você também pode inserir uma nova atividade entre duas atividades. Para fazer isso, clique no link **+** na transição entre as atividades, selecione a atividade desejada e a configure no painel direito.

Para remover uma atividade, selecione-a na tela e clique no link **Excluir** nas propriedades da atividade.

>[!TIP]
>
>Você tem a opção de personalizar o nome das transições entre cada atividade. Para fazer isso, selecione a transição e altere seu rótulo no painel direito.

## Gerenciar atividades {#manage}

Ao adicionar atividades, os botões de ação ficam disponíveis no painel de propriedades, permitindo que você execute várias operações. Você pode:

* **Excluir** a atividade da tela.
* **Desativar/Ativar** a atividade. Quando o workflow é executado, as atividades desativadas e as atividades a seguir no mesmo caminho não são executadas e o workflow é interrompido.
* **Copiar** a atividade. É possível colá-la em qualquer workflow clicando no link **+** em uma transição e selecionando &quot;Colar 1 atividade&quot;.
* Acessar o da atividade **Logs e tarefas**.
* **Pausar/Retomar** a atividade. Quando o workflow é executado, ele é pausado na atividade pausada. A tarefa correspondente, bem como todas as que a seguem no mesmo caminho, não são executadas.

![](assets/activity-action.png){zoomable=&quot;yes&quot;}{width="50%"}

## Exemplo {#example}

Este é um exemplo de fluxo de trabalho criado para enviar um email a todos os clientes (exceto clientes do VIP) com um email interessados em máquinas de café.

![](assets/workflow-example.png){zoomable=&quot;yes&quot;}{zoomable=&quot;yes&quot;}

Para isso, as atividades abaixo foram adicionadas:

* A **[!UICONTROL Bifurcar]** atividade que divide o fluxo de trabalho em três caminhos (um para cada conjunto de clientes),
* **[!UICONTROL Criar público-alvo]** atividades para direcionar os três conjuntos de clientes:

   * Clientes com um email,
   * Clientes pertencentes ao público-alvo pré-existente &quot;Interessado em máquina(s) de café&quot;,
   * Clientes pertencentes ao público &quot;VIP ou recompensa&quot; pré-existente.

* A **[!UICONTROL Combinar]** atividade que agrupa clientes com um email e aqueles interessados em máquinas de café,
* A **[!UICONTROL Combinar]** atividade que exclui clientes VIP,
* Um **[!UICONTROL Entrega de email]** atividade que envia um email para os clientes resultantes.

Após concluir o workflow, adicione en **[!UICONTROL Fim]** atividade no final do diagrama. Essa atividade permite marcar visualmente o final de um fluxo de trabalho e não tem impacto funcional.

Depois de criar o diagrama de workflow com êxito, você pode executá-lo e acompanhar o progresso de suas várias tarefas. [Saiba como iniciar um workflow e monitorar sua execução](start-monitor-workflows.md)
