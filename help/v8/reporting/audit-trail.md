---
product: campaign
title: Trilha de auditoria
description: Saiba como monitorar sua instância com a Trilha de auditoria do Campaign
feature: Audit Trail, Monitoring, Workflows
exl-id: f4b4a33f-8250-4f4e-b2dc-129c56f9ea0f
source-git-commit: 5323f3db8b29376b15b400a67765c6c0eda37479
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 1%

---

# Trilha de auditoria{#audit-trail}

Na Interface do Usuário da Web do Adobe Campaign, o recurso **[!UICONTROL Trilha de auditoria]** fornece aos usuários total visibilidade de todas as modificações feitas em entidades importantes na sua instância, normalmente aquelas que afetam significativamente uma operação suave da instância.

>[!IMPORTANT]
>
>* A Adobe Campaign Web User Interface não está auditando alterações feitas em direitos de usuário, modelos, personalização ou campanhas.
>* A trilha de auditoria só pode ser gerenciada por administradores da instância.

O recurso **[!UICONTROL Trilha de auditoria]** registra constantemente um log detalhado de ações e eventos que ocorrem na instância do Adobe Campaign em tempo real. Ele oferece um método conveniente para acessar um registro cronológico de dados, abordando queries como: o status dos workflows, os indivíduos mais recentes para modificá-los ou as atividades executadas pelos usuários na instância.

+++ Saiba mais sobre entidades disponíveis da Trilha de auditoria

* **A trilha de auditoria do esquema do Source** permite monitorar atividades e modificações recentes feitas em seus esquemas no console do cliente do Campaign V8.

  Para obter informações detalhadas sobre schemas, consulte a [Documentação do Campaign v8](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas).

* A **trilha de auditoria do fluxo de trabalho** permite acompanhar atividades e alterações recentes feitas nos fluxos de trabalho, incluindo seus estados atuais, como:

   * Start
   * Pause
   * Stop
   * Restart
   * Limpeza que é igual ao histórico de Expurgação da ação
   * Simular qual é igual ao Início da ação no modo de simulação
   * Ativar que é igual à ação Executar tarefas pendentes agora
   * Unconditional Stop

  Para obter mais informações sobre fluxos de trabalho, consulte esta [página](../workflows/gs-workflows.md).

* A **Trilha de auditoria de opção** permite monitorar atividades e modificações recentes feitas em suas opções no Campaign V8.

  Para obter mais informações sobre opções, consulte esta [página](https://experienceleague.adobe.com/en/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options).

* **Trilha de auditoria de entrega** permite que você verifique as atividades e as últimas modificações feitas em suas entregas.

  Para obter mais informações sobre entregas, consulte esta [página](../msg/gs-deliveries.md).

* **Conta externa** permite que você verifique modificações feitas em contas externas no Campaign V8, usadas por processos técnicos, como workflows técnicos ou workflows da campanha.

  Para obter mais informações sobre a conta externa, consulte esta [página](../administration/external-account.md).

* **O mapeamento de entrega** permite monitorar atividades e modificações recentes feitas no mapeamento de entrega no Campaign V8.

  Para obter mais informações sobre mapeamento de entrega, consulte esta [página](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/add-profiles/target-mappings).

* O **Aplicativo Web** permite verificar as modificações feitas em formulários Web no Campaign V8 usados para criar páginas com campos de entrada e seleção e que podem incluir dados do banco de dados.

  Para obter mais informações sobre o aplicativo Web, consulte esta [página](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/content/webapps).

* A **Oferta** permite que você verifique as atividades e as últimas modificações feitas em suas ofertas.

  Para obter mais informações sobre ofertas, consulte esta [página](../msg/offers.md).

* **Operador** permite monitorar atividades e modificações recentes feitas aos seus Operadores no Campaign V8.

  Para obter mais informações sobre operadores, consulte esta [página](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/offers/interaction-settings/interaction-operators).

+++

## Acessando a Trilha de auditoria {#accessing-audit-trail}

Para acessar a **[!UICONTROL Trilha de auditoria]** da sua instância:

1. No menu **[!UICONTROL Administração]**, selecione **[!UICONTROL Trilha de auditoria]**.

   ![](assets/audit-trail-1.png)

1. A janela **[!UICONTROL Trilha de auditoria]** é aberta com a lista de suas entidades. A Interface do usuário da Web do Adobe Campaign audita a criação, edição e exclusão de ações para workflows, opções, deliveries e esquemas.

   Selecione uma das entidades para saber mais sobre as últimas modificações.

1. A janela **[!UICONTROL Entidade de auditoria]** fornece informações mais detalhadas sobre a entidade escolhida, como:

   * **[!UICONTROL Tipo]**: Fluxo de Trabalho, Opções, Entregas ou Esquemas.
   * **[!UICONTROL Entidade]**: nome interno de suas atividades.
   * **[!UICONTROL Modificado por]**: nome de usuário da última pessoa que modificou esta entidade pela última vez.
   * **[!UICONTROL Ação]**: última ação executada nesta entidade, Criada, Modificada ou Excluída.
   * **[!UICONTROL Data de modificação]**: data da última ação executada nesta entidade.

   O bloco de código fornece mais informações sobre o que foi alterado exatamente em sua entidade.

   ![](assets/audit-trail-2.png)
