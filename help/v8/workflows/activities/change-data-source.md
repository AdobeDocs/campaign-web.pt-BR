---
audience: end-user
title: Usar a atividade de workflow Alterar fonte de dados
description: Saiba como usar a atividade de workflow Alterar fonte de dados
exl-id: 4dd28746-7bc7-49fc-91ac-3312af02ef45
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 9%

---

# Alterar fonte de dados {#change-data-source}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="Alterar fonte de dados"
>abstract="Use a nova atividade de direcionamento do fluxo de trabalho Alterar fonte de dados para alterar a fonte de dados usada pela tabela de trabalho do fluxo de trabalho. Essa atividade oferece mais flexibilidade, permitindo gerenciar dados em seus diferentes bancos de dados e melhorar o desempenho."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="Consulte as notas de versão"

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_data_source"
>title="Alterar fonte de dados"
>abstract="A variável **Alterar fonte de dados** A atividade permite selecionar uma fonte de dados diferente para a tabela de Trabalho do fluxo de trabalho."

A variável **Alterar fonte de dados** a atividade é um **direcionamento** atividade. Essa atividade permite alterar a fonte de dados usada pela tabela de Trabalho do workflow. Isso proporciona mais flexibilidade, permitindo que você gerencie dados em seus diferentes bancos de dados e melhore o desempenho.

Nos workflows, os dados transportados de uma atividade para outra por meio de transições são armazenados em um **Tabela de trabalho**. Por padrão, as tabelas de trabalho são criadas no mesmo banco de dados da origem dos dados processados. Por exemplo, ao consultar a tabela &quot;Perfis&quot;, armazenada no banco de dados em nuvem, uma tabela de Trabalho é criada no mesmo banco de dados em nuvem.

Em alguns casos, os dados não estão disponíveis no banco de dados atual ou não são eficientes o suficiente para executar operações unitárias. Portanto, talvez seja necessário forçar o workflow a usar um banco de dados diferente para executar essas operações adicionando um **[!UICONTROL Alterar fonte de dados]** atividade.

Informações detalhadas sobre a arquitetura do Campaign estão disponíveis em [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/architecture/architecture.html)

<!--

Let's say you want to send to your  VIP customers a unique offer code that they can redeem on your online store. To do this, you need to:

1. Query VIP customers on the "Profiles" table located on the Cloud database,
1. Retrieve an offer code for each targeted profile through API calls,
1. Update each profile with the assigned offer code,
1. Send an email to the profiles with their offer code.

In this situation, it is recommended to execute the offer code assignment operation on the local database, which is better suited for unitary operations. To do this, you need to add a **[!UICONTROL Change data source]** activity before the operation in order to execute it on the Campaign local database.

Before executing the operation, the working table is copied to the local database so that the operation can run there. Once done, the system detects that the profiles that we want to update are on another location. The data is therefore automatically copied back to the Cloud database where the "Profiles" table is located.
-->

## Configurar a atividade Alterar fonte de dados {#configure}

Siga estas etapas para configurar o **Alterar dimensão** atividade:

![](../assets/workflow-change-data-source-add.png)

1. Adicionar um **Alterar fonte de dados** atividade ao seu fluxo de trabalho.

1. Defina a fonte de dados para onde deseja mover a tabela de Trabalho:

   * **[!UICONTROL Banco de dados padrão do Campaign (PostgreSQL)]**: use o banco de dados local padrão do Campaign.
   * **[!UICONTROL Conta externa FDA]**: use bancos de dados externos da nuvem conectados ao Adobe Campaign por meio do recurso Federated Data Access.

     >[!AVAILABILITY]
     >
     >A configuração do Campaign e a conexão com sistemas externos são restritas a usuários avançados e só estão disponíveis no console do cliente. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=pt-BR){target="_blank"}

1. Configure seu fluxo de trabalho para executar as operações desejadas usando a nova fonte de dados.

<!--
## Example {#example}

The workflow belows illustrates the use case detailed earlier, i.e. sending VIP customers offer codes that they can redeem on our online store.

-->
