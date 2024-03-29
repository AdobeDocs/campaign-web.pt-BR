---
audience: end-user
title: Visualizar conteúdo do delivery
description: Saiba como pré-visualizar o conteúdo de delivery com a interface do usuário da Web do Campaign
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
source-git-commit: 81fa26e44739d70218b949712a41a3d520900fa0
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 3%

---


# Visualizar o conteúdo da mensagem {#preview-content}

Use o [!DNL Campaign] recurso de simulação de conteúdo para pré-visualizar o conteúdo da mensagem antes de enviá-la. Isso permite controlar a personalização e verificar como ela é exibida aos recipients.

Para pré-visualizar o conteúdo do delivery, siga as etapas abaixo.

1. Navegue até a tela de edição de conteúdo do seu delivery ou até [Email Designer](../email/get-started-email-designer.md).

1. Clique em **[!UICONTROL Simular conteúdo]** botão.

   ![](assets/simulate-button.png){zoomable=&quot;yes&quot;}

1. Selecione os perfis a serem usados para visualizar seu conteúdo. Para fazer isso, clique no link **[!UICONTROL Adicionar perfil(s) de teste]** (para email e SMS) ou o botão **[!UICONTROL Adicionar assinante(s)]** (para notificações por push).

1. Você pode combinar perfis e perfis de teste para visualizar sua mensagem de email ou SMS.

   * A variável **[!UICONTROL Perfis de teste]** A guia lista todos os perfis de teste, que são destinatários adicionais e fictícios no banco de dados. [Saiba como trabalhar com perfis de teste](../audience/test-profiles.md)

   * A variável **[!UICONTROL Perfis]** A guia lista todos os perfis armazenados no banco de dados. [Saiba como trabalhar com perfis](../audience/about-recipients.md)

   ![](assets/simulate-select-profiles.png){zoomable=&quot;yes&quot;}

1. Ao navegar pelo perfil de teste ou pelas listas de perfis, você pode usar filtros para refinar a pesquisa. Por exemplo, é possível definir uma regra para localizar todos os perfis de teste com **[!UICONTROL Cliente Potencial]** status. [Saiba como adicionar regras usando o modelador de consultas](../query/query-modeler-overview.md).

   ![](assets/simulate-test-profile-filter.png){zoomable=&quot;yes&quot;}

1. Clique em **[!UICONTROL Selecionar]** para confirmar a seleção.

   Uma pré-visualização do conteúdo do delivery é exibida no painel direito do **[!UICONTROL Simular]** tela. Os elementos personalizados são substituídos pelos dados do perfil selecionado no painel esquerdo.

   ![](assets/simulate-preview.png){zoomable=&quot;yes&quot;}

1. Se você tiver adicionado vários perfis, é possível alternar entre eles na lista para visualizar o conteúdo do delivery correspondente. Você também pode adicionar mais perfis de teste e limpar a seleção usando os botões correspondentes no painel esquerdo.

1. Para deliveries de email, você pode ajustar a variável **[!UICONTROL Nível de zoom]** e visualize seu conteúdo no desktop ou dispositivo móvel usando o ícone dedicado no canto superior direito.

1. No **[!UICONTROL Simular]** também é possível:
   * Enviar provas para destinatários específicos para validação - [Saiba mais](test-deliveries.md)
   * Acessar os logs das provas enviadas - [Saiba mais](test-deliveries.md#access-test-deliveries)
   * Somente para email, verifique a renderização do conteúdo da mensagem em clientes de email populares - [Saiba mais](email-rendering.md)



