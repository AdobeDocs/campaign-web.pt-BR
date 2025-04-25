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
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: ht
source-wordcount: '621'
ht-degree: 100%

---

# Como tornar o conteúdo dinâmico? {#gs-dynamic-content}

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_dashboard"
>title="Personalização"
>abstract="O editor de personalização permite selecionar, organizar, personalizar e validar todos os dados para criar uma experiência personalizada para seu conteúdo. É possível personalizar as mensagens para cada destinatário aproveitando os dados do perfil e criar conteúdo condicional para adaptar cada mensagem ao respectivo destinatário, mostrando apenas o conteúdo relevante. "

Como profissional de marketing, é fundamental focar em clientes que estejam genuinamente interessados em suas ofertas e envolvê-los com um conteúdo eficaz e relevante. Dada a variedade diversificada de destinatários que você encontra, criar vários conteúdos de marketing para atrair pessoas diferentes pode ser um processo demorado e trabalhoso. É aqui que o conteúdo dinâmico se torna essencial.

Os recursos de conteúdo dinâmico do Adobe Campaign Web permitem que você personalize seu conteúdo com base nas informações coletadas sobre os destinatários. Por usar conteúdo dinâmico, você garante que suas ações de marketing sejam mais relevantes, evitando comercializar produtos ou serviços indesejados ou desnecessários. Essa abordagem torna o conteúdo mais atraente e aumenta a probabilidade de ele ser lido. Além disso, permite personalizar o conteúdo, fazendo com que os destinatários sintam que estão recebendo informações de uma pessoa em vez de uma máquina.

## Como tornar o conteúdo dinâmico? {#make-content-dyn}

É possível criar conteúdo dinâmico para sua mensagem inserindo construções JavaScript no editor de expressões do Campaign Web. No envio de mensagens, o Adobe Campaign interpreta essas expressões para entregar o conteúdo correto a cada um de seus destinatários:

* **Personalizar suas mensagens** para cada destinatário específico aproveitando dados de perfil, como nome, interesses, onde vive, o que comprou e muito mais. É possível selecionar qualquer campo disponível no banco de dados do editor de personalização relacionado ao destinatário, à mensagem ou à entrega. Esses atributos de personalização podem ser inseridos na linha de assunto ou no corpo das mensagens. A sintaxe a seguir insere a cidade do destinatário no conteúdo: `<%= recipient.location.city %>`.

  [Descrição: exemplo de inserção da cidade do destinatário na linha de assunto usando atributos de personalização.](assets/perso-subject-line.png){zoomable="yes"}{width="800" align="center"}

* **Criar conteúdo condicional** para adaptar suas entregas a cada destinatário e mostrar apenas conteúdo relevante para um determinado cliente, com base nas informações que você tem sobre ele. Isso permite exibir imagens e/ou blocos de texto específicos com base em condições. Por exemplo, adapte um banner de email com base na assinatura do destinatário de um serviço específico.

  [Descrição: exemplo de conteúdo condicional em um banner de email com base na assinatura do destinatário.](assets/condition-sample.png){zoomable="yes"}{width="800" align="center"}

➡️ [Conheça este recurso no vídeo](#video)

## Acesso ao editor de expressão {#access}

O Adobe Campaign Web fornece um editor de expressão que permite selecionar, organizar, personalizar e validar todos os dados para criar uma experiência personalizada para seu conteúdo. O editor de expressão está disponível para todos os canais nos campos com o ícone **[!UICONTROL Abrir caixa de diálogo de personalização]**, como o campo de linha de assunto ou por meio dos links de email e componentes de conteúdo de texto e botão.

Veja alguns exemplos de como acessar o editor de expressão dependendo do conteúdo que você deseja tornar dinâmico:

* *Acesso ao editor de expressão a partir do campo Nome do remetente*

  [Descrição: exemplo de acesso ao editor de expressão a partir do campo Nome do remetente.](assets/expression-editor-access.png){zoomable="yes"}{width="800" align="center"}

* *Acesso ao editor de expressão a partir de um componente de texto de email*

  [Descrição: exemplo de acesso ao editor de expressão a partir de um componente de texto de email.](assets/expression-editor-access-email.png){zoomable="yes"}{width="800" align="center"}

* *Acesso ao editor de expressão a partir de um link em um email*

  [Descrição: exemplo de acesso ao editor de expressão a partir de um link em um email.](assets/perso-link-insert-icon.png){zoomable="yes"}{width="800" align="center"}

>[!NOTE]
>
>Além do editor de expressão, também é possível usar um criador de conteúdo condicional dedicado ao criar um email. [Saiba como criar conteúdo condicional em emails](conditions.md)

## Vídeo tutorial {#video}

Saiba como tornar o conteúdo da mensagem dinâmico por meio do editor de expressão para personalizar a sua mensagem ou adicionar um conteúdo condicional.

>[!VIDEO](https://video.tv.adobe.com/v/3425795?quality=12)