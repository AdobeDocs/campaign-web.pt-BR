---
title: Como tornar o conteúdo dinâmico?
description: Saiba como tornar o conteúdo dinâmico utilizando personalização e conteúdo condicional.
audience: automating
content-type: reference
topic-tags: workflow-general-operation
context-tags: workflow,overview;workflow,main
feature: Workflows
role: Data Architect
level: Intermediate
exl-id: cce1da98-924b-415b-99d9-f4def4a4e874
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: ht
source-wordcount: '532'
ht-degree: 100%

---

# Como tornar o conteúdo dinâmico? {#gs-dynamic-content}

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_dashboard"
>title="Personalização"
>abstract="O editor de expressão permite selecionar, organizar, personalizar e validar todos os dados para criar uma experiência personalizada para o seu conteúdo. É possível personalizar as mensagens para cada destinatário aproveitando os dados do perfil e criar conteúdo condicional para adaptar cada mensagem, mostrando apenas o conteúdo relevante. "

Como profissional de marketing, é fundamental direcionar o público-alvo que está genuinamente interessado em suas ofertas e engajá-lo com fornecimento de conteúdo eficaz e relevante. Dada a variedade diversificada de destinatários que você encontra, criar vários conteúdos de marketing para atrair pessoas diferentes, pode ser demorado e dispendioso. É aqui que o conteúdo dinâmico entra em cena.

Os recursos de conteúdo dinâmico do Adobe Campaign Web permitem personalizar o conteúdo com base nas informações coletadas sobre os destinatários. Ao utilizar o conteúdo dinâmico, você garante que seus esforços de marketing sejam mais relevantes, evitando o anúncio de produtos ou serviços indesejados ou desnecessários. Essa abordagem torna o conteúdo mais atraente e aumenta a probabilidade de ele ser lido. Além disso, permite personalizar o conteúdo, fazendo com que os destinatários sintam que estão recebendo informações de uma pessoa em vez de uma máquina.

## Como tornar o conteúdo dinâmico? {#make-content-dyn}

Você pode tornar o conteúdo da mensagem dinâmico inserindo construções JavaScript no editor de expressão do Campaign Web. No envio da mensagem, essas expressões são interpretadas pelo Adobe Campaign para entregar o conteúdo correto a cada um dos destinatários:

* **Personalizar suas mensagens** para cada destinatário específico aproveitando dados de perfil, como nome, interesses, onde vive, o que comprou e muito mais. É possível selecionar qualquer campo disponível no banco de dados do editor de personalização relacionado ao destinatário, à mensagem ou à entrega. Esses atributos de personalização podem ser inseridos na linha de assunto ou no corpo das mensagens. A sintaxe a seguir insere a cidade do destinatário no conteúdo: &lt;%= recipient.location.city %>.

  ![](assets/perso-subject-line.png){zoomable="yes"}{width="800" align="center"}

* **Criar conteúdo condicional** para adaptar suas entregas a cada destinatário e mostrar apenas conteúdo relevante para um determinado cliente, com base nas informações que você tem sobre ele. Isso permite exibir imagens e/ou blocos de texto específicos com base em condições. Por exemplo, adapte um banner de email com base na assinatura do destinatário de um serviço específico.

  ![](assets/condition-sample.png){zoomable="yes"}{width="800" align="center"}

## Acesso ao editor de expressão {#access}

O Adobe Campaign Web fornece um editor de expressão onde é possível selecionar, organizar, personalizar e validar todos os dados para criar uma experiência personalizada para o seu conteúdo. O editor de expressão está disponível para todos os canais, em todos os campos com o ícone de **[!UICONTROL Abrir caixa de diálogo de personalização]**, como o campo da linha de assunto ou links de email e componentes de conteúdo de texto/botão.

Estes são alguns exemplos de como acessar o editor de expressão, dependendo do conteúdo que deseja tornar dinâmico:

* *Acesso ao editor de expressão a partir do campo Nome do remetente*

  ![](assets/expression-editor-access.png){zoomable="yes"}{width="800" align="center"}

* *Acesso ao editor de expressão a partir de um componente de texto de email*

  ![](assets/expression-editor-access-email.png){zoomable="yes"}{width="800" align="center"}

* *Acesso ao editor de expressão a partir de um link em um email*

  ![](assets/perso-link-insert-icon.png){zoomable="yes"}{width="800" align="center"}

>[!NOTE]
>
>Além do editor de expressão, ao criar um email, você também pode aproveitar um construtor de conteúdo condicional dedicado. [Saiba como criar conteúdo condicional em emails](conditions.md)
