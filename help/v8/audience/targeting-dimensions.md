---
title: Dimensões de direcionamento
description: Saiba mais sobre dimensões de direcionamento no Adobe Campaign Web
exl-id: b910649a-7300-4f99-8f40-3a8965572ee9
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 18%

---

# Dimensões de direcionamento {#targeting-dimensions}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Selecione o targeting dimension"
>abstract="A dimensão de direcionamento permite definir a população-alvo da operação: destinatários, beneficiários de contrato, operadores, assinantes, etc. Por padrão, para emails e SMS, o target é selecionado na tabela integrada Recipients. Para notificações por push, o target dimension padrão é Aplicativos do assinante."

Targeting dimension, também conhecido como. target mapping, é o tipo de dados que uma operação está tratando. Ele permite definir a população direcionada: perfis, beneficiários de contrato, operadores, assinantes etc.

## Dimensões de direcionamento de workflows {#workflow}

O targeting dimension de um workflow é definido pelo primeiro **[!UICONTROL Criar público-alvo]** e é usada em todas as outras atividades até o fim do workflow. Por exemplo, se você realizar um query nos perfis do banco de dados, a transição de saída conterá dados do tipo &quot;recipient&quot; e será transmitida para a próxima atividade.

Observe que é possível alternar o targeting dimension em um workflow usando um [Alterar atividade da dimensão](../workflows/activities/change-dimension.md). Isso permite, por exemplo, consultar o banco de dados em uma tabela específica, como compras ou assinaturas, e alterar o targeting dimension para Recipients para enviar deliveries aos perfis correspondentes.

Ao selecionar um targeting dimension (nas configurações do fluxo de trabalho ou em atividades como **Criar público-alvo**, **Reconciliação** ou **Alterar dimensão**), uma seleção de esquemas usados com frequência é exibida por padrão na lista. Para mostrar todos os esquemas disponíveis, alterne no **[!UICONTROL Mostrar todos os esquemas]** botão. A seleção da opção é salva para cada usuário.

![](assets/targeting-dimension-show-all.png){zoomable=&quot;yes&quot;}

## Dimensões de direcionamento {#list}

Por padrão, modelos de delivery de email e SMS têm como alvo perfis. O target dimension, portanto, usa os campos da variável **nms:recipient** tabela. Para notificações por push, a dimensão de destino padrão é **Aplicativos de assinante nms:appSubscriptionRcp**, que está vinculado à tabela de recipients.

Você também pode usar outros target mappings integrados nos workflows e deliveries listados abaixo:

| Nome | Use para | Esquema |
|---|---|---|
| Recipients | Delivery para perfis/recipients (tabela de recipients integrada) | nms:recipient |
| Visitantes | Enviar delivery aos visitantes cujos perfis foram coletados por meio de referência (marketing viral), por exemplo. | mns:visitor |
| Subscrições | Enviar delivery aos perfis que assinam um serviço de informação, como um boletim informativo | nms:subscription |
| Assinaturas do visitante | Entregar aos visitantes que são inscritos em um serviço de informações | nms:visitorSub |
| Operadores | Entregar aos operadores do Adobe Campaign | nms:operator |
| Arquivo externo | Entregar por meio de um arquivo que contenha todas as informações necessárias para a entrega | Nenhum schema vinculado, nenhum target inserido |
| Aplicativos de assinante | Entregar aos perfis que assinaram um aplicativo | nms:appSubscriptionRcp |

Além disso, você pode criar um novo target mapping dependendo das suas necessidades. Esta operação é executada somente a partir do console do cliente. Saiba mais em [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html#new-mapping){target="_blank"}.
