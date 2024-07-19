---
audience: end-user
title: Visualizar conteúdo do delivery
description: Saiba como pré-visualizar o conteúdo de delivery com a interface do usuário da Web do Campaign
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
source-git-commit: 81fa26e44739d70218b949712a41a3d520900fa0
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 1%

---


# Visualizar o conteúdo da mensagem {#preview-content}

Use o recurso de simulação de conteúdo do [!DNL Campaign] para visualizar o conteúdo da sua mensagem antes de enviá-la. Isso permite controlar a personalização e verificar como ela é exibida aos recipients.

Para pré-visualizar o conteúdo do delivery, siga as etapas abaixo.

1. Navegue até a tela de edição de conteúdo da sua entrega ou para o [Designer de email](../email/get-started-email-designer.md).

1. Clique no botão **[!UICONTROL Simular conteúdo]**.

   ![](assets/simulate-button.png){zoomable="yes"}

1. Selecione os perfis a serem usados para visualizar seu conteúdo. Para fazer isso, clique no botão **[!UICONTROL Adicionar perfil(is) de teste]** (para email e SMS) ou no botão **[!UICONTROL Adicionar assinante(s)]** (para notificações por push).

1. Você pode combinar perfis e perfis de teste para visualizar sua mensagem de email ou SMS.

   * A guia **[!UICONTROL Perfis de teste]** lista todos os perfis de teste, que são destinatários adicionais e fictícios no banco de dados. [Saiba como trabalhar com perfis de teste](../audience/test-profiles.md)

   * A guia **[!UICONTROL Perfis]** lista todos os perfis armazenados no banco de dados. [Saiba como trabalhar com perfis](../audience/about-recipients.md)

   ![](assets/simulate-select-profiles.png){zoomable="yes"}

1. Ao navegar pelo perfil de teste ou pelas listas de perfis, você pode usar filtros para refinar a pesquisa. Por exemplo, você pode definir uma regra para localizar todos os perfis de teste com o status **[!UICONTROL Prospecto]**. [Saiba como adicionar regras usando o modelador de consultas](../query/query-modeler-overview.md).

   ![](assets/simulate-test-profile-filter.png){zoomable="yes"}

1. Clique em **[!UICONTROL Selecionar]** para confirmar a seleção.

   Uma visualização do conteúdo da entrega é exibida no painel direito da tela **[!UICONTROL Simular]**. Os elementos personalizados são substituídos pelos dados do perfil selecionado no painel esquerdo.

   ![](assets/simulate-preview.png){zoomable="yes"}

1. Se você tiver adicionado vários perfis, é possível alternar entre eles na lista para visualizar o conteúdo do delivery correspondente. Você também pode adicionar mais perfis de teste e limpar a seleção usando os botões correspondentes no painel esquerdo.

1. Para deliveries de email, você pode ajustar o **[!UICONTROL nível de zoom]** e visualizar seu conteúdo no desktop ou dispositivo móvel usando o ícone dedicado no canto superior direito.

1. Na tela **[!UICONTROL Simular]**, também é possível:
   * Enviar provas a destinatários específicos para validação - [Saiba mais](test-deliveries.md)
   * Acessar os logs das provas enviadas - [Saiba mais](test-deliveries.md#access-test-deliveries)
   * Somente para email, verifique a renderização do conteúdo da mensagem em clientes de email populares - [Saiba mais](email-rendering.md)



