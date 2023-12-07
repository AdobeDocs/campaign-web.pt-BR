---
audience: end-user
title: Conheça a interface
description: Interface da web do Campaign v8
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
badge: label="Beta"
source-git-commit: c5eaa8f5db6135c6d921258f7e047c1ff1cc975d
workflow-type: tm+mt
source-wordcount: '1521'
ht-degree: 98%

---

# Conheça a interface {#user-interface}

A nova interface da Web do Campaign v8 oferece uma experiência de usuário moderna e intuitiva para simplificar o design e a entrega da campanha de marketing. A nova interface é integrada aos aplicativos e soluções da Adobe Experience Cloud.


>[!NOTE]
>
>Esta documentação é atualizada com frequência para refletir as alterações recentes na interface do produto. Entretanto, algumas capturas de tela podem diferir ligeiramente da sua interface.


## Menu de navegação esquerdo {#user-interface-left-nav}

Navegue pelos links à esquerda para acessar os recursos do Campaign Web v8. Vários links exibem listas de objetos que podem ser classificados e filtrados. Você também pode configurar colunas para exibir todas as informações necessárias. Consulte esta [seção](#list-screens). Algumas telas de lista são do tipo somente leitura. Os itens exibidos no menu de navegação esquerdo e nas listas dependem das permissões de usuário. Saiba mais sobre permissões [nesta seção](permissions.md).

![](assets/home.png)

### Página inicial {#user-interface-home}

Esta tela inclui links e recursos importantes para um acesso rápido aos principais recursos do Campaign Web v8.

>[!CONTEXTUALHELP]
>id="acw_homepage_recent"
>title="Recentes"
>abstract="A lista **Recentes** fornece atalhos para as entregas criadas e modificadas recentemente. Esta lista mostra o canal, status, proprietário, datas de criação e modificação."

A lista **Recentes** fornece atalhos para as entregas criadas e modificadas recentemente. Esta lista mostra o canal, status, proprietário, datas de criação e modificação. Clique no link **Mostrar mais** para carregar mais entregas.

Os **indicadores principais de desempenho** permitem verificar a eficácia da plataforma por meio de KPIs comuns. Saiba mais sobre esses KPIs [nesta página](../reporting/kpis.md).


Acesse as principais páginas de ajuda do Campaign Web v8 na seção **Aprendizado** na página inicial.

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


### Gerenciamento de clientes {#user-interface-customer-management}

Na seção GERENCIAMENTO DE CLIENTES, você pode visualizar os destinatários, públicos-alvo e assinaturas. Essas listas são do tipo somente leitura.

* **Recipients**: acessa o banco de dados de recipients. Por padrão, você pode ver o endereço de email, o nome e o sobrenome. Saiba mais sobre destinatários [nesta seção](../audience/about-recipients.md).
* **Públicos-alvos**: esta é a lista de públicos. Por padrão, é possível ver o tipo, a origem, as datas de criação/última modificação e o rótulo. É possível filtrar a lista por origem. Saiba mais sobre públicos-alvo e listas [nesta seção](../audience/about-recipients.md).
* **Assinaturas**: navegue pelas listas de assinaturas. Por padrão, é possível ver o tipo, o modo e o rótulo. Saiba mais sobre como gerenciar assinaturas e seus cancelamentos na [documentação do Adobe Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html?lang=pt-BR){target="_blank"}.

### Gestão de decisões {#decision-management}

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Ofertas"
>abstract="Navegue pelas listas de ofertas e modelos de ofertas que foram criados no console usando o módulo **Interação**. Essas listas são do tipo somente leitura."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/offers.html?lang=pt-BR" text="Adicionar ofertas à uma entrega"

Na seção GESTÃO DE DECISÕES, é possível visualizar as ofertas e os modelos de oferta. Essas listas são do tipo somente leitura.

* **Ofertas**: navegue pela lista de ofertas e modelos de ofertas que foram criados no console usando o módulo **Interação**. Por padrão, é possível exibir o status, a data inicial/final e o ambiente. É possível filtrar a lista por status e datas de início/término. Os modelos de oferta também estão disponíveis.

Saiba como criar e enviar ofertas por email e SMS [nesta seção](../content/offers.md).



## Ajuda contextual {#user-interface-help}

Uma ajuda contextual está disponível na interface. Quando disponível, clique no ícone `?` para exibir informações de ajuda e links de documentações relacionadas.

![](assets/context-help.png){width="40%" align="left"}

Com a nova versão beta, o **Assistente de conhecimento habilitado por IA** incorporado na ajuda contextual revoluciona a pesquisa de documentação e as respostas a perguntas práticas, verificando facilmente vastos repositórios de documentação e identificando instantaneamente as informações exatas de que você precisa.

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
>id="acw_recipients_creation_details"
>title="Detalhes dos destinatários"
>abstract="Detalhes dos destinatários"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="Informações de contato dos destinatários"
>abstract="Informações de contato dos destinatários"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title="Endereço dos destinatários"
>abstract="Endereço dos destinatários"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="Conta dos destinatários"
>abstract="Conta dos destinatários"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="Campos personalizados dos destinatários"
>abstract="Campos personalizados dos destinatários"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_nolongercontact"
>title="Os destinatários não contatam mais"
>abstract="Os destinatários não contatam mais"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_othersfields"
>title="Destinatários Outros"
>abstract="Destinatários Outros"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_cardoverview"
>title="Visão geral do cartão dos destinatários"
>abstract="Visão geral do cartão dos destinatários"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_touchpoints"
>title="Touchpoints dos destinatários"
>abstract="Touchpoints dos destinatários"

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_list"
>title="Lista de assinaturas dos destinatários"
>abstract="Lista de assinaturas dos destinatários"

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
>id="acw_recipients_testprofiles_additionaldata"
>title="Dados adicionais de perfis de teste"
>abstract="Dados adicionais de perfis de teste"




>[!CONTEXTUALHELP]
>id="acw_subscriptions_delivery_template"
>title="Modelo de entrega de assinaturas"
>abstract="Modelo de entrega de assinaturas"





>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="Páginas de destino"
>abstract="Páginas de destino"

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="Propriedades das páginas de aterrissagem"
>abstract="Propriedades das páginas de aterrissagem"

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="Páginas das páginas de destino"
>abstract="Páginas das páginas de destino"

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="Programação das páginas de destino"
>abstract="Programação das páginas de destino"

>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="Página principal das páginas de destino"
>abstract="Página principal das páginas de destino"

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="Assinatura das páginas de destino"
>abstract="Assinatura das páginas de destino"

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="Chamada para ação das páginas de destino"
>abstract="Chamada para ação das páginas de destino"

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="Simulação de páginas de destino"
>abstract="Simulação de páginas de destino"




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
>id="acw_contenttemplate_menu"
>title="Modelo de conteúdo"
>abstract="Modelo de conteúdo"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_properties"
>title="Propriedades do modelo de conteúdo"
>abstract="Propriedades do modelo de conteúdo"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_design"
>title="Design do modelo de conteúdo"
>abstract="Design do modelo de conteúdo"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_selection"
>title="Seleção do modelo de conteúdo"
>abstract="Seleção do modelo de conteúdo"





>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation"
>title="Atividade de reconciliação"
>abstract="Use a atividade **Reconciliação** para vincular dados não identificados aos recursos existentes."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="Direcionamento de reconciliação"
>abstract="Direcionamento de reconciliação"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="Regras de reconciliação"
>abstract="Regras de reconciliação"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting_selection"
>title="Dimensão de targeting dimension"
>abstract="Dimensão de targeting dimension"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_field"
>title="Campo de seleção de reconciliação"
>abstract="Campo de seleção de reconciliação"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_attribute"
>title="Atributo de seleção de reconciliação"
>abstract="Atributo de seleção de reconciliação"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_condition"
>title="Condição de criação de reconciliação"
>abstract="Condição de criação de reconciliação"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_complement"
>title="Complemento de geração de reconciliação"
>abstract="Complemento de geração de reconciliação"

>[!CONTEXTUALHELP]
>id="acw_orchestration_keep_unreconciled_data"
>title="Opção para manter dados não reconciliados da reconciliação"
>abstract="Opção para manter dados não reconciliados da reconciliação"



>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_complement"
>title="Complemento de geração de combinação"
>abstract="Complemento de geração de combinação"

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_segments"
>title="Segmentos para a atividade de divisão"
>abstract="Segmentos para a atividade de divisão"




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
>id="acw_audiences_properties"
>title="Propriedades de público-alvo"
>abstract="Propriedades de público-alvo"

>[!CONTEXTUALHELP]
>id="acw_audiences_count"
>title="Contagem de público-alvo"
>abstract="Contagem de público-alvo"


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
>id="acw_subscriptions_totalnumber_subscribers"
>title="Número total de assinaturas"
>abstract="Número total de assinaturas"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overtheperiod_subscribers"
>title="Assinaturas durante o período"
>abstract="Assinaturas durante o período"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overallevolution_subscribers"
>title="Evolução geral das assinaturas"
>abstract="Evolução geral das assinaturas"


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




>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="Atividade Carregar arquivo"
>abstract="Atividade Carregar arquivo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_samplefile"
>title="Arquivo de amostra"
>abstract="Arquivo de amostra"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_nameofthefile"
>title="Nome do arquivo"
>abstract="Nome do arquivo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetdb"
>title="Banco de dados de públicos-alvo"
>abstract="Banco de dados de públicos-alvo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_rejectmgt"
>title="Gerenciamento de rejeições da atividade Carregar arquivo"
>abstract="Gerenciamento de rejeições da atividade Carregar arquivo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition"
>title="Transição de saída do gerenciamento de rejeições"
>abstract="Transição de saída do gerenciamento de rejeições"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition_reject"
>title="Transição de saída do gerenciamento de rejeições para recusas"
>abstract="Transição de saída do gerenciamento de rejeições para recusas"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_formatting"
>title="Formatação da atividade Carregar arquivo"
>abstract="Formatação da atividade Carregar arquivo"




>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_customcondition"
>title="Condição personalizada"
>abstract="Condição personalizada"

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_ruleproperties"
>title="Propriedades da regra"
>abstract="Propriedades da regra"

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_selectaudience"
>title="Selecionar público-alvo"
>abstract="Selecionar público-alvo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_predefinedfilter"
>title="Filtro predefinido"
>abstract="Filtro predefinido"

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_group"
>title="Grupo"
>abstract="Grupo"
