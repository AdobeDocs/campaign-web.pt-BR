---
audience: end-user
title: Novidades do Campaign Web v8
description: Conheça o novo recurso que vem com o Campaign Web v8
exl-id: 3d8c07be-665e-46af-ba5d-f04b25b40880
badge: label="Beta"
source-git-commit: e2ff9efcedbfc46f9d943c30fabb1b3b39c43b74
workflow-type: tm+mt
source-wordcount: '962'
ht-degree: 50%

---


# Novidades {#new}


Temos o prazer de apresentar a versão BETA da interface do usuário da Web do Adobe Campaign. Nossa versão mais recente contém recursos intuitivos projetados para simplificar a criação de campanhas personalizadas entre canais, gerar resultados excepcionais e oferecer uma vantagem competitiva em todos os canais.

## Versão Beta{#beta-release}

No momento, essa nova interface da Web do Campaign está disponível apenas para **Profissionais beta** com os seguintes recursos:

**Experiência moderna, intuitiva e unificada**

A nova interface do Campaign Web oferece uma nova experiência de usuário, alinhada a todas as soluções e aplicativos da Adobe Experience Cloud. Ele oferece:

* Acesso à nova interface e a outras soluções Adobe com uma sessão de usuário única e compartilhada
* Nova experiência de navegação, com todos os menus e pastas disponíveis no painel esquerdo
* Alternadores de soluções e organizações da barra superior
* Integração unificada do Shell, com acesso direto à comunidade, centro de ajuda e suporte

**Novos recursos avançados e processos ininterruptos**

* Nova interface da tela de workflow para criar e gerenciar seus processos
* Conteúdo dinâmico para oferecer experiências altamente direcionadas e personalizadas para seu público-alvo
* Integração nativa com públicos-alvo da Adobe Experience Platform
* Gerenciamento de modelos para workflows, entregas, campanhas e conteúdo

Saiba mais sobre a nova interface [nesta página](../get-started/user-interface.md).

**Criar, iniciar e medir sua campanha**

Use a nova interface do Campaign Web para:

* Criar conteúdo de email personalizado com o Designer de email - [Saiba mais](../content/edit-content.md)
* Enviar campanhas entre canais, incluindo SMS e notificações por push.
* Definir os públicos-alvo com o construtor de regras - [Saiba mais](../audience/about-audiences.md)
* Visualizar, testar e enviar suas mensagens de email - [Saiba mais](../monitor/prepare-send.md)
* Monitore o envio e meça os resultados com relatórios internos - [Saiba mais](../reporting/delivery-reports.md)


## Atualizações mais recentes


**Resumo da versão beta**

* Habilitar composição de dados (federada) para Públicos-alvo e Personalização.
* Utilizar a tecnologia de IA para aprimorar a geração de conteúdo de email.
* Sincronizar ativos e modelos de HTML completo com perfeição.
* Organize e gerencie com eficiência suas pastas e recursos.
* Crie páginas de aterrissagem envolventes e eficientes.
* Mais atividades de workflow: acesse atividades adicionais, como dimensão de alteração, desduplicação e deliveries recorrentes para aprimorar os workflows da campanha.

**Principais novos recursos**

* Mais atividades de workflow do Campaign

  Turbine suas campanhas de marketing com nosso conjunto expandido de atividades de workflow. Descubra novas possibilidades de automação e otimização, permitindo que você crie jornadas do cliente mais dinâmicas e personalizadas.

  Desde a segmentação avançada até acionadores condicionais, nossas atividades adicionais de fluxo de trabalho capacitam você a fornecer mensagens direcionadas e a impulsionar um melhor desempenho da campanha.

* Gerar IA para conteúdo de email

  Diga adeus à criação manual de conteúdo e olá para campanhas eficientes orientadas por dados com o poder da Gen AI.  Nossa tecnologia Gen AI utiliza algoritmos avançados para gerar conteúdo altamente envolvente e personalizado. Impulsione taxas de abertura, taxas de click-through e conversões mais altas com a geração de conteúdo inteligente da Gen AI.

  Mantenha-se à frente da concorrência e eleve seu jogo de marketing por email com a Gen AI sobre conteúdo de email.


* Gerenciamento de filtro predefinido

  Introdução Ao Gerenciamento De Filtros Predefinidos. A interface da Web do Campaign agora oferece uma interface fácil de usar para gerenciar e personalizar facilmente filtros predefinidos para atender às suas necessidades específicas. Crie uma vez e salve para uso futuro. [Saiba mais](../personalization/predefined-filters.md)


* Público-alvo

  Criar um público-alvo de entrega nunca foi tão fácil! Com o construtor de regras mais recente, agora é possível definir critérios de filtragem para recipients ou qualquer outro targeting dimension do banco de dados. Além disso, você pode aproveitar seu público-alvo da AEP (Adobe Experience Platform) para refinar ainda mais seu público-alvo e maximizar o impacto da campanha.

* Ofertas com SMS e Push

  A nova interface da Web agora permite integrar ofertas com SMS e notificações por push, além de email. Alcance seu público em seus dispositivos móveis, fornecendo promoções e notificações oportunas.

  Aumente seus esforços de marketing aproveitando o poder das ofertas integradas por meio de SMS e notificações por push em nossa plataforma avançada de Web.

* Integração do Adobe Experience Manager (AEM)

  Com nossa integração com o AEM estendida para a interface da Web, você pode gerenciar ativos facilmente e sincronizar modelos completos de HTML, permitindo criar experiências digitais envolventes sem qualquer problema.

  Elevar e simplificar seus recursos de gerenciamento de conteúdo na interface da Web com essa integração para aumentar a produtividade.

## Transição para a interface do Campaign Web

Como usuário do Campaign, você ainda pode acessar o console do cliente para criar e gerenciar recursos e componentes do Campaign. Os dados e as configurações são sincronizados de um ambiente para outro. Saiba mais [nesta seção](../get-started/get-started.md#about-campaign-client-consoleac-client).

Além disso, todos os seus dados e configurações já disponíveis no console do cliente, estarão visíveis na interface do Campaign Web, no painel de navegação Explorer, à esquerda. Saiba mais sobre a visualização do Explorer [nesta seção](../get-started/user-interface.md#explorer-user-interface-explorer).

Com a versão Campaign Web Beta, a interface reflete as permissões do usuário. Saiba mais sobre permissões no [esta página](../get-started/permissions.md)

## Atualizações de terminologia {#terminology-updates}

Como um usuário existente do Campaign, observe que alguns conceitos foram renomeados para alinhar-se aos padrões de terminologia mais recentes. Essas alterações se aplicam somente à interface do Campaign Web e não se refletem no console do cliente. Elas estão detalhadas abaixo.

* Agora, as provas são **Testar emails**: para enviar uma prova, use o botão **Teste** na interface da entrega de email. O público-alvo das provas agora é referenciado como **Perfis de teste**. [Saiba mais](../preview-test/test-deliveries.md).
* Agora, os seed addresses são usados como **Perfis de teste**: envie o email de teste para os seed addresses, que são destinatários adicionais no banco de dados. [Saiba mais](../preview-test/test-deliveries.md).
* A análise da entrega agora é a **preparação da entrega**. Quando precisar iniciar a análise, clique no botão **Preparar**. [Saiba mais](../monitor/prepare-send.md).
* A Visualização de email agora está disponível através do botão **Simular conteúdo**. [Saiba mais](../preview-test/preview-test.md)
* As listas agora são **Públicos-alvo**. [Saiba mais](../audience/about-audiences.md).

## Limitações{#limitations-alpha}

As limitações abaixo se aplicam a esta versão Alfa:

* Os objetos editáveis são: Deliveries, Campanhas, Workflows, Públicos-alvo, Serviços de assinatura, Filtros predefinidos e Modelos. Os outros são para somente leitura. Use os filtros para navegar por todos eles.
* Os públicos-alvo não podem ser salvos para uso futuro.
* A interface de Administração não está disponível.
* As métricas de relatório (como aberturas e dados de rastreamento) são atualizadas a cada hora.
* Os KPIs do painel de entrega são atualizados a cada 5 minutos. - mas a preparação da Entrega é em tempo real.
* As Notificações da Adobe Experience Cloud e a Ajuda unificada disponíveis na barra superior ainda não estão integradas.

