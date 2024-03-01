---
audience: end-user
title: Matriz de recursos da interface web e do console do cliente do Campaign
description: Lista de recursos compatíveis com a interface web do Campaign
exl-id: 4bcac01f-be1d-497c-937d-0c82f0d6b17d
source-git-commit: 81ee3c7ce46826089f68d2da1ff1a45e7fa93473
workflow-type: tm+mt
source-wordcount: '2179'
ht-degree: 95%

---

# Console do cliente do Campaign e Campaign Web {#capabilities-matrix}

Os principais recursos do Campaign estão disponíveis na interface do Campaign Web. Essa interface foi desenvolvida principalmente para que os profissionais de marketing planejem, iniciem e avaliem suas campanhas de marketing. Todos os recursos estão listados [nesta página](../rn/whats-new.md).

A personalização da plataforma do Campaign com base nas necessidades de negócios e dados, assim como a conexão com outros sistemas, são gerenciadas no console do cliente do Campaign. Como consequência, alguns recursos e configurações só podem ser acessados, criados ou gerenciados no console do cliente do Campaign. Alguns estarão disponíveis em uma atualização posterior da interface do Campaign Web.

<!--
**Homepage**

* Home page dashboard
* Home page customization-->

## Gerenciamento de campanhas {#campaign-mgt-capabilities}

Com a interface do Campaign Web, é possível criar campanhas entre canais conforme detalhado [nesta seção](../campaigns/gs-campaigns.md). Os recursos a seguir estão disponíveis somente no console do cliente do Campaign. Eles não podem ser acessados na interface do Campaign Web, mas alguns estão visíveis no [menu Explorer](user-interface.md#user-interface-explorer).

Use os links fornecidos para navegar pela documentação do Campaign v8 (console do cliente) e saber como usar esses recursos.

* **Calendário de marketing**. O calendário da campanha mostra todos os programas, planos, campanhas e entregas em uma linha do tempo global. Esse recurso só está disponível no console do cliente. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html?lang=pt-BR#campaign-calendar){target="_blank"}
* **Programas e planos**. Cada campanha faz parte de um programa que, por sua vez, pertence a um plano. Na interface do Campaign Web, todas as campanhas são associadas por padrão a um plano e programa incorporados. Você só pode criar e gerenciar planos e programas no console do cliente. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html?lang=pt-BR#work-with-plan-and-program){target="_blank"}
* **Gerenciamento de provedores, orçamento e custos**. Você pode configurar provedores de serviços envolvidos nos processos realizadas em suas campanhas, incluindo estruturas de custo, o que permite gerenciar seus orçamentos em cada programa e campanha. Esse recurso só está disponível no console do cliente. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/providers--stocks-and-budgets.html?lang=pt-BR){target="_blank"}
* **Marketing distribuído** (marketing central e local) O Adobe Campaign oferece um aplicativo de marketing distribuído para a implementação de campanhas cooperativas entre entidades centrais (sede, departamentos de marketing etc.) e entidades locais (pontos de vendas, agências regionais etc.). Esse recurso só está disponível no console do cliente. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/automation/distributed-marketing/about-distributed-marketing.html?lang=pt-BR){target="_blank"}
* **Gerenciamento de recursos de marketing** (MRM), metas, simulações e controle de custos. O Adobe Campaign oferece um aplicativo de gerenciamento de recursos de marketing (MRM) que permite controlar ações de marketing de maneira colaborativa, fornecendo gerenciamento completo e rastreamento em tempo real das tarefas, orçamentos e recursos de marketing envolvidos. Esse recurso só está disponível no console do cliente. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/automation/mrm/about-marketing-resource-management.html?lang=pt-BR){target="_blank"}
* **Gerenciamento de tarefas**. Como parte do aplicativo MRM, as tarefas do Campaign podem ser criadas, atribuídas, rastreadas e monitoradas no painel da campanha. Esse recurso só está disponível no console do cliente. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/automation/mrm/creating-and-managing-tasks.html?lang=pt-BR){target="_blank"}

## Canais de comunicação {#channels-capabilities}

Com a interface do Campaign Web, você pode criar, projetar e enviar **emails**, **SMS** e **notificações por push**, além de medir o impacto dessas mensagens usando vários relatórios exclusivos, conforme detalhado [nesta seção](../msg/gs-messages.md). No entanto, no momento os seguintes canais **não** estão disponíveis: in-app, correspondência direta, LINE, central de atendimento, canal personalizado, marketing social com o X (Twitter).

Use os links fornecidos para navegar pela documentação do Campaign v8 (console do cliente) e saber mais sobre esses canais.

* **Correspondência direta**. O canal de correspondência direta permite enviar uma correspondência física aos clientes, fornecedores ou outras pessoas, como avisos, faturas, demonstrativos, ofertas de marketing e muito mais. Este canal só está disponível no console do cliente.  [Saiba mais](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-direct-mail/about-direct-mail-channel.html?lang=pt-BR){target="_blank"}
* **Mensagens LINE**. O LINE é um aplicativo para mensagens instantâneas, chamadas de voz e vídeo gratuitas, disponível em todos os dispositivos móveis e para PC. O Adobe Campaign permite enviar mensagens LINE somente a partir do console do cliente. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/line.html?lang=pt-BR){target="_blank"}
* **Central de atendimento e canais personalizados**. A central de atendimento e outros canais personalizados podem ser implementados em seu ambiente do Campaign. Esses canais só podem ser disponibilizados por meio do console do cliente. [Saiba mais na documentação do Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/communication-channels.html?lang=pt-BR#other-channels){target="_blank"}
* **Marketing social** com o X (Twitter). Você interage com seus clientes via X (Twitter) publicando mensagens e enviando mensagens diretas. Esse recurso, que acompanha o complemento de marketing social, só está disponível no console do cliente - [Saiba mais](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-tw.html?lang=pt-BR){target="_blank"}

## Páginas de destino e aplicativos web {#Webapps-capabilities}

O Adobe Campaign permite criar, projetar e compartilhar páginas de destino. A experiência das páginas de destino foi totalmente reimaginada na nova interface. Consulte [esta seção](../landing-pages/get-started-lp.md) e descubra como criar, projetar e publicar uma página de destino na interface web do Campaign.

Como consequência, no console do cliente do Campaign não é possível editar, atualizar ou modificar uma página de destino criada na interface web, e vice-versa. Os seguintes tipos de aplicativos web não estão disponíveis na interface web do Campaign. No entanto, eles estão visíveis na lista de páginas de destino. Use os links fornecidos para navegar pela documentação do Campaign Classic v7 e saber mais sobre estes aplicativos web:

* **Aplicativos web**. O Adobe Campaign permite criar e publicar aplicativos web dinâmicos e interativos com informações pré-carregadas do banco de dados e conteúdo adaptado aos direitos do usuário conectado. Esse recurso só está disponível no console do cliente. [Saiba mais na documentação do Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-applications/about-web-applications.html?lang=pt-BR){target="_blank"}
* **Formulários web**. As páginas da web e de destino criadas no console do cliente estão visíveis na interface web do Campaign, mas não podem ser editadas ou modificadas. Algumas opções podem diferir entre o designer de página da web do console do cliente e o designer da página de destino que acompanha a interface web do Campaign. [Saiba mais na documentação do Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-forms/about-web-forms.html?lang=pt-BR){target="_blank"}
* **Pesquisas online**. Você pode criar pesquisas online e coletar respostas somente no console do cliente. Esse recurso não está disponível na interface do Campaign Web.  [Saiba mais na documentação do Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/online-surveys/about-surveys.html?lang=pt-BR){target="_blank"}


## Perfis, perfis de teste e públicos-alvo {#profiles-audiences-capabilities}

Você pode criar, gerenciar e atualizar perfis e perfis de teste no console do cliente do Campaign e na interface web do Campaign. Todas as alterações executadas em uma interface são visíveis na outra. No entanto, algumas configurações específicas de destinatário e parâmetros avançados podem estar ausentes na nova interface do Campaign Web.

Observe que o termo “destinatário” foi alterado para “perfil” na nova interface web, e “seed addresses” agora são “perfis de teste”

<!--Audience composition is a new capability coming with Campaign Web user interface. As a consequence, in Campaign client console, you cannot edit, update or modify an [audience created with the Query modeler](../query/query-modeler-overview.md). -->

Todos os públicos-alvo criados no console do cliente do Campaign ou na Adobe Experience Platform estão disponíveis na interface do Campaign Web.

Conforme descrito na [documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/import-profiles.html?lang=pt-BR#import-jobs){target="_blank"}, os processos de importação e exportação instantâneos não estão disponíveis na interface do Campaign Web.<!--To import profiles into Campaign Web user interface, you must create a workflow as detailed in [this section]().-->

## Mensagens transacionais {#mc-capabilities}

Atualmente, os recursos de mensagens transacionais que acompanham o pacote de produtos do Centro de mensagens não estão disponíveis na nova interface do Campaign Web.

Navegue pela [documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/real-time/transactional.html?lang=pt-BR){target="_blank"} e saiba mais sobre os recursos de mensagens em tempo real, como:

* Criação e execução de mensagens em tempo real por email, SMS e push
* Enriquecimento e personalização de mensagem
* Relatórios e monitoramento de mensagens transacionais

## Design de conteúdo {#content-capabilities}

O novo Designer de email integrado na interface do Adobe Campaign Web permite criar emails atrativos e personalizados por meio de uma interface intuitiva de arrastar e soltar. Caso esteja começando do zero, importando um conteúdo existente ou aproveitando modelos existentes, é possível criar e ajustar o conteúdo para cada email. [Saiba mais](../email/edit-content.md)

Com essa nova interface, é possível gerenciar a sincronização de modelos de email no Adobe Experience Manager e integrar ao Adobe Experience Manager as a Cloud Service.

Observe que, por enquanto, os recursos a seguir não estão disponíveis na interface do Campaign Web. Use os links fornecidos para navegar pela documentação do Campaign v8 (console do cliente) e saber mais sobre esses recursos.

* **Criação de blocos de personalização individuais**. Além dos blocos de personalização padrão, você pode criar blocos personalizados no console do cliente. Esse recurso não está disponível na interface do Campaign Web. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/personalize/personalization-blocks.html?lang=pt-BR#create-custom-personalization-blocks){target="_blank"}
* **Conteúdo de formulários personalizados**. O módulo de gestão de conteúdo permite criar e gerenciar formulários para ajudar seus usuários a criar conteúdo no Campaign. Esse recurso só está disponível com o console do cliente. [Saiba mais na documentação do Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/content-management/about-content-management.html?lang=pt-BR){target="_blank"}
* **AMP para emails**. O novo formato do AMP permite incluir componentes do AMP em suas mensagens e melhorar a experiência de email com conteúdo relevante e acionável. Esse recurso só está disponível no console do cliente. [Saiba mais na documentação do Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-emails/defining-interactive-content.html?lang=pt-BR){target="_blank"}
<!--
* Content from a URL`*`
* Email fragments`*`
* Multivariant / Multilingual use case`*`-->

## Tipologias e regras de tipologia {#rules-capabilities}

Tipologias são conjuntos de regras executadas durante a fase de preparação para aplicar várias regras de filtragem simultaneamente a uma entrega. Elas permitem que os profissionais de marketing padronizem práticas comerciais em todas as entregas, pois possibilitam controlar, filtrar e priorizar o envio de entregas.

As regras de tipologia podem ser selecionadas para uma entrega ou um modelo de entrega na interface do Campaign Web, conforme detalhado [nesta seção](../advanced-settings/delivery-settings.md#typology). No entanto, a criação, o gerenciamento e a personalização das regras de tipologia só estão disponíveis no console do cliente do Campaign.

Use os links fornecidos para explorar a documentação do Campaign v8 (console do cliente) e saber mais sobre as regras de tipologia:

* Criação de regras de controle. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html?lang=pt-BR){target="_blank"}
* Criação de regras de fadiga e pressão. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=pt-BR){target="_blank"}
* Criação de regras de filtragem. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/filtering-rules.html?lang=pt-BR){target="_blank"}
* Gerenciamento de regras de tipologia. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/apply-rules.html?lang=pt-BR){target="_blank"}
* Simulação de campanha. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-simulations.html?lang=pt-BR){target="_blank"}
* Codificação JavaScript para criação de regras de tipologia. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=pt-BR#use-cases-on-pressure-rules){target="_blank"}

## Fluxos de trabalho {#wf-capabilities}

O Campaign Web traz uma nova interface reformulada da tela do fluxo de trabalho para projetar e gerenciar seus processos. As principais atividades do fluxo de trabalho já estão disponíveis em seu novo design, enquanto algumas serão disponibilizadas em uma atualização futura. Saiba mais sobre os recursos de fluxo de trabalho, incluindo medidas de proteção e limitações [nesta seção](../get-started/guardrails.md).

Observe que os seguintes recursos só estão disponíveis no console do cliente do Campaign:

* Script em workflows
* Atividades de ETL: Exportar, Editar esquema, Carregamento de dados, Extrair dados, Código SQL

Saiba mais sobre as atividades de fluxo de trabalho disponíveis na documentação de fluxo de trabalho do Adobe Campaign v8 (console), acessando [esta página](https://experienceleague.adobe.com/docs/campaign/automation/workflows/wf-activities/activities.html?lang=pt-BR){target="_blank"}.

## Gestão de ofertas {#offer-capabilities}

Você pode enviar ofertas em suas entregas criadas na interface do Adobe Campaign Web. Essas ofertas devem ter sido criadas no console do cliente usando o módulo **[!UICONTROL Interação]**. O design da oferta, as regras de elegibilidade e a gestão de ofertas estão disponíveis somente no console do cliente do Campaign. [Saiba mais](../msg/offers.md)

Saiba como gerenciar um catálogo de ofertas na [documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=pt-BR){target="_blank"}.

## Integrações com as soluções da Adobe Experience Cloud {#exc-capabilities}

A nova interface moderna do Campaign simplifica a criação de campanhas de marketing e a entrega e oferece consistência, além de outras soluções da Adobe, como a Adobe Experience Platform e o Adobe Experience Manager.

As seguintes integrações podem ser acessadas no console do cliente do Adobe Campaign, mas ainda não estão disponíveis na interface do Campaign Web. Use os links fornecidos para explorar a documentação do Campaign v8 (console do cliente) e saber mais sobre essas integrações:

* Uso de dados do Adobe Analytics e compartilhamento de KPI. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html?lang=pt-BR){target="_blank"}
* Compartilhamento de público-alvo com a Adobe Experience Cloud (Adobe Audience Manager). [Saiba mais](https://experienceleague.adobe.com/docs/campaign-classic/using/integrating-with-adobe-experience-cloud/audience-sharing/sharing-audiences-with-adobe-experience-cloud.html?lang=pt-BR){target="_blank"}
* Integração com o Adobe Target. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-at.html?lang=pt-BR){target="_blank"}
* Integração com os Adobe Experience Cloud Triggers. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-triggers.html?lang=pt-BR){target="_blank"}

## Relatórios {#reporting-capabilities}

A nova interface do Campaign Web inclui um conjunto de novos relatórios e KPIs para todos os canais: relatórios de entrega, relatórios de campanha e relatórios globais. Saiba mais [nesta seção](../reporting/gs-reports.md)

Alguns recursos só estão disponíveis no console do cliente. Navegue pelos links fornecidos para encontrar a [documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html?lang=pt-BR){target="_blank"} e saber mais.

* Relatório de capacidade de entrega e renderização da caixa de entrada integrados. [Saiba mais](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/inbox-rendering.html?lang=pt-BR){target="_blank"}
* Personalizações de relatórios. [Saiba mais](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/creating-a-new-report.html?lang=pt-BR){target="_blank"}
* Análise descritiva. [Saiba mais](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/analyzing-populations/about-descriptive-analysis.html?lang=pt-BR){target="_blank"}
* Análise de campanha e relatórios de cubo. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/campaign-v8/analytics/reports/cubes/gs-cubes.html?lang=pt-BR){target="_blank"}
* Compartilhamento de relatórios agendado em PDF, CSV ou por meio de um link [Saiba mais](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/configuring-access-to-the-report.html?lang=pt-BR){target="_blank"}

## Modelagem e ingestão de dados {#data-capabilities}

A interface do Campaign Web não possui os recursos a seguir. Eles só estão disponíveis no console do cliente:

### Contas externas {#external}

O Adobe Campaign inclui um conjunto de contas externas predefinidas para se conectar a sistemas externos. Como admin do sistema do Campaign, você pode criar e gerenciar contas externas somente no console do cliente.[Saiba mais](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/external-accounts.html?lang=pt-BR){target="_blank"}

### Criação e extensão de esquema {#schema}

A criação, modificação e extensão de esquemas são restritas a usuários avançados. Esses recursos só estão disponíveis no console do cliente. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/schemas.html?lang=pt-BR){target="_blank"}

### Recursos de gerenciamento de dados de workflows {#data}

O Gerenciamento de dados combina um conjunto de atividades para resolver problemas complexos de direcionamento, oferecendo ferramentas mais eficientes e flexíveis, como Carregamento de dados, Extração (arquivo), Atualização de dados, Edição de esquema ou Fluxos de trabalho técnicos de Importação/exportação. [Descubra os recursos de gerenciamento de dados de fluxos de trabalho no console do cliente](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html?lang=pt-BR#data-management){target="_blank"}

>[!NOTE]
>
>Embora algumas dessas atividades estejam disponíveis somente no console do cliente, algumas estão disponíveis na interface da Web do Campaign, como **Enriquecimento**, **Carregar arquivo** ou **Alterar dimensão** atividades. [Saiba mais sobre atividades de direcionamento e gerenciamento de dados na interface do usuário da Web do Campaign](../workflows/activities/about-activities.md#targeting)

### Configuração do Federated Data Access {#fda}

A configuração do Campaign e a conexão com sistemas externos são restritas a usuários avançados e só estão disponíveis no console do cliente. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=pt-BR){target="_blank"}

## Aprovações {#approvals-capabilities}

A interface do Campaign Web não permite o gerenciamento de aprovações de conteúdo, entregas, fluxos de trabalho, campanhas e públicos-alvo. Só estão disponíveis no console do cliente.

Saiba como gerenciar aprovações em fluxos de trabalho na [documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/automation/workflows/executing-a-workflow/define-approvals.html?lang=pt-BR){target="_blank"}.


Saiba como gerenciar aprovações de entrega, conteúdo e público-alvo em campanhas na [documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-approval.html?lang=pt-BR){target="_blank"}.


## Permissões {#permissions-capabilities}

Os usuários do Campaign só podem acessar a interface do Campaign Web com sua Adobe ID, por meio do Adobe Identity Management System (IMS). As permissões concedidas a usuários também se aplicam na interface do Campaign Web.

As permissões são definidas no Adobe Admin Console e no console do cliente do Adobe Campaign, conforme detalhado [nesta seção](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html?lang=pt-BR). Não é possível realizar nenhuma ação relacionada a permissões na interface do Adobe Campaign Web.


## Monitoramento {#monitoring-capabilities}

Os recursos de monitoramento da plataforma do Campaign só estão disponíveis no console do cliente e no Painel de controle do Campaign. Eles não estão disponíveis na interface do Campaign Web.

Navegue pelos links fornecidos para a documentação do Campaign v8 (console do cliente) e a documentação do Painel de controle para saber mais.

* [Monitoramento de fluxo de trabalho](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/monitor-technical-workflows.html?lang=pt-BR){target="_blank"}
* [Mapa de calor do fluxo de trabalho](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/heatmap.html?lang=pt-BR){target="_blank"}
* [Monitoramento de desempenho](https://experienceleague.adobe.com/docs/control-panel/using/performance-monitoring/about-performance-monitoring.html?lang=pt-BR){target="_blank"}
* [Monitoramento da capacidade de entrega](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/monitoring-deliverability.html?lang=pt-BR){target="_blank"}




