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
source-git-commit: bf5ff77b695a5a8584bad7784597bf1521bcb23e
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 12%

---


# Introdução ao conteúdo dinâmico

Fornecer conteúdo relevante para seus clientes é fundamental para garantir que você atraia uma variedade de clientes e jogue o interesse deles para que o conteúdo de marketing seja lido.

Para aproveitar ao máximo cada campanha de marketing, o Adobe Campaign oferece uma maneira de criar uma experiência personalizada para diferentes grupos e indivíduos, fornecendo conteúdo dinâmico personalizado que fala com os clientes em seu nível, aproveitando as informações coletadas sobre eles.

* **Personalizar suas mensagens** para cada recipient específico aproveitando dados de perfil, como nome, interesses, onde vivem, o que compraram e muito mais.

  Você pode selecionar qualquer campo disponível no banco de dados no editor de personalização relacionado ao recipient, à mensagem ou ao delivery. Esses atributos de personalização podem ser inseridos na linha de assunto ou no corpo das mensagens. A sintaxe a seguir insere a cidade do recipient no conteúdo: &lt;%= recipient.location.city %>.

  ![](assets/perso-subject-line.png){width="800" align="center"}

* **Criar conteúdo condicional** para adaptar seus deliveries a cada recipient e mostrar apenas o conteúdo relevante para um determinado cliente com base nas informações que você tem sobre eles. Isso permite exibir blocos de texto e/ou imagens específicos com base em condições. Por exemplo, adapte um banner de email com base na assinatura dos recipients a um serviço específico.

  ![](assets/condition-sample.png){width="800" align="center"}

* **Usar blocos de personalização** para economizar tempo e aproveitar o conteúdo personalizado facilmente reutilizável em suas mensagens. O Campaign vem com um conjunto de blocos de personalização contendo uma renderização específica que você pode inserir nas entregas. Por exemplo, você pode adicionar um logotipo, uma mensagem de saudação ou um link para a mirror page de uma mensagem de email. Os blocos de conteúdo estão disponíveis em uma entrada dedicada no editor de personalização.

  ![](assets/content-blocks.png){width="800" align="center"}

## Acessar o editor de expressão {#access}

O Adobe Campaign V8 Web fornece um editor de expressão onde você pode selecionar, organizar, personalizar e validar todos os dados para criar uma experiência personalizada para o seu conteúdo. O editor de expressão está disponível para todos os canais, em todos os campos com o **[!UICONTROL Abrir caixa de diálogo de personalização]** ícone, como o campo da linha de assunto ou links de email e componentes de conteúdo de texto/botão.

Estes são alguns exemplos de como acessar o editor de expressão dependendo do conteúdo que você deseja tornar dinâmico:

* *Acessando o editor de expressão no campo Nome do remetente*

  ![](assets/expression-editor-access.png){width="800" align="center"}

* *Acesso ao editor de expressão por meio de um componente de texto de email*

  ![](assets/expression-editor-access-email.png){width="800" align="center"}

* *Acesso ao editor de expressão por meio de um link em um email*

  ![](assets/perso-link-insert-icon.png){width="800" align="center"}

>[!NOTE]
>
>Além do editor de expressão, você também pode aproveitar um construtor de conteúdo condicional dedicado ao criar um email. [Saiba como criar conteúdo condicional em emails](conditions.md)

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
