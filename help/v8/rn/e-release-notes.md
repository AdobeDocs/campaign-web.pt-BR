---
title: Notas de versão antecipadas da interface de usuário da Web do Campaign v8
description: Descubra novos recursos que acompanharão a próxima versão da interface da Web do Campaign
hide: true
hidefromtoc: true
source-git-commit: c40278f2424b8d6bdc396b3253ac999c23ed8312
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 1%

---

# Notas de versão antecipadas {#e-release}

A interface do usuário da Web do Adobe Campaign oferece continuamente novos recursos, melhorias nos recursos existentes e correções de erros. Todas as alterações são consolidadas no final de cada mês no [notas de versão](release-notes.md).

**As notas de versão anteriores abaixo estão sujeitas a alterações sem aviso prévio até a data de disponibilidade do lançamento**. Links, telas e documentação atualizada são publicados no [notas de versão](release-notes.md), na data de lançamento.

## Notas de versão de junho {#24-6-release}

**Data de lançamento**: 18 a 19 de junho de 2024

Os seguintes recursos e melhorias estão disponíveis para todos os usuários a partir da versão de junho.

### Fragmentos de conteúdo {#24-6-1}

Agora você pode criar, usar e gerenciar **visual** e **expressão** fragmentos para reunir rapidamente seus emails e modelos de conteúdo. Um fragmento é um componente reutilizável pré-criado que pode ser referenciado em vários emails no Adobe Campaign para obter um processo de design aprimorado e acelerado.

### Seed lists {#24-6-2}

Uma lista de seeds, também conhecido como. **Grupo de interceptação**, é uma lista de seed addresses. É usado para incluir endereços específicos em seus deliveries e, em seguida, direcionar perfis que não correspondem aos critérios de destino definidos. Dessa forma, os recipients que estiverem fora do público-alvo do delivery podem recebê-lo, como qualquer outro recipient do target receberia. Você pode usar seed addresses ao enviar provas ou para proteger sua lista de mala direta.

### Alertas de entrega {#24-6-3}

O recurso de Alerta de delivery é um sistema de gerenciamento de alertas que permite que um grupo de usuários receba automaticamente notificações contendo informações sobre a execução de seus deliveries.

### Planos e programas {#24-6-4}

Agora você pode criar planos e programas para organizar suas campanhas. Ao definir uma hierarquia de pastas, você pode organizar suas campanhas em programas e os programas em planos.

### Aprimoramentos {#improvements-24-6}

* **Reconciliação na atividade de Enriquecimento**: a atividade Enrichment agora pode ser usada para reconciliar dados do schema de banco de dados do Campaign com dados de outro schema ou com dados provenientes de um schema temporário, como dados carregados usando uma atividade Load file. Por exemplo, você pode usar essa opção para reconciliar o país de um perfil, especificado em um arquivo carregado, com um dos países disponíveis na tabela dedicada do banco de dados do Campaign.
