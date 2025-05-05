---
audience: end-user
title: Usar a atividade de workflow Alterar fonte de dados
description: Saiba como usar a atividade de workflow Alterar fonte de dados
exl-id: 4dd28746-7bc7-49fc-91ac-3312af02ef45
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 13%

---

# Alterar fonte de dados {#change-data-source}

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_data_source"
>title="Alterar fonte de dados"
>abstract="A atividade **Alterar fonte de dados** permite selecionar uma fonte de dados diferente para a tabela de trabalho do fluxo de trabalho."

A atividade **Alterar fonte de dados** é uma atividade de **direcionamento**. Essa atividade permite alterar a fonte de dados usada pela tabela de Trabalho do workflow. Isso proporciona mais flexibilidade, permitindo que você gerencie dados em seus diferentes bancos de dados e melhore o desempenho.

Nos fluxos de trabalho, os dados transportados de uma atividade para outra por meio de transições são armazenados em uma **Tabela de trabalho** temporária. Por padrão, as tabelas de trabalho são criadas no mesmo banco de dados da origem dos dados processados. Por exemplo, ao consultar a tabela &quot;Perfis&quot;, armazenada no banco de dados em nuvem, uma tabela de Trabalho é criada no mesmo banco de dados em nuvem.

Em alguns casos, os dados não estão disponíveis no banco de dados atual ou não são eficientes o suficiente para executar operações unitárias. Portanto, talvez seja necessário forçar o fluxo de trabalho a usar um banco de dados diferente para executar essas operações adicionando uma atividade **[!UICONTROL Alterar fonte de dados]**.

Informações detalhadas sobre a arquitetura do Campaign estão disponíveis na [documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/architecture/architecture.html?lang=pt-BR).

>[!IMPORTANT]
>
>Observe que as atividades **[!UICONTROL Alterar Dimensão]** e **[!UICONTROL Alterar Fonte de Dados]** não devem ser adicionadas em uma linha. Se você precisar usar ambas as atividades consecutivamente, inclua uma atividade **[!UICONTROL Enriquecimento]** entre elas. Isso garante a execução adequada e evita possíveis conflitos ou erros.

<!--

Let's say you want to send VIP customers a unique offer code that they can redeem on your online store. To do this, you need to:

1. Query VIP customers on the "Profiles" table located on the Cloud database,
1. Retrieve an offer code for each targeted profile through API calls,
1. Update each profile with the assigned offer code,
1. Send an email to the profiles with their offer code.

In this situation, it is recommended to execute the offer code assignment operation on the local database, which is better suited for unitary operations. To do this, you need to add a **[!UICONTROL Change data source]** activity before the operation in order to execute it on the Campaign local database.

Before executing the operation, the working table is copied to the local database so that the operation can run there. Once done, the system detects that the profiles that we want to update are on another location. The data is therefore automatically copied back to the Cloud database where the "Profiles" table is located.
-->

## Configurar a atividade Alterar fonte de dados {#configure}

Siga estas etapas para configurar a atividade **Alterar fonte de dados**:

![Captura de tela mostrando como adicionar a atividade Alterar fonte de dados a um fluxo de trabalho.](../assets/workflow-change-data-source-add.png)

1. Adicione uma atividade **Alterar fonte de dados** ao seu fluxo de trabalho.

1. Defina a fonte de dados para onde deseja mover a tabela de Trabalho:

   * **[!UICONTROL Banco de dados padrão do Campaign (PostgreSQL)]**: usar o banco de dados local padrão do Campaign.
   * **[!UICONTROL Conta externa FDA]**: use bancos de dados externos da nuvem conectados à Adobe Campaign por meio do recurso Federated Data Access.

     >[!AVAILABILITY]
     >
     >A configuração do Campaign e a conexão com sistemas externos são restritas a usuários avançados e só estão disponíveis no console do cliente. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=pt-BR){target="_blank"}

1. Configure seu fluxo de trabalho para executar as operações desejadas usando a nova fonte de dados.

<!--
## Example {#example}

The workflow below illustrates the use case detailed earlier, sending VIP customers offer codes that they can redeem on our online store.

-->