---
title: Notas de versão mais recentes
description: Conheça o novo recurso incluído na interface do Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: ht
source-wordcount: '342'
ht-degree: 100%

---

# Notas de versão {#latest-release}


>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Novidades"
>abstract="As versões da interface do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem mais escalável e em fases para a implantação de recursos. As notas de versão são atualizadas várias vezes por mês. **A versão de março está disponível**, incluindo o canal Correspondência direta, a nova atividade de fluxo de trabalho Alterar fonte de dados e outras melhorias."


<!--Last update: **March 19, 2024**-->

As versões da interface do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem mais escalável e em fases para a implantação de recursos. Devido a isso, essas notas de versão são atualizadas várias vezes por mês. Verifique-as regularmente.

>[!AVAILABILITY]
>
>Esta versão está disponível para todos os usuários a partir do [Campaign (console) v8.6](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=pt-BR). Saiba mais sobre as versões e atualizações do console do cliente do Adobe Campaign na [documentação do Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=pt-BR){target="_blank"}.

## Notas de versão de março {#24-3-release}

**Data de lançamento**: 19 a 20 de março de 2024

### Canal de correspondência direta {#24-3-dm}

O canal de **Correspondência direta** agora está disponível para uso em fluxos de trabalho e como entregas independentes. A correspondência direta é um canal offline que permite criar, personalizar e gerar arquivos de extração e compartilhá-los com seus provedores de correspondência direta para enviar emails a seus clientes. [Leia mais](../direct-mail/gs-direct-mail.md)

![](../assets/do-not-localize/direct-mail.gif)

### Nova atividade de fluxo de trabalho Alterar fonte de dados {#24-3-change-data-source}

A atividade de direcionamento **Alterar fonte de dados** permite alterar a fonte de dados de uma tabela de trabalho do fluxo de trabalho. Essa atividade oferece mais flexibilidade, permitindo gerenciar dados em seus diferentes bancos de dados e melhorar o desempenho. [Leia mais](../workflows/activities/change-data-source.md)

![](../assets/do-not-localize/change-data-source.gif)

### Melhoria da atividade do fluxo de trabalho Divisão {#24-3-split}

Agora é possível usar a opção **Gerar todos os subconjuntos na mesma tabela** na atividade de fluxo de trabalho **Divisão** para agrupar todos os subconjuntos em uma única transição de saída. [Leia mais](../workflows/activities/split.md)

### Modelador de consulta {#24-3-query-modeler}

* O modelador de consultas agora está disponível para uso no Designer de email. Ele permite criar condições ao criar conteúdo condicional. [Leia mais](../personalization/conditions.md)
* Os valores predefinidos agora estão disponíveis para atributos de tipo de data ao criar uma condição personalizada. [Leia mais](../query/build-query.md)
* Os operadores não podem mais ser adicionados em uma nova transição no diagrama. Eles só podem ser adicionados em uma transição já existente antes de filtrar componentes para agrupá-los. [Leia mais](../query/build-query.md)
