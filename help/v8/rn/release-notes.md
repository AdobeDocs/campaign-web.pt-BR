---
title: Notas de versão mais recentes
description: Conheça o novo recurso incluído na interface do Campaign Web
source-git-commit: 21d856f9651f3a392ba9d927bc26082ce9759396
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 9%

---

# Notas de versão {#latest-release}


>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Novidades"
>abstract="As versões da interface do usuário da Web do Adobe Campaign operam em um modelo de entrega contínua que permite uma abordagem mais escalável e em fases para a implantação de recursos. As notas de versão são atualizadas várias vezes por mês."
>
>"**March release is now live**, including Direct mail channel, the new Change data source workflow activity, and other improvements."


<!--Last update: **March 19, 2024**-->

As versões da interface do usuário da Web do Adobe Campaign operam em um modelo de entrega contínua que permite uma abordagem mais escalável e em fases para a implantação de recursos. Devido a isso, essas notas de versão são atualizadas várias vezes por mês. Verifique-as regularmente.

>[!AVAILABILITY]
>
>Esta versão está disponível para todos os usuários a partir de [Versão v8.6 do Campaign (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=pt-BR). Saiba mais sobre as versões e atualizações do console do cliente do Adobe Campaign em [Documentação do Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=pt-BR){target="_blank"}.

## Versão de março {#24-3-release}

**Data de lançamento**: 19 a 20 de março de 2024

### Canal de correspondência direta {#24-3-dm}

**Correspondência direta** O canal agora está disponível para uso em workflows e como deliveries independentes. A correspondência direta é um canal offline que permite criar, personalizar e gerar arquivos de extração e compartilhá-los com seus provedores de correspondência direta para enviar emails a seus clientes. [Leia mais](../direct-mail/gs-direct-mail.md)

![](../assets/do-not-localize/direct-mail.gif)

### Nova atividade de fluxo de trabalho Alterar fonte de dados {#24-3-change-data-source}

A variável **Alterar fonte de dados** a atividade de direcionamento permite alterar a fonte de dados usada pela tabela de trabalho do workflow. Essa atividade oferece mais flexibilidade, permitindo gerenciar dados em seus diferentes bancos de dados e melhorar o desempenho. [Leia mais](../workflows/activities/change-data-source.md)

![](../assets/do-not-localize/change-data-source.gif)

### Dividir a melhoria da atividade do fluxo de trabalho {#24-3-split}

Agora você pode usar o **Gerar todos os subconjuntos na mesma tabela** opção no **Split** atividade de workflow para agrupar todos os subconjuntos em uma única transição de output. [Leia mais](../workflows/activities/split.md)

### Modelador de consulta {#24-3-query-modeler}

* O modelador de consultas agora está disponível para uso no Designer de email. Ele permite criar condições ao criar conteúdo condicional. [Leia mais](../personalization/conditions.md)
* Os valores predefinidos agora estão disponíveis para atributos de tipo de data ao criar uma condição personalizada. [Leia mais](../query/build-query.md)
* Os operadores não podem mais ser adicionados em uma nova transição no diagrama. Eles só podem ser adicionados em uma transição existente antes de filtrar componentes para agrupá-los. [Leia mais](../query/build-query.md)
