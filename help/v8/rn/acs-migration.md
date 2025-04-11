---
audience: end-user
title: Transição do Campaign Standard para o Adobe Campaign Web
description: Conheça a interface do Campaign Web
exl-id: 4cf406af-4cf5-434d-b1c7-a7c102f8dc2f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 16%

---

# Transição do Campaign Standard para o Campaign v8 {#acs-to-ac}

Os usuários do Adobe Campaign Standard agora estão qualificados para a transição para o Adobe Campaign Managed Cloud Services v8. Essa transição oferece vários benefícios:

* **Infraestrutura de TI robusta**: o Managed Cloud Services v8 fornece uma infraestrutura de TI mais robusta, garantindo melhor desempenho, confiabilidade e escalabilidade para campanhas.
* **Suporte aprimorado**: a equipe do Managed Cloud Services oferece assistência de alto nível para garantir uma transição suave e um monitoramento contínuo da plataforma. O suporte inclui solução de problemas e manutenção proativa.
* **Integração com o Adobe Experience Platform**: o Managed Cloud Services v8 se conecta perfeitamente com o Adobe Experience Platform, permitindo que os usuários aproveitem seus dados e entreguem campanhas personalizadas e de impacto em todos os canais.
* **Experiência e interface de usuário consistentes**: a transição para o Managed Cloud Services v8 não interrompe os fluxos de trabalho. Os usuários continuam aproveitando a interface e a experiência familiares, minimizando a curva de aprendizado das equipes.

**Como usuário do Campaign Standard em transição para o Campaign v8, saiba como iniciar [neste documento](../../adoption/home.md).**

<!--
As a Campaign Standard user, we now offer you a way to migrate to Adobe Campaign v8. You will benefit from both the new Campaign Web interface and the v8 console.
-->

## Principais recursos {#key-features}

Os usuários do Campaign v8 têm acesso à nova interface da Web do Campaign e ao console v8. Os dados e as configurações são sincronizados entre ambientes. Todos os dados e configurações disponíveis no console do cliente estão visíveis na interface da Web do Campaign, acessível na navegação à esquerda do Explorer. [Saiba mais](../get-started/user-interface.md#user-interface-explorer)

A interface da Web do Campaign foi projetada para que os profissionais de marketing criem e orquestrem campanhas com facilidade. Os principais recursos da interface do usuário da Web do Campaign v8 incluem:

* **Experiência moderna, amigável e unificada**. [Saiba mais](../get-started/connect-to-campaign.md).
* **Novos recursos avançados e processos simples**. [Saiba mais](../get-started/user-interface.md).
* **Modelador de consultas simplificado e intuitivo**. [Saiba mais](../query/query-modeler-overview.md).
* **Recursos internos de gerenciamento de campanhas em vários canais**. [Saiba mais](../msg/gs-messages.md).
* **Atividades de fluxo de trabalho de campanha reprojetadas**. [Saiba mais](../workflows/gs-workflows.md).
* **Fácil criação e gerenciamento de perfis**. [Saiba mais](../audience/about-recipients.md).
* **Filtros predefinidos**. [Saiba mais](../get-started/predefined-filters.md).
* **Conversor do HTML para design de email**. [Saiba mais](../email/existing-content.md).
* **SMS com ofertas**. [Saiba mais](../msg/offers.md).

O console do cliente do Campaign foi projetado para administradores e desenvolvedores configurarem e personalizarem o ambiente. Os principais recursos disponíveis no console do cliente do Campaign estão detalhados em [esta documentação](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/new/whats-new){target="_blank"}.

>[!NOTE]
>
>Saiba mais sobre os recursos compatíveis e não compatíveis e a interoperabilidade entre a interface de usuário da Web do Campaign e o console do cliente do Campaign [nesta página](../get-started/capability-matrix.md).

## Terminologia {#terminology}

A maioria dos conceitos são semelhantes entre o Campaign v8 e o Campaign Standard. No entanto, existem algumas diferenças de terminologia. Os exemplos incluem:

<!--
* Profiles are **Recipients** in the console. [Learn more](../audience/gs-audiences-recipients.md).
* Test profiles are **Seed addresses**. [Learn more](../preview-test/test-deliveries.md).
* The delivery preparation is the **Delivery analysis**. [Learn more](../monitor/prepare-send.md).
* Audiences are **Lists**. [Learn more](../audience/gs-audiences-recipients.md).
-->

<!--
* Custom resources are **Schemas**
* Messages are referred to as **Deliveries**
* Roles are configured with **Named Rights**
* Security Groups are **Operator Groups**
* Organizational units are managed through **Folder Permissions**
* Product users are **Operators** in the client console
* Delivery preparation is the **Delivery analysis** in the client console
-->

## Recursos específicos {#new-features}

Para garantir uma transição suave para o Campaign v8, os principais recursos do Campaign Standard foram adicionados ao Campaign v8. Estes recursos estão detalhados em [esta documentação](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=pt-BR){target="_blank} e estão disponíveis somente para usuários em transição do Campaign Standard.

* **Dynamic Reporting**: o Dynamic Reporting fornece relatórios personalizáveis em tempo real para medir o impacto das atividades de marketing. Ele inclui acesso aos dados do perfil para análise demográfica por dimensões, como gênero, cidade e idade, juntamente com dados funcionais de campanha de email, como aberturas e cliques. [Saiba mais](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html?lang=pt-BR){target="_blank"}.

* **Marcas centralizadas**: o Adobe Campaign permite que as empresas definam diretrizes técnicas e visuais da marca. Os usuários podem apresentar uma marca consistente aos clientes, desde logotipos a aspectos técnicos, como remetente de email, URL ou domínios. [Saiba mais](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=pt-BR).

* **REST APIs**: os usuários migrados do Campaign Standard podem usar as REST APIs para criar integrações com o Adobe Campaign e criar ecossistemas, conectando o Adobe Campaign a outras tecnologias. [Saiba mais](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=pt-BR){target="_blank"}.

* **Páginas de aterrissagem**: as páginas de aterrissagem do Campaign v8 incluem melhorias para garantir a paridade de recursos com o Campaign Standard. Saiba mais nas[ notas de versão](../rn/release-notes.md#new-24-4) e na [documentação](../landing-pages/get-started-lp.md) da página de destino.

* **Fragmentos visuais**: os fragmentos visuais são componentes visuais reutilizáveis referenciados em uma ou mais entregas de email ou modelos de conteúdo. Modificar um fragmento atualiza todo o conteúdo usando-o. Essa funcionalidade permite que os usuários de marketing pré-criem vários blocos de conteúdo personalizados para a montagem rápida de mensagens em um processo de design aprimorado. [Saiba mais](../content/use-visual-fragments.md).

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->