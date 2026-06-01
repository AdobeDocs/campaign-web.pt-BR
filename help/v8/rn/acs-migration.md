---
audience: end-user
title: Transição do Campaign Standard para o Adobe Campaign Web
description: Conheça a interface do Campaign Web
exl-id: 4cf406af-4cf5-434d-b1c7-a7c102f8dc2f
TQID: https://experienceleague.adobe.com/nD7hOr0bHeBrGYrxutHio-M2EEJM4mYPVoaPelYzJXs
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2: id: a075b2c1-7748-4328-b7f6-343aa314616aid: b12f6872-9271-4369-85e5-86969a0b99a2id: c309ee4e-82e4-4f7e-b608-ef345678c34eid: d5ef99fa-df0c-4153-bf94-105ad0724167
subfeature_v2: id: bf97c196-a4d1-4fa3-a151-e68a114c8ac0
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 096132b46c985e1b23ca0fc6fbcf06a70e1630c7
workflow-type: tm+mt
source-wordcount: 570
ht-degree: 96%

---

# Transição do Campaign Standard para o Campaign v8 {#acs-to-ac}

Os usuários do Adobe Campaign Standard agora podem fazer a transição para o Adobe Campaign Managed Cloud Services v8. Essa transição oferece vários benefícios:

* **Infraestrutura de TI robusta**: o Managed Cloud Services v8 fornece uma infraestrutura de TI mais robusta, garantindo melhor desempenho, confiabilidade e escalabilidade para campanhas.
* **Suporte aprimorado**: a equipe do Managed Cloud Services oferece assistência de alto nível para garantir transições descomplicadas e monitoramento contínuo da plataforma. O suporte inclui solução de problemas e manutenção proativa.
* **Integração com a Adobe Experience Platform**: o Managed Cloud Services v8 se conecta perfeitamente com a Adobe Experience Platform, permitindo que os usuários aproveitem seus dados ao máximo e entreguem campanhas personalizadas e impactantes em todos os canais.
* **Interface e experiência consistentes**: a transição para o Managed Cloud Services v8 não interrompe os fluxos de trabalho. Os usuários continuam a desfrutar de uma interface e experiência familiares, minimizando a curva de aprendizado das equipes.

**Caso seja um usuário do Campaign Standard que está migrando para o Campaign v8, saiba como começar [neste documento](../../adoption/home.md).**

<!--
As a Campaign Standard user, we now offer you a way to migrate to Adobe Campaign v8. You will benefit from both the new Campaign Web interface and the v8 console.
-->

## Principais recursos {#key-features}

Como usuário do Campaign v8, você terá acesso à nova interface do Campaign Web e ao console da v8. Os dados e as configurações são sincronizados entre ambientes. Todos os dados e configurações disponíveis no console do cliente ficam visíveis na interface do Campaign Web, acessível pela navegação à esquerda do Explorer. [Saiba mais](../get-started/user-interface.md#user-interface-explorer)

A interface do Campaign Web foi projetada para que profissionais de marketing possam criar e orquestrar campanhas facilmente. Os principais recursos da interface do Campaign Web v8 incluem:

* **Experiência moderna, intuitiva e unificada**. [Saiba mais](../get-started/connect-to-campaign.md).
* **Novos recursos avançados e processos contínuos**. [Saiba mais](../get-started/user-interface.md).
* **Modelador de consulta simplificado e intuitivo**. [Saiba mais](../query/query-modeler-overview.md).
* **Recursos integrados de gerenciamento de campanhas entre canais**. [Saiba mais](../msg/gs-messages.md).
* **Atividades de fluxo de trabalho de campanha redesenhadas**. [Saiba mais](../workflows/gs-workflows.md).
* **Fácil criação e gerenciamento de perfis**. [Saiba mais](../audience/about-recipients.md).
* **Filtros predefinidos**. [Saiba mais](../get-started/predefined-filters.md).
* **Conversor de HTML para design de email**. [Saiba mais](../email/existing-content.md).
* **SMS com ofertas**. [Saiba mais](../msg/offers.md).

O console do cliente do Campaign foi projetado para que admins e desenvolvedores configurem e personalizem seus ambientes. Os principais recursos disponíveis no console do cliente do Campaign estão detalhados [nesta documentação](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/new/whats-new){target="_blank"}.

>[!NOTE]
>
>Saiba mais sobre os recursos compatíveis e incompatíveis e a interoperabilidade entre a interface do Campaign Web e o console do cliente do Campaign [nesta página](../get-started/capability-matrix.md).

<!--
## Terminology {#terminology}
Most concepts are similar between Campaign v8 and Campaign Standard. However, there are a few terminology differences. Examples include:
* Profiles are **Recipients** in the console. [Learn more](../audience/gs-audiences-recipients.md).
* Test profiles are **Seed addresses**. [Learn more](../preview-test/test-deliveries.md).
* The delivery preparation is the **Delivery analysis**. [Learn more](../monitor/prepare-send.md).
* Audiences are **Lists**. [Learn more](../audience/gs-audiences-recipients.md).
* Custom resources are **Schemas**
* Messages are referred to as **Deliveries**
* Roles are configured with **Named Rights**
* Security Groups are **Operator Groups**
* Organizational units are managed through **Folder Permissions**
* Product users are **Operators** in the client console
* Delivery preparation is the **Delivery analysis** in the client console
-->

## Recursos específicos {#new-features}

Para garantir uma transição tranquila para o Campaign v8, os principais recursos do Campaign Standard foram adicionados ao Campaign v8:

* **Relatórios dinâmicos**: fornecem relatórios personalizáveis em tempo real para medir o impacto das atividades de marketing. Inclui acesso a dados de perfil para análise demográfica por dimensões como gênero, cidade e idade, além de dados funcionais de campanhas de email, como aberturas e cliques. [Saiba mais](../reporting/dynamic-reporting/get-started-reporting.md).

* **Marcas centralizadas**: o Adobe Campaign permite que as empresas definam as diretrizes técnicas e visuais da marca. Os usuários podem apresentar uma marca consistente aos clientes, desde logotipos a aspectos técnicos, como remetente de email, URL ou domínios. [Saiba mais](../administration/branding/branding-gs.md).

* **APIs REST**: os usuários que migraram do Campaign Standard podem usar as APIs REST para criar integrações com o Adobe Campaign e produzir ecossistemas, conectando o Adobe Campaign a outras tecnologias. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=pt-BR){target="_blank"}.

* **Páginas de destino**: as páginas de destino do Campaign v8 incluem melhorias para garantir a paridade de recursos com o Campaign Standard. Saiba mais nas[ notas de versão](../rn/release-notes.md#new-24-4) e na [documentação](../landing-pages/get-started-lp.md) da página de destino.

* **Fragmentos visuais**: os fragmentos visuais são componentes visuais reutilizáveis que podem ser referenciados em uma ou mais entregas de email ou em modelos de conteúdo. Modificar um fragmento atualiza todo o conteúdo que o utiliza. Essa funcionalidade permite que usuários de marketing pré-criem vários blocos de conteúdo personalizados para produzir mensagens rapidamente com um processo de design avançado. [Saiba mais](../content/use-visual-fragments.md).

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->