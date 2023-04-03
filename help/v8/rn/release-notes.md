---
audience: end-user
title: Notas de versão do Campaign Web v8
description: Notas de versão do Campaign Web v8
exl-id: 3d8c07be-665e-46af-ba5d-f04b25b40880
badge: label="Alpha" type="Informative"
source-git-commit: 15c37b0651b1d15dd80571c504aaca59d848b619
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---


# Notas de versão {#release-notes}

Esta página lista todos os recursos e melhorias mais recentes do Campaign Web v8.

## Versão alfa{#alpha-release}

No momento, essa nova interface da Web do Campaign está disponível somente para **Médicos alfa** com os seguintes recursos:

**Experiência moderna, intuitiva e unificada**

A nova interface do usuário da Web do Campaign oferece uma nova experiência de usuário, alinhada a todas as soluções e aplicativos da Adobe Experience Cloud. Ele oferece:

* Acesso à nova interface e a outras soluções do Adobe com uma sessão de usuário única e compartilhada
* Nova experiência de navegação, com todos os menus e pastas disponíveis no painel esquerdo
* Alternadores de soluções e organizações da barra superior
* Integração Unificada do Shell, com acesso direto à comunidade, centro de ajuda e suporte
<!--
No search and pulse notifications in Alpha
-->

Saiba mais sobre a nova interface do usuário no [esta página](../get-started/user-interface.md).

**Criar, iniciar e medir sua campanha de email**

Use a nova interface do usuário do Campaign Web para:

* Projetar conteúdo de email personalizado com o designer de email - [Saiba mais](../content/edit-content.md)
* Definir públicos-alvo com o construtor de regras - [Saiba mais](../audience/about-audiences.md)
* Visualizar, testar e enviar suas mensagens de email - [Saiba mais](../monitor/prepare-send.md)
* Monitore o envio e meça os resultados com relatórios internos - [Saiba mais](../reporting/reports.md)

<!--
add info somewhere to remind users that
* they still have access to their console (+ link to v8 console doc)
* they keep their existing data (example: will be able to use their existing delivery templates to create deliveries)
-->


## Atualizações de terminologia{#terminology-updates}

Como um usuário existente do Campaign, observe que alguns conceitos foram renomeados para alinhar-se aos padrões de terminologia mais recentes. Essas alterações se aplicam somente à interface do usuário da Web do Campaign e não são refletidas no Console do cliente. Elas estão resumidas abaixo.

* Agora, as provas são **Testar emails**: para enviar uma prova, use o **Teste** na interface do usuário do delivery de email. O target do target das provas agora é referenciado como **Testar perfis**
* Agora os seed addresses são usados como **Testar perfis**: envie o email de teste para seed addresses, que são recipients adicionais e fictícios no banco de dados
* A análise de delivery agora é o **preparação do delivery**. Quando precisar iniciar a análise, clique no botão **Preparar** botão
* A Visualização de email agora está disponível através do **Simular conteúdo** botão
* As listas agora são **Públicos-alvo**

## Limitações{#limitations-alpha}

Alguns recursos importantes do Campaign, como campanhas entre canais e gerenciamento de workflow, estarão disponíveis com a versão Beta.

As limitações abaixo se aplicam a esta versão Alfa:

* Os únicos objetos editáveis são Deliveries. Os outros são somente leitura. Use filtros para navegar por todos.
* Esta versão foi criada para campanhas por email. Outros canais ainda não são compatíveis.
* A interface de usuário Administração não está disponível.
* As métricas de relatório (como aberturas e dados de rastreamento) são atualizadas a cada hora.
* Os KPIs do painel de delivery são atualizados a cada 5 minutos. - mas a preparação do Delivery é em tempo real.
* As Notificações da Adobe Experience Cloud e a Ajuda unificada disponíveis na barra superior ainda não estão integradas.

