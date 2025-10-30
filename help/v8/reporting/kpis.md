---
title: Indicadores-chave de desempenho
description: Saiba como entender os indicadores principais de desempenho
exl-id: 4b182219-100b-4101-919b-b0b770dd8515
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '1191'
ht-degree: 38%

---

# Indicadores-chave de desempenho {#kpis}

>[!CONTEXTUALHELP]
>id="acw_homepage_kpi"
>title="Indicadores principais de desempenho"
>abstract="A seção **Indicadores-chave de desempenho** permite verificar a eficiência da plataforma por meio de KPIs comuns."

<!-- à enlever? -->

>[!CONTEXTUALHELP]
>id="acw_keyindicators_spam"
>title="Spam"
>abstract="KPI de spam"

Navegue até a página inicial para verificar os indicadores principais de desempenho da sua plataforma. Esses indicadores mostram o número e a porcentagem de mensagens entregues, abertas, clicadas, unsubscriptions e taxas de erro.

As métricas são calculadas para deliveries enviados nos sete dias anteriores por padrão. É possível alterar o período na lista suspensa na seção superior direita do cartão. As mensagens enviadas para perfis de teste são excluídas.

É possível selecionar o canal a ser exibido. Por padrão, esses indicadores refletem as métricas do canal de email.

![Captura de tela mostrando o cartão KPI com métricas para o canal de email.](assets/kpi.png){zoomable="yes"}

## Mensagem entregue {#ui-delivered-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_delivered"
>title="Entregue"
>abstract="Essa métrica mostra, para o canal selecionado, a soma de todas as mensagens processadas com sucesso e a porcentagem de mensagens entregues com sucesso em comparação ao número total de mensagens enviadas."

O número de mensagens entregues reflete a taxa de capacidade de entrega. Nunca pode ser 100% pelos seguintes motivos: alguns endereços ou números de telefone podem estar errados, os bloqueadores de spam em provedores de email podem rejeitar suas mensagens ou podem ocorrer problemas de entrega.

O indicador **Entregue** mostra os seguintes KPIs para cada canal:

* Porcentagem do número de mensagens entregues com êxito em comparação ao número total de mensagens enviadas.

* Soma de todas as mensagens processadas com sucesso.

No Adobe Campaign, a regra para marcar uma mensagem como “Entregue” é:

Contagem de mensagens para as quais o campo &quot;seed address&quot; é igual a &quot;Não&quot; e com um status igual a &quot;Considerado pelo provedor de serviços&quot; (para SMS), &quot;Enviado&quot; (para Emails) ou &quot;Recebido no celular&quot; (para notificações por push).

## Total de aberturas {#ui-open-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_opens"
>title="Aberturas"
>abstract="Essa métrica mostra, para o canal selecionado, a soma de todas as mensagens abertas e a porcentagem de mensagens abertas em comparação ao número total de mensagens entregues com sucesso."

O total de aberturas é calculado rastreando o número total de vezes que uma mensagem é aberta, independentemente de quantos recipients individuais geram essas aberturas. Esse indicador só está disponível para emails.

O indicador **Opens** mostra os seguintes KPIs para cada canal:

* Porcentagem do número de mensagens abertas em comparação ao número total de mensagens entregues com êxito.

* Soma de todas as mensagens abertas por canal.

O Adobe Campaign detecta a abertura da mensagem quando o destinatário faz o download das imagens do email. Os emails do HTML e Multipart/alternative incluem uma imagem de 0 pixel, que permite detectar mensagens que foram abertas. Como as mensagens em formato de texto não incluem imagens, é impossível detectar se foram abertas. Os valores calculados com base na abertura de mensagem são sempre estimativas devido à margem de erro vinculada à exibição de imagem.

## Índice de click-through {#ui-click-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_clicks"
>title="Cliques"
>abstract="Essa métrica mostra, para o canal selecionado, a soma de todos os URLs clicados nas mensagens e a porcentagem de cliques em comparação ao número total de mensagens entregues com sucesso."

Adicione URLs no conteúdo da mensagem para redirecionar os recipients para uma página específica. A taxa de cliques mede o número e a porcentagem de recipients que clicaram em um link na mensagem.

O indicador **Clicks** mostra os seguintes KPIs para cada canal:

* Porcentagem do número de cliques em comparação ao número total de mensagens entregues com sucesso.

* Número de pessoas distintas que clicaram pelo menos uma vez em um delivery. Os links de unsubscription e links para a mirror page de email são excluídos.

Essas métricas são baseadas na tabela Consolidated tracking (`nms:trackingStats`). Essa tabela de agregação é usada por motivos de desempenho ao exibir relatórios, em vez da tabela de logs de rastreamento de recipient (`nms:trackingLogRcp`). Ele não é calculado em tempo real. A tabela é gerada alguns minutos após os logs de rastreamento serem recuperados.

## Taxas de assinatura {#ui-sub-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_subscriptions"
>title="Assinaturas"
>abstract="Esta métrica mostra, para o canal selecionado, a soma de todas as assinaturas de um serviço e a porcentagem de assinaturas em comparação com o número total de mensagens entregues com sucesso."

Os recipients podem optar por receber comunicações por email e SMS.

O indicador **Assinaturas** mostra os seguintes KPIs para cada canal:

* Porcentagem do número de assinaturas em comparação ao número total de mensagens entregues com êxito.

>[!NOTE]
>
> Os KPIs de assinatura e cancelamento de assinatura variam de acordo com o tipo de serviço. Por exemplo, as assinaturas e unsubscriptions por email englobam todos os serviços relacionados a email, sejam eles resultantes de ações manuais ou formulários web. É importante distinguir essa abordagem da métrica de cancelamento de subscrição no nível do delivery, que rastreia os cliques no link de unsubscription em vez de usuários reais com assinatura cancelada.

## Taxas de cancelamentos de assinatura {#ui-unsub-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_unsubscriptions"
>title="Unsubscriptions"
>abstract="Essa métrica mostra, para o canal selecionado, a soma de todos os cancelamentos de assinatura de um serviço e a porcentagem de cancelamentos de assinatura em comparação ao número total de mensagens entregues com sucesso."

Os recipients devem poder recusar o email e o SMS por meio de um link de cancelamento de subscrição dedicado no conteúdo do email ou respondendo PARAR a um SMS.

O indicador **Unsubscriptions** mostra os seguintes KPIs para cada canal:

* Porcentagem do número de unsubscriptions em comparação ao número total de mensagens entregues com sucesso.

* Soma de todos os cliques em um link de cancelamento de subscrição, ou seja, com uma categoria de URL igual a &quot;Opt out&quot;.

>[!NOTE]
>
> Os KPIs de assinatura e cancelamento de assinatura variam de acordo com o tipo de serviço. Por exemplo, as assinaturas e unsubscriptions por email englobam todos os serviços relacionados a email, sejam eles resultantes de ações manuais ou formulários web. É importante distinguir essa abordagem da métrica de cancelamento de subscrição no nível do delivery, que rastreia os cliques no link de unsubscription em vez de usuários reais com assinatura cancelada.

## Taxas de erro {#ui-error-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_errors"
>title="Erros"
>abstract="Número total de erros acumulados durante entregas e processamentos automáticos de rejeição. A taxa associada é a relação com o número de mensagens a serem entregues."

Algumas mensagens enviadas pela plataforma do Adobe Campaign podem não chegar ao destino. Isso pode acontecer quando o endereço do usuário ou o telefone tem erros de digitação, se o recipient alterou seu endereço de email ou se a caixa de entrada está cheia. Se uma mensagem não puder ser enviada a um perfil, o servidor remoto enviará automaticamente uma mensagem de erro ao Adobe Campaign. Este erro é qualificado para determinar se o endereço de email, o número de telefone ou o dispositivo deve ir para a quarentena.

Verifique e atualize seu banco de dados regularmente e verifique se todos os perfis estão ativos e reais. Os erros de delivery podem ser temporários ou permanentes — rejeição temporária ou permanente — dependendo do motivo pela qual a mensagem não foi entregue.

O indicador **Erros** mostra os seguintes KPIs para cada canal:

* Porcentagem do número de erros em comparação ao número total de mensagens a serem entregues.

* Número total de erros acumulados durante as entregas e o processamento automático de reassociação.

## Mensagem enviada {#ui-sent-kpi}

<!--DRAFT - This section requires a validation-->

>[!CONTEXTUALHELP]
>id="acw_keyindicators_sent"
>title="Enviado"
>abstract="Essa métrica mostra, para o canal de correspondência direta, a soma de todas as mensagens enviadas e a porcentagem de mensagens enviadas ao provedor, em comparação com o número total de mensagens preparadas durante a fase de preparo da entrega."

Durante a fase de preparação, o arquivo de extração de correspondência direta é gerado, mas as informações relacionadas aos recipients (logs do delivery) não são atualizadas. O status de um delivery muda de Pending delivery para Sent quando o usuário do Campaign confirma o envio do delivery. Em seguida, o delivery é definido como Finished.

Nunca pode ser 100% das mensagens enviadas em comparação ao total de mensagens preparadas, pois alguns endereços podem estar ausentes ou incompletos.

O indicador **Enviado** mostra os seguintes KPIs para o canal de correspondência direta:

* Porcentagem do número de mensagens enviadas em comparação ao número total de mensagens preparadas.

* Soma de todas as mensagens enviadas.