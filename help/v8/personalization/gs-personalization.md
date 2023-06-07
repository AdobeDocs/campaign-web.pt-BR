---
title: Introdução ao conteúdo dinâmico
description: Saiba como tornar seu conteúdo dinâmico usando personalização, conteúdo condicional e blocos de conteúdo incorporados.
audience: automating
content-type: reference
topic-tags: workflow-general-operation
context-tags: workflow,overview;workflow,main
feature: Workflows
role: Data Architect
level: Intermediate
source-git-commit: 218f433eb72a0ed928732c96ebee64294daee852
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 36%

---


# Introdução ao conteúdo dinâmico

Para aproveitar ao máximo cada campanha de marketing, o Adobe Campaign oferece uma maneira de fornecer conteúdo dinâmico personalizado que fala com os clientes em seu nível. Com base nos dados do perfil, use os recursos de personalização para criar uma experiência personalizada para diferentes grupos e indivíduos: você pode adaptar suas mensagens a cada recipient específico, aproveitando os dados e as informações que tem sobre eles. Pode ser seu nome, interesses, onde vivem, o que compraram e muito mais.

Use o Campaign para criar conteúdo dinâmico e enviar mensagens personalizadas. Os recursos de personalização podem ser combinados para melhorar suas mensagens e criar uma experiência do usuário personalizada.

É possível tornar o conteúdo da mensagem dinâmico inserindo:

* **Campos de personalização**

   Os campos de personalização são usados na personalização de primeiro nível das mensagens. Você pode selecionar qualquer campo disponível no banco de dados no editor de personalização. Para uma entrega, é possível selecionar qualquer campo relacionado ao recipient, à mensagem ou à entrega. Esses atributos de personalização podem ser inseridos na linha de assunto ou no corpo das mensagens.

   ![](assets/perso-subject-line.png)

   A sintaxe a seguir insere a cidade do recipient no conteúdo: &lt;%= recipient.location.city %>.

* **Conteúdo condicional**

   Configure o conteúdo condicional para adicionar personalização dinâmica com base no perfil do destinatário, por exemplo. Blocos de texto e/ou imagens são inseridos quando uma determinada condição for satisfeita. Você pode definir a versão alternativa do conteúdo quando a condição não for verdadeira.

* **Blocos de conteúdo incorporados**

   O Campaign vem com um conjunto de blocos de personalização contendo uma renderização específica que você pode inserir nas entregas. Por exemplo, você pode adicionar um logotipo, uma mensagem de saudação ou um link para a mirror page de uma mensagem de email. Os blocos de conteúdo estão disponíveis em uma entrada dedicada no editor de personalização.

   ![](assets/perso-content-blocks.png)

## Onde posso adicionar conteúdo dinâmico?

O Adobe Campaign V8 Web fornece um editor de expressão onde você pode selecionar, organizar, personalizar e validar todos os dados para criar uma experiência personalizada para o seu conteúdo.

O editor de expressão está disponível para todos os canais, em todos os campos com o ícone Abrir caixa de diálogo de personalização, como o campo de linha de assunto ou componentes de conteúdo de texto e botão em emails.

![](assets/expression-editor-access.png)

![](assets/expression-editor-access-email.png)

Além disso, um construtor de conteúdo condicional dedicado pode ser acessado ao projetar um email. [Saiba como criar conteúdo condicional em emails](conditions.md)

## Vamos nos aprofundar um pouco mais

Agora que você entende como tornar seu conteúdo dinâmico, é hora de se aprofundar nessas seções de documentação para começar a trabalhar com o recurso.

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="personalize.md">
<img alt="Personalizar conteúdo" src="assets/do-not-localize/dynamic-personalization.jpg">
</a>
<div>
<a href="personalize.md"><strong>Adicionar personalização</strong></a>
</div>
<p>
</td>
<td>
<a href="conditions.md">
<img alt="Lead" src="assets/do-not-localize/dynamic-conditional.jpg">
</a>
<div><a href="conditions.md"><strong>Adicionar conteúdo condicional</strong>
</div>
<p>
</td>
<td>
<a href="content-blocks.md">
<img alt="Pouco frequente" src="assets/do-not-localize/dynamic-content-blocks.jpg">
</a>
<div>
<a href="content-blocks.md"><strong>Adicionar blocos de conteúdo incorporados</strong></a>
</div>
<p></td>
</tr></table>
