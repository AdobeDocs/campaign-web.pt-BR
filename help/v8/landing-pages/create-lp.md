---
title: Criar uma landing page
description: Saiba como configurar e publicar uma landing page no Campaign Web
feature: Landing Pages
exl-id: d4a49048-5ab1-4b69-9e12-1ffa235c51f4
source-git-commit: e5a17ad1f8316d201dc3b4bc6ce20d61aea7a9c9
workflow-type: tm+mt
source-wordcount: '1376'
ht-degree: 34%

---

# Criar e publicar landing pages {#create-lp}

>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="Criar e gerenciar landing pages"
>abstract="O Adobe Campaign permite criar, projetar e compartilhar páginas de destino para direcionar usuários a páginas da web nas quais é possível gerenciar casos de uso de aquisição, assinaturas ou cancelamentos de assinaturas e listas de bloqueio, utilizando como base os modelos integrados."

A interface do usuário da Web do Campaign permite criar, projetar e publicar páginas de aterrissagem. Depois de publicado, você pode inserir um link para o formulário em um delivery. Depois que os recipients clicam nesse link, eles são direcionados para a página de aterrissagem correspondente.

[!DNL Adobe Campaign] O vem com quatro modelos para gerenciar os seguintes casos de uso: **aquisição**, **subscrição**, **unsubscription**, e **➡ incluir na lista de bloqueios**. [Saiba mais](lp-use-cases.md)

## Acessar páginas de destino {#access-landing-pages}

Para acessar a lista de landing pages, selecione **[!UICONTROL Gerenciamento de campanhas]** > **[!UICONTROL Landing pages]** no menu esquerdo.

![](assets/lp-inventory.png){zoomable=&quot;yes&quot;}

A variável **[!UICONTROL Landing pages]** o inventário exibe todos os itens criados. É possível filtrá-los usando a variável **Mostrar filtros** botão. É possível restringir os resultados a um [pasta](../get-started/permissions.md#folders) usando a lista suspensa ou adicione regras usando o [modelador de consultas](../query/query-modeler-overview.md).

![](assets/lp-inventory-filter.png){zoomable=&quot;yes&quot;}

<!--From this list, you can access the [landing page Live report](../reports/lp-report-live.md) or [landing page Global report](../reports/lp-report-global.md) for published items.-->

>[!CAUTION]
>
>Não é possível exibir ou editar landing pages criadas no console do cliente (formulários web) na interface do usuário da Web do Campaign. Saiba mais na [Documentação do console do Campaign](https://experienceleague.adobe.com/docs/campaign/campaign-v8/content/webapps.html?lang=pt-BR){target="_blank"}.

<!--If you unpublish a landing page which is referenced in a message, the link to the landing page will be broken and an error page will be displayed. You cannot delete a published landing page. To delete it, you must first unpublish it.-->

É possível duplicar ou excluir uma landing page. Clique nas reticências ao lado de uma landing page para selecionar a ação desejada.

## Criar uma landing page {#create-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="Definir as propriedades da landing page"
>abstract="Preencha os campos de propriedades, como o rótulo, e modifique o esquema, se necessário. Além disso, você pode editar o nome interno, alterar a pasta onde a landing page está armazenada e fornecer uma descrição."

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="Defina o conteúdo de cada página"
>abstract="Ajuste o conteúdo de cada página que faz parte desta página de destino, como o próprio formulário, a página de confirmação que é exibida ao enviar o formulário ou a página para a qual os usuários são direcionados em caso de erros."

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="Agendar a landing page"
>abstract="Você pode definir uma data inicial e uma data final para sua landing page. Quando a página chegar ao final do período de validade, o formulário não estará mais disponível. A página **Expiração** será exibida em seu lugar."

>[!CONTEXTUALHELP]
>id="acw_landingpages_preload"
>title="Definir opções de pré-carregamento"
>abstract="Quando a opção **Preencher previamente com os dados referenciados no formulário** estiver selecionada, visitantes da página de destino quem correspondem a um perfil do banco de dados terão as informações do seu perfil pré-carregadas automaticamente no formulário. Com a opção **Ignorar pré-carregamento na ausência de ID** selecionada, cada perfil inserido será adicionado ao banco de dados após a aprovação do formulário."

>[!CONTEXTUALHELP]
>id="acw_landingpages_storage"
>title="Definir opções de armazenamento"
>abstract="A seção de pré-carregamento permite indicar como localizar o registro a ser atualizado no banco de dados."

<!--The main steps to create landing pages are as follows:

![](assets/lp-creation-process.png){zoomable="yes"}-->

Para criar uma landing page, siga estas etapas:

1. No **[!UICONTROL Landing pages]** inventário, clique em **[!UICONTROL Criar página de destino]**.

   ![](assets/lp-create-button.png){zoomable=&quot;yes&quot;}

1. Selecione um modelo:
   * **[!UICONTROL Aquisição]**: este é o template padrão para landing pages, que permite capturar e atualizar dados de perfil.
   * **[!UICONTROL Inscrição]**: use este template para permitir que os usuários assinem um [serviço](../audience/manage-services.md).
   * **[!UICONTROL Cancelar assinatura]**: esse template pode ser usado em um delivery enviado aos assinantes de um serviço, para permitir que eles cancelem a assinatura deste [serviço](../audience/manage-services.md).
   * **[!UICONTROL ➡ Incluir na lista de bloqueios]**: esse template deve ser usado quando um perfil clica em um link de opt-out em um delivery e não deseja mais ser contatado.

   ![](assets/lp-templates.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Saiba como implementar os diferentes casos de uso correspondentes a cada modelo no [esta página](lp-use-cases.md).

1. Clique em **[!UICONTROL Create]**.

1. Preencha o **[!UICONTROL Propriedades]** campos como o rótulo.

   Por padrão, as landing pages são armazenadas no **[!UICONTROL Aplicações web]** pasta. Você pode alterá-la navegando até o local desejado no **[!UICONTROL Opções adicionais]**. [Saiba como trabalhar com pastas](../get-started/permissions.md#folders)

   ![](assets/lp-properties.png){zoomable=&quot;yes&quot;}

1. No **[!UICONTROL Pré-carregamento de dados]** , as duas opções abaixo são selecionadas por padrão:

   * Quando a opção **[!UICONTROL Preencher previamente com os dados referenciados no formulário]** estiver selecionada, visitantes da página de destino quem correspondem a um perfil do banco de dados terão as informações do seu perfil pré-carregadas automaticamente no formulário. O usuário só precisa preencher os campos ausentes e atualizar os valores existentes, se necessário. Isso permite mesclar dados de perfis existentes, em vez de criar duplicatas.

   * A variável **[!UICONTROL Ignorar pré-carregamento se nenhuma ID]** deve ser selecionada se você não deseja atualizar os perfis. Nesse caso, cada perfil inserido será adicionado ao banco de dados após a aprovação do formulário. Essa opção é usada, por exemplo, quando o formulário é postado em um site.

1. Uma landing page pode ter páginas subsequentes. Para adicionar páginas, navegue até **[!UICONTROL Páginas]** e clique no botão **[!UICONTROL Editar conteúdo]** para cada página que você deseja criar para essa página de aterrissagem. O conteúdo de cada página já está pré-preenchido. Edite-as conforme necessário. [Saiba mais](lp-content.md)

   ![](assets/lp-pages.png){zoomable=&quot;yes&quot;}

1. A variável **[!UICONTROL Atualizar o registro pré-carregado]** for selecionada por padrão. Ela permite atualizar os perfis armazenados no banco de dados por meio da landing page. A caixa de pré-carregamento permite indicar como localizar o registro a ser atualizado no banco de dados.

   Você também pode escolher entre os campos no contexto atual da landing page, aqueles que serão usados para localizar o perfil correspondente no banco de dados. Para fazer isso, desmarque a opção **[!UICONTROL Atualizar o registro pré-carregado]** e marque os campos desejados em **[!UICONTROL Opções de reconciliação]**.

   ![](assets/lp-storage.png){zoomable=&quot;yes&quot;}

1. Você pode definir uma data inicial e uma data final para sua landing page. Selecionar **[!UICONTROL Ativar agendamento]** e defina as datas.

   ![](assets/lp-schedule.png){zoomable=&quot;yes&quot;}

   * A landing page é publicada automaticamente na data/hora de início especificada.

     >[!NOTE]
     >
     >Se nenhuma data de início for definida, a landing page será ativada assim que for publicada.

   * Quando a página atinge a data final, <!--the landing page is automatically unpublished and -->o formulário não está mais disponível. A página **[!UICONTROL Expiração]** será exibida em seu lugar.

     >[!NOTE]
     >
     >Por motivos de segurança e desempenho da plataforma, a Adobe recomenda que você defina uma data de término.

1. Clique em **[!UICONTROL Revisar e publicar]**.

Depois de definir todas as configurações e [projetado](lp-content.md) em todas as páginas, é possível [test](#test-landing-page) e [publicar](#publish-landing-page) sua landing page, conforme detalhado abaixo.

## Testar a landing page {#test-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="Simular a landing page"
>abstract="Você pode ver uma pré-visualização da landing page na interface do Campaign Web ou abri-la em uma nova guia do navegador da web."

>[!CONTEXTUALHELP]
>id="ac_preview_lp_profiles"
>title="Visualizar e testar a página de destino"
>abstract="Depois de definir as configurações e o conteúdo da página de destino, você pode usar perfis de teste para visualizar."

Depois que as configurações e o conteúdo da landing page forem definidos, você poderá usar perfis de teste para pré-visualizá-la. Se você inseriu [conteúdo personalizado](../personalization/gs-personalization.md), você poderá verificar como esse conteúdo é exibido na página de aterrissagem, usando os dados do perfil de teste.

>[!CAUTION]
>
>Você deve ter perfis de teste disponíveis para poder visualizar suas mensagens e enviar provas. [Saiba mais sobre perfis de teste](../audience/test-profiles.md)

Para testar a landing page, siga estas etapas:

1. Depois de clicar em **[!UICONTROL Revisar e publicar]**, selecione o **[!UICONTROL Simular conteúdo]** no painel da página de aterrissagem para acessar a seleção de perfil de teste.

   ![](assets/lp-simulate-content.png){zoomable=&quot;yes&quot;}

1. No **[!UICONTROL Simular]** selecione um ou mais perfis de teste.

   As etapas para selecionar perfis de teste são as mesmas que ao testar uma mensagem. Eles são detalhados na seção [Pré-visualização e teste](../preview-test/preview-test.md) seção.

1. Selecionar **[!UICONTROL Abrir pré-visualização]** para testar sua landing page.

   ![](assets/lp-open-preview.png){zoomable=&quot;yes&quot;}

1. A visualização da landing page é aberta em uma nova guia. Os elementos personalizados são substituídos pelos dados do perfil de teste selecionado.

   Se você selecionou a variável **[!UICONTROL Preencher previamente com os dados referenciados no formulário]** nas configurações da página de aterrissagem, os campos de formulário são automaticamente preenchidos com os dados correspondentes do perfil de teste.<!--TBC-->

   ![](assets/lp-preview.png){zoomable=&quot;yes&quot;}

1. Selecione outros perfis de teste para visualizar a renderização de cada variante da página de aterrissagem.

<!--Can you preview Confirmation/Error/Expiration pages?-->

## Publicar a página de destino {#publish-landing-page}

Quando a landing page estiver pronta e validada, publique-a para disponibilizá-la para uso em um delivery usando o botão correspondente.

Depois de publicado:

* A landing page é adicionada à lista de landing pages com a **[!UICONTROL Publicado]** status. Agora ela está ativa e pronta para ser referenciada em seu conteúdo.

* Você pode copiar e colar o **[!UICONTROL URL da landing page]** que é exibido na parte superior da página em um navegador da web para visualizar sua landing page.

>[!CAUTION]
>
>Para testar ou aproveitar totalmente sua página de destino, você não deve copiar e colar o link diretamente em um navegador da web ou em suas entregas. Use o botão [Simular conteúdo](#test-landing-page) para testá-la e siga as etapas descritas em [nesta seção](lp-use-cases.md) para fazer o uso correto da sua landing page.

![](assets/lp-published.png){zoomable=&quot;yes&quot;}

Você pode monitorar os impactos da sua landing page por meio de logs<!--and specific reports-->. Clique em **[!UICONTROL Logs]** botão.
