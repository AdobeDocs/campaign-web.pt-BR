---
title: Indicadores-chave de desempenho
description: Saiba como entender os indicadores principais de desempenho
exl-id: 4b182219-100b-4101-919b-b0b770dd8515
source-git-commit: 5b42671173e7fd7f024eb7eb03a0836eae7ef622
workflow-type: tm+mt
source-wordcount: '1199'
ht-degree: 79%

---

# Indicadores-chave de desempenho {#kpis}

>[!CONTEXTUALHELP]
>id="acw_homepage_kpi"
>title="Indicadores-chave de desempenho"
>abstract="A seção **Indicadores-chave de desempenho** permite verificar a eficiência da plataforma por meio de KPIs comuns."

<!-- à enlever? -->
>[!CONTEXTUALHELP]
>id="acw_keyindicators_spam"
>title="Spam"
>abstract="KPI de spam"

Navegue até a página inicial para verificar os indicadores principais de desempenho da sua plataforma. Esses indicadores mostram o número e a porcentagem de mensagens entregues, abertas, clicadas, com unsubscription e taxas de erro.

As métricas são calculadas para entregas enviadas nos 7 dias anteriores por padrão. É possível alterar o período na lista suspensa na seção superior direita do cartão. As mensagens enviadas para perfis de teste são excluídas.

É possível selecionar o canal a ser exibido. Por padrão, esses indicadores refletem as métricas do canal de email.

![](assets/kpi.png){zoomable="yes"}

## Mensagem entregue {#ui-delivered-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_delivered"
>title="Entregue"
>abstract="Essa métrica mostra, para o canal selecionado, a soma de todas as mensagens processadas com sucesso e a porcentagem de mensagens entregues com sucesso em comparação ao número total de mensagens enviadas."

O número de mensagens entregues reflete a taxa de capacidade de entrega. Essa métrica nunca pode ser de 100% pelos seguintes motivos: alguns endereços ou números de telefone podem estar errados, os bloqueadores de spam em provedores de email podem rejeitar mensagens ou podem ocorrer problemas na capacidade de entrega.

O indicador **Entregue** mostra os seguintes KPIs para cada canal:

* Porcentagem do número de mensagens entregues com sucesso em comparação ao número total de mensagens enviadas.

* Soma de todas as mensagens processadas com sucesso.

No Adobe Campaign, a regra para marcar uma mensagem como “Entregue” é:

Contagem de mensagens para as quais o campo “seed address” é igual a “Não” e com um status igual a “Levada em consideração pelo provedor de serviços” (para SMS) ou “Enviada” (para Email) ou “Recebida no celular” (para notificações por Push).


## Total de aberturas {#ui-open-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_opens"
>title="Aberturas"
>abstract="Essa métrica mostra, para o canal selecionado, a soma de todas as mensagens abertas e a porcentagem de mensagens abertas em comparação ao número total de mensagens entregues com sucesso."

O total de aberturas é calculado rastreando o número total de vezes que uma mensagem é aberta, independentemente de quantos destinatários individuais geram essas aberturas. Esse indicador só está disponível para emails.

O indicador **Aberturas** mostra os seguintes KPIs para cada canal:

* Porcentagem do número de mensagens abertas em comparação ao número total de mensagens entregues com sucesso.

* Soma de todas as mensagens abertas por canal.

O Adobe Campaign detecta a abertura da mensagem quando o destinatário faz o download das imagens do email. Os emails em HTML e Multipart/alternative incluem uma imagem de 0 pixel, que permite detectar mensagens que foram abertas. Como as mensagens em formato de texto não incluem imagens, é impossível detectar se foram abertas ou não. Os valores calculados com base na abertura de mensagem são sempre estimativas, devido à margem de erro vinculada à exibição de imagem.



## Índice de click-through {#ui-click-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_clicks"
>title="Cliques"
>abstract="Essa métrica mostra, para o canal selecionado, a soma de todos os URLs clicados nas mensagens e a porcentagem de cliques em comparação ao número total de mensagens entregues com sucesso."

É possível adicionar URLs no conteúdo da mensagem, o que redireciona os destinatários para uma página específica. O Índice de click-through mede o número e a porcentagem de destinatários que clicaram em um link na mensagem.

O indicador **Cliques** mostra os seguintes KPIs para cada canal:

* Porcentagem do número de cliques em comparação ao número total de mensagens entregues com sucesso.

* Número de pessoas distintas que clicaram pelo menos uma vez em uma entrega. Os links de unsubscription e os links para mirror pages de email são excluídos.

Essas métricas são baseadas na tabela Rastreamento consolidado (`nms:trackingStats`). Essa tabela agregada é usada por motivos de desempenho ao exibir relatórios, em vez da tabela Logs de rastreamento de destinatários (`nms:trackingLogRcp`), e não é calculada em tempo real. A tabela é gerada alguns minutos após os logs de rastreamento serem recuperados.


## Taxas de assinatura {#ui-sub-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_subscriptions"
>title="Assinaturas"
>abstract="Esta métrica mostra, para o canal selecionado, a soma de todas as assinaturas de um serviço e a porcentagem de assinaturas em comparação com o número total de mensagens entregues com sucesso."


Os recipients podem aceitar comunicações por email e SMS.

O indicador **Assinaturas** mostra os KPIs a seguir. Para cada canal, a porcentagem do número de assinaturas em comparação ao número total de mensagens entregues com êxito.


>[!NOTE]
>
> Os KPIs de assinatura e cancelamento de assinatura variam de acordo com o tipo de serviço. Por exemplo, as assinaturas e unsubscriptions por email englobam todos os serviços relacionados a email, sejam eles resultantes de ações manuais ou formulários web. É importante distinguir essa abordagem da métrica de cancelamento de subscrição no nível do delivery, que rastreia os cliques no link de unsubscription em vez de usuários reais com assinatura cancelada.

## Taxas de cancelamentos de assinatura {#ui-unsub-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_unsubscriptions"
>title="Unsubscriptions"
>abstract="Essa métrica mostra, para o canal selecionado, a soma de todos os cancelamentos de assinatura de um serviço e a porcentagem de cancelamentos de assinatura em comparação ao número total de mensagens entregues com sucesso."


Os destinatários devem poder se desvincular de emails e SMS por meio de um link de unsubscription dedicado no conteúdo do email ou respondendo PARAR a um SMS.

O indicador **Unsubscriptions** mostra os seguintes KPIs para cada canal:

* Porcentagem do número de unsubscriptions em comparação ao número total de mensagens entregues com sucesso.

* Soma de todos os cliques em um link de unsubscription, ou seja, com uma categoria de URL correspondente a “Recusar”.


>[!NOTE]
>
> Os KPIs de assinatura e cancelamento de assinatura variam de acordo com o tipo de serviço. Por exemplo, as assinaturas e unsubscriptions por email englobam todos os serviços relacionados a email, sejam eles resultantes de ações manuais ou formulários web. É importante distinguir essa abordagem da métrica de cancelamento de subscrição no nível do delivery, que rastreia os cliques no link de unsubscription em vez de usuários reais com assinatura cancelada.

## Taxas de erro {#ui-error-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_errors"
>title="Erros"
>abstract="Número total de erros acumulados durante entregas e processamentos automáticos de rejeição. A taxa associada é a relação com o número de mensagens a serem entregues."

Algumas mensagens enviadas pela plataforma do Adobe Campaign podem não chegar ao destino. Isso pode acontecer quando o endereço ou telefone do usuário ou usuária tem erros de digitação, quando o endereço de email foi alterado ou quando a caixa de entrada está cheia. Se uma mensagem não puder ser enviada a um perfil, o servidor remoto enviará automaticamente uma mensagem de erro ao Adobe Campaign. Esse erro é analisado para determinar se o endereço de email, o número de telefone ou o dispositivo deve ser colocado em quarentena.

Por isso é recomendado sempre verificar e atualizar o banco de dados e certificar-se de que todos os perfis estão ativos e são reais. Os erros de entrega podem ser temporários ou permanentes (rejeição temporária ou permanente) dependendo do motivo pelo qual a mensagem não foi entregue.

O indicador **Erros** mostra os seguintes KPIs para cada canal:

* Porcentagem do número de erros em comparação ao número total de mensagens a serem entregues.

* Número total de erros acumulados durante as entregas e o processamento automático de reassociação.

## Mensagem enviada {#ui-sent-kpi}

<!--DRAFT - This section requires a validation-->

>[!CONTEXTUALHELP]
>id="acw_keyindicators_sent"
>title="Enviado"
>abstract="Esta métrica mostra, para o canal de correspondência direta, a soma de todas as mensagens enviadas, e a porcentagem de mensagens enviadas ao fornecedor, em comparação com o número total de mensagens preparadas durante a fase de preparo da entrega."

Durante a fase de preparação, o arquivo de extração de correspondência direta é gerado, mas as informações relacionadas aos recipients (ou seja, logs do delivery) não são atualizadas.  O status de um delivery movido de Pending delivery para Sent quando o usuário do Campaign confirma o envio do delivery. Em seguida, o delivery é definido como Finished.

Nunca pode ser 100% das mensagens enviadas em comparação ao total de mensagens preparadas, pois alguns endereços podem estar ausentes ou incompletos.

O indicador **Enviado** mostra os seguintes KPIs para o canal de correspondência direta:

* Porcentagem do número de mensagens enviadas em comparação ao número total de mensagens preparadas.

* Soma de todas as mensagens enviadas.

