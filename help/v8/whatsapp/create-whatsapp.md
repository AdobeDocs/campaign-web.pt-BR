---
audience: end-user
title: Criar uma entrega de WhatsApp
description: Saiba como criar um delivery de WhatsApp na interface do usuário da Web do Adobe Campaign
feature: Whatsapp
topic: Content Management
role: User
level: Beginner
exl-id: cac6f675-59e0-431d-8c20-f24ef16d7bf2
hide: true
source-git-commit: aa1a7c48d1708e73e4d6c6bbe4decd2e5ca69102
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 3%

---


# Criar uma mensagem de WhatsApp {#create-whatsapp}

A **interface da Web do Adobe Campaign** permite criar mensagens do WhatsApp que usam modelos aprovados pela Meta, personalizá-las para cada perfil e testá-las antes de enviá-las.


+++ Saiba mais sobre elementos de mensagem e chamadas para ação compatíveis

Os seguintes tipos de mensagem são suportados no WhatsApp:

| Recurso de mensagem | Descrição |
|-|-|
| Cabeçalhos | Texto opcional que aparece acima do corpo da mensagem. |
| Texto | Aceita conteúdo dinâmico por meio de parâmetros. |
| Imagem do cabeçalho | Imagem opcional que aparece acima do corpo da mensagem. |
| Corpo de texto | Aceita conteúdo dinâmico por meio de parâmetros. |
| Texto do rodapé | Aceita conteúdo dinâmico por meio de parâmetros. |

+++


## Criar uma entrega de WhatsApp {#create-whatsapp-journey-campaign}

>[!IMPORTANT]
>
>O feedback de mensagens do WhatsApp não é suportado atualmente.

Na interface do usuário da Web do Adobe Campaign, siga as etapas abaixo para criar uma entrega independente do WhatsApp.

1. Navegue até o menu **[!UICONTROL Entregas]** e clique em **[!UICONTROL Criar entrega]**.

   ![](assets/whatsapp-create-1.png)

1. Escolha **[!UICONTROL WhatsApp]** e selecione um modelo de entrega. [Saiba mais sobre modelos](../msg/delivery-template.md).

   ![](assets/whatsapp-create-2.png)

1. Clique em **[!UICONTROL Criar entrega]** para confirmar.

1. Clique em **[!UICONTROL Configurações]** para obter as opções avançadas vinculadas ao seu modelo. [Saiba mais](../advanced-settings/delivery-settings.md)

   ![](assets/whatsapp-create-3.png)

1. Insira um **[!UICONTROL Rótulo]** para a entrega. Use **[!UICONTROL Opções adicionais]** se precisar de nome interno, pasta, código de entrega, descrição ou natureza, mesmo padrão de outros canais.

1. Clique em **[!UICONTROL Selecionar público-alvo]** para direcionar um público-alvo existente ou criar um. [Saiba mais sobre públicos](../audience/about-recipients.md).

1. Clique em **[!UICONTROL Editar conteúdo]** para abrir o editor de conteúdo do WhatsApp. Consulte [Definir seu conteúdo do WhatsApp](#whatsapp-content)).

   ![](assets/whatsapp-create-4.png)

1. Você pode habilitar **[!UICONTROL Habilitar o agendamento]** para enviar em uma data e hora específicas. [Saiba mais](../msg/gs-deliveries.md#gs-schedule).


## Definir o conteúdo do WhatsApp{#whatsapp-content}

>[!BEGINSHADEBOX]

Antes de criar sua mensagem do WhatsApp na interface da Web do Adobe Campaign, crie e envie seu modelo no Meta. [Saiba mais](https://www.facebook.com/business/help/2055875911147364?id=2129163877102343)

Seu modelo do WhatsApp deve ser aprovado pela Meta antes do uso. A aprovação geralmente leva algumas horas, mas pode levar até 24 horas. [Saiba mais](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/#approval-process)

>[!ENDSHADEBOX]

1. Na página de configuração de entrega da interface da Web do Adobe Campaign, clique em **[!UICONTROL Editar conteúdo]** para configurar a mensagem do WhatsApp.

1. Escolha Marketing como sua **Categoria do modelo**:

   [Saiba mais sobre as categorias de modelo](https://developers.facebook.com/docs/whatsapp/updates-to-pricing/new-template-guidelines/#template-category-guidelines)

   ![](assets/whatsapp-design-1.png)

1. No menu suspenso **Modelo do WhatsApp**, selecione seu modelo aprovado pela Meta.

   [Saiba mais sobre como criar modelos do WhatsApp](https://www.facebook.com/business/help/2055875911147364?id=2129163877102343)

   ![](assets/whatsapp-design-2.png)

1. Se o modelo aprovado pela Meta incluir uma imagem, forneça a **[!UICONTROL URL da imagem]**.

   ![](assets/whatsapp-design-3.png)

1. No campo **espaço reservado para Personalization**, use o editor de personalização para mapear campos e expressões de perfil para os parâmetros do modelo. [Saiba mais](../personalization/personalize.md).

   ![](assets/whatsapp-design-4.png)

Quando a mensagem estiver pronta:

* **Entrega autônoma ou de campanha**: use **[!UICONTROL Revisar e enviar]** e **[!UICONTROL Enviar]** no painel de entrega.

* **Fluxo de trabalho**: abra a entrega da atividade de fluxo de trabalho quando a execução a disponibilizar e use o painel de entrega da mesma maneira. [Saiba mais](../workflows/start-monitor-workflows.md)

Você pode acompanhar os resultados dos **[!UICONTROL Relatórios]** pontos de entrada da entrega e [relatórios da entrega](../reporting/delivery-reports.md).
