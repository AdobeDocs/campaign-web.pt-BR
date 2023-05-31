---
audience: end-user
title: Criar fluxos de trabalho com o Adobe Campaign Web
description: Saiba como criar fluxos de trabalho com o Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
source-git-commit: f3474086eb3b44f07ab1020f1ddc6cad394c50c4
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 4%

---


# Criar um fluxo de trabalho {#create}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="Propriedades do fluxo de trabalho"
>abstract="A confirmar"

## Criar o workflow {#create-workflow}

A primeira etapa para criar o workflow na Web do Campaign v8 é criá-lo como um workflow independente ou diretamente em uma campanha e definir suas propriedades gerais. Para fazer isso, siga estas etapas:

1. Comece decidindo se deseja criar um workflow independente ou integrá-lo diretamente em uma campanha:

   * **Fluxo de trabalho independente**: Navegue até o menu Workflows e clique no botão Create workflow no canto superior direito.
   * **Fluxo de trabalho de campanha:** Navegue até o menu Campanhas e abra a campanha em que deseja criar um novo fluxo de trabalho. Clique no botão Create workflow no canto superior direito da guia Workflows.

   A caixa de diálogo Propriedades do workflow é exibida.

   ![](assets/workflow-create.png)

1. Selecione o template a ser usado para criar o workflow e fornecer um rótulo para o workflow.

   Os templates de workflow contêm atividades pré-configuradas e configurações gerais de propriedade que podem ser reutilizadas para criar novos workflows. Eles são criados no console do cliente. [Saiba como trabalhar com modelos](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/build-a-workflow.html#workflow-templates)

1. Expanda a seção Opções adicionais se desejar definir configurações específicas para o workflow, como a pasta de armazenamento e o fuso horário. [Saiba como configurar propriedades de fluxo de trabalho](workflow-settings.md)

1. Clique no botão Create workflow para confirmar a criação do workflow.

Com o fluxo de trabalho criado, agora é possível começar a orquestrar as várias tarefas que ele executará usando uma tela visual dedicada. [Saiba como orquestrar atividades de workflow](#build)

## Orquestrar atividades de fluxo de trabalho {#build}

Depois que você tiver [criou um workflow](create-workflow.md), seja no menu de workflow ou em uma campanha, você pode começar a orquestrar as diferentes tarefas que ele executará. Para fazer isso, uma tela visual é fornecida, permitindo que você crie um diagrama de workflow. Neste diagrama, é possível adicionar várias atividades e conectá-las em ordem sequencial.

Nessa etapa da configuração, o diagrama é exibido com um ícone de início, representando o início do workflow. Para adicionar sua primeira atividade, clique no botão + conectado ao ícone de início.

Uma lista de atividades que podem ser adicionadas ao diagrama é exibida. As atividades disponíveis dependem da sua posição no diagrama de workflow. Por exemplo, ao adicionar sua primeira atividade, você pode iniciar seu workflow direcionando um público-alvo, dividindo o caminho do workflow ou definindo uma atividade Wait para atrasar a execução do workflow. Por outro lado, após uma atividade Criar público-alvo, você pode refinar seu público-alvo com atividades de direcionamento, enviar um delivery para seu público com atividades de canal ou organizar o processo de fluxo de trabalho com atividades de controle de fluxo.

![](assets/workflow-start.png)

Depois que uma atividade é adicionada ao diagrama, um painel direito é exibido, permitindo configurar a atividade recém-adicionada com configurações específicas. Informações detalhadas sobre como configurar cada atividade estão disponíveis em [nesta seção](workflow-activities.md).

![](assets/workflow-configure-activities.png)

Repita esse processo e adicione quantas atividades desejar, dependendo das tarefas que deseja que seu workflow execute. Observe que você também pode inserir uma nova atividade entre duas atividades. Para fazer isso, clique no botão + na transição entre as atividades, selecione a atividade desejada e a configure no painel direito.

Para remover uma atividade, selecione-a na tela e clique no ícone Excluir nas propriedades da atividade.

>[!TIP]
>
>Você tem a opção de personalizar o nome das transições entre cada atividade. Para fazer isso, selecione a transição e altere seu rótulo no painel direito.

Após concluir o workflow, adicione a atividade en End no final do diagrama. Essa atividade permite marcar visualmente o final de um fluxo de trabalho e não tem impacto funcional.

Depois de criar o diagrama de workflow com êxito, você pode executá-lo e acompanhar o progresso de suas várias tarefas. [Saiba como iniciar e monitorar a execução de um workflow](start-monitor-workflows.md)
