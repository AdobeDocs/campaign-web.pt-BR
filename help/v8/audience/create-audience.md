---
audience: end-user
title: Criar públicos
description: Saiba como criar públicos-alvo no Adobe Campaign Web
badge: label="Beta"
source-git-commit: 44a280446f9e7f801607dd40326b56fd79ec34e9
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 1%

---


# Criar públicos {#create-audiences}

O Campaign Web permite criar fluxos de trabalho em que você pode combinar públicos existentes em uma tela visual e aproveitar várias atividades (dividir, excluir...) para criar novos públicos.

Depois de concluído, os públicos-alvo resultantes são salvos na Web do Campaign junto com os públicos-alvo existentes e podem ser aproveitados em entregas ou campanhas independentes para segmentar os indivíduos.

## Criar seu primeiro público-alvo {#create}

Para criar um público-alvo, siga estas etapas:

1. Navegue até a **[!UICONTROL Públicos-alvo]** e clique em **[!UICONTROL Criar público-alvo]** no canto superior direito.
1. Forneça um rótulo para o público.
1. Expanda a seção Opções adicionais para configurar parâmetros do Advancer para o público-alvo.

   >[!NOTE]
   >
   >Por padrão, os públicos-alvo são criados no menu do explorador Perfis e Destinos/Listas. É possível alterar o local de armazenamento padrão no **[!UICONTROL Pasta]** campo.

1. Depois que as configurações de público forem definidas, clique em **[!UICONTROL Criar público-alvo]** botão.

1. Uma tela de workflow é exibida, com duas atividades padrão:

   * **[!UICONTROL Criar público-alvo]**: o ponto de partida do fluxo de trabalho. Essa atividade permite selecionar um ou vários públicos-alvo como base para o fluxo de trabalho,
   * **[!UICONTROL Salvar público-alvo]**: a última etapa do fluxo de trabalho. Essa atividade permite salvar o resultado do fluxo de trabalho em um novo público-alvo.

1. Configure seu workflow adicionando quantas atividades forem necessárias. Para obter mais informações sobre como configurar as várias atividades, consulte o [documentação de workflows](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >As atividades de canal não estão disponíveis para uso em fluxos de trabalho de público.

   ![](assets/audience-creation-canvas.png)

1. Quando o workflow estiver pronto, clique em **[!UICONTROL Início]** para executá-lo.

1. O workflow é salvo na variável **[!UICONTROL Fluxos de trabalho]** e o(s) público(s) resultante(s) na **[!UICONTROL Públicos-alvo]** lista. [Saiba como acessar públicos](access-audiences.md)
