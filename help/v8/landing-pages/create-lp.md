---
title: Criar uma landing page
description: Saiba como configurar e publicar uma landing page no Campaign Web
badge: label="Disponibilidade limitada"
source-git-commit: 2a02015d9d7a7de67f0bcffd328d37080c0f50c4
workflow-type: tm+mt
source-wordcount: '1005'
ht-degree: 10%

---

# Criar e publicar páginas de destino {#create-lp}

>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="Criar e gerenciar páginas de destino"
>abstract="O Adobe Campaign permite criar e projetar páginas de destino para direcionar seus usuários para formulários online, onde eles podem aceitar ou recusar receber suas comunicações ou assinar um serviço específico, como um boletim informativo."

Para direcionar seus clientes para uma página da Web definida que você deseja exibir ao clicar em um link específico, crie uma página de aterrissagem em [!DNL Adobe Campaign], criar o conteúdo, testá-lo e publicá-lo.

## Acessar páginas de destino {#access-landing-pages}

Para acessar a lista de landing pages, selecione **[!UICONTROL Gerenciamento de campanhas]** > **[!UICONTROL Landing pages]** no menu esquerdo.

![](assets/lp-inventory.png)

A variável **[!UICONTROL Landing pages]** o inventário exibe todos os itens criados. É possível filtrá-los usando a variável **Mostrar filtros** botão. É possível restringir os resultados a um [pasta](../get-started/permissions.md#folders) usando a lista suspensa ou adicione regras usando o [modelador de consultas](../query/query-modeler-overview.md).

![](assets/lp-inventory-filter.png)

<!--From this list, you can access the [landing page Live report](../reports/lp-report-live.md) or [landing page Global report](../reports/lp-report-global.md) for published items.-->

>[!NOTE]
>
>Não é possível exibir landing pages criadas no console do cliente no Campaign Web. Saiba mais na [Documentação do console do Campaign](https://experienceleague.adobe.com/docs/campaign/campaign-v8/content/webapps.html){target="_blank"}.

<!--If you unpublish a landing page which is referenced in a message, the link to the landing page will be broken and an error page will be displayed. You cannot delete a published landing page. To delete it, you must first unpublish it.-->

É possível duplicar ou excluir uma landing page. Clique nos três pontos ao lado de uma landing page para selecionar a ação desejada.

## Criar uma landing page {#create-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="Definir as propriedades da landing page"
>abstract="Preencha os campos de propriedades, como o rótulo, e modifique o esquema, se necessário. Além disso, você pode editar o nome interno, alterar a pasta onde a landing page está armazenada e fornecer uma descrição."

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="Definir o conteúdo das páginas"
>abstract="Edite o conteúdo de cada página que faz parte desta página de aterrissagem."

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="Agendar a página de aterrissagem"
>abstract="É possível definir uma data de início e uma data de término para a landing page. Quando a página expira, a variável **Expiração** é exibida."


>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="Definir as configurações da página principal"
>abstract="A página principal é exibida imediatamente depois que as pessoas clicam no link de página de destino que consta em um email ou site."

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="Definir a página de aterrissagem da sua assinatura"
>abstract="Uma página de subscrição permite que seus clientes assinem um serviço."

<!--The main steps to create landing pages are as follows:

![](assets/lp-creation-process.png)-->

1. No **[!UICONTROL Landing pages]** inventário, clique em **[!UICONTROL Criar página de destino]**.

   ![](assets/lp-create-button.png)

1. Selecione um modelo:
   * **[!UICONTROL Aquisição]**: este é o template padrão para landing pages, que permite capturar e atualizar dados do perfil.
   * **[!UICONTROL Inscrição]**: use esse template para oferecer assinaturas de um serviço.
   * **[!UICONTROL Cancelar assinatura]**: esse template pode ser vinculado a partir de um email enviado aos assinantes de um serviço, para permitir que eles cancelem a assinatura desse serviço.
   * **[!UICONTROL ➡ Incluir na lista de bloqueios]**: esse template deve ser usado quando um perfil não deseja mais ser contatado pelo Campaign. Saiba mais sobre o gerenciamento de inclui na lista de bloqueios

   ![](assets/lp-templates.png)

1. Clique em **[!UICONTROL Create]**.

1. Preencha os campos de propriedades, como o rótulo. Por padrão, as landing pages são armazenadas no **[!UICONTROL Aplicações web]** pasta. Você pode alterá-la navegando até o local desejado no **[!UICONTROL Opções adicionais]**. [Saiba como trabalhar com pastas](../get-started/permissions.md#folders)

   ![](assets/lp-properties.png)

1. No **[!UICONTROL Pré-carregamento de dados]** , as duas opções abaixo são selecionadas por padrão:

   * A variável **[!UICONTROL Preencher previamente com os dados referenciados no formulário]** permite pré-carregar automaticamente os dados que correspondem aos campos de entrada e mesclagem no formulário.

   * A variável **[!UICONTROL Ignorar pré-carregamento se nenhuma ID]** deve ser selecionada se você não deseja atualizar os perfis. Nesse caso, cada perfil inserido será adicionado ao banco de dados após a aprovação do formulário. Essa opção é usada, por exemplo, quando o formulário é postado em um site.

1. No **[!UICONTROL Páginas]** clique na guia **[!UICONTROL Editar conteúdo]** para cada página que você deseja criar para essa página de aterrissagem. O conteúdo de cada página já está pré-preenchido. Edite-as conforme necessário. [Saiba mais](lp-content.md)

   ![](assets/lp-pages.png)

1. A variável **[!UICONTROL Atualizar o registro pré-carregado]** é selecionada por padrão. Se quiser atualizar os perfis armazenados no banco de dados por meio da landing page, use uma caixa de pré-carregamento. A caixa de pré-carregamento permite indicar como localizar o registro a ser atualizado no banco de dados. Você também pode escolher entre os campos no contexto atual da landing page, aqueles que serão usados para localizar o perfil correspondente no banco de dados.

   ![](assets/lp-storage-schedule.png)

1. É possível definir uma data de início e uma data de término para a landing page. Selecionar **[!UICONTROL Ativar agendamento]** e defina as datas. Quando a página expira, a variável **[!UICONTROL Expiração]** é exibida.

1. Clique em **[!UICONTROL Revisar e publicar]**.

Depois de configurar e projetar todas as páginas, é possível [test](#test-landing-page) e [publicar](#publish-landing-page) sua landing page.

## Testar a página de destino {#test-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="Simular sua página de aterrissagem"
>abstract="Você pode pré-visualizar sua landing page na interface da Web do Campaign ou abri-la em uma nova guia do navegador da Web."

>[!CONTEXTUALHELP]
>id="ac_preview_lp_profiles"
>title="Visualizar e testar a página de destino"
>abstract="Depois de definir as configurações e o conteúdo da página de destino, você pode usar perfis de teste para visualizar."

Depois que as configurações e o conteúdo da landing page forem definidos, você poderá usar perfis de teste para pré-visualizá-la. Se você inseriu [conteúdo personalizado](../personalization/gs-personalization.md), você poderá verificar como esse conteúdo é exibido na página de aterrissagem, usando os dados do perfil de teste.

>[!CAUTION]
>
>Você deve ter perfis de teste disponíveis para poder visualizar suas mensagens e enviar provas. Saiba como [criar perfis de teste](../audience/test-profiles.md).

1. Na interface da landing page, clique na guia **[!UICONTROL Simular conteúdo]** botão para acessar a seleção de perfil de teste.

   ![](assets/lp-simulate-content.png)

1. No **[!UICONTROL Simular]** selecione um ou mais perfis de teste.

   As etapas para selecionar perfis de teste são as mesmas que ao testar uma mensagem. Eles são detalhados na seção [Pré-visualização e teste](../preview-test/preview-test.md) seção.

1. Selecionar **[!UICONTROL Abrir pré-visualização]** para testar sua landing page.

   ![](assets/lp-open-preview.png)

1. A visualização da landing page é aberta em uma nova guia. Os elementos personalizados são substituídos pelos dados do perfil de teste selecionado.

   ![](assets/lp-preview.png)

1. Selecione outros perfis de teste para visualizar a renderização de cada variante da página de aterrissagem.

<!--Can you preview Confirmation/Error/Expiration pages?-->

## Publicar a página de destino {#publish-landing-page}

Quando a landing page estiver pronta, você poderá publicá-la para disponibilizá-la para uso em uma mensagem.

Quando a landing page for publicada, ela será adicionada à lista de landing pages com a **[!UICONTROL Publicado]** status. Agora ele está ativo e pronto para ser usado.

![](assets/lp-published.png)

Depois de publicado, você pode copiar e colar o **[!UICONTROL URL da landing page]** que é exibido na parte superior da página em um navegador da web.

Você pode monitorar os impactos na página de aterrissagem por meio de logs e relatórios específicos.