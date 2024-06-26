---
title: Notas de versão antecipadas da interface do Campaign Web v8
description: Conheça os novos recursos incluídos na próxima versão da interface do Campaign Web
hide: true
hidefromtoc: true
exl-id: a4c6ecb7-d657-46de-aa55-90c4cb45164b
source-git-commit: e9bba947dd1065287e698d20cf1b6b55c423003b
workflow-type: ht
source-wordcount: '355'
ht-degree: 100%

---

# Notas de versão antecipadas {#e-release}

A interface do Adobe Campaign Web está sempre fornecendo novos recursos, melhorias de recursos existentes e correções de erros. As alterações são consolidadas no final de cada mês e incluídas nas [notas de versão](release-notes.md).

**As notas de versão antecipadas abaixo estão sujeitas a alterações sem aviso prévio até a data de disponibilidade do lançamento**. Links, telas e a documentação atualizada são publicados nas [notas de versão](release-notes.md) na data do lançamento.

## Notas de versão de junho {#24-6-release}

**Data de lançamento**: 18 a 19 de junho de 2024

Os seguintes recursos e melhorias estão disponíveis para todos os usuários a partir da versão de junho.

### Fragmentos de conteúdo  {#24-6-1}

Agora é possível criar, usar e gerenciar fragmentos **visuais** e **de expressão** para montar rapidamente seus emails e modelos de conteúdo. Um fragmento é um componente reutilizável pré-criado que pode ser referenciado em vários emails no Adobe Campaign para obter um processo de design aprimorado e acelerado.

### Listas de seeds {#24-6-2}

Uma lista de seeds (também conhecida como **Grupo de interceptação**) contém vários seed addresses. Ela é usada para incluir endereços específicos em suas entregas e direcionar perfis que não correspondem aos critérios de destino definidos. Dessa forma, os destinatários que não pertencem ao público-alvo da entrega podem recebê-la, assim como qualquer outro destinatário. Você pode usar seed addresses ao enviar provas ou para proteger sua lista de mala direta.

### Alerta de entrega {#24-6-3}

O recurso Alerta de entrega é um sistema de gerenciamento de alertas que permite que um grupo de usuários receba automaticamente notificações sobre a execução de suas entregas.

### Planos e programas {#24-6-4}

Agora é possível criar planos e programas para organizar suas campanhas. Ao definir uma hierarquia de pastas, você pode organizar suas campanhas em programas e os programas em planos.

### Melhorias {#improvements-24-6}

* **Reconciliação na atividade de enriquecimento**: a atividade de enriquecimento agora pode ser usada para reconciliar dados do esquema de banco de dados do Campaign com dados provenientes de um esquema alternativo ou de um esquema temporário, como dados carregados usando uma atividade Carregar arquivo. Por exemplo, é possível usar essa opção para reconciliar o país de um perfil, que é especificado em um arquivo carregado, com um dos países disponíveis na tabela dedicada do banco de dados do Campaign.
