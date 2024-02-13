---
audience: end-user
title: Gerenciar ativos com o Adobe Experience Manager as a Cloud Service
description: Saiba como gerenciar conteúdo com o Adobe Experience Manager as a Cloud Service
badge: label="Disponibilidade limitada"
source-git-commit: 6fd2fa72e482883802c96f0888ea79f2b16b7152
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 3%

---

# Gerenciar modelos com [!DNL Adobe Experience Manager as a Cloud service]{#aem-assets}

## Introdução ao [!DNL Adobe Experience Manager as a Cloud service]{#create-aem}

A integração da interface da Web do Adobe Campaign com o Adobe Experience Manager facilita o gerenciamento simplificado de conteúdo de delivery de email e formulários diretamente na plataforma do Adobe Experience Manager.

![](assets/do-not-localize/book.png)[Saiba mais sobre o Adobe Experience Manager as a Cloud Service](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/sites/authoring/getting-started/quick-start.html?lang=en)

## Criar um modelo no [!DNL Adobe Experience Manager as a Cloud service]{#create-aem-template}

1. Navegue até o [!DNL Adobe Experience Manager] instância do autor e clique em Experiência Adobe no canto superior esquerdo da página. Escolher **[!UICONTROL Sites]** no menu.

1. Access **[!UICONTROL Campanhas > Nome da sua marca > Área principal > Nome da sua página]**.

1. Clique em **[!UICONTROL Criar]** e selecione **[!UICONTROL Página]** no menu suspenso.

   ![](assets/aem_1.png)

1. Selecione o **[!UICONTROL Email do Adobe Campaign]** Crie um modelo e nomeie o informativo.

   ![](assets/aem_2.png)

1. Personalize seu conteúdo de email adicionando componentes, como campos de personalização do Adobe Campaign. [Saiba mais](https://experienceleague.adobe.com/docs/experience-manager-65/content/sites/authoring/aem-adobe-campaign/campaign.html?lang=en#editing-email-content)

1. Quando o email estiver pronto, navegue até o **[!UICONTROL Informações da página]** e clique em **[!UICONTROL Iniciar fluxo de trabalho]**.

   ![](assets/aem_3.png)

1. Na primeira lista suspensa, selecione **[!UICONTROL Aprovar o Adobe Campaign]** como modelo de workflow e clique em **[!UICONTROL Iniciar fluxo de trabalho]**.

1. Um aviso de isenção de responsabilidade será exibido na parte superior da página informando: `This page is subject to the workflow Approve for Adobe Campaign`. Clique em **[!UICONTROL Concluído]** ao lado do aviso para confirmar a revisão e clique em **[!UICONTROL Ok]**.

   ![](assets/aem_4.png)

1. Clique em **[!UICONTROL Concluído]** novamente e selecione **[!UICONTROL Aprovação de informativo]** no **[!UICONTROL Próxima etapa]** menu suspenso.

Seu boletim informativo agora está pronto e sincronizado no Adobe Campaign.

## Importar um modelo do Adobe Experience Manager as a Cloud Service{#aem-templates-perso}

Quando o template de Experience Manager estiver disponível na Adobe Campaign Web como um template de conteúdo, você poderá identificar e incorporar o conteúdo necessário para o email, incluindo personalização.

1. No Campaign Web, a partir da **[!UICONTROL Entregas]** clique em **[!UICONTROL Criar entrega]**.

1. Na janela de modelo de email, selecione a caixa de diálogo incorporada **[!UICONTROL Entrega de email com conteúdo AEM]** modelo.

   ![](assets/aem_5.png)

1. Insira um **[!UICONTROL Rótulo]** para o delivery e configure opções adicionais com base nas suas necessidades:

   * **[!UICONTROL Nome interno]**: atribua um identificador exclusivo ao delivery.

   * **[!UICONTROL Pasta]**: armazene o delivery em uma pasta específica.

   * **[!UICONTROL Código de entrega]**: use esse campo para organizar seus deliveries com base em sua própria convenção de nomenclatura.

   * **[!UICONTROL Descrição]**: especifique uma descrição para o delivery.

   * **[!UICONTROL Natureza]**: especifique a natureza do email para fins de classificação.

1. Definir um **[!UICONTROL Público]** ao seu email. [Saiba mais](../email/create-email.md#define-audience)

1. Clique em **[!UICONTROL Editar conteúdo]**.

1. No **[!UICONTROL Editar conteúdo]** clique em **[!UICONTROL Selecionar conteúdo AEM]**.

   ![](assets/aem_6.png)

1. Navegue pelo modelo do AEM e selecione aquele que será importado para o Campaign Web.

   ![](assets/aem_8.png)

1. Se forem feitas alterações nos modelos diretamente no Adobe Experience Manager, basta selecionar **[!UICONTROL Atualizar conteúdo AEM]** para ter a versão mais recente do modelo.

1. Para remover a vinculação entre o Experience Manager e o Campaign ou personalizar ainda mais seu modelo de Experience Manager no Designer de email, clique em **[!UICONTROL Desvincular conteúdo AEM]**.

   ![](assets/aem_9.png)

1. Se você adicionou conteúdo personalizado ao seu modelo de Experience Manager, clique em **[!UICONTROL Simular conteúdo]** para visualizar como ele aparecerá na mensagem usando perfis de teste.

[Saiba mais sobre perfis de pré-visualização e teste](../preview-test/preview-content.md)

1. Ao visualizar a pré-visualização da mensagem, todos os elementos personalizados são substituídos automaticamente pelos dados correspondentes do perfil de teste selecionado.

   Se necessário, perfis de teste adicionais podem ser adicionados por meio do **[!UICONTROL Gerenciar perfis de teste]** botão.

Seu delivery está pronto para ser enviado.
