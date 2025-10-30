---
audience: end-user
title: Gerenciar ativos com o Adobe Experience Manager as a Cloud Service
description: Saiba como gerenciar conteúdo com o Adobe Experience Manager as a Cloud Service
exl-id: 43b186c8-294e-4cbe-b269-e127065515ed
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 5%

---

# Gerenciar modelos com [!DNL Adobe Experience Manager as a Cloud Service]{#aem-assets}

## Introdução ao [!DNL Adobe Experience Manager as a Cloud Service]{#create-aem}

A integração da interface da Web do Adobe Campaign com o Adobe Experience Manager permite o gerenciamento simplificado de conteúdo e formulários de delivery de email diretamente na plataforma do Adobe Experience Manager.

![](assets/do-not-localize/book.png) [Saiba mais sobre o Adobe Experience Manager as a Cloud Service](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/sites/authoring/getting-started/quick-start.html?lang=en)

## Criar um modelo em [!DNL Adobe Experience Manager as a Cloud Service]{#create-aem-template}

1. Navegue até a instância de autor do [!DNL Adobe Experience Manager] e clique em Adobe Experience no canto superior esquerdo da página. Escolha **[!UICONTROL Sites]** no menu.

1. Acesse **[!UICONTROL Campanhas > Nome da sua marca > Área principal > Nome da sua página]**.

1. Clique em **[!UICONTROL Criar]** e selecione **[!UICONTROL Página]** no menu suspenso.

   ![Captura de tela mostrando o botão &quot;Criar&quot; e a opção &quot;Página&quot; no menu suspenso.](assets/aem_1.png)

1. Selecione o modelo do **[!UICONTROL Email do Adobe Campaign]** e nomeie o informativo.

   ![[Captura de tela mostrando a seleção de modelo e o campo de nomenclatura do &quot;Email do Adobe Campaign&quot;.]](assets/aem_2.png)

1. Personalize seu conteúdo de email adicionando componentes, como campos de personalização do Adobe Campaign. [Saiba mais](https://experienceleague.adobe.com/docs/experience-manager-65/content/sites/authoring/aem-adobe-campaign/campaign.html?lang=en#editing-email-content)

1. Com o email pronto, navegue até o menu **[!UICONTROL Informações da página]** e clique em **[!UICONTROL Iniciar fluxo de trabalho]**.

   ![Captura de tela mostrando o menu &quot;Informações da página&quot; e a opção &quot;Iniciar fluxo de trabalho&quot;.](assets/aem_3.png)

1. Na primeira lista suspensa, selecione **[!UICONTROL Aprovar Adobe Campaign]** como modelo de fluxo de trabalho e clique em **[!UICONTROL Iniciar fluxo de trabalho]**.

1. Um aviso de isenção de responsabilidade será exibido na parte superior da página informando, `This page is subject to the workflow Approve for Adobe Campaign`. Clique em **[!UICONTROL Concluído]** ao lado do aviso de isenção de responsabilidade para confirmar a revisão e clique em **[!UICONTROL Ok]**.

   ![Captura de tela mostrando o aviso de isenção de responsabilidade e o botão &quot;Concluído&quot;.](assets/aem_4.png)

1. Clique novamente em **[!UICONTROL Concluir]** e selecione **[!UICONTROL Aprovação de informativo]** na lista suspensa **[!UICONTROL Próxima etapa]**.

Seu boletim informativo agora está pronto e sincronizado no Adobe Campaign.

## Importar um modelo do Adobe Experience Manager as a Cloud Service{#aem-templates-perso}

Quando o template do Experience Manager estiver disponível na Adobe Campaign Web como um template de conteúdo, você poderá identificar e incorporar o conteúdo necessário para o email, incluindo personalização.

1. Na Web do Campaign, no menu **[!UICONTROL Deliveries]**, clique em **[!UICONTROL Criar delivery]**.

1. Na janela de modelo de email, selecione o modelo interno **[!UICONTROL Entrega de email com conteúdo do AEM]**.

   ![Captura de tela mostrando a seleção do modelo &quot;Entrega de email com conteúdo do AEM&quot;.](assets/aem_5.png)

1. Insira um **[!UICONTROL Rótulo]** para a entrega e configure opções adicionais com base nas suas necessidades:

   * **[!UICONTROL Nome interno]**: atribua um identificador exclusivo à entrega.
   * **[!UICONTROL Pasta]**: armazene a entrega em uma pasta específica.
   * **[!UICONTROL Código de entrega]**: use este campo para organizar suas entregas com base em sua própria convenção de nomenclatura.
   * **[!UICONTROL Descrição]**: especifique uma descrição para a entrega.
   * **[!UICONTROL Natureza]**: especifique a natureza do email para fins de classificação.

1. Defina um **[!UICONTROL Público-alvo]** para seu email. [Saiba mais](../email/create-email.md#define-audience)

1. Clique em **[!UICONTROL Editar conteúdo]**.

1. No menu **[!UICONTROL Editar conteúdo]**, clique em **[!UICONTROL Selecionar conteúdo do AEM]**.

   ![Captura de tela mostrando a opção &quot;Selecionar conteúdo do AEM&quot; no menu &quot;Editar conteúdo&quot;.](assets/aem_6.png)

1. Navegue pelo modelo do AEM e selecione aquele que será importado para o Campaign Web.

   ![Captura de tela mostrando a interface de seleção de modelo do AEM.](assets/aem_8.png)

1. Observe que o conteúdo não é sincronizado automaticamente. Se forem feitas alterações nos modelos diretamente no Adobe Experience Manager, selecione **[!UICONTROL Atualizar conteúdo do AEM]** para atualizar para a versão mais recente do modelo.

1. Para remover a vinculação entre o Experience Manager e o Campaign, ou para personalizar ainda mais seu modelo do Experience Manager no Designer de email, clique em **[!UICONTROL Desvincular conteúdo do AEM]**.

   ![Captura de tela mostrando a opção &quot;Desvincular conteúdo do AEM&quot;.](assets/aem_9.png)

1. Se você adicionou conteúdo personalizado ao seu modelo do Experience Manager, clique em **[!UICONTROL Simular conteúdo]** para visualizar como ele aparecerá na mensagem usando perfis de teste.

[Saiba mais sobre perfis de visualização e teste](../preview-test/preview-content.md)

1. Ao visualizar a pré-visualização da mensagem, todos os elementos personalizados são substituídos automaticamente pelos dados correspondentes do perfil de teste selecionado.

   Se necessário, adicione perfis de teste adicionais através do botão **[!UICONTROL Gerenciar perfis de teste]**.

Seu delivery está pronto para ser enviado.