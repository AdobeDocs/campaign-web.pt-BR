---
title: Introdução a perfis e públicos
description: Saiba como trabalhar com perfis e públicos no Campaign Web
exl-id: 71a1ec92-cd79-4654-9ae3-9a92a01c6279
badge: label="Disponibilidade limitada"
source-git-commit: 9e6f0a5894ae0b31d275f978553d7fc73ba9c2eb
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 18%

---

# Introdução a perfis e públicos {#about-profiles}

## Perfis e públicos {#about}

No Adobe Campaign, a população alvo de uma entrega é um público-alvo. Um público-alvo é um conjunto de perfis que compartilham comportamentos e/ou características semelhantes. Esta coleção de pessoas pode ser gerada, selecionada ou carregada [conforme detalhado abaixo](#audiences).

## Dimensões de direcionamento {#targeting-dimensions}

Targeting dimension, também conhecido como. target mapping, é o tipo de dados que uma operação está tratando. Ele permite definir a população direcionada: perfis, beneficiários de contrato, operadores, assinantes etc.

O targeting dimension de um workflow é definido pelo primeiro **[!UICONTROL Criar público-alvo]** e é usada em todas as outras atividades até o fim do workflow. Por exemplo, se você realizar um query nos perfis do banco de dados, a transição de saída conterá dados do tipo &quot;recipient&quot; e será transmitida para a próxima atividade.

Observe que é possível alternar o targeting dimension em um workflow usando um [Alterar atividade da dimensão](../workflows/activities/change-dimension.md). Isso permite, por exemplo, consultar o banco de dados em uma tabela específica, como compras ou assinaturas, e alterar o targeting dimension para Recipients para enviar deliveries aos perfis correspondentes.

Por padrão, modelos de delivery de email e SMS têm como alvo perfis. O target dimension, portanto, usa os campos da variável **nms:recipient** tabela. Para notificações por push, a dimensão de destino padrão é **Aplicativos de assinante nms:appSubscriptionRcp**, que está vinculado à tabela de recipients.

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
