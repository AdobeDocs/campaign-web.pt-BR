---
audience: end-user
title: Criar fluxos de trabalho com o Adobe Campaign Web
description: Saiba como criar um fluxo de trabalho com o Adobe Campaign Web
badge: label="Disponibilidade limitada"
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
source-git-commit: c18f73c08d0cc2590c1c59f05a710a1f25db040e
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 19%

---


# Criar o workflow {#create-first-workflow}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="Propriedades do fluxo de trabalho"
>abstract="Nesta tela, escolha o modelo a ser usado para criar o fluxo de trabalho e especifique um rótulo. Expanda a seção OPÇÕES ADICIONAIS para definir mais configurações, como o nome interno do fluxo de trabalho, sua pasta, fuso horário e grupo supervisor. É altamente recomendável selecionar um grupo supervisor, para que, se ocorrer um erro, os(as) operadores(as) sejam alertados(as)."


>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="Lista de fluxos de trabalho na campanha"
>abstract="A guia **Fluxos de trabalho** lista todos os fluxos de trabalho vinculados à campanha atual. Clique no nome de um fluxo de trabalho para editar. Use o botão **Criar fluxo de trabalho** para adicionar um novo fluxo de trabalho à campanha."

Você pode criar workflows independentes ou dentro de uma campanha. A primeira etapa é selecionar um template e definir suas propriedades gerais. Em seguida, você pode definir configurações adicionais, conforme necessário.

Para fazer isso, siga estes passos:

1. Para criar um **Fluxo de trabalho independente**, navegue até o **Fluxos de trabalho** menu. Para criar um **Fluxo de trabalho de campanha**, navegue até o **Campanhas** e abra a campanha para a qual deseja criar um novo workflow.

1. Clique em **[!UICONTROL Criar fluxo de trabalho]** no canto superior direito da tela.

   ![](assets/workflow-create.png)

1. No fluxo de trabalho **Propriedades** selecione o template a ser usado para criar o workflow (também é possível usar o template incorporado padrão). [Saiba mais sobre modelos de fluxo de trabalho](#workflow-templates).

1. Insira um rótulo para o fluxo de trabalho. Além disso, recomendamos que você adicione uma descrição ao workflow, no campo dedicado da **[!UICONTROL Opções adicionais]** seção da tela.

1. Expanda a **[!UICONTROL Opções adicionais]** seção para definir mais configurações para o workflow. Saiba como configurar as propriedades do fluxo de trabalho no [esta página](workflow-settings.md#properties)

   ![](assets/workflow-additional-options.png)

1. Clique em **[!UICONTROL Criar fluxo de trabalho]** para confirmar a criação do workflow.

Seu workflow agora é criado e está disponível na lista de workflows. Agora é possível acessar a tela visual e começar a adicionar, configurar e orquestrar as tarefas que serão executadas. [Saiba como orquestrar atividades de workflow](orchestrate-activities.md).

## Trabalhar com modelos de fluxo de trabalho {#workflow-templates}

>[!CONTEXTUALHELP]
>id="acw_workflow_template_for_campaign"
>title="Templates de workflow"
>abstract="Os modelos de fluxo de trabalho contêm configurações e atividades predefinidas que podem ser reutilizadas para criar novos fluxos de trabalho."

>[!CONTEXTUALHELP]
>id="acw_workflow_template_creation_properties"
>title="Propriedades do fluxo de trabalho"
>abstract="Os templates de workflow contêm configurações e atividades predefinidas que podem ser reutilizadas para criar novos workflows. Nesta tela, insira o rótulo do template de workflow e defina suas configurações, como o nome interno, a pasta e as pastas de execução, o fuso horário e o grupo supervisor."

Os templates de workflow contêm configurações e atividades predefinidas que podem ser reutilizadas para criar novos workflows. É possível selecionar o template do workflow nas propriedades do workflow, ao criar um workflow. Um template vazio é fornecido por padrão.

Você pode criar um modelo a partir de um fluxo de trabalho existente ou criar um novo modelo do zero. Ambos os métodos são detalhados abaixo.

>[!BEGINTABS]

>[!TAB Criar um modelo a partir de um fluxo de trabalho existente]

Para criar um template de workflow a partir de um workflow existente, siga estas etapas:

1. Abra para o **Fluxos de trabalho** e navegue até o fluxo de trabalho para salvar como modelo.
1. Clique nos três pontos à direita do nome do workflow e escolha **Copiar como modelo**.

   ![](assets/wf-copy-as-template.png)

1. Na janela pop-up, confirme a criação do template.
1. Na tela do modelo de fluxo de trabalho, marque, adicione e configure as atividades conforme necessário.
1. Navegue até as configurações, no **Configurações** para alterar o nome do template de workflow e insira uma descrição.
1. Selecione o **pasta** e **pasta de execução** do modelo. A pasta é o local onde o modelo de fluxo de trabalho é salvo. A pasta de execução é a pasta onde os workflows criados com base nesse template são salvos.

   ![](assets/wf-settings-template.png)

   As outras propriedades são comuns a workflows. Saiba mais [nesta página](workflow-settings.md#properties)

1. Salve as alterações.

O template de workflow agora está disponível na lista de templates. Você pode criar um workflow com base nesse template. Esse workflow será pré-configurado com as configurações e atividades definidas no template.


>[!TAB Criar um modelo do zero]


Para criar um template de workflow do zero, siga estas etapas:

1. Abra para o **Fluxos de trabalho** e navegue até o menu **Modelos** guia. Você pode ver a lista de modelos de workflow disponíveis.
1. Clique em **[!UICONTROL Criar modelo]** no canto superior direito da tela.
1. Insira o rótulo e abra as opções adicionais para inserir uma descrição do template de workflow.
1. Selecione a pasta e a pasta de execução do modelo. A pasta é o local onde o modelo de fluxo de trabalho é salvo. A pasta de execução é a pasta onde os workflows criados com base nesse template são salvos.

   ![](assets/new-wf-template.png)

   As outras propriedades são comuns a workflows. Saiba mais [nesta página](workflow-settings.md#properties)

1. Clique em **Criar** botão para confirmar as configurações.
1. Na tela do modelo de fluxo de trabalho, adicione e configure as atividades conforme necessário.

   ![](assets/wf-template-activities.png)

1. Salve as alterações.

O template de workflow agora está disponível na lista de templates. Você pode criar um workflow com base nesse template. Esse workflow será pré-configurado com as configurações e atividades definidas no template.

>[!ENDTABS]
