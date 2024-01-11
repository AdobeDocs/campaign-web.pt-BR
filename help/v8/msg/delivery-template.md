---
product: campaign
title: Usar modelos de entrega
description: Saiba como criar e usar modelos de entrega no Campaign Web
feature: Email, Push, SMS, Direct Mail, Cross Channel Orchestration
role: User
level: Beginner
badge: label="Disponibilidade limitada"
exl-id: cd3d4c2d-7bb2-4574-aeb8-6aac0683ec59
source-git-commit: f8f29849bbd3e97b4168a0bac175a3cdc3e651df
workflow-type: tm+mt
source-wordcount: '1087'
ht-degree: 17%

---

# Usar modelos de entrega {#work-with-delivery-templates}

>[!CONTEXTUALHELP]
>id="acw_delivery_template_for_campaign"
>title="Modelos de entrega"
>abstract="Para um processo de design acelerado e aprimorado, você pode criar templates do delivery para reutilizar facilmente o conteúdo e as configurações personalizadas em suas campanhas. Essa funcionalidade permite padronizar a aparência criativa para ser mais rápido na execução e na inicialização de campanhas."

Para um processo de design acelerado e aprimorado, você pode criar templates do delivery para reutilizar facilmente o conteúdo e as configurações personalizadas em suas campanhas. Essa funcionalidade permite padronizar a aparência criativa para ser mais rápido na execução e na inicialização de campanhas.

Um modelo pode incluir:

* A variável **pasta** e **pasta de execução** do modelo. A pasta é o local onde o template do delivery é salvo. A pasta de execução é a pasta onde os deliveries criados com base nesse template são salvos.
* [Tipologias](../advanced-settings/delivery-settings.md#typology),
* O endereço do remetente,
* Um [público](../audience/about-recipients.md), incluindo [grupos de controle](../audience/control-group.md),
* Personalizado [conteúdo](../email/edit-content.md),
* [Campos personalizados](../personalization/personalize.md) e [conteúdo condicional](../personalization/conditions.md),
* Links para [mirror page](../email/mirror-page.md) e cancelar assinatura [links](../email/message-tracking.md),
* Outras propriedades de entrega, como validade de recurso, parâmetros de nova tentativa ou configurações de quarentena.

>[!NOTE]
>
>Os modelos de entrega são diferentes de [modelos de conteúdo](../email/create-email-templates.md), que permitem reutilizar apenas o conteúdo de seus emails e começar a criar conteúdo com um dos modelos de email de amostra fornecidos prontos para uso.


## Acessar e gerenciar modelos de entrega {#access-manage-templates}

>[!CONTEXTUALHELP]
>id="acw_delivery_templates"
>title="Trabalho com modelos de entrega"
>abstract="Use modelos de entrega para criar e salvar configurações de entrega para uso futuro em suas campanhas. É possível criar modelos de entrega do zero, duplicar um modelo já existente ou converter uma entrega em um modelo."


Para acessar a lista de modelos de conteúdo, selecione **[!UICONTROL Campaign Management]** > **[!UICONTROL Entregas]** no menu esquerdo e navegue até a janela **Modelos** guia.

![](assets/templates-tab.png)

Todos os modelos que foram [criado](#create-a-delivery-template) no ambiente atual são exibidas.

É possível filtrar modelos de conteúdo em canais e pastas. Você também pode definir filtros avançados criando uma regra usando atributos de delivery. [Saiba mais sobre o modelador de consultas](../audience/../query/query-modeler-overview.md)

![](assets/templates-filters.png)

Para editar um modelo, clique no item desejado na lista. A partir daí:

* Você pode modificar o conteúdo, as propriedades, o público-alvo e qualquer oferta anexada a ele.
* Você também pode testar seu template. [Saiba mais](#test-template)

![](assets/templates-edition.png)

Para excluir ou [duplicado](#copy-an-existing-template) um modelo, selecione a ação correspondente no campo **[!UICONTROL Mais ações]** menu, no menu **[!UICONTROL Modelos]** ou em uma tela de edição de modelo.

![](assets/templates-more-actions.png)

>[!NOTE]
>
>Quando um template é editado ou excluído, os deliveries criados usando esse template não são afetados.

## Criar um modelo da entrega {#create-a-delivery-template}

Para criar um template do delivery, você pode:

* Duplicação de um template existente - [Saiba mais](#copy-an-existing-template)
* Converter um delivery existente em um template - [Saiba mais](#convert-an-existing-delivery)
* Criar um template do delivery do zero - [Saiba mais](#create-a-new-template)

### Duplicação de um template de delivery existente {#copy-an-existing-template}

O Campaign vem com um conjunto de modelos integrados para cada canal: email, push, SMS. A maneira mais fácil de criar um modelo de entrega é duplicar e personalizar um modelo integrado.

>[!NOTE]
>
>Você também pode duplicar qualquer modelo personalizado.

Para duplicar um modelo de entrega, siga as etapas abaixo:

1. Navegue até o **Modelos** , no menu **Entregas** menu esquerdo. [Saiba mais](#access-manage-templates)
1. Clique em **[!UICONTROL Mais ações]** à direita do nome do modelo desejado e selecione  **[!UICONTROL Duplicar]**.

   Você também pode selecionar um modelo na lista e selecionar essa opção na tela de edição do modelo.

1. Confirme a duplicação.

   ![](assets/templates-duplicate-confirm.png)

1. O novo painel de modelo é aberto na tela central. Edite as configurações do template conforme necessário.

   ![](assets/templates-duplicated-item.png)

1. Clique em **[!UICONTROL Revisão]** botão para salvar e revisar o modelo. Você ainda pode editar todas as configurações, excluí-las e duplicá-las.

   ![](assets/templates-review-screen.png)

1. Teste a renderização do template, se necessário. [Saiba mais](#test-template)

O novo modelo é adicionado à variável [**Modelos** lista](#access-manage-templates). Agora você pode selecioná-lo ao criar uma nova entrega.

### Conversão de uma entrega em um modelo {#convert-an-existing-delivery}

Qualquer entrega pode ser convertida em um modelo para ações futuras de entrega repetida.

Para salvar um delivery como template, siga as etapas abaixo:

1. Navegue até o **[!UICONTROL Gerenciamento de campanhas]** > **[!UICONTROL Entregas]** menu.
1. No **[!UICONTROL Procurar]** clique na guia **[!UICONTROL Mais ações]** à direita do nome do delivery desejado e selecione **[!UICONTROL Copiar como modelo]**.

   ![](assets/templates-convert-delivery.png)

   Você também pode selecionar um modelo na lista e selecionar essa opção na tela de edição do modelo.

1. Confirme a duplicação.

1. O novo painel de modelo é aberto na tela central. Edite as configurações do template conforme necessário.

1. Clique em **[!UICONTROL Revisão]** botão para salvar e revisar o modelo. Você ainda pode editar todas as configurações, excluí-las e duplicá-las.

1. Teste a renderização do template, se necessário. [Saiba mais](#test-template)

O novo modelo é adicionado à variável [**Modelos** lista](#access-manage-templates). Agora você pode selecioná-lo ao criar uma nova entrega.

### Criar um novo modelo de entrega {#create-a-new-template}

>[!NOTE]
>
>Para evitar erros de configuração, a Adobe recomenda que você [duplique um modelo integrado](#copy-an-existing-template) e personalize suas propriedades ao invés de criar um novo modelo.

Para configurar um modelo de entrega do zero, siga as etapas abaixo:

1. Navegue até o **Modelos** , no menu **Entregas** menu esquerdo. [Saiba mais](#access-manage-templates)
1. Clique em **[!UICONTROL Criar modelo]** botão.

   ![](assets/templates-create-button.png)

1. Selecione o canal que deseja usar para o modelo.
1. O modelo de entrega integrado para esse canal é usado por padrão para ajudar você a criar seu próprio modelo. Use o botão dedicado à direita do canal selecionado para selecionar outro template, se necessário.

   ![](assets/templates-channel-browse.png)

1. Clique em **[!UICONTROL Criar modelo]** botão novamente.

1. Definir as propriedades do template, [público](../audience/add-audience.md) e conteúdo dependendo do canal selecionado.

   >[!NOTE]
   >
   >Saiba mais sobre os canais de entrega e como projetar os respectivos conteúdos nas seções abaixo:
   >
   > * [Canal de email](../email/create-email.md)
   > * [Canal de notificação por push](../push/gs-push.md)
   > * [Canal de SMS](../sms/create-sms.md)

1. Além disso, para modelos de email, as configurações avançadas, como regras de tipologia e mapeamentos de público alvo, podem ser acessadas por meio da **[!UICONTROL Configurações]** localizado na parte superior direita da tela. [Saiba mais](../advanced-settings/delivery-settings.md)

1. Clique em **[!UICONTROL Revisão]** botão para salvar e revisar o modelo. Você ainda pode editar todas as configurações, excluí-las e duplicá-las.

1. Teste a renderização do template, se necessário. [Saiba mais](#test-template)

O novo modelo é adicionado à variável [**Modelos** lista](#access-manage-templates). Agora você pode selecioná-lo ao criar uma nova entrega.

## Testar um template de delivery {#test-template}

Você pode testar a renderização de qualquer template do delivery, seja criado do zero ou de um conteúdo existente. Para fazer isso, siga as etapas abaixo.

1. Navegue até o **Modelos** guia pelo menu **[!UICONTROL Gerenciamento de campanhas]** > **[!UICONTROL Entregas]** e selecione qualquer modelo. [Saiba mais](#access-manage-templates)

1. Clique em **[!UICONTROL Simular conteúdo]** botão na parte superior direita da tela.

   ![](assets/templates-simulate-button.png)

1. Selecione um ou mais perfis de teste para verificar a renderização de email. Você também pode selecionar perfis reais do banco de dados. [Saiba mais sobre perfis de teste](../audience/test-profiles.md)

1. Alterne entre os diferentes perfis para obter uma representação personalizada da mensagem de acordo com o perfil selecionado. Você também pode ajustar o nível de zoom e escolher a exibição da área de trabalho ou móvel.

[Saiba mais sobre visualização de conteúdo](../preview-test/preview-content.md)

   ![](assets/templates-stimulate.png)

1. Feche a janela para voltar à tela de edição de modelo.

>[!NOTE]
>
>Não é possível usar a renderização de email ou enviar testes em um template do delivery.


