---
title: Dimensões de direcionamento
description: Saiba mais sobre dimensões de direcionamento no Adobe Campaign Web
exl-id: b910649a-7300-4f99-8f40-3a8965572ee9
source-git-commit: 395109aeb603ecce53eda89adff70a9ef36fde17
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 24%

---

# Dimensões de direcionamento {#targeting-dimensions}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Selecione a dimensão de direcionamento"
>abstract="A dimensão de direcionamento permite definir a população-alvo da operação: destinatários, beneficiários de contrato, operadores, assinantes, etc. Por padrão, para emails e SMS, o público-alvo é selecionado na tabela integrada Destinatários. Para notificações por push, a dimensão de direcionamento padrão é Aplicativos do assinante."

Targeting dimension, também conhecido como. target mapping, é o tipo de dados que uma operação está tratando. Ele permite definir a população direcionada: perfis, beneficiários de contrato, operadores, assinantes etc.

## Dimensões de direcionamento de workflows {#workflow}

O targeting dimension de um fluxo de trabalho é definido pela primeira atividade **[!UICONTROL Build audience]** e é usado em todas as outras atividades até o fim do fluxo de trabalho. Por exemplo, se você realizar um query nos perfis do banco de dados, a transição de saída conterá dados do tipo &quot;recipient&quot; e será transmitida para a próxima atividade.

Observe que você pode alternar o targeting dimension em um fluxo de trabalho usando uma [Atividade Change dimension](../workflows/activities/change-dimension.md). Isso permite, por exemplo, consultar o banco de dados em uma tabela específica, como compras ou assinaturas, e alterar o targeting dimension para Recipients para enviar deliveries aos perfis correspondentes.

Ao selecionar uma dimensão de direcionamento (nas configurações do fluxo de trabalho ou em atividades como **Criar público-alvo**, **Reconciliação** ou **Alterar dimensão**), uma seleção de esquemas usados com frequência é exibida por padrão na lista. Para mostrar todos os esquemas disponíveis, alterne no botão **[!UICONTROL Mostrar todos os esquemas]**. A seleção da opção é salva para cada usuário.

![](assets/targeting-dimension-show-all.png){zoomable="yes"}

## Dimensões de direcionamento {#list}

Por padrão, modelos de delivery de email e SMS têm como alvo perfis. Sua dimensão de destino, portanto, usa os campos da tabela **nms:recipient**. Para notificações por push, a dimensão de destino padrão é **Subscriber applications nms:appSubscriptionRcp**, que está vinculada à tabela de destinatários.

Você também pode usar outros target mappings integrados nos workflows e deliveries listados abaixo:

| Nome | Use para | Esquema |
|---|---|---|
| Destinatários | Delivery para perfis/recipients (tabela de recipients integrada) | nms:recipient |
| Visitantes | Enviar delivery aos visitantes cujos perfis foram coletados por meio de referência (marketing viral), por exemplo. | mns:visitor |
| Subscrições | Enviar delivery aos perfis que assinam um serviço de informação, como um boletim informativo | nms:subscription |
| Assinaturas do visitante | Entregar aos visitantes que são inscritos em um serviço de informações | nms:visitorSub |
| Operadores | Entregar aos operadores do Adobe Campaign | nms:operator |
| Arquivo externo | Entregar por meio de um arquivo que contenha todas as informações necessárias para a entrega | Nenhum schema vinculado, nenhum target inserido |
| Aplicativos de assinante | Entregar aos perfis que assinaram um aplicativo | nms:appSubscriptionRcp |

Além disso, você pode criar um novo target mapping dependendo das suas necessidades. Esta operação é executada somente a partir do console do cliente. Saiba mais na [documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html#new-mapping){target="_blank"}.
