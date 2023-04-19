---
audience: end-user
title: Descubra a interface
description: Interface do usuário da Web do Campaign v8
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
badge: label="Alpha" type="Positive"
source-git-commit: 403f1e5fcb353f4c89f12066854853b51861293b
workflow-type: tm+mt
source-wordcount: '1369'
ht-degree: 34%

---

# Descubra a interface {#user-interface}

>[!CONTEXTUALHELP]
>id="acw_homepage_learnmore"
>title="Descubra a interface"
>abstract="A nova interface da Web do Campaign v8 oferece uma experiência do usuário integrada, intuitiva e consistente."

A nova interface da Web do Campaign v8 oferece uma experiência do usuário moderna e intuitiva para simplificar o design e o delivery da campanha de marketing. Essa nova interface é integrada ao Adobe Experience Platform.

<!--
Key concepts when browsing the user interface are common with Adobe Experience Platform. Refer to [Adobe Experience Platform documentation](https://experienceleague.adobe.com/docs/experience-platform/landing/platform-ui/ui-guide.html#adobe-experience-platform-ui-guide) for more details.
-->

>[!NOTE]
>
>Essa documentação é atualizada com frequência para refletir as alterações mais recentes na interface do usuário do produto. No entanto, algumas capturas de tela podem diferir ligeiramente da interface do usuário.


<!--
* console + web interface (overview, why use each of them)
* web UI made up of read-only lists that can be configured, show how to add columns
-->

## Menu de navegação esquerdo

Navegue pelos links à esquerda para acessar os recursos da Web do Campaign v8. Vários links exibem listas de objetos que podem ser classificados e filtrados. Você também pode configurar colunas para exibir todas as informações necessárias. Consulte esta [seção](#list-screens). Todas as telas de lista são somente leitura, exceto a lista de entrega de email. Clicar em qualquer item de lista para edição/visualização não está disponível em Alfa. Todas as listas serão editáveis em versões futuras. Os itens exibidos no menu de navegação esquerdo dependem das permissões do usuário.

![](assets/home.png)

### Página inicial

Esta tela inclui links e recursos importantes para um acesso rápido aos principais recursos da Web do Campaign v8. O **Recentes** fornece atalhos para os deliveries criados e modificados recentemente. Esta lista mostra as datas de criação e modificação e o status.

<!--
* Banner
* KPIs on email channel (cross-deliveries): open rate, delivery rate, etc
* Recent items
* Learning cards
-->

Acesse as páginas de ajuda da chave da Web do Campaign v8 na seção inferior da página inicial.

<!--
show global KPIs, recent items + left menu to access features)
CONTROL PANEL not alpha
Global report not alpha
-->

### Explorer

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="Explorer"
>abstract="O menu **Explorer** exibe a mesma hierarquia de pastas do console do cliente. Navegue por todos os componentes, pastas e esquemas do Campaign v8. Todas as telas de lista são somente leitura, exceto a lista de entrega de email."

O menu **Explorer** exibe a mesma hierarquia de pastas do console do cliente. Navegue por todos os componentes, pastas e esquemas do Campaign v8. Todas as telas de lista são somente leitura, exceto a lista de entrega de email.

Os itens exibidos no Explorer dependem das permissões do usuário.

Como em qualquer tela de lista, você pode configurar colunas para personalizar a exibição para exibir todas as informações necessárias. Consulte esta [seção](#list-screens).

Para obter mais informações sobre o explorador do Campaign, consulte esta seção [documentação](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/ac-ui/campaign-ui.html#ac-explorer-ui){target="_blank"}.
<!--
Explorer' menu in web UI to navigate through console content: console navtree second view in addition to the left menu lists with filters. The Explorer gives the real folder hierarchy from the console. Make sure you find your deliveries in sub-folders. All lists can be accessed in read-only. No Create/Edit. You can configure lists (colums). All schema fields, linked tables are available. 

If you need to view your lists of recipients (age, gender), transactions or live transactional messages. To view each/edit -> console.

Navtree view depends on permissions (same as console).
-->

### Gerenciamento de campanhas

>[!CONTEXTUALHELP]
>id="acw_campaigns_list"
>title="Campanhas"
>abstract="Esta é a lista das suas campanhas. É possível exibir informações úteis, como datas de início/término/última modificação e status. Você pode filtrar a lista por status ou datas de início/término. Os modelos do Campaign também estão disponíveis. Essas listas são somente leitura."

>[!CONTEXTUALHELP]
>id="acw_deliveries_list"
>title="Entregas"
>abstract="Navegue pela lista de entregas. Você pode visualizar estado, última data de modificação e principais KPIs. Você pode filtrar a lista por estado, data de contato ou canal. Clique numa entrega de email para abrir seu painel. Outros itens são somente leitura. Os templates de entrega também estão disponíveis."

* **Campanhas** - Esta é a lista de suas campanhas. Por padrão, você pode exibir suas datas de início/término/última modificação, bem como seu status. Você pode filtrar a lista por status ou datas de início/término. Os modelos do Campaign também estão disponíveis. Essas listas são somente leitura.

* **Deliveries** - Navegue pela lista de deliveries. Por padrão, você pode visualizar seu estado, a última data de modificação, bem como os KPIs principais. Você pode filtrar a lista por estado, data de contato ou canal. Clique em um delivery de email para abrir seu painel e obter uma visão geral dos detalhes do delivery. Os deliveries em outros canais são somente leitura. Os templates de delivery também estão disponíveis no modo somente leitura. Você pode usar o Console do cliente para editá-los. Veja isso [documentação](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/create-templates.html){target="_blank"}.

   Use o **Mais ações** para excluir ou duplicar um delivery.

   ![](assets/more-actions.png){width="70%" align="left"}

### Gerenciamento de clientes

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Recipients"
>abstract="Acessar o banco de dados de recipients. É possível visualizar informações úteis, como endereço de email, nome e sobrenome. Esta lista é somente leitura."

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Públicos"
>abstract="Esta é a sua lista de públicos. É possível visualizar o tipo, a origem, as datas de criação/última modificação e o rótulo. É possível filtrar a lista por origem. Esta lista é somente leitura."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Listas de assinaturas"
>abstract="Navegar pelas listas de assinaturas. É possível visualizar o tipo, o modo e o rótulo. Esta lista é somente leitura."

* **Recipients** - Acesse o banco de dados do recipient. Por padrão, você pode exibir o endereço de email, o nome e o sobrenome. Esta lista é somente leitura.
* **Públicos-alvo** - Esta é a sua lista de públicos-alvo. Por padrão, é possível exibir o tipo, a origem, as datas de criação/última modificação e o rótulo. É possível filtrar a lista por origem. Esta lista é somente leitura.
* **Listas de assinaturas** - Navegue pelas listas de assinaturas. Por padrão, é possível exibir o tipo, o modo e o rótulo. Esta lista é somente leitura.
* **Workflows para construção do target** - Acesse a lista de workflows do Campaign. Por padrão, você pode visualizar o estado, as datas e o ambiente do último/próximo processamento. É possível filtrar a lista por estado, data do último processamento e tipo de fluxo de trabalho. Os modelos de fluxo de trabalho também estão disponíveis. Essas listas são somente leitura.

### Gestão de decisões

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Ofertas"
>abstract="Navegar pela lista de ofertas de interação. Por padrão, é possível visualizar o status, as datas de início/término e o ambiente. É possível filtrar a lista por estado e datas de início/término. Os modelos de oferta também estão disponíveis. Essas listas são somente leitura."

* **Ofertas** - Navegue pela lista de ofertas do Interaction. Por padrão, é possível visualizar o status, as datas de início/término e o ambiente. É possível filtrar a lista por estado e datas de início/término. Os modelos de oferta também estão disponíveis. Essas listas são somente leitura.

## Barra superior

A barra superior da interface permite:

* compartilhar seu feedback como um testador Alfa
* alternar entre organizações e instâncias
* alternar entre seus aplicativos Adobe Experience Cloud
* acesse páginas de ajuda, entre em contato com o suporte e compartilhe comentários. Você pode pesquisar artigos e vídeos de ajuda no campo de pesquisa.

![](assets/unified-shell.png){width="70%" align="left"}
<!--
Org / Sub-org switcher to switch between instances. Only one for Alpha. Later: intermerdiate screen with Control Panel (beta). if v8 + ACS with one card per ACS instance. Maybe quickly explain the menu for Alpha?
-->

## Configurar telas de lista {#list-screens}

Vários links no menu de navegação esquerdo, por exemplo **Deliveries** ou **Campanhas**, exibir listas de objetos. Essas telas de lista são somente leitura, exceto a lista de delivery de email.

Para localizar itens mais rapidamente, você pode usar a barra de pesquisa ou filtrar a lista com base em critérios contextuais.

![](assets/filter.png){width="70%" align="left"}

As listas são exibidas em colunas. É possível exibir informações adicionais alterando a configuração da coluna. Para fazer isso, clique no ícone no canto superior direito da lista. Você pode adicionar ou remover colunas e alterar a ordem em que são exibidas.

![](assets/columns.png){width="70%" align="left"}

Você pode classificar itens na lista clicando em qualquer cabeçalho de coluna. Uma seta é exibida (para cima ou para baixo) indicando que a lista está classificada nessa coluna. Para colunas numéricas ou de datas, a seta para cima indica que a lista é classificada em ordem crescente, enquanto a seta para baixo indica uma ordem decrescente. Para colunas de sequência ou alfanuméricas, os valores são listados em ordem alfabética.

## Ajuda contextual e guia de integração

Uma ajuda contextual está disponível na interface do . Quando disponível, clique no botão **?** ícone para exibir informações de ajuda e links de documentação relacionados.

![](assets/context-help.png){width="70%" align="left"}

Um guia de integração também está disponível para ajudar você a começar a usar o Campaign v8 Web. Clique no ícone no canto inferior direito, escolha um dos cenários passo a passo disponíveis e siga as instruções.

![](assets/onboarding.png){width="70%" align="left"}

## Navegadores compatíveis {#browsers}

O Campaign v8 Web foi projetado para funcionar de maneira ideal na versão mais recente do Google Chrome, Safari e Microsoft Edge. Você pode ter problemas ao usar determinados recursos em versões mais antigas ou outros navegadores.

## Preferências de idioma {#language-pref}

O Campaign v8 Web está disponível atualmente nos seguintes idiomas:

<table>
<tr>
<td>
<p>Inglês (EUA) - EN-US</p>
<p>Francês - FR</p>
<p>Alemão - DE</p>
<p>Italiano - IT</p>
</td>
<td>
<p>Espanhol - ES</p>
<p>Português (Brasil) - PTBR</p>
<p>Japonês - JP</p>
</td>
<td>
<p>Coreano - KR</p>
<p>Chinês simplificado - CHS</p>
<p>Chinês tradicional - CHT</p>
</td>
</tr>
</table>

O idioma padrão da interface é determinado pelo idioma preferencial especificado no perfil do usuário.

Para alterar seu idioma:

1. Clique no ícone do perfil, na parte superior direita, e selecione **Preferências**.

   ![](assets/preferences.png){width="70%" align="left"}

1. Em seguida, clique no idioma exibido sob seu endereço de email.

   ![](assets/preferences2.png)

1. Selecione o idioma preferido e clique em **Salvar**. Você pode selecionar um segundo idioma caso o componente que está usando não esteja localizado em seu primeiro idioma.

   ![](assets/select-language.png)

<!--
## Supported browsers {#browsers}

Adobe Campaign interface is designed to work optimally in the latest version of Google Chrome. You might have trouble using certain features on older versions or other browsers.
-->



<!--
######## This part stores the contextualHelp definition for WebUI BETA ###########
######## These blocks should be dispatched in the appropriate pages when available ###########
######## PLEASE DO NOT DELETE ###########
REFER TO 
https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CALPHA%3E-+Official+list
-->

>[!CONTEXTUALHELP]
>id="acw_sms_report_overview"
>title="Resumo do relatório de SMS"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_push_report_overview"
>title="Resumo do relatório de push"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="Modelo de notificação por push"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_properties"
>title="Propriedades de criação de campanha"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_schedule"
>title="Cronograma de criação de campanha"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_properties_advanced"
>title="Atributos avançados do Construtor de regras"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_sent"
>title="Métricas enviadas"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_errors"
>title="Métricas de erros"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_android_content"
>title="Encaminhar conteúdo do Android"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_content"
>title="Encaminhar conteúdo do iOS"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_content"
>title="Conteúdo do SMS"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_sms_preview_option_app_target"
>title="Assinantes do aplicativo"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_email_preview_option_test_target"
>title="População de ensaio"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_email_preview_mode"
>title="Modo de visualização"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_enrichmentdata"
>title="Dados de enriquecimento"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_dashboard"
>title="Personalização"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="Seleção de arquivo"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Arquivo de amostra"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="Definição de colunas"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="Parâmetros de formatação"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sending"
>title="Envio de relatórios"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_tracking"
>title="Rastreamento de relatórios"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_overview"
>title="Visão geral dos relatórios"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_target"
>title="Relatório de estatísticas do target"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_selection"
>title="Geração de relatórios agregada selecionar um delivery"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_campaign_properties"
>title="Propriedades da campanha"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="Lista de fluxos de trabalho"
>abstract="TBD"

<!--BETA-->
>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Campos de desduplicação"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Configurações de desduplicação"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Complemento de desduplicação"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Complemento Dimension"
>abstract="TBD"
