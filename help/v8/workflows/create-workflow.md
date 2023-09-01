---
audience: end-user
title: Criar fluxos de trabalho com o Adobe Campaign Web
description: Saiba como criar fluxos de trabalho com o Adobe Campaign Web
badge: label="Beta"
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
source-git-commit: 9fb4a5057ec05877ffbadc85d1198ab24faf8972
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 25%

---


# Criar o workflow {#create-first-workflow}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="Propriedades do fluxo de trabalho"
>abstract="Nesta tela, escolha o modelo a ser usado para criar o fluxo de trabalho e especifique um rótulo. Expanda a seção Opções adicionais para definir configurações específicas, como a pasta de armazenamento do fluxo de trabalho ou o fuso horário."

A primeira etapa para criar o workflow na Web do Campaign v8 é criá-lo como um workflow independente ou diretamente em uma campanha e definir suas propriedades gerais. Para fazer isso, siga estes passos:

1. Comece decidindo se deseja criar um workflow independente ou integrá-lo diretamente em uma campanha:

   * **Fluxo de trabalho independente**: Navegue até o menu Workflows e clique no botão Create workflow no canto superior direito.
   * **Fluxo de trabalho de campanha:** Navegue até o menu Campanhas e abra a campanha em que deseja criar um novo fluxo de trabalho. Clique no botão Create workflow no canto superior direito da guia Workflows.

   A caixa de diálogo Propriedades do workflow é exibida.

   ![](assets/workflow-create.png)

1. Selecione o template a ser usado para criar o workflow e fornecer um rótulo para o workflow.

   Os templates de workflow contêm atividades pré-configuradas e configurações gerais de propriedade que podem ser reutilizadas para criar novos workflows. Eles são criados no console cliente. [Saiba como trabalhar com modelos](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/build-a-workflow.html#workflow-templates)

1. Expanda a **[!UICONTROL Opções adicionais]** se desejar definir configurações específicas para o workflow, como a pasta de armazenamento e o fuso horário. [Saiba como configurar propriedades de fluxo de trabalho](workflow-settings.md)

1. Clique em **[!UICONTROL Criar fluxo de trabalho]** para confirmar a criação do workflow.

Com o fluxo de trabalho criado, agora é possível começar a orquestrar as várias tarefas que ele executará usando uma tela visual dedicada. [Saiba como orquestrar atividades de workflow](orchestrate-activities.md)
