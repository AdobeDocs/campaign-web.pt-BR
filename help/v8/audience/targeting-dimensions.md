---
title: Dimensões de direcionamento
description: Saiba mais sobre dimensões de direcionamento no Adobe Campaign Web
exl-id: b910649a-7300-4f99-8f40-3a8965572ee9
source-git-commit: 93a79b471c236e5bf67da0dbd0d76274598dcb0e
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 15%

---

# Dimensões de direcionamento {#targeting-dimensions}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Selecione a dimensão de direcionamento"
>abstract="O targeting dimension permite definir o público alvo da operação: recipients, beneficiários de contrato, operadores, assinantes e muito mais. Por padrão, para emails e SMS, o público-alvo é selecionado na tabela integrada Destinatários. Para notificações por push, a dimensão de direcionamento padrão é Aplicativos do assinante."

O targeting dimension, também conhecido como target mapping, é o tipo de dados manipulado por uma operação. Ele define a população direcionada, como perfis, beneficiários de contrato, operadores ou assinantes.

## Dimensões de direcionamento de workflows {#workflow}

O targeting dimension de um fluxo de trabalho é definido pela primeira atividade **[!UICONTROL Build audience]** e é usado em todas as atividades subsequentes até o fim do fluxo de trabalho. Por exemplo, ao consultar perfis do banco de dados, a transição de saída contém dados do tipo &quot;recipient&quot;, que são transmitidos para a próxima atividade.

Alterne a targeting dimension em um fluxo de trabalho usando uma [Atividade Change dimension](../workflows/activities/change-dimension.md). Isso permite consultar o banco de dados em uma tabela específica, como compras ou assinaturas, e alterar o targeting dimension para Recipients para enviar deliveries aos perfis correspondentes.

Ao selecionar uma dimensão de direcionamento (nas configurações do fluxo de trabalho ou em atividades como **Criar público-alvo**, **Reconciliação** ou **Alterar dimensão**), uma lista de esquemas usados com frequência é exibida por padrão. Para mostrar todos os esquemas disponíveis, alterne o botão **[!UICONTROL Mostrar todos os esquemas]**. A seleção da opção é salva para cada usuário.

![Captura de tela mostrando a interface da dimensão de direcionamento com o botão &quot;Mostrar todos os esquemas&quot; habilitado.](assets/targeting-dimension-show-all.png){zoomable="yes"}

## Dimensões de direcionamento {#list}

Por padrão, modelos de delivery de email e SMS têm como alvo perfis. Sua dimensão de destino usa os campos da tabela **nms:recipient**. Para notificações por push, a dimensão de destino padrão é **Subscriber applications nms:appSubscriptionRcp**, que está vinculada à tabela de destinatários.

Use outros target mappings integrados em workflows e deliveries, conforme listado abaixo:

| Nome | Use para entregar para | Esquema |
|-----------------------|-------------------------------------------------------|-------------------------|
| Destinatários | Perfis/recipients (tabela de recipients integrada) | nms:recipient |
| Visitantes | Visitantes cujos perfis foram coletados por meio de referência (marketing viral, por exemplo) | mns:visitor |
| Subscrições | Perfis inscritos em um serviço de informação, como um boletim informativo | nms:subscription |
| Assinaturas do visitante | Visitantes inscritos em um serviço de informação | nms:visitorSub |
| Operadores | Operadores do Adobe Campaign | nms:operator |
| Arquivo externo | Entrega por meio de um arquivo contendo todas as informações necessárias | Nenhum schema vinculado, nenhum target inserido |
| Aplicativos de assinante | Perfis inscritos em um aplicativo | nms:appSubscriptionRcp |

Além disso, crie novos target mappings com base nas necessidades específicas. Execute esta operação somente no console do cliente. Saiba mais na [documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=pt-BR#new-mapping){target="_blank"}.