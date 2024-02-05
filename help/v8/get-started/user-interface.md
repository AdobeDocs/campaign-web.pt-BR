---
audience: end-user
title: Conheça a interface
description: Interface de usuário da Web do Adobe Campaign
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
badge: label="Disponibilidade limitada"
source-git-commit: 5e5580c8dd7ddd4d545d7e77c9ed26e9500ec313
workflow-type: tm+mt
source-wordcount: '1601'
ht-degree: 93%

---

# Conheça a interface {#user-interface}

A nova interface da Web do Adobe Campaign oferece uma experiência do usuário moderna e intuitiva para simplificar o design e o delivery de campanhas de marketing. A nova interface é integrada aos aplicativos e soluções da Adobe Experience Cloud.

Saiba como se conectar ao Adobe Campaign e conheça as noções básicas de navegação da Experience Cloud [neste artigo](connect-to-campaign.md).


>[!NOTE]
>
>Esta documentação é atualizada com frequência para refletir as alterações recentes na interface do produto. Entretanto, algumas capturas de tela podem diferir ligeiramente da sua interface.

## Página inicial do Campaign {#user-interface-home}

>[!CONTEXTUALHELP]
>id="acw_homepage_recent"
>title="Recentes"
>abstract="A lista **Recentes** fornece atalhos para as entregas criadas e modificadas recentemente. Esta lista mostra o canal, status, proprietário, datas de criação e modificação."

A página inicial do Campaign permite uma navegação rápida e fácil pelos principais recursos, indicadores e componentes.

A seção superior da página inicial fornece detalhes sobre as atualizações mais recentes e os novos recursos disponíveis no produto, com links para as notas de versão e a documentação detalhada. Use a seta esquerda para rolar pelos cartões de recursos.

![](assets/home.png)

Os **indicadores principais de desempenho** permitem verificar a eficácia da plataforma por meio de KPIs comuns. Saiba mais sobre esses KPIs [nesta página](../reporting/kpis.md).

A lista **Recentes** fornece atalhos para as entregas criadas e modificadas recentemente. Esta lista mostra o canal, status, proprietário, datas de criação e modificação. Clique no link **Mostrar mais** para carregar mais entregas.

Além disso, você pode acessar as principais páginas de ajuda da Web do Adobe Campaign na **Aprendizado** seção da página.

## Menu de navegação esquerdo {#user-interface-left-nav}

Navegue pelos links à esquerda para acessar os recursos da Web do Adobe Campaign. Vários links exibem listas de objetos que podem ser classificados e filtrados. Você também pode configurar colunas para exibir todas as informações necessárias. Consulte esta [seção](#list-screens). Algumas telas de lista são do tipo somente leitura. Os itens exibidos no menu de navegação esquerdo e nas listas dependem das permissões de usuário. Saiba mais sobre permissões [nesta seção](permissions.md).


### Explorer {#user-interface-explorer}

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="Explorer"
>abstract="O menu **Explorer** exibe todos os componentes e objetos do Campaign com a mesma hierarquia de pastas que a do console do cliente. Navegue por todos os componentes, pastas e esquemas do Campaign v8, verifique as permissões associadas e crie pastas e subpastas neste menu."

O menu **Explorer** exibe todos os recursos e objetos do Campaign com a mesma hierarquia de pastas que a do console do cliente. Navegue por todos os componentes, pastas e esquemas do Campaign v8 e crie entregas, fluxos de trabalhos e campanhas.

Os itens exibidos no **Explorer** dependem das permissões de usuário. Também é possível adicionar pastas e subpastas, caso você tenha os direitos adequados. Saiba mais sobre permissões [nesta seção](permissions.md).

Você pode configurar colunas para personalizar a exibição e visualizar todas as informações necessárias. Consulte esta [seção](#list-screens). Também é possível adicionar pastas e subpastas, conforme detalhado [nesta seção](permissions.md#folders).

Para obter mais informações sobre o Explorer do Campaign, a hierarquia de pastas e os recursos, consulte a [documentação do Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/campaign-ui.html?lang=pt-BR#ac-explorer-ui){target="_blank"}.

### Gerenciamento de campanhas {#user-interface-campaign-management}

Na seção GERENCIAMENTO DE CAMPANHA, é possível acessar campanhas de marketing, entregas e workflows.

* **Campanhas** - Esta é a lista de suas campanhas e modelos de campanha. Por padrão, para cada campanha, é possível visualizar as datas de início/término/criação/última modificação, o status atual e o nome do operador de campanha que a criou. É possível filtrar a lista por status, datas de início/término, pasta ou criar um filtro avançado para definir seus próprios critérios de filtragem. Saiba mais sobre campanhas [nesta seção](../campaigns/gs-campaigns.md).

* **Entregas**: navegue pela lista de entregas. Você pode visualizar o estado, a data da última modificação, bem como os principais KPIs. É possível filtrar a lista por status, data de contato ou canal. Clique em uma entrega de email para abrir o painel e obter uma visão geral dos detalhes da entrega. As entregas em outros canais são do tipo somente leitura. Saiba mais sobre entregas [nesta seção](../msg/gs-messages.md).

  Use o botão **Mais ações** para excluir ou duplicar uma entrega.

  ![](assets/more-actions.png){width="70%" align="left"}

* **Workflows** - Nessa tela, é possível acessar a lista completa de workflows e modelos de workflows. É possível verificar o status, as datas da última/próxima execução e criar um novo workflow ou um novo modelo de workflow. É possível filtrar a lista com os mesmos critérios de outros objetos. Além disso, é possível filtrar os workflows que pertencem ou não a uma campanha. Saiba mais sobre fluxos de trabalho [nesta seção](../workflows/gs-workflows.md).


### Gerenciamento de conteúdo {#user-interface-content-management}

Na seção GERENCIAMENTO DE COUNTEÚDO, você pode visualizar os modelos e fragmentos de conteúdo.

* **Modelos de conteúdo**: para um processo de design acelerado e aprimorado, você pode criar modelos independentes e reutilizar facilmente o conteúdo personalizado no [!DNL Adobe Campaign]. Disponível apenas para emails, essa funcionalidade permite que os usuários orientados por conteúdo trabalhem em modelos independentes para que a equipe de marketing possa reutilizá-los e adaptá-los em suas próprias campanhas de email. Saiba mais [nesta seção](../email/create-email-templates.md).

<!--
* **Fragments** -
-->

### Gerenciamento de clientes {#user-interface-customer-management}

Na seção GERENCIAMENTO DE CLIENTES, é possível visualizar perfis, públicos-alvo e assinaturas. Essas listas são do tipo somente leitura.

* **Perfis**: crie e gerencie perfis e acesse o banco de dados do destinatário. Por padrão, você pode ver o endereço de email, o nome e o sobrenome. Saiba mais sobre perfis [nesta seção](../audience/about-recipients.md).
* **Públicos-alvos**: esta é a lista de públicos. Por padrão, é possível ver o tipo, a origem, as datas de criação/última modificação e o rótulo. É possível filtrar a lista por origem. Saiba mais sobre públicos-alvo e listas [nesta seção](../audience/about-recipients.md).
* **Serviços de assinatura**: navegue pelas listas de assinaturas. Por padrão, é possível ver o tipo, o modo e o rótulo. Saiba mais sobre como gerenciar assinaturas e seus cancelamentos na [documentação do Adobe Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html?lang=pt-BR){target="_blank"}.
* **Filtros predefinidos**: filtros personalizados que são criados e salvos para uso futuro. Eles podem ser usados como atalhos durante qualquer operação de filtragem com o modelador de consultas, por exemplo, ao filtrar uma lista de dados ou criar o público-alvo de uma entrega. Saiba mais [nesta seção](predefined-filters.md).


### Gestão de decisões {#decision-management}

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Ofertas"
>abstract="Navegue pelas listas de ofertas e modelos de ofertas que foram criados no console usando o módulo **Interação**. Essas listas são do tipo somente leitura."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/offers.html?lang=pt-BR" text="Adicionar ofertas à uma entrega"

Na seção GESTÃO DE DECISÕES, é possível visualizar as ofertas e os modelos de oferta. Essas listas são do tipo somente leitura.

* **Ofertas**: navegue pela lista de ofertas e modelos de ofertas que foram criados no console usando o módulo **Interação**. Por padrão, é possível exibir o status, a data inicial/final e o ambiente. É possível filtrar a lista por status e datas de início/término. Os modelos de oferta também estão disponíveis.

Saiba como criar e enviar ofertas por email e SMS [nesta seção](../msg/offers.md).

### Relatórios {#left-nav-reporting}

* **Relatórios**: a entrada **Relatório** oferece um resumo geral consolidado das métricas de tráfego e engajamento de cada canal no ambiente do Campaign. Esses relatórios consistem em vários dispositivos, cada um oferecendo uma perspectiva distinta sobre a campanha ou o desempenho de entrega. Saiba mais [nesta seção](../reporting/global-reports.md).


## Ajuda contextual {#user-interface-help}

Uma ajuda contextual está disponível na interface. Quando disponível, clique no ícone `?` para exibir informações de ajuda e links de documentações relacionadas.

![](assets/do-not-localize/context-help.png){width="40%" align="left"}

Atualmente lançado como uma versão Beta na nova interface do Campaign, o **Assistente de conhecimento habilitado para IA** incorporado na ajuda contextual revoluciona a pesquisa de documentação e a resposta a perguntas &quot;como&quot;, com uma verificação fácil através de vastos repositórios de documentação, localizando instantaneamente as informações precisas de que você precisa.

Graças aos recursos da IA generativa do Campaign, esse assistente transforma sua experiência, facilitando a recuperação de informações e a solução de problemas. Caso esteja buscando orientação numa tarefa complexa ou navegando por documentos extensos, o Assistente de conhecimento habilitado por IA é seu companheiro perfeito, fornecendo eficiência e precisão incomparáveis em todas as interações.

Saiba mais [nesta seção](using-ai.md).



## Saiba mais {#learn-more}

Saiba como procurar, pesquisar e filtrar listas disponíveis no ambiente do Campaign [nesta página](list-filters.md).



<!--
######## This part stores the contextualHelp definition for WebUI BETA ###########
######## These blocks should be dispatched in the appropriate pages when available ###########
######## PLEASE DO NOT DELETE ###########
REFER TO 
https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=neolane&title=v8+WebUI+Contextual+Help+%3CALPHA%3E-+Official+list
-->


>[!CONTEXTUALHELP]
>id="acw_push_permission_for_segment"
>title="Permissão necessária"
>abstract="Seu administrador precisa lhe conceder permissão para que você possa criar um segmento."

>[!CONTEXTUALHELP]
>id="acw_push_overview_edit"
>title="Permissão necessária"
>abstract="Seu administrador precisa lhe conceder permissão para que você possa criar um segmento."

<!-- Workflows-->


<!-- delivery template settings-->


>[!CONTEXTUALHELP]
>id="acw_global_reporting_sending"
>title="Envio de relatórios globais"
>abstract="As métricas dos relatórios de rastreamento podem ser vistas nesta tela"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_tracking"
>title="Rastreamento de relatórios globais"
>abstract="As métricas dos relatórios de rastreamento podem ser vistas nesta tela"

>[!CONTEXTUALHELP]
>id="acw_campaign_workflow_list"
>title="Lista de workflows em uma campanha"
>abstract="Lista de workflows em uma campanha"

<!-- delivery settings-->


<!-- FOR BETA (alignment) -->
<!--https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CBETA%3E-+Official+list-->


<!-- FOR GA -->
<!-- Aligned with https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CGA%3E-+Official+list -->

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_list"
>title="Criação de destinatários"
>abstract="Criação de destinatários"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_cardoverview"
>title="Visão geral do cartão dos destinatários"
>abstract="Visão geral do cartão dos destinatários"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_touchpoints"
>title="Touchpoints dos destinatários"
>abstract="Touchpoints dos destinatários"

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_selection"
>title="Seleção de assinaturas dos destinatários"
>abstract="Seleção de assinaturas dos destinatários"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_eligible_list"
>title="Lista qualificada de ofertas dos destinatários"
>abstract="Lista qualificada de ofertas dos destinatários"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_preview_proposition"
>title="Visualização de ofertas dos destinatários"
>abstract="Visualização de ofertas dos destinatários"

>[!CONTEXTUALHELP]
>id="acw_recipients_readonlyprofile"
>title="Perfil somente leitura de destinatários"
>abstract="Perfil somente leitura de destinatários"



>[!CONTEXTUALHELP]
>id="acw_orchestration_query_enrichment_noneditable"
>title="Atividade não editável"
>abstract="Atividade não editável"


>[!CONTEXTUALHELP]
>id="acw_fragments_menu"
>title="Fragmentos"
>abstract="Fragmentos"

>[!CONTEXTUALHELP]
>id="acw_fragments_save"
>title="Salvar fragmentos"
>abstract="Salvar fragmentos"

>[!CONTEXTUALHELP]
>id="acw_fragments_create"
>title="Criação de fragmentos"
>abstract="Criação de fragmentos"

>[!CONTEXTUALHELP]
>id="acw_fragments_properties"
>title="Propriedades dos fragmentos"
>abstract="Propriedades dos fragmentos"

>[!CONTEXTUALHELP]
>id="acw_fragments_type"
>title="Tipo de fragmentos"
>abstract="Tipo de fragmentos"

>[!CONTEXTUALHELP]
>id="acw_fragments_list"
>title="Lista de fragmentos"
>abstract="Lista de fragmentos"

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="Detalhes de fragmentos"
>abstract="Detalhes de fragmentos"




>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_savefilter"
>title="Filtro de salvamento de conteúdo condicional"
>abstract="Filtro de salvamento de conteúdo condicional"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_selectfilter"
>title="Filtro de seleção de conteúdo condicional"
>abstract="Filtro de seleção de conteúdo condicional"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectline"
>title="Conteúdo condicional na linha de assunto"
>abstract="Conteúdo condicional na linha de assunto"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectlinecondition"
>title="Condição da linha de assunto do conteúdo condicional"
>abstract="Condição da linha de assunto do conteúdo condicional"


>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_testprofiles"
>title="Simular perfis de teste"
>abstract="Simular perfis de teste"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_profiles_selection"
>title="Simular seleção de perfis de teste"
>abstract="Simular seleção de perfis de teste"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_send_testprofiles"
>title="Simular envio de perfis de teste"
>abstract="Simular envio de perfis de teste"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_email_log"
>title="Simular log de email"
>abstract="Simular log de email"


>[!CONTEXTUALHELP]
>id="acw_directmail_content"
>title="Conteúdo da correspondência direta"
>abstract="Conteúdo da correspondência direta"

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_file"
>title="Propriedades do arquivo de Correspondência direta"
>abstract="Propriedades do arquivo de Correspondência direta"

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_content"
>title="Propriedades de conteúdo de Correspondência direta"
>abstract="Propriedades de conteúdo de Correspondência direta"


<!--
Deprecated IDs - to remove in GA: -->

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="Exibir atributos avançados"
>abstract="Por padrão, somente os atributos mais comuns são exibidos na lista de atributos. Ative o botão **Exibir atributos avançados** para ver todos os atributos disponíveis para a lista atual na paleta esquerda do construtor de regras, como nós, agrupamentos, links 1-1 e links 1-N."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_advancedfields"
>title="Campos avançados do construtor de regras"
>abstract="Por padrão, somente os atributos mais comuns são exibidos na lista de atributos. Ative o botão **Exibir atributos avançados** para ver todos os atributos disponíveis para a lista atual na paleta esquerda do construtor de regras, como nós, agrupamentos, links 1-1 e links 1-N."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_properties_advanced"
>title="Atributos avançados do construtor de regras"
>abstract="Por padrão, somente os atributos mais comuns são exibidos na lista de atributos. Ative o botão **Exibir atributos avançados** para ver todos os atributos disponíveis para a lista atual na paleta esquerda do construtor de regras, como nós, agrupamentos, links 1-1 e links 1-N."



>[!CONTEXTUALHELP]
>id="acw_contenttemplate_readonlymode"
>title="Este modelo é do tipo somente leitura"
>abstract="A confirmar"

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_generatesubsets"
>title="Gerar todos os subconjuntos na mesma tabela"
>abstract="A confirmar"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_defaultlp"
>title="Páginas de aterrissagem padrão"
>abstract="A confirmar"