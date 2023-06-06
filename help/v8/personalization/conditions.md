---
title: Criação de conteúdo condicional
description: Saiba como definir condições para personalizar seu conteúdo na interface do Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Alpha" type="Positive"
exl-id: b650a859-e27d-4a36-a725-a1f5bb31e014
source-git-commit: 5598a82bf745659b8c1db8cb51b1a82cfd184093
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 8%

---

# Criar conteúdo condicional{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Criação de conteúdo condicional"
>abstract="Crie conteúdo condicional para definir a personalização dinâmica com base no perfil do recipient, substituindo automaticamente blocos de texto e imagens quando determinadas condições forem atendidas. Esse recurso pode levar suas campanhas a novos patamares e fornecer experiências personalizadas e altamente direcionadas ao seu público-alvo."


O conteúdo condicional é um recurso poderoso que permite criar personalização dinâmica com base no perfil do recipient, substituindo automaticamente blocos de texto e imagens quando determinadas condições são atendidas. Esse recurso pode levar suas campanhas a novos patamares e fornecer experiências personalizadas e altamente direcionadas ao seu público-alvo.

Ao configurar campos de conteúdo condicional, você pode criar personalização dinâmica avançada com base no perfil do recipient, por exemplo. Blocos de texto, links, linha de assunto e/ou imagens são substituídos no conteúdo da mensagem quando uma determinada condição é atendida. Por exemplo, você pode exibir &quot;Sr.&quot; ou &quot;Sra.&quot; de acordo com o valor do campo Gênero no banco de dados do Adobe Campaign ou incluir um link diferente com base no idioma preferencial do recipient.

## Sintaxe de personalização{#perso-syntax}



## Trabalhar com condições no editor de personalização{#condition-perso-editor}

Para definir um conteúdo condicional para um delivery:

1. Abra um delivery e edite o conteúdo.
1. Clique em **[!UICONTROL Abrir caixa de diálogo de personalização]** ícone, por exemplo, para SMS, à direita do campo Mensagem.

   ![](assets/open-perso-editor-sms.png)

1. No editor de personalização, navegue até **[!UICONTROL Funções auxiliares]**.
1. Clique no ícone &quot;+&quot; ao lado da guia **Se** função. A seguinte linha é adicionada à tela central:
   `<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`
1. Substituir `<FIELD>` por um campo de personalização Por exemplo, a empresa do recipient: `recipient.company`.
1. Substituir `<VALUE>` por um valor a ser satisfeito. Por exemplo, `ADOBE`.




## Amostra: linha de assunto condicional de SMS{#condition-subject-line}

Para criar uma linha de assunto condicional para uma mensagem SMS, siga as etapas abaixo:

1. Abra um delivery e edite o conteúdo.
1. Clique no ícone Abrir caixa de diálogo de personalização, à direita da linha de assunto.
1. No editor de personalização, navegue até


```sql
<% if 
(recipient.email == 'recipient@domain.com' ) 
{ % >
<table>
    <tr>
        <td>variant A</td>
    </tr>
</table>
< % } 
else 
{ % >
<table>
    <tr>
        <td>variant B< td>
    </tr>
</table>
< % } 
%>
```
