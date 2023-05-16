---
audience: end-user
title: Notas de versão do Campaign Web v8
description: Notas de versão do Campaign Web v8
exl-id: 3d8c07be-665e-46af-ba5d-f04b25b40880
badge: label="Alpha" type="Positive"
source-git-commit: b5af5099d62e0e424fffdd8eb74d67f12777b0f2
workflow-type: ht
source-wordcount: '416'
ht-degree: 100%

---


# Notas de versão {#release-notes}

Esta página lista todos os recursos e melhorias mais recentes do Campaign Web v8.

## Versão Alfa{#alpha-release}

No momento, essa nova interface do Campaign Web está disponível somente para os **Profissionais alfa** com os seguintes recursos:

**Experiência moderna, intuitiva e unificada**

A nova interface do Campaign Web oferece uma nova experiência de usuário, alinhada a todas as soluções e aplicativos da Adobe Experience Cloud. Ele oferece:

* Acesso à nova interface e a outras soluções Adobe com uma sessão de usuário única e compartilhada
* Nova experiência de navegação, com todos os menus e pastas disponíveis no painel esquerdo
* Alternadores de soluções e organizações da barra superior
* Integração unificada do Shell, com acesso direto à comunidade, centro de ajuda e suporte
<!--
No search and pulse notifications in Alpha
-->

Saiba mais sobre a nova interface [nesta página](../get-started/user-interface.md).

**Criar, iniciar e medir sua campanha de email**

Use a nova interface do Campaign Web para:

* Criar conteúdo de email personalizado com o Designer de email - [Saiba mais](../content/edit-content.md)
* Definir os públicos-alvo com o construtor de regras - [Saiba mais](../audience/about-audiences.md)
* Visualizar, testar e enviar suas mensagens de email - [Saiba mais](../monitor/prepare-send.md)
* Monitore o envio e meça os resultados com relatórios internos - [Saiba mais](../reporting/reports.md)

<!--
add info somewhere to remind users that
* they still have access to their console (+ link to v8 console doc)
* they keep their existing data (example: will be able to use their existing delivery templates to create deliveries)
-->


## Atualizações de terminologia{#terminology-updates}

Como um usuário existente do Campaign, observe que alguns conceitos foram renomeados para alinhar-se aos padrões de terminologia mais recentes. Essas alterações se aplicam somente à interface do Campaign Web e não são refletidas no Console do cliente. Elas estão detalhadas abaixo.

* Agora, as provas são **Testar emails**: para enviar uma prova, use o botão **Teste** na interface da entrega de email. O público-alvo do direcionamento das provas agora é referenciado como **Perfis de teste**
* Agora os seed addresses são usados para **Perfis de teste**: envie o email de teste para os seed addresses, que são os recipients adicionais e fictícios no banco de dados
* A análise da entrega agora é a **preparação da entrega**. Quando precisar iniciar a análise, clique no botão **Preparar**
* A Visualização de email agora está disponível através do botão **Simular conteúdo**
* As listas agora são **Públicos**

## Limitações{#limitations-alpha}

Alguns dos recursos principais do Campaign, como campanhas entre canais e gerenciamento de fluxo de trabalho, estarão disponíveis com a versão Beta.

As limitações abaixo se aplicam a esta versão Alfa:

* Os únicos objetos editáveis são as Entregas. Os outros são para somente leitura. Use os filtros para navegar por todos eles.
* Esta versão foi criada para campanhas por email únicas. Outros canais ainda não são compatíveis.
* A interface de Administração não está disponível.
* As métricas de relatório (como aberturas e dados de rastreamento) são atualizadas a cada hora.
* Os KPIs do painel de entrega são atualizados a cada 5 minutos. - mas a preparação da Entrega é em tempo real.
* As Notificações da Adobe Experience Cloud e a Ajuda unificada disponíveis na barra superior ainda não estão integradas.

