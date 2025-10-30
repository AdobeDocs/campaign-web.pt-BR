---
title: Dimensões de filtragem e direcionamento
description: Saiba mais sobre direcionamento e dimensões de filtragem na interface do usuário da Web do Adobe Campaign
exl-id: b910649a-7300-4f99-8f40-3a8965572ee9
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 18%

---

# Dimensões de filtragem e direcionamento {#targeting-dimensions}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Selecione a dimensão de direcionamento"
>abstract="A dimensão de direcionamento permite definir a população alvo da operação: destinatários, beneficiários de contrato, operadores, assinantes, etc. Por padrão, para emails e SMS, o público-alvo é selecionado na tabela integrada Destinatários. Para notificações por push, a dimensão de direcionamento padrão é Aplicativos do assinante."

O targeting dimension, também conhecido como target mapping, é o tipo de dados manipulado por uma operação. Ele define a população direcionada, como perfis, beneficiários de contrato, operadores ou assinantes. A dimensão de filtro permite aplicar filtros ao público-alvo fazendo referência a critérios relacionados sem alterar a dimensão de direcionamento principal.

## Dimensões de direcionamento {#targeting}

O targeting dimension de um fluxo de trabalho é definido pela primeira atividade **[!UICONTROL Build audience]** e é usado em todas as atividades subsequentes até o fim do fluxo de trabalho. Por exemplo, ao consultar perfis do banco de dados, a transição de saída contém dados do tipo &quot;recipient&quot;, que são transmitidos para a próxima atividade.

Alterne a targeting dimension em um fluxo de trabalho usando uma [Atividade Change dimension](../workflows/activities/change-dimension.md). Isso permite consultar o banco de dados em uma tabela específica, como compras ou assinaturas, e alterar o targeting dimension para Recipients para enviar deliveries aos perfis correspondentes.

Ao selecionar uma dimensão de direcionamento (nas configurações do fluxo de trabalho ou em atividades como **Criar público-alvo**, **Reconciliação** ou **Alterar dimensão**), uma lista de esquemas usados com frequência é exibida por padrão. Para mostrar todos os esquemas disponíveis, alterne o botão **[!UICONTROL Mostrar todos os esquemas]**. A seleção da opção é salva para cada usuário.

![Captura de tela mostrando a interface da dimensão de direcionamento com o botão &quot;Mostrar todos os esquemas&quot; habilitado.](assets/targeting-dimension-show-all.png){zoomable="yes"}

Por padrão, modelos de delivery de email e SMS têm como alvo perfis. Sua dimensão de destino usa os campos da tabela **nms:recipient**. Para notificações por push, a dimensão de destino padrão é **Subscriber applications nms:appSubscriptionRcp**, que está vinculada à tabela de destinatários.

Use outros target mappings integrados em workflows e deliveries, conforme listado abaixo:

| Nome | Use para entregar para | Esquema |
|-----------------------|-------------------------------------------------------|-------------------------|
| Destinatários | Perfis/recipients (tabela de recipients integrada) | nms:recipient |
| Visitantes | Visitantes cujos perfis foram coletados por meio de referência (marketing viral, por exemplo) | mns:visitor |
| Assinaturas | Perfis inscritos em um serviço de informação, como um boletim informativo | nms:subscription |
| Assinaturas do visitante | Visitantes inscritos em um serviço de informação | nms:visitorSub |
| Operadores | Operadores do Adobe Campaign | nms:operator |
| Arquivo externo | Entrega por meio de um arquivo contendo todas as informações necessárias | Nenhum esquema vinculado, nenhum target inserido |
| Aplicativos de assinante | Perfis inscritos em um aplicativo | nms:appSubscriptionRcp |

Além disso, crie novos target mappings com base nas necessidades específicas. Execute esta operação somente no console do cliente. Saiba mais na [documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html#new-mapping){target="_blank"}.

## Dimensões de filtro {#filtering}

A dimensão de direcionamento permite definir a população-alvo da operação: destinatários, beneficiários de contrato, operadores, assinantes, etc. A dimensão de filtro permite aplicar filtros a essa população fazendo referência a dados relacionados sem alterar o targeting dimension principal. Por exemplo, você pode selecionar o público com base em critérios específicos, como titulares de contratos ou assinantes de boletins informativos.

As dimensões de filtro estão disponíveis somente na atividade **Compilar Público-alvo**.

Para selecionar clientes que tenham mantido uma apólice de seguro de vida por mais de 5 anos, escolha o seguinte:

* Dimensão de direcionamento: **Clientes**
* Dimensão do filtro: **Titular do contrato**.

Você pode então definir as condições de filtragem na atividade **Criar público-alvo**. Consulte esta [página](../workflows/activities/build-audience.md).

Durante a seleção de targeting dimension, somente as dimensões de filtro compatíveis são exibidas na interface. Essas duas dimensões devem estar relacionadas, de modo que o conteúdo da lista de dimensões do filtro depende do targeting dimension selecionado no primeiro campo.
