---
audience: end-user
title: Enviar usando ondas
description: Saiba mais sobre as configurações de entrega no Campaign Web
badge: label="Disponibilidade limitada"
source-git-commit: 3bfcf3c5a5e054995993d38a073733fef8ea4be9
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 81%

---


# Enviar usando ondas {#send-using-waves}

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_definition"
>title="Definição de ondas"
>abstract="Defina ondas para dividir as entregas em vários lotes em vez de enviar grandes volumes de mensagens ao mesmo tempo."

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_size"
>title="Tamanho da onda"
>abstract="O tamanho da onda é necessário. Insira um valor numérico (número de mensagens) ou uma porcentagem (0 a 100%) no campo de tamanho."

Para balancear a carga, você pode dividir entregas em vários lotes. Configure o número de lotes e sua proporção com relação à entrega inteira.

>[!NOTE]
>
>Você só poderá definir o tamanho e o atraso entre duas ondas consecutivas. Os critérios de seleção de recipient para cada onda não podem ser configurados.

1. Abra o [configurações de entrega](delivery-settings.md#retries) e vá para a página **[!UICONTROL Entrega]** guia.
1. Selecione a opção **[!UICONTROL Send using multiple waves]** e clique no link **[!UICONTROL Define waves...]**.

1. Para configurar ondas, você pode:

   * **[!UICONTROL Agendar várias ondas do mesmo tamanho]**.

     Por exemplo, se você inserir **[!UICONTROL 30%]** no campo correspondente, cada onda representará 30% das mensagens incluídas na entrega, exceto a última, que representará 10% das mensagens.

     ![](assets/waves-same-size.png)

     No **[!UICONTROL Interval]** especifique o atraso entre o início de duas ondas consecutivas. Por exemplo, se você inserir **[!UICONTROL 2d]**, a primeira onda começará imediatamente, a segunda onda começará em dois dias, a terceira onda em quatro dias e assim por diante.

   * **[!UICONTROL Agendar ondas de acordo com um calendário]**.

     Na coluna **[!UICONTROL Start]**, especifique o atraso entre o início de duas ondas consecutivas. Na coluna **[!UICONTROL Size]**, insira um número fixo ou uma porcentagem.

     No exemplo abaixo, a primeira onda representa 25% do número total de mensagens incluídas na entrega e iniciará imediatamente. As próximas duas ondas completam a entrega e são definidas para começar em intervalos de seis horas.

     ![](assets/waves-calendar.png)

     Uma regra de controle de tipologia específica, **[!UICONTROL Verificação de agendamento de onda]**, garante que a última onda seja planejada antes do limite da validade do delivery. As tipologias de campanha e suas regras são configuradas no **[!UICONTROL Tipologia]** das configurações de delivery. Saiba mais sobre regras de controle no [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html).

     >[!IMPORTANT]
     >
     >Certifique-se de que as últimas ondas não excedam o prazo da entrega, que é definido na guia **[!UICONTROL Validity]**. Caso contrário, algumas mensagens podem não ser enviadas. [Saiba mais](delivery-settings.md#validity)
     >
     >Você também deverá permitir tempo suficiente para novas tentativas ao configurar as últimas ondas. [Saiba mais](delivery-settings.md#retries)

1. Para monitorar seus envios, vá para a [logs do delivery](../monitor/delivery-logs.md).

Você pode ver as entregas que já foram enviadas nas ondas processadas (status **[!UICONTROL Sent]**) e as entregas a serem enviadas nas ondas restantes (status **[!UICONTROL Pending]**).

Os dois exemplos abaixo são os casos de uso mais comuns para usar várias ondas.

* **Durante o processo de aumento**

  Quando os emails são enviados usando uma nova plataforma, os provedores de serviços de Internet (ISPs) suspeitam de endereços IP que não são reconhecidos. Se grandes volumes de emails forem enviados repentinamente, os ISPs freqüentemente os marcam como spam.

  Para evitar ser marcado como spam, você poderá aumentar progressivamente o volume enviado usando ondas. Isso deve garantir o desenvolvimento suave da fase de inicialização e permitir que você reduza a taxa geral de endereços inválidos.

  Para fazer isso, use a opção **[!UICONTROL Schedule waves according to a calendar]**. Por exemplo, defina a primeira onda para 10%, a segunda para 15% e assim por diante.

  ![](assets/waves-ramp-up.png)

* **Campanhas envolvendo uma central de atendimento**

  Ao gerenciar uma campanha de fidelidade por telefone, sua organização tem uma capacidade limitada para processar o número de chamadas para contatar os assinantes.

  Usando ondas, você poderá restringir o número de mensagens a 20 por dia, que é a capacidade diária de processamento de uma central de atendimento.

  Para fazer isso, selecione a opção **[!UICONTROL Schedule multiple waves of the same size]**. Insira **[!UICONTROL 20]** como o tamanho da onda e **[!UICONTROL 1d]** no campo **[!UICONTROL Period]**.

  ![](assets/waves-call-center.png)