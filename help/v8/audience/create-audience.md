---
audience: end-user
title: Criar públicos
description: Saiba como criar públicos-alvo no Adobe Campaign Web
badge: label="Beta"
source-git-commit: 4b005f3feb70b8c5cf0f4cd9c5ba54547bd9261a
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 2%

---


# Criar públicos {#create-audiences}


>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Configurações do público-alvo"
>abstract="Insira o nome do público-alvo e as opções adicionais."

O Campaign Web permite criar fluxos de trabalho em que você pode combinar públicos existentes em uma tela visual. Ao incorporar várias atividades de workflow, como **Split** ou **Excluir**, você pode gerar públicos-alvo novos e refinados.

Depois de criar o fluxo de trabalho, os públicos resultantes são automaticamente armazenados no Campaign Web junto com os existentes. Esses públicos-alvo podem ser direcionados em campanhas ou deliveries independentes.

Para criar um público-alvo, siga estas etapas:

1. Navegue até a **[!UICONTROL Públicos-alvo]** e clique no botão **[!UICONTROL Criar público-alvo]** localizado no canto superior direito.
1. Forneça um rótulo para o público.
1. Expanda a **[!UICONTROL Opções adicionais]** seção para configurar parâmetros avançados de público-alvo.

   Por padrão, os públicos-alvo são criados na **[!UICONTROL Perfis e públicos alvo]** / **[!UICONTROL Listas]** menu do explorador. É possível alterar o local de armazenamento padrão usando o **[!UICONTROL Pasta]** campo.

   ![](assets/audiences-settings.png)

1. Depois de definir as configurações de público-alvo, clique no **[!UICONTROL Criar público-alvo]** botão.

1. Uma tela de workflow é exibida, apresentando duas atividades padrão:

   * **[!UICONTROL Criar público-alvo]**: este é o ponto de partida do fluxo de trabalho, permitindo criar um público-alvo e usá-lo como base para ele.
   * **[!UICONTROL Salvar público-alvo]**: representa a etapa final do fluxo de trabalho, permitindo salvar os resultados como um novo público-alvo.

1. Personalize o fluxo de trabalho adicionando quantas atividades forem necessárias. Para obter mais informações sobre como configurar atividades de workflow, consulte [documentação de workflows](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >As atividades de canal não estão disponíveis para uso em fluxos de trabalho de público.

   ![](assets/audience-creation-canvas.png)

1. Quando o workflow estiver pronto, clique em **[!UICONTROL Início]** para executá-lo.

1. O workflow é salvo na variável **[!UICONTROL Fluxos de trabalho]** lista, enquanto os públicos resultantes estão acessíveis na **[!UICONTROL Públicos-alvo]** lista. [Saiba como monitorar e gerenciar públicos](access-audiences.md)
