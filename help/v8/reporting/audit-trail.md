---
product: campaign
title: Trilha de auditoria
description: Saiba como monitorar sua instância com a Trilha de auditoria do Campaign
feature: Audit Trail, Monitoring, Workflows
exl-id: f4b4a33f-8250-4f4e-b2dc-129c56f9ea0f
source-git-commit: bb61fdb34fecb4131d4069965cda8a3a5099b6bc
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 6%

---

# Trilha de auditoria{#audit-trail}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn5"
>title="Trilha de auditoria"
>abstract="O novo recurso de Trilha de auditoria fornece um registro detalhado e cronológico de todas as ações e eventos realizados em sua instância do Adobe Campaign em tempo real. "
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=pt-BR" text="Consulte as notas de versão"


Na interface da Web do Adobe Campaign, a variável **[!UICONTROL Trilha de auditoria]** O recurso fornece aos usuários total visibilidade de todas as modificações feitas em entidades importantes na sua instância, normalmente aquelas que afetam significativamente uma operação suave da instância.

>[!IMPORTANT]
>
>* A Adobe Campaign Web User Interface não está auditando alterações feitas em direitos de usuário, modelos, personalização ou campanhas.
>* A trilha de auditoria só pode ser gerenciada por administradores da instância.

**[!UICONTROL Trilha de auditoria]** Esse recurso registra constantemente um log detalhado de ações e eventos que ocorrem na instância do Adobe Campaign em tempo real. Ele oferece um método conveniente para acessar um registro cronológico de dados, abordando queries como: o status dos workflows, os indivíduos mais recentes para modificá-los ou as atividades executadas pelos usuários na instância.

+++ Saiba mais sobre entidades disponíveis da Trilha de auditoria

* **Trilha de auditoria do esquema de origem** O permite monitorar atividades e modificações recentes feitas em seus esquemas no console do cliente do Campaign V8.

  Para obter informações detalhadas sobre schemas, consulte [Documentação do Campaign v8](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas).

* **Trilha de auditoria do fluxo de trabalho** permite rastrear atividades e alterações recentes feitas em workflows, incluindo seus estados atuais, como:

   * Start
   * Pause
   * Stop
   * Restart
   * Limpeza que é igual ao histórico de Expurgação da ação
   * Simular qual é igual ao Início da ação no modo de simulação
   * Ativar que é igual à ação Executar tarefas pendentes agora
   * Unconditional Stop

  Para obter mais informações sobre fluxos de trabalho, consulte esta [página](../workflows/gs-workflows.md).

* **Trilha de auditoria da opção** permite monitorar atividades e modificações recentes feitas em suas opções no Campaign V8.

  Para obter mais informações sobre opções, consulte esta [página](https://experienceleague.adobe.com/en/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options).

* **Trilha de auditoria da entrega** permite verificar as atividades e últimas modificações feitas em seus deliveries.

  Para obter mais informações sobre deliveries, consulte este [página](../msg/gs-deliveries.md).

* **Conta externa** permite verificar modificações feitas em contas externas no Campaign V8, usadas por processos técnicos, como workflows técnicos ou workflows da campanha.

  Para obter mais informações sobre contas externas, consulte este [página](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/external-accounts).

* **Mapeamento de entrega** permite monitorar atividades e modificações recentes feitas no mapeamento de delivery no Campaign V8.

  Para obter mais informações sobre mapeamento de delivery, consulte esta [página](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/add-profiles/target-mappings).

* **Aplicativo web** permite verificar as modificações feitas nos formulários web no Campaign V8 usados para criar páginas com campos de entrada e seleção e que podem incluir dados do banco de dados.

  Para obter mais informações sobre aplicativos web, consulte esta [página](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/content/webapps).

* **Oferta** O permite verificar as atividades e as últimas modificações feitas em suas ofertas.

  Para obter mais informações sobre ofertas, consulte esta [página](../msg/offers.md).

* **Operador** O permite monitorar atividades e modificações recentes feitas aos Operadores no Campaign V8.

  Para obter mais informações sobre operadores, consulte esta [página](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/offers/interaction-settings/interaction-operators).

+++

## Acessando a Trilha de auditoria {#accessing-audit-trail}

Para acessar o da instância **[!UICONTROL Trilha de auditoria]**:

1. No **[!UICONTROL Administração]** selecione **[!UICONTROL Trilha de auditoria]** .

   ![](assets/audit-trail-1.png)

1. A variável **[!UICONTROL Trilha de auditoria]** é aberta com a lista das entidades. A Interface do usuário da Web do Adobe Campaign audita a criação, edição e exclusão de ações para workflows, opções, deliveries e esquemas.

   Selecione uma das entidades para saber mais sobre as últimas modificações.

1. A variável **[!UICONTROL Entidade de auditoria]** fornece informações mais detalhadas sobre a entidade escolhida, como:

   * **[!UICONTROL Tipo]** : Fluxo de trabalho, Opções, Deliveries ou Esquemas.
   * **[!UICONTROL Entidade]** : Nome interno das atividades.
   * **[!UICONTROL Modificado por]** : Nome de usuário da última pessoa que modificou essa entidade pela última vez.
   * **[!UICONTROL Ação]** : Última ação executada nesta entidade, Criada, Modificada ou Excluída.
   * **[!UICONTROL Data de modificação]** : Data da última ação executada nesta entidade.

   O bloco de código fornece mais informações sobre o que foi alterado exatamente em sua entidade.

   ![](assets/audit-trail-2.png)
