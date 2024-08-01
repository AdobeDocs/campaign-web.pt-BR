---
title: Notas de versão antecipadas da interface do Campaign Web v8
description: Conheça os novos recursos incluídos na próxima versão da interface do Campaign Web
hide: true
hidefromtoc: true
exl-id: a4c6ecb7-d657-46de-aa55-90c4cb45164b
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: ht
source-wordcount: '401'
ht-degree: 100%

---

# Notas de versão antecipadas {#e-release}

A interface do Adobe Campaign Web está sempre fornecendo novos recursos, melhorias de recursos existentes e correções de erros. As alterações são consolidadas no final de cada mês e incluídas nas [notas de versão](release-notes.md).

**As notas de versão antecipadas abaixo estão sujeitas a alterações sem aviso prévio até a data de disponibilidade do lançamento**. Links, telas e a documentação atualizada são publicados nas [notas de versão](release-notes.md) na data do lançamento.

## Notas de versão de julho {#24-7-release}

**Data de lançamento**: 30 a 31 de julho de 2024

Os seguintes recursos e melhorias estão disponíveis a partir da versão de julho.

### Fragmentos de conteúdo {#24-7-1}

Agora você pode criar e usar fragmentos de conteúdo. Um fragmento de conteúdo é um componente reutilizável que pode ser referenciado em uma ou mais mensagens. Ao modificar um fragmento, todos os conteúdos que o usam serão atualizados. Essa funcionalidade permite pré-construir vários blocos de conteúdo personalizados que podem ser usados por usuários de marketing para montar rapidamente o conteúdo de mensagens em um processo de design aprimorado.

Dois tipos de fragmentos estão disponíveis:

* **Fragmentos de expressão** são expressões predefinidas disponíveis em uma entrada dedicada no editor de expressão.
* **Fragmentos visuais** são blocos visuais predefinidos que podem ser reutilizados em várias entregas de email ou em modelos de conteúdo. [Saiba mais](../content/fragments.md)

  >[!AVAILABILITY]
  >
  >**Fragmentos visuais** estão em disponibilidade limitada (LA). Esse recurso é restrito a clientes que estão migrando **do Adobe Campaign Standard para o Adobe Campaign v8** e não pode ser implantado em nenhum outro ambiente.

### Listas de seeds {#24-7-2}

Uma lista de seeds (também conhecida como **Grupo de interceptação**) contém vários seed addresses. Ela é usada para incluir endereços específicos em suas entregas e direcionar perfis que não correspondem aos critérios de destino definidos. Dessa forma, os destinatários que não pertencem ao público-alvo da entrega podem recebê-la, assim como qualquer outro destinatário. Você pode usar seed addresses ao enviar provas ou para proteger sua lista de mala direta.

### Modelos de notificação por push avançada {#24-7-3}

Agora é possível enviar notificações por push avançadas. Uma notificação por push avançada é uma forma aprimorada de notificação em dispositivos móveis que vai além das mensagens de texto simples, incorporando elementos multimídia, como imagens, botões interativos ou outros conteúdos de mídia avançada. Com esta versão, um conjunto de modelos para notificações por push avançadas agora está disponível para seus aplicativos iOS e Android.

>[!AVAILABILITY]
>
>Esse recurso exige uma atualização para o Campaign v8.6.3 ou v8.7.2. Saiba mais nas [notas de versão do console do cliente do Campaign v8](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/releases/release-notes)

### Melhorias {#improvements-24-7}

**Gerenciamento de pastas**: agora é possível gerenciar permissões e restrições em pastas.
