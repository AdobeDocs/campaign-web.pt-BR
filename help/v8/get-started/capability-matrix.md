---
audience: end-user
title: Matriz de recursos da interface do usuário da Web/console do cliente do Campaign
description: Lista de recursos compatíveis com a interface da Web do Campaign
exl-id: 4bcac01f-be1d-497c-937d-0c82f0d6b17d
source-git-commit: 45e5b528837614cdbd537d0a92e71265f65f97db
workflow-type: tm+mt
source-wordcount: '2151'
ht-degree: 3%

---

# Console do cliente do Campaign e da Web do Campaign {#capabilities-matrix}

Os principais recursos do Campaign estão disponíveis na interface da Web do Campaign. Essa interface foi projetada principalmente para que os profissionais de marketing planejem, iniciem e avaliem suas campanhas de marketing. Todos os recursos estão listados [nesta página](../rn/whats-new.md).

A personalização da plataforma do Campaign com base nas necessidades de negócios e dados, e a conexão com outros sistemas são gerenciadas no console do cliente do Campaign. Como consequência, alguns recursos e configurações só podem ser acessados, criados ou gerenciados no console do cliente do Campaign. Alguns estarão disponíveis em uma atualização posterior da interface da Web do Campaign.

<!--
**Homepage**

* Home page dashboard
* Home page customization-->

## Gerenciamento de campanhas {#campaign-mgt-capabilities}

Com a interface da Web do Campaign, é possível criar campanhas entre canais conforme detalhado [nesta seção](../campaigns/gs-campaigns.md). Os recursos a seguir estão disponíveis somente no console do cliente do Campaign. Eles não podem ser acessados na interface da Web do Campaign, mas alguns podem ser visualizados no [Menu Explorer](user-interface.md#user-interface-explorer).

Use os links fornecidos para navegar pela documentação do Campaign v8 (console do cliente) e saber como usar esses recursos.

* **Calendário de marketing**. O calendário da campanha mostra todos os programas, planos, campanhas e deliveries em uma linha do tempo global. Esse recurso só está disponível no console do cliente. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html#campaign-calendar){target="_blank"}
* **Programas e planos**. Cada campanha pertence a um programa que pertence a um plano. Na interface do usuário da Web do Campaign, todas as campanhas são associadas a um plano e programa incorporados padrão. Você só pode criar e gerenciar planos e programas no console do cliente. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html#work-with-plan-and-program){target="_blank"}
* **Provedores, orçamento e gerenciamento de custos**. Você pode configurar provedores de serviços envolvidos nas tarefas realizadas em suas campanhas, incluindo estruturas de custo, e gerenciar seus orçamentos em cada programa e campanha. Esse recurso só está disponível no console do cliente. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/providers--stocks-and-budgets.html){target="_blank"}
* **Marketing distribuído** (Marketing central/local). O Adobe Campaign oferece um aplicativo de Marketing distribuído para implementar campanhas cooperativas entre entidades centrais (sede, departamentos de marketing etc.) e entidades locais (pontos de vendas, agências regionais etc.). Esse recurso só está disponível no console do cliente. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/automation/distributed-marketing/about-distributed-marketing.html?lang=pt-BR){target="_blank"}
* **Gerenciamento de recursos de marketing** (MRM), metas, simulações e controle de custos. O Adobe Campaign oferece um aplicativo de Gestão de Recursos de Marketing (MRM) que permite controlar ações de marketing em um modo colaborativo fornecendo gerenciamento completo e rastreamento em tempo real das tarefas, orçamentos e recursos de marketing envolvidos. Esse recurso só está disponível no console do cliente. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/automation/mrm/about-marketing-resource-management.html){target="_blank"}
* **Gerenciamento de tarefas**. Como parte do aplicativo MRM, as tarefas do Campaign podem ser criadas, atribuídas, rastreadas e monitoradas no painel de campanha. Esse recurso só está disponível no console do cliente. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/automation/mrm/creating-and-managing-tasks.html){target="_blank"}

## Canais de comunicação {#channels-capabilities}

Com a interface da Web do Campaign, você pode criar, projetar e enviar **email**, **SMS** e **notificações por push** e medir seu impacto usando vários relatórios exclusivos, conforme detalhado [nesta seção](../msg/gs-messages.md). No entanto, os seguintes canais estão **não** disponível: no aplicativo, correspondência direta, LINE, Call center/canal personalizado, marketing social com X (Twitter).

Use os links fornecidos para navegar pela documentação do Campaign v8 (console do cliente) e saber mais sobre esses canais.

* **Correspondência direta**. O canal de correspondência direta permite enviar uma correspondência física aos clientes, fornecedores ou outros, como avisos, faturas, demonstrativos, ofertas de marketing e muito mais. Este canal só está disponível no console do cliente.  [Saiba mais](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-direct-mail/about-direct-mail-channel.html){target="_blank"}
* **Mensagens LINE**. O LINE é um aplicativo para mensagens instantâneas, chamadas de voz e vídeo gratuitos, disponível em todos os dispositivos móveis e no PC. O Adobe Campaign permite enviar mensagens LINE somente a partir do console do cliente. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/line.html){target="_blank"}
* **Call center e canais personalizados**. A central de atendimento e outros canais personalizados podem ser implementados em seu ambiente do Campaign. Esses canais só podem estar disponíveis no console do cliente. [Saiba mais na documentação do Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/communication-channels.html#other-channels){target="_blank"}
* **Marketing social** com X (Twitter). Você interage com seus clientes via X (Twitter) postando mensagens e enviando mensagens diretas. Esse recurso, que vem com o complemento Social Marketing, só está disponível no console do cliente - [Saiba mais](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-tw.html?lang=pt-BR){target="_blank"}

## Landing pages e aplicações web {#Webapps-capabilities}

O Adobe Campaign permite criar, projetar e compartilhar páginas de aterrissagem. A experiência das páginas de destino foi totalmente reimaginada na nova interface. Descubra como criar, projetar e publicar uma página de aterrissagem na interface da Web do Campaign [nesta seção](../landing-pages/get-started-lp.md).

Como consequência, no console do cliente do Campaign, não é possível editar, atualizar ou modificar uma landing page criada na interface da Web, e vice-versa. Os seguintes tipos de aplicativos Web não estão disponíveis na interface do usuário da Web do Campaign. No entanto, elas estão visíveis na lista de páginas de aterrissagem. Use os links fornecidos para navegar pela documentação do Campaign Classic v7 e saber mais sobre estes aplicativos web:

* **Aplicações web**. O Adobe Campaign permite criar e publicar aplicações web dinâmicas e interativas com dados pré-carregados do banco de dados e conteúdo adaptado aos direitos do usuário conectado. Esse recurso só está disponível no console do cliente. [Saiba mais na documentação do Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-applications/about-web-applications.html){target="_blank"}
* **Formulários web**. As páginas da Web e de aterrissagem criadas no console do cliente estão visíveis na interface do usuário da Web do Campaign, mas não podem ser editadas ou modificadas. Algumas opções podem diferir entre o designer da página da Web do console do cliente e o designer da página de aterrissagem que vem com a interface do usuário da Web do Campaign. [Saiba mais na documentação do Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-forms/about-web-forms.html?lang=pt-BR){target="_blank"}
* **Pesquisas online**. Você pode criar pesquisas online e coletar respostas somente do console do cliente. Esse recurso não está disponível na interface da Web do Campaign.  [Saiba mais na documentação do Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/online-surveys/about-surveys.html){target="_blank"}


## Perfis, perfis de teste e públicos {#profiles-audiences-capabilities}

Você pode criar, gerenciar e atualizar perfis e perfis de teste no console do cliente do Campaign e na interface do usuário da Web do Campaign. Todas as alterações executadas em uma interface do usuário são visíveis na outra. No entanto, algumas configurações específicas de recipient e parâmetros avançados podem estar ausentes na nova interface do usuário da Web do Campaign.

Observe que o termo &quot;recipient&quot; foi alterado para &quot;profile&quot; na nova interface do usuário da Web e &quot;Seed addresses&quot; agora são &quot;Test profiles&quot;

<!--Audience composition is a new capability coming with Campaign Web user interface. As a consequence, in Campaign client console, you cannot edit, update or modify an [audience created with the Query modeler](../query/query-modeler-overview.md). -->

Todos os públicos-alvo criados no console do cliente do Campaign ou no Adobe Experience Platform estão disponíveis na interface da Web do Campaign.

Trabalhos de importação/exportação de uma só vez, conforme descrito em [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/import-profiles.html#import-jobs){target="_blank"} não estão disponíveis na interface da Web do Campaign. <!--To import profiles into Campaign Web user interface, you must create a workflow as detailed in [this section]().-->

## Mensagens transacionais {#mc-capabilities}

Os recursos de mensagens transacionais que acompanham o pacote de produtos do Centro de mensagens não estão disponíveis na nova interface do usuário da Web do Campaign.

Navegue pelo [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/real-time/transactional.html){target="_blank"} e saiba mais sobre os recursos de mensagens em tempo real, como:

* Criação e execução de mensagens em tempo real por email, SMS e push
* Enriquecimento e personalização de mensagem
* Relatórios e monitoramento de mensagens transacionais

## Design de conteúdo {#content-capabilities}

O novo Email Designer que vem com a interface de usuário da Adobe Campaign Web permite criar e-mails atraentes e personalizados por meio de uma interface intuitiva de arrastar e soltar. Esteja você iniciando do zero, importando um conteúdo existente ou utilizando modelos existentes, é possível projetar e refinar todo o conteúdo de cada email. [Saiba mais](../email/edit-content.md)

Com essa nova interface do usuário, é possível gerenciar a sincronização de modelos de email no Adobe Experience Manager e integrar ao Adobe Experience Manager as a Cloud Service.

Observe que os recursos a seguir não estão disponíveis por enquanto na interface do usuário da Web do Campaign. Use os links fornecidos para navegar pela documentação do Campaign v8 (console do cliente) e saber mais sobre esses recursos.

* **Criação de bloco de personalização personalizado**. Além dos blocos de personalização padrão, você pode criar blocos personalizados no console do cliente. Esse recurso não está disponível na interface da Web do Campaign. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/personalize/personalization-blocks.html#create-custom-personalization-blocks){target="_blank"}
* **Conteúdo de formulários personalizados**. O módulo de Gestão de conteúdo permite criar e gerenciar formulários para ajudar seus usuários a criar conteúdo no Campaign. Esse recurso só está disponível com o console do cliente. [Saiba mais na documentação do Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/content-management/about-content-management.html){target="_blank"}
* **AMP para emails**. O novo formato do AMP for Email permite incluir componentes do AMP em suas mensagens e melhorar a experiência de email com um conteúdo rico e acionável. Esse recurso só está disponível no console do cliente. [Saiba mais na documentação do Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-emails/defining-interactive-content.html){target="_blank"}
<!--
* Content from a URL`*`
* Email fragments`*`
* Multivariant / Multilingual use case`*`-->

## Tipologias e regras de tipologia {#rules-capabilities}

Tipologias são conjuntos de regras de tipologia executadas durante a fase de preparação para aplicar facilmente várias regras de filtragem a uma entrega de uma vez. Eles permitem que os profissionais de marketing padronizem práticas comerciais em todos os deliveries, pois permitem controlar, filtrar e priorizar o envio de deliveries.

As regras de tipologia podem ser selecionadas para um delivery ou um template de delivery na interface do usuário da Web do Campaign, conforme detalhado [nesta seção](../advanced-settings/delivery-settings.md#typology). No entanto, a criação, o gerenciamento e a personalização das regras de tipologia e da tipologia só estão disponíveis no console do cliente do Campaign.

Use os links fornecidos para procurar a documentação do Campaign v8 (console do cliente) e saber mais sobre as regras de tipologia:

* Criação de regras de controle. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html){target="_blank"}
* Criação de regras de fadiga/pressão. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=pt-BR){target="_blank"}
* Criação de regras de filtragem. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/filtering-rules.html){target="_blank"}
* Gerenciamento de regras de tipologia. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/apply-rules.html){target="_blank"}
* Simulação de campanha. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-simulations.html){target="_blank"}
* Codificação JavaScript para criação de regras de tipologia. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html#use-cases-on-pressure-rules){target="_blank"}

## Workflows {#wf-capabilities}

A nova interface do usuário da Web do Campaign traz uma interface reformulada da tela do fluxo de trabalho para projetar e gerenciar seus processos. As principais atividades do fluxo de trabalho já estão disponíveis em seu novo design. Algumas serão disponibilizadas em uma atualização futura. Saiba mais sobre os recursos de fluxo de trabalho, incluindo medidas de proteção e limitações [nesta seção](../get-started/guardrails.md).

Observe que os seguintes recursos só estão disponíveis no console do cliente do Campaign:

* Script em workflows
* Atividades de ETL: Exportar, Editar esquema, Carregamento de dados, Extrair dados, Código SQL

Saiba mais sobre atividades de fluxo de trabalho disponíveis na documentação de fluxo de trabalho do Adobe Campaign v8 (console) [aqui](https://experienceleague.adobe.com/docs/campaign/automation/workflows/wf-activities/activities.html){target="_blank"}.

## Gerenciamento de ofertas {#offer-capabilities}

Você pode enviar ofertas em seus deliveries criados na interface do usuário da Web do Adobe Campaign. Essas ofertas devem ter sido criadas no console do cliente usando o **[!UICONTROL Interação]** módulo. O design da oferta, as regras de qualificação e o gerenciamento de ofertas estão disponíveis somente no console do cliente do Campaign. [Saiba mais](../msg/offers.md)

Saiba como gerenciar um catálogo de ofertas na [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=pt-BR){target="_blank"}.

## Integrações com as soluções da Adobe Experience Cloud {#exc-capabilities}

A nova interface moderna do Campaign simplifica o design e o delivery de campanhas de marketing, além de oferecer consistência com outras soluções de Adobe, incluindo Adobe Experience Platform e Adobe Experience Manager.

As seguintes integrações estão disponíveis no console do cliente Adobe Campaign e ainda não estão disponíveis na interface da Web do Campaign. Use os links fornecidos para navegar pela documentação do Campaign v8 (console do cliente) e saber mais sobre essas integrações:

* Uso de dados do Adobe Analytics e compartilhamento de KPI. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html){target="_blank"}
* Compartilhamento de público com a Adobe Experience Cloud (Adobe Audience Manager). [Saiba mais](https://experienceleague.adobe.com/docs/campaign-classic/using/integrating-with-adobe-experience-cloud/audience-sharing/sharing-audiences-with-adobe-experience-cloud.html){target="_blank"}
* Integração com o Adobe Target. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-at.html){target="_blank"}
* Integração com o Adobe Experience Cloud Triggers. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-triggers.html){target="_blank"}

## Relatórios {#reporting-capabilities}

A nova interface do usuário da Web do Campaign vem com um conjunto de novos relatórios e KPIs para todos os canais: relatórios de delivery, relatórios de campanha e relatórios globais. Saiba mais [nesta seção](../reporting/gs-reports.md)

Alguns recursos só estão disponíveis no console do cliente. Navegue pelos links fornecidos para navegar pelo [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html?lang=pt-BR){target="_blank"} e saiba mais.

* Relatório de capacidade de entrega e renderização da caixa de entrada integrados. [Saiba mais](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/inbox-rendering.html){target="_blank"}
* Personalizações de relatórios. [Saiba mais](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/creating-a-new-report.html){target="_blank"}
* Análise descritiva. [Saiba mais](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/analyzing-populations/about-descriptive-analysis.html){target="_blank"}
* Análise de campanha/Relatórios de cubo. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/campaign-v8/analytics/reports/cubes/gs-cubes.html?lang=pt-BR){target="_blank"}
* Compartilhamento de relatórios de acordo com a programação como um PDF e CSV ou link. [Saiba mais](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/configuring-access-to-the-report.html){target="_blank"}

## Modelagem e assimilação de dados {#data-capabilities}

A interface da Web do Campaign não exibe os recursos a seguir. Eles só estão disponíveis no console do cliente.

Navegue pelos links fornecidos na [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html?lang=pt-BR){target="_blank"} para saber mais.

* **Contas externas**. O Adobe Campaign vem com um conjunto de contas externas predefinidas para se conectar com sistemas externos. Como administrador do sistema do Campaign, você pode criar e gerenciar contas externas somente do console do cliente.[Saiba mais](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/external-accounts.html){target="_blank"}
* **Criação e extensão de esquema**. A criação, a modificação e a extensão de esquema são restritas aos usuários avançados. Esses recursos só estão disponíveis no console do cliente. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/schemas.html){target="_blank"}
* **Gestão de dados** atividades de workflow. O Gerenciamento de dados combina um conjunto de atividades para resolver problemas complexos de definição de metas oferecendo ferramentas mais eficientes e flexíveis. Essas atividades incluem: carregamento de dados, extração (arquivo), atualização de dados, edição de esquema e importação/exportação de workflows técnicos. Eles só estão disponíveis no console do cliente. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#data-management){target="_blank"}
* **Federated Data Access**. A configuração do Campaign e a conexão com sistemas externos são restritas a usuários avançados e só estão disponíveis no console do cliente. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=pt-BR){target="_blank"}

## Aprovações {#approvals-capabilities}

A interface da Web do Campaign não exibe o gerenciamento de aprovação para conteúdo, deliveries, workflows, campanhas e targets. Eles só estão disponíveis no console do cliente.

Saiba como gerenciar aprovações em workflows na [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/automation/workflows/executing-a-workflow/define-approvals.html){target="_blank"}.


Saiba como gerenciar aprovações de entrega, conteúdo e público-alvo em campanhas no [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-approval.html){target="_blank"}.


## Permissões {#permissions-capabilities}

Os usuários do Campaign só podem acessar a interface da Web do Campaign com sua Adobe ID, por meio do Adobe Identity Management System (IMS). As permissões concedidas aos usuários também se aplicam à interface da Web do Campaign.

As permissões são definidas no console do cliente do Adobe Admin Console e do Adobe Campaign, conforme detalhado [nesta seção](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html?lang=pt-BR). Nenhuma ação sobre permissões é possível na interface da Web do Adobe Campaign.


## Monitoramento {#monitoring-capabilities}

Os recursos de monitoramento da plataforma do Campaign só estão disponíveis no console do cliente e no Painel de controle do Campaign. Eles não aparecem na interface da Web do Campaign.

Navegue pelos links fornecidos para a documentação do Campaign v8 (console do cliente) e a documentação do Painel de controle para saber mais.

* [Monitoramento de workflow](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/monitor-technical-workflows.html){target="_blank"}
* [Mapa de calor do fluxo de trabalho](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/heatmap.html){target="_blank"}
* [Monitoramento de desempenho](https://experienceleague.adobe.com/docs/control-panel/using/performance-monitoring/about-performance-monitoring.html?lang=pt-BR){target="_blank"}
* [Monitoramento da capacidade de entrega](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/monitoring-deliverability.html){target="_blank"}




