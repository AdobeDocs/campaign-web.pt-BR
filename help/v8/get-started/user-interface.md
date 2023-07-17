---
audience: end-user
title: Conheça a interface
description: Interface da web do Campaign v8
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
badge: label="Alfa"
source-git-commit: 768484c1fc67ac9aa2a2fbac6d00183fb81dbe63
workflow-type: tm+mt
source-wordcount: '1536'
ht-degree: 99%

---

# Conheça a interface {#user-interface}

>[!CONTEXTUALHELP]
>id="acw_homepage_learnmore"
>title="Conheça a interface"
>abstract="A nova interface da Campaign Web v8 oferece ao usuário uma experiência integrada, intuitiva e consistente."

A nova interface da Web do Campaign v8 oferece uma experiência de usuário moderna e intuitiva para simplificar o design e a entrega da campanha de marketing. Essa nova interface é integrada à Adobe Experience Platform.


>[!NOTE]
>
>Esta documentação é atualizada com frequência para refletir as alterações recentes na interface do produto. Entretanto, algumas capturas de tela podem diferir ligeiramente da sua interface.


## Menu de navegação esquerdo {#user-interface-left-nav}

Navegue pelos links à esquerda para acessar os recursos do Campaign Web v8. Vários links exibem listas de objetos que podem ser classificados e filtrados. Você também pode configurar colunas para exibir todas as informações necessárias. Consulte esta [seção](#list-screens). Todas as telas de lista são do tipo somente leitura, exceto a lista de entrega de email. A opção de clicar em qualquer item de lista para editar/visualizar não está disponível na versão Alfa. Todas as listas serão editáveis em versões futuras. Os itens exibidos no menu de navegação esquerdo dependem das permissões do usuário.

![](assets/home.png)

### Página inicial {#user-interface-home}

Esta tela inclui links e recursos importantes para um acesso rápido aos principais recursos do Campaign Web v8.

A lista **Recentes** fornece atalhos para as entregas criadas e modificadas recentemente. Esta lista mostra o canal, status, proprietário, datas de criação e modificação.

Acesse as principais páginas de ajuda do Campaign Web v8 na seção **Aprendizado** na página inicial.

### Explorer {#user-interface-explorer}

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="Explorer"
>abstract="O menu **Explorer** exibe todos os componentes e objetos do Campaign com a mesma hierarquia de pastas que a do console do cliente. Navegue por todos os componentes, pastas e esquemas do Campaign v8 e crie entregas, workflows e campanhas. Todas as outras listas são de somente leitura."

O menu **Explorer** exibe todos os recursos e objetos do Campaign com a mesma hierarquia de pastas que a do console do cliente. Navegue por todos os componentes, pastas e esquemas do Campaign v8 e crie entregas, workflows e campanhas. Todas as outras listas são de somente leitura.

Os itens exibidos no explorador dependem das permissões do usuário.

Como em qualquer tela de lista, você pode configurar as colunas para personalizar a exibição e mostrar todas as informações necessárias. Consulte esta [seção](#list-screens).

Para obter mais informações sobre o Explorer do Campaign, a hierarquia de pastas e os recursos, consulte a [documentação do Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/campaign-ui.html?lang=pt-BR#ac-explorer-ui){target="_blank"}.

### Gerenciamento de campanhas {#user-interface-campaign-management}

>[!CONTEXTUALHELP]
>id="acw_campaigns_list"
>title="Campanhas"
>abstract="É a lista das suas campanhas. É possível exibir informações úteis, como datas de início/término/última modificação e status. Você pode filtrar a lista por status ou datas iniciais/finais. Clique no botão “Criar campanha” para adicionar uma nova campanha. Selecione uma campanha para exibir seu conteúdo, entregas e detalhes. Navegue até a guia “Modelos” para exibir e criar modelos."



Na seção GERENCIAMENTO DE CAMPANHA, é possível acessar campanhas de marketing, entregas e workflows.

* **Campanhas** - Esta é a lista de suas campanhas e modelos de campanha. Por padrão, para cada campanha, é possível visualizar as datas de início/término/criação/última modificação, o status atual e o nome do operador de campanha que a criou. É possível filtrar a lista por status, datas de início/término, pasta ou criar um filtro avançado para definir seus próprios critérios de filtragem. Saiba mais sobre campanhas [nesta seção](../campaigns/gs-campaigns.md).

* **Entregas**: navegue pela lista de entregas. Você pode visualizar o estado, a data da última modificação, bem como os principais KPIs. É possível filtrar a lista por estado, data de contato ou canal. Clique em uma entrega de email para abrir o painel e obter uma visão geral dos detalhes da entrega. As entregas em outros canais são do tipo somente leitura. Saiba mais sobre entregas [nesta seção](../msg/gs-messages.md).

  Use o botão **Mais ações** para excluir ou duplicar uma entrega.

  ![](assets/more-actions.png){width="70%" align="left"}

* **Workflows** - Nessa tela, é possível acessar a lista completa de workflows e modelos de workflows. É possível verificar o status, as datas da última/próxima execução e criar um novo workflow ou um novo modelo de workflow. É possível filtrar a lista com os mesmos critérios de outros objetos. Além disso, é possível filtrar os workflows que pertencem ou não a uma campanha. Saiba mais sobre fluxos de trabalho [nesta seção](../workflows/gs-workflows.md).


### Gerenciamento de clientes {#user-interface-customer-management}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Recipients"
>abstract="Acesse o banco de dados de recipients. É possível visualizar informações úteis, como endereço de email, nome e sobrenome. Essa lista é do tipo somente leitura."

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Públicos-alvo"
>abstract="É a sua lista de públicos. É possível exibir o tipo, a origem, as datas de criação/última modificação e o rótulo. É possível filtrar a lista por origem. Essa lista é do tipo somente leitura."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Listas de assinaturas"
>abstract="Navegar pelas listas de assinaturas. É possível exibir o tipo, o modo e o rótulo. Essa lista é do tipo somente leitura."


Na seção GERENCIAMENTO DE CLIENTES, você pode visualizar os destinatários, públicos-alvo e assinaturas. Essas listas são de somente leitura.

* **Recipients**: acessa o banco de dados de recipients. Por padrão, você pode ver o endereço de email, o nome e o sobrenome. Saiba mais sobre destinatários em [documentação do Adobe Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/gs-audiences.html?lang=pt-BR){target="_blank"}.
* **Públicos**: esta é a lista de públicos. Por padrão, é possível ver o tipo, a origem, as datas de criação/última modificação e o rótulo. É possível filtrar a lista por origem. Saiba mais sobre públicos-alvo e listas na [documentação do Adobe Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html?lang=pt-BR){target="_blank"}.
* **Assinaturas**: navegue pelas listas de assinaturas. Por padrão, é possível ver o tipo, o modo e o rótulo. Saiba mais sobre como gerenciar assinaturas e seus cancelamentos na [documentação do Adobe Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html?lang=pt-BR){target="_blank"}.

### Gestão de decisões

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Ofertas"
>abstract="Você pode navegar pela lista de ofertas de interação. Por padrão, é possível exibir o status, a data inicial/final e o ambiente. É possível filtrar a lista por estado e data inicial/final. Os modelos de oferta também estão disponíveis. Essas listas são do tipo somente leitura."

* **Ofertas**: navegue pela lista de ofertas de interação. Por padrão, é possível exibir o status, a data inicial/final e o ambiente. É possível filtrar a lista por estado e data inicial/final. Os modelos de oferta também estão disponíveis. Essas listas são do tipo somente leitura.

Saiba como criar e gerenciar ofertas na [documentação do Adobe Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=pt-BR){target="_blank"}.

## Barra superior

Use a barra superior da interface para:

* compartilhar seu feedback como um testador Alfa
* alternar entre organizações e instâncias
* alternar entre os aplicativos da Adobe Experience Cloud
* acessar páginas de ajuda, entrar em contato com o suporte e compartilhar feedback. Você pode pesquisar artigos e vídeos de ajuda no campo de pesquisa.

![](assets/unified-shell.png){width="50%" align="left"}
<!--
Org / Sub-org switcher to switch between instances. Only one for Alpha. Later: intermerdiate screen with Control Panel (beta). if v8 + ACS with one card per ACS instance. Maybe quickly explain the menu for Alpha?
-->

## Ajuda contextual {#contextual-help}

Uma ajuda contextual está disponível na interface. Quando disponível, clique no ícone `?` para exibir informações de ajuda e links de documentações relacionadas.

![](assets/context-help.png){width="40%" align="left"}

<!--An on-boarding guide is also available to help you get started with Campaign v8 Web. Click the icon in the bottom right corner, choose one of the available step-by-step scenarios, and simply follow the instructions.

![](assets/onboarding.png){width="70%" align="left"}-->

## Navegadores compatíveis {#browsers}

O Campaign Web v8 foi desenvolvido para funcionar de maneira ideal na versão mais recente do Google Chrome, Safari e Microsoft Edge. Você pode ter problemas ao usar determinados recursos em versões mais antigas ou em outros navegadores.

## Preferências de idioma {#language-pref}

Atualmente, o Campaign Web v8 está disponível nos seguintes idiomas:

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

Para alterar o idioma:

1. Clique no ícone do perfil, na parte superior direita, e selecione **Preferências**.
1. Em seguida, clique no link de idioma exibido sob o seu endereço de email.
1. Selecione o idioma de sua preferência e clique em **Salvar**. Você pode selecionar um segundo idioma caso o componente que está usando não esteja localizado em seu primeiro idioma.


<!--
######## This part stores the contextualHelp definition for WebUI BETA ###########
######## These blocks should be dispatched in the appropriate pages when available ###########
######## PLEASE DO NOT DELETE ###########
REFER TO 
https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=neolane&title=v8+WebUI+Contextual+Help+%3CALPHA%3E-+Official+list
-->





>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_enrichmentdata"
>title="Dados de enriquecimento"
>abstract="A confirmar"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sending"
>title="Envio de relatórios"
>abstract="Consulte os indicadores de envio para os relatórios da campanha."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_tracking"
>title="Rastreamento de relatórios"
>abstract="Consulte os indicadores de rastreamento para os relatórios da campanha."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_overview"
>title="Visão geral dos relatórios"
>abstract="Métricas principais para a sua entrega."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_target"
>title="Relatório de estatísticas do público alvo"
>abstract="Esta seção exibe métricas específicas de acordo com os públicos-alvo."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_selection"
>title="Relatórios agregados para entregas"
>abstract="Selecione pelo menos duas entregas para exibir um relatório de dados agregado."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Campos de desduplicação"
>abstract="A confirmar"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Configurações de desduplicação"
>abstract="A confirmar"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Complemento de desduplicação"
>abstract="A confirmar"

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Complemento de dimensão"
>abstract="A confirmar"

>[!CONTEXTUALHELP]
>id="acw_push_permission_for_segment"
>title="Permissão necessária"
>abstract="Seu administrador precisa lhe conceder permissão para que você possa criar um segmento."

>[!CONTEXTUALHELP]
>id="acw_push_overview_edit"
>title="Permissão necessária"
>abstract="Seu administrador precisa lhe conceder permissão para que você possa criar um segmento."






>[!CONTEXTUALHELP]
>id="acw_deliveries_metrics_newquarantines"
>title="Nova métrica de quarentenas"
>abstract="Nova métrica de quarentena."


>[!CONTEXTUALHELP]
>id="acw_keyindicators_delivered"
>title="Entregue"
>abstract="KPI Entregue"

>[!CONTEXTUALHELP]
>id="acw_keyindicators_opens"
>title="Aberturas"
>abstract="Abre o KPI"

>[!CONTEXTUALHELP]
>id="acw_keyindicators_clicks"
>title="Cliques"
>abstract="KPI de Cliques"

>[!CONTEXTUALHELP]
>id="acw_keyindicators_unsubscriptions"
>title="Cancelamentos de assinatura"
>abstract="KPI de cancelamentos de assinatura"

>[!CONTEXTUALHELP]
>id="acw_keyindicators_spam"
>title="Spam"
>abstract="KPI de spam"

>[!CONTEXTUALHELP]
>id="acw_keyindicators_errors"
>title="Erros"
>abstract="KPI de erros"


>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="Lista de workflow"
>abstract="Lista de workflows disponíveis para sua campanha. Use o botão “Criar workflow” para adicionar um workflow à campanha."

>[!CONTEXTUALHELP]
>id="acw_orchestration_saveaudience_outbound"
>title="Transição de saída para salvar público"
>abstract="tbc"


<!-- delivery template settings-->

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_tracking_validity"
>title="Período de validade"
>abstract="Essa opção define a duração do rastreamento ativado nos URLs."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_duration"
>title="Duração da entrega"
>abstract="O campo Duração da entrega permite inserir o limite de novas tentativas de entrega globais. Isso significa que o Adobe Campaign envia as mensagens começando na data de início e, em seguida, para mensagens que retornam somente um erro, tentativas regulares e configuráveis são executadas até que o limite de validade seja atingido."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_resources_validity"
>title="Limite da validade de recursos"
>abstract="O campo Limite da validade é usado para recursos carregados, principalmente para a mirror page ou imagens. Esses recursos são válidos por um tempo limitado: quando o limite é atingido, os recursos não estarão mais disponíveis."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_approval"
>title="Modo de aprovação"
>abstract="Cada etapa de uma entrega pode estar sujeita à aprovação para garantir o monitoramento e o controle totais dos vários processos."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_retries"
>title="Número máximo de tentativas"
>abstract="Se uma mensagem falhar devido a um erro temporário, as tentativas serão executadas até o fim da duração da entrega."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_recipient_importance"
>title="Importância do recipient"
>abstract="A importância do recipient é uma fórmula usada para determinar quais recipients são mantidos quando as regras de tipologia de capacidade são excedidas."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_weight"
>title="Peso da entrega"
>abstract="Os pesos das entregas permitem identificar entregas de alta prioridade dentro da estrutura do gerenciamento de pressão. As mensagens com o peso mais alto têm prioridade."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_typology"
>title="Tipologia"
>abstract="A tipologia permite controlar, filtrar e monitorar o envio de entregas."
