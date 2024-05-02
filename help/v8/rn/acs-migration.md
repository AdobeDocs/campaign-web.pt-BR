---
audience: end-user
title: Transição do Campaign Standard para o Adobe Campaign Web
description: Conheça a interface da Web do Campaign
source-git-commit: 4c1f68f0e89b2b84b8845b2759ef3b0dc9b12033
workflow-type: tm+mt
source-wordcount: '593'
ht-degree: 7%

---


# Transição de Campaign Standard para o Campaign v8{#welcome}

<!--
We are thrilled to annonce that you, as a Campaign Standard user, can now benefit from the new version of Adobe Campaign Web User Interface. The migration is seemless and will allow you to use all the intuitive features designed to simplify the creation of personalized cross-channel campaigns. Campaign Web User Interface also brings a connected canvas with Adobe Experience Platform for a unified experience.
-->

Bem-vindo ao Adobe Campaign Managed Cloud Services v8.

Estamos animados em anunciar que os usuários do Adobe Campaign Standard agora estão qualificados para a transição para o Adobe Campaign Managed Cloud Services v8. Essa transição traz muitos benefícios:

* Infraestrutura de TI robusta: com o Managed Cloud Service v8, os clientes podem utilizar uma infraestrutura de TI mais robusta, garantindo desempenho, confiabilidade e escalabilidade aprimorados para suas campanhas.
* Suporte aprimorado: nossa equipe de Cloud Service gerenciados tem o compromisso de fornecer assistência de primeira linha para garantir uma transição suave e o monitoramento contínuo de sua plataforma. Desde a solução de problemas até a manutenção proativa, temos a solução para você.
* Integração com o Adobe Experience Platform: o Managed Cloud Service v8 se conecta perfeitamente com o Adobe Experience Platform, permitindo que os clientes aproveitem todo o potencial de seus dados e ofereçam campanhas personalizadas e de impacto em todos os canais.
* Interface do usuário e experiência consistentes: tenha certeza de que a transição para o Managed Cloud Service v8 não interromperá seu fluxo de trabalho. Você continuará desfrutando da interface de usuário familiar e da experiência do usuário, garantindo uma curva de aprendizado mínima para sua equipe.

<!--
As a Campaign Standard user, we now offer you a way to migrate to Adobe Campaign v8. You will benefit from both the new Campaign Web interface and the v8 console.
-->

## Principais recursos {#key-features}

Vamos detalhar quais recursos principais o Campaign v8 oferecerá:

* Experiência moderna, amigável e unificada. [Saiba mais](../get-started/connect-to-campaign.md).
* Novos recursos poderosos e processos ininterruptos. [Saiba mais](../get-started/user-interface.md)
* Novo modelador de consultas simplificado e intuitivo. [Saiba mais](../query/query-modeler-overview.md)
* Recursos integrados de gerenciamento de campanhas em vários canais. [Saiba mais](../msg/gs-messages.md)
* Atividades de workflow de campanha novas e reprojetadas. [Saiba mais](../workflows/gs-workflows.md)
* Público-alvo com o modelador de consultas. [Saiba mais](../query/query-modeler-overview.md)
* Fácil criação e gerenciamento de perfis. [Saiba mais](../audience/about-recipients.md)
* Ajuda contextual baseada em IA. [Saiba mais](../get-started/using-ai.md)
* Filtros predefinidos. [Saiba mais](../get-started/predefined-filters.md)
* Conversor de HTML para design de email. [Saiba mais](../email/existing-content.md)
* SMS com ofertas. [Saiba mais](../msg/offers.md)

## Console e interface da Web {#console}

Como usuário do Campaign v8, você terá acesso à nova interface da Web do Campaign e ao console do v8. Os dados e as configurações são sincronizados de um ambiente para outro. Todos os dados e configurações disponíveis no console do cliente estão visíveis na interface da Web do Campaign, a partir da navegação à esquerda do Explorer. [Saiba mais](../get-started/user-interface.md#user-interface-explorer)

Recursos compatíveis e não compatíveis e interoperabilidade entre a interface da Web do Campaign e o console do cliente do Campaign [nesta página](../get-started/capability-matrix.md)

## Terminologia {#terminology}

A maioria dos conceitos é semelhante entre a interface da Web do Campaign e o Campaign Standard. No entanto, existem algumas diferenças. Estes são alguns exemplos de diferenças de terminologia entre o Campaign Standard e a interface da Web do Campaign:

<!--
* Profiles are **Recipients** in the console. [Learn more](../audience/gs-audiences-recipients.md).
* Test profiles are **Seed addresses**. [Learn more](../preview-test/test-deliveries.md).
* The delivery preparation is the **Delivery analysis**. [Learn more](../monitor/prepare-send.md).
* Audiences are **Lists**. [Learn more](../audience/gs-audiences-recipients.md).
-->

* Os recursos personalizados são **Esquemas** na interface da Web do Campaign.
* As atividades de marketing não existem mais.
* As mensagens são **Entregas**.
* Os operadores são **Usuários**.
* Os direitos nomeados são **Funções**.
* Os grupos de operadores são **Grupos de Segurança**.
* As permissões de pasta são **Unidades organizacionais**

## Novos recursos {#new-features}

Para poder fazer a transição, adicionamos [principais recursos](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html) do Campaign Standard para a v8:

* **Relatórios dinâmicos**: o Dynamic Reporting fornece relatórios totalmente personalizáveis e em tempo real para medir o impacto de suas atividades de marketing. Ele adiciona acesso aos dados do perfil, permitindo a análise demográfica por dimensões de perfil, como gênero, cidade e idade, além de dados funcionais de campanha de email, como aberturas e cliques. [Saiba mais](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html)

* **Marca centralizada**: todas as empresas têm diretrizes técnicas e visuais da marca. Com o Adobe Campaign, você pode definir um conjunto de especificações para apresentar uma marca consistente aos seus clientes, de logotipos a aspectos técnicos, como remetente de email, URL ou domínios. [Saiba mais](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html)

* **Rest APIs** - Como usuário migrado do Campaign Standard, você pode usar as APIs Rest para criar integrações com o Adobe Campaign e criar seu próprio ecossistema, conectando o Adobe Campaign ao painel de tecnologias que você usa. [Saiba mais](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html)

* **Landing pages** - Muitas melhorias foram trazidas para o Campaign v8 para garantir que você não perca nenhum recurso. Saiba mais na [notas de versão](../rn/release-notes.md#new-24-4) e a landing page [documentação](../landing-pages/get-started-lp.md).

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->