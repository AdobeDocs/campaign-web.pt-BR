---
product: campaign
title: Usar modelos de entrega
description: Saiba como criar e usar modelos de entrega no Campaign Web
feature: Email, Push, SMS, Direct Mail, Cross Channel Orchestration
role: User
level: Beginner
exl-id: cd3d4c2d-7bb2-4574-aeb8-6aac0683ec59
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '1102'
ht-degree: 19%

---

# Usar modelos de entrega {#work-with-delivery-templates}

>[!CONTEXTUALHELP]
>id="acw_delivery_template_for_campaign"
>title="Modelos de entrega"
>abstract="Para acelerar e aprimorar o processo de design, crie modelos de entrega para reutilizar conteúdo e configurações personalizados em suas campanhas. Essa funcionalidade padroniza a aparência criativa, permitindo a execução e a inicialização mais rápidas de campanhas."

Para acelerar e aprimorar o processo de design, crie modelos de entrega para reutilizar conteúdo e configurações personalizados em suas campanhas. Essa funcionalidade padroniza a aparência criativa, permitindo a execução e a inicialização mais rápidas de campanhas.

Um modelo inclui:

* A **pasta** e a **pasta de execução** do modelo. A pasta é o local onde o template do delivery é salvo. A pasta de execução é a pasta onde os deliveries criados com base nesse template são salvos.
* [Tipologias](../advanced-settings/delivery-settings.md#typology),
* O endereço do remetente,
* Um [público-alvo](../audience/about-recipients.md), incluindo [grupos de controle](../audience/control-group.md),
* Personalizar [conteúdo](../email/edit-content.md),
* [Campos personalizados](../personalization/personalize.md) e [conteúdo condicional](../personalization/conditions.md),
* Links para [mirror page](../email/mirror-page.md) e unsubscription [links](../email/message-tracking.md),
* Outras propriedades de entrega, como validade de recurso, parâmetros de nova tentativa ou configurações de quarentena.

>[!NOTE]
>
>Os modelos de entrega são diferentes dos [modelos de conteúdo](../content/create-email-templates.md), que permitem reutilizar somente o conteúdo de seus emails e começar a criar conteúdo com um dos modelos de email de exemplo fornecidos prontos para uso.

## Acessar e gerenciar modelos de entrega {#access-manage-templates}

>[!CONTEXTUALHELP]
>id="acw_delivery_templates"
>title="Trabalho com modelos de entrega"
>abstract="Use modelos de entrega para criar e salvar configurações de entrega para uso futuro em suas campanhas. Crie modelos de entrega do zero, duplique um modelo já existente ou converta uma entrega em um modelo."

Para acessar a lista de modelos de conteúdo, selecione **[!UICONTROL Gerenciamento de Campanha]** > **[!UICONTROL Entregas]** no menu esquerdo e navegue até a guia **Modelos**.

![A guia Modelos no menu Entregas](assets/templates-tab.png){zoomable="yes"}

Todos os modelos criados no ambiente atual são exibidos.

Você pode filtrar modelos de conteúdo por canais e pastas. Você também pode definir filtros avançados criando uma regra usando atributos de delivery. [Saiba mais sobre o modelador de consultas](../audience/../query/query-modeler-overview.md)

![Opções de filtragem para modelos](assets/templates-filters.png){zoomable="yes"}

Para editar um modelo, clique no item desejado na lista. A partir daí:

* Modifique o conteúdo, as propriedades, o público-alvo e todas as ofertas anexadas a ele.
* Teste seu modelo. [Saiba mais](#test-template)

![Editando um modelo](assets/templates-edition.png){zoomable="yes"}

Para excluir ou [duplicar](#copy-an-existing-template) um modelo, selecione a ação correspondente no menu **[!UICONTROL Mais ações]**, na lista **[!UICONTROL Modelos]** ou em uma tela de edição de modelo.

![Mais menu de ações para modelos](assets/templates-more-actions.png){zoomable="yes"}

>[!NOTE]
>
>Quando um template é editado ou excluído, os deliveries criados usando esse template não são afetados.

## Criar um modelo da entrega {#create-a-delivery-template}

Para criar um template do delivery, você pode:

* Duplicar um modelo existente - [Saiba mais](#copy-an-existing-template)
* Converter uma entrega existente em um modelo - [Saiba mais](#convert-an-existing-delivery)
* Criar um modelo de entrega do zero - [Saiba mais](#create-a-new-template)

### Duplicação de um template de delivery existente {#copy-an-existing-template}

O Campaign inclui modelos integrados para cada canal: email, push e SMS. A maneira mais fácil de criar um modelo de entrega é duplicar e personalizar um modelo integrado.

>[!NOTE]
>
>Você também pode duplicar qualquer modelo personalizado.

Para duplicar um template de delivery, siga estas etapas:

1. Navegue até a guia **Modelos** no menu esquerdo **Entregas**. [Saiba mais](#access-manage-templates)
1. Clique no botão **[!UICONTROL Mais ações]** à direita do nome do modelo desejado e selecione **[!UICONTROL Duplicar]**.

   Você também pode selecionar um modelo na lista e escolher essa opção na tela de edição do modelo.

1. Confirme a duplicação.

   ![Caixa de diálogo de confirmação para duplicar um modelo](assets/templates-duplicate-confirm.png){zoomable="yes"}

1. O novo painel de modelo é aberto na tela central. Edite as configurações do template conforme necessário.

   ![Painel de modelo duplicado](assets/templates-duplicated-item.png){zoomable="yes"}

1. Clique no botão **[!UICONTROL Revisar]** para salvar e revisar seu modelo. Ainda é possível editar todas as configurações, excluí-las e duplicá-las.

   ![Tela de revisão para um modelo](assets/templates-review-screen.png){zoomable="yes"}

1. Teste a renderização do template, se necessário. [Saiba mais](#test-template)

O novo modelo foi adicionado à lista [**Modelos**](#access-manage-templates). Agora você pode selecioná-lo ao criar uma nova entrega.

### Conversão de uma entrega em um modelo {#convert-an-existing-delivery}

Qualquer entrega pode ser convertida em um modelo para ações futuras de entrega repetida.

Para salvar um delivery como template, siga estas etapas:

1. Navegue até o menu **[!UICONTROL Gerenciamento de campanha]** > **[!UICONTROL Entregas]**.
1. Na guia **[!UICONTROL Procurar]**, clique no botão **[!UICONTROL Mais ações]** à direita do nome de entrega desejado e selecione **[!UICONTROL Copiar como modelo]**.

   ![Opção para copiar uma entrega como modelo](assets/templates-convert-delivery.png){zoomable="yes"}

   Você também pode selecionar um modelo na lista e escolher essa opção na tela de edição do modelo.

1. Confirme a duplicação.

1. O novo painel de modelo é aberto na tela central. Edite as configurações do template conforme necessário.

1. Clique no botão **[!UICONTROL Revisar]** para salvar e revisar seu modelo. Ainda é possível editar todas as configurações, excluí-las e duplicá-las.

1. Teste a renderização do template, se necessário. [Saiba mais](#test-template)

O novo modelo foi adicionado à lista [**Modelos**](#access-manage-templates). Agora você pode selecioná-lo ao criar uma nova entrega.

### Criar um novo modelo de entrega {#create-a-new-template}

>[!NOTE]
>
>Para evitar erros de configuração, a Adobe recomenda [duplicar um modelo interno](#copy-an-existing-template) e personalizar suas propriedades em vez de criar um novo modelo.

Para configurar um template do delivery do zero, siga estas etapas:

1. Navegue até a guia **Modelos** no menu esquerdo **Entregas**. [Saiba mais](#access-manage-templates)
1. Clique no botão **[!UICONTROL Criar modelo]**.

   ![Botão Criar modelo](assets/templates-create-button.png){zoomable="yes"}

1. Selecione o canal que deseja usar para o modelo.
1. O modelo de entrega integrado para esse canal é usado por padrão para ajudar você a criar seu próprio modelo. Use o botão dedicado à direita do canal selecionado para selecionar outro template, se necessário.

   ![Seleção de canal para um novo modelo](assets/templates-channel-browse.png){zoomable="yes"}


1. Clique novamente no botão **[!UICONTROL Criar modelo]**.

1. Defina as propriedades do modelo, [público-alvo](../audience/add-audience.md) e conteúdo, dependendo do canal selecionado.

   >[!NOTE]
   >
   >Saiba mais sobre os canais de entrega e como projetar os respectivos conteúdos nas seções abaixo:
   >
   > * [Canal de email](../email/create-email.md)
   > * [Canal de notificação por push](../push/gs-push.md)
   > * [Canal de SMS](../sms/create-sms.md)

1. Além disso, para modelos de email, as configurações avançadas, como regras de tipologia e mapeamentos de destino, podem ser acessadas por meio do botão **[!UICONTROL Configurações]**, localizado na parte superior direita da tela. [Saiba mais](../advanced-settings/delivery-settings.md)

1. Clique no botão **[!UICONTROL Revisar]** para salvar e revisar seu modelo. Ainda é possível editar todas as configurações, excluí-las e duplicá-las.

1. Teste a renderização do template, se necessário. [Saiba mais](#test-template)

O novo modelo foi adicionado à lista [**Modelos**](#access-manage-templates). Agora você pode selecioná-lo ao criar uma nova entrega.

## Testar um template de delivery {#test-template}

Você pode testar a renderização de qualquer template do delivery, seja criado do zero ou de um conteúdo existente. Para fazer isso, siga estes passos:

1. Navegue até a guia **Modelos** por meio do menu **[!UICONTROL Gerenciamento de campanha]** > **[!UICONTROL Entregas]** e selecione qualquer modelo. [Saiba mais](#access-manage-templates)

1. Clique no botão **[!UICONTROL Simular conteúdo]** na parte superior direita da tela.

   ![Botão Simular conteúdo](assets/templates-simulate-button.png){zoomable="yes"}

1. Selecione um ou mais perfis de teste para verificar a renderização de email. Você também pode selecionar perfis reais do banco de dados. [Saiba mais sobre perfis de teste](../audience/test-profiles.md)

1. Alterne entre os diferentes perfis para obter uma representação personalizada da mensagem de acordo com o perfil selecionado. Você também pode ajustar o nível de zoom e escolher a exibição da área de trabalho ou móvel.

[Saiba mais sobre visualização de conteúdo](../preview-test/preview-content.md)

   ![Visualização de conteúdo simulado](assets/templates-stimulate.png){zoomable="yes"}

1. Feche a janela para retornar à tela de edição do modelo.

>[!NOTE]
>
>Não é possível usar a renderização de email ou enviar provas em um template do delivery.