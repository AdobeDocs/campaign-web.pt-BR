---
audience: end-user
title: Trabalhar com atividades de fluxo de trabalho
description: Saiba como usar as atividades de fluxo de trabalho
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
TQID: https://experienceleague.adobe.com/Yt-mvqKULJIMshitpuuU03U7Dl2m0DnhWoP8kdBoaUI
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
  - id: a658c786-869b-4194-a780-2594d663adda
subfeature_v2:
  - id: d1110311-2ca4-442b-be37-088a6db845ee
  - id: fcb46c0f-76e1-48bc-9dd0-fcf9d97526cf
topic_v2:
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
source-git-commit: 9bb8a5cdd958a693afccff5468df5911237044b2
workflow-type: tm+mt
source-wordcount: 583
ht-degree: 19%

---

# Sobre atividades de fluxo de trabalho {#workflow-activities}

As atividades de fluxo de trabalho são agrupadas em três categorias. Dependendo do contexto, as atividades disponíveis podem ser diferentes.

Todas as atividades estão detalhadas nas seções abaixo:

* [Atividades de direcionamento e gestão de dados](#targeting)
* [Atividades do canal](#channel)
* [Atividades de controle de fluxo](#flow-control)

![Visão geral das atividades do fluxo de trabalho](../assets/workflow-activities.png)

## Atividades de direcionamento {#targeting}

Essas atividades são específicas para direcionamento. Eles permitem criar um ou mais públicos-alvo de direcionamento definindo um público-alvo e dividindo ou combinando esses públicos-alvo usando operações de interseção, união ou exclusão.

* [Criar público-alvo](build-audience.md): defina sua população de destino. Selecione um público existente ou use o modelador de consultas para definir sua própria consulta. Você também pode configurar **Dados de enriquecimento** (disponíveis para consultas).
* [Alterar fonte de dados](change-data-source.md): altere a fonte de dados da tabela de trabalho do seu fluxo de trabalho.
* [Alterar dimensão](change-dimension.md): altere a targeting dimension ao criar seu fluxo de trabalho.
* [Combinar](combine.md): executar segmentação na população de entrada. Use uma união, uma interseção ou uma exclusão.
* [Desduplicação](deduplication.md): remova duplicatas nos resultados das atividades de entrada.
* [Enriquecimento](enrichment.md): defina dados adicionais para processar em seu fluxo de trabalho. Configure a atividade para concluir a transição de saída com dados adicionais.
* [Consulta incremental](incremental-query.md): consulte o banco de dados de acordo com o agendamento. Cada vez que essa atividade é executada, ela exclui os resultados das execuções anteriores, direcionando somente para os novos elementos.
* [Reconciliação](reconciliation.md): defina o vínculo entre os dados no banco de dados do Adobe Campaign e os dados em uma tabela de trabalho, como dados carregados de um arquivo externo.
* [Salvar público-alvo](save-audience.md): atualize um público-alvo existente ou crie um novo público-alvo a partir da população computada upstream em um fluxo de trabalho.
* [Split](split.md): segmente a população de entrada em vários subconjuntos.

## Atividades de gerenciamento de dados {#data}

Essas atividades são específicas para manipular e enriquecer dados de população.

* [Extrair arquivo](extract-file.md): exporte dados do Adobe Campaign para outro sistema como um arquivo externo.
* [Carregar arquivo](load-file.md): trabalhar com perfis e dados armazenados em um arquivo externo.
* [Transferir arquivo](transfer-file.md): receber ou enviar arquivos, testar a presença de arquivos ou listar arquivos em um servidor. O protocolo usado pode ser o protocolo servidor para servidor ou o protocolo HTTP.
* [Código JavaScript](javascript-code.md): execute um trecho de código JavaScript no contexto de um fluxo de trabalho.
* [Serviços de assinatura](subscription-services.md): assine ou cancele a assinatura de vários perfis para ou de um serviço em uma única ação.
* [Atualizar dados](update-data.md): execute atualizações em massa nos campos do banco de dados. Várias opções permitem personalizar a atualização dos dados.

## Atividades do canal {#channel}

O Adobe Campaign Web permite automatizar e executar campanhas de marketing em vários canais. Combine atividades de canal na tela para criar workflows entre canais que acionam ações com base no comportamento do cliente. As seguintes atividades do **Canal** estão disponíveis: Notificações por push de email, SMS, Android e iOS. [Saiba como configurar uma entrega no contexto de um fluxo de trabalho](channels.md).

## Atividades de controle de fluxo {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_start"
>title="Atividade de término"
>abstract="A atividade **Iniciar** permite marcar graficamente o início de um fluxo de trabalho. Essa atividade não tem impacto funcional e, portanto, é opcional."

As atividades a seguir são específicas para organizar e executar fluxos de trabalho. Sua principal tarefa é coordenar as outras atividades:

* [Sinal externo](external-signal.md): acione a execução de um fluxo de trabalho a partir de outro fluxo de trabalho ou de uma chamada de API.
* [Bifurcação](fork.md): crie transições de saída para iniciar várias atividades simultaneamente.
* [Ingressar](join.md): sincroniza várias ramificações de execução de um fluxo de trabalho.
* [Agendador](scheduler.md): agendar quando o fluxo de trabalho será iniciado.
* **Início** e [Fim](end.md): marca graficamente o início e o fim de um fluxo de trabalho. Eles são opcionais e não têm impacto funcional por conta própria.

  >[!NOTE]
  >
  >Observe que a atividade **Start** é adicionada automaticamente a todos os fluxos de trabalho criados antes da versão 26.3. Ele não é inserido por padrão em novos workflows.

* [Test](test.md): habilitar transições com base em condições especificadas.
* [Aguardar](wait.md): pausar temporariamente a execução de uma parte de um fluxo de trabalho.