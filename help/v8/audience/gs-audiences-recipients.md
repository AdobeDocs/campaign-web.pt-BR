---
title: Trabalhar com destinatários e públicos-alvo
description: Saiba como trabalhar com recipients e públicos no Campaign Web
badge: label="Beta"
exl-id: 71a1ec92-cd79-4654-9ae3-9a92a01c6279
source-git-commit: 5183dd0045c7f13e79f65eca5b31dfd4cde2f31d
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 18%

---

# Trabalhar com destinatários e públicos-alvo {#about-recipients}

## Destinatários e públicos {#about}

No Adobe Campaign, a população alvo de uma entrega é um público-alvo. Um público-alvo é um conjunto de pessoas que compartilham comportamentos e/ou características semelhantes. Esta coleção de pessoas pode ser gerada, selecionada ou carregada [conforme detalhado abaixo](#audiences).

Na maioria dos casos comuns, o público-alvo é composto de perfis, que são armazenados como [recipients](#recipients) no Adobe Campaign. Também é possível trabalhar com outros target mappings alterando a dimensão conforme explicado [nesta seção](#targeting-dimensions).

## Dimensões de direcionamento {#targeting-dimensions}

Targeting dimension, também conhecido como. target mapping, é o tipo de dados que uma operação está tratando. Ele permite definir a população direcionada: recipients, beneficiários de contrato, operadores, assinantes etc.

O targeting dimension de um workflow é definido pelo primeiro **[!UICONTROL Criar público-alvo]** e é usada em todas as outras atividades até o fim do workflow. Por exemplo, se você realizar um query nos recipients do banco de dados, a transição de saída conterá dados do tipo recipient e será transmitida para a próxima atividade.

Observe que é possível alternar o targeting dimension em um workflow usando um [Alterar atividade da dimensão](../workflows/activities/change-dimension.md). Isso permite, por exemplo, consultar o banco de dados em uma tabela específica, como compras ou assinaturas, e alterar o targeting dimension para Recipients para enviar deliveries aos recipients correspondentes.

Por padrão, templates de delivery de email e SMS têm como target **[!UICONTROL Destinatários]**. O target dimension, portanto, usa os campos da variável **nms:recipient** tabela. Para notificações por push, a dimensão de destino padrão é **Aplicativos de assinante nms:appSubscriptionRcp**, que está vinculado à tabela de recipients.

Você também pode usar outros target mappings integrados nos workflows e deliveries listados abaixo:

| Nome | Use para | Esquema |
|---|---|---|
| Recipients | Entregar aos destinatários (tabela de destinatários integrada) | nms:recipient |
| Visitantes | Enviar delivery aos visitantes cujos perfis foram coletados por meio de referência (marketing viral), por exemplo. | mns:visitor |
| Subscrições | Entregar aos recipients que assinam um serviço de informações, como um boletim informativo | nms:subscription |
| Assinaturas do visitante | Entregar aos visitantes que são inscritos em um serviço de informações | nms:visitorSub |
| Operadores | Entregar aos operadores do Adobe Campaign | nms:operator |
| Arquivo externo | Entregar por meio de um arquivo que contenha todas as informações necessárias para a entrega | Nenhum schema vinculado, nenhum target inserido |
| Aplicativos de assinante | Enviar delivery aos recipients que assinaram um aplicativo | nms:appSubscriptionRcp |

Além disso, você pode criar um novo target mapping dependendo das suas necessidades. Isso é executado no console do cliente. Saiba mais em [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html#new-mapping){target="_blank"}.
