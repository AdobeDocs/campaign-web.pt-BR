---
audience: end-user
title: Edição do conteúdo de email
description: Saiba como começar a criar conteúdo usando o Designer de email na interface do Campaign Web
exl-id: a5b966bb-09da-4a50-98d4-010fdfbb75cf
source-git-commit: eccd1ce6f95682d3dcfc224061f747f7da0b6681
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 45%

---


# Introdução ao Designer de email {#get-started-email-designer}

Após criar um email no Adobe Campaign, é necessário definir seu conteúdo.

O Designer de email permite criar emails atraentes e personalizados por meio de uma interface intuitiva de arrastar e soltar. Esteja você iniciando do zero, importando conteúdo existente ou aproveitando modelos existentes, projete e refine todo o conteúdo para cada email, seja ele promocional ou transacional.

<!--Built to deliver HTML optimized for responsive design, the Email Designer allows you to easily define and apply visibility conditions and dynamic content to an email, template, or content fragment directly through the user interface. You can seamlessly switch between the drag and drop interface and HTML code at the click of a button.

The Email Designer allows you to create email content and email content templates. It is compatible with simple emails, transactional emails, A/B test emails, multilingual emails, and recurring emails.-->

* Use os recursos de design de email do [!DNL Campaign] para criar emails responsivos com facilidade. [Saiba mais](create-email-content.md)

* Melhorar a experiência dos clientes criando emails personalizados com base em seus atributos de perfil. [Saiba mais](../personalization/personalize.md)

* Configure campos de conteúdo condicional para criar personalizações dinâmicas com base no perfil do destinatário. [Saiba mais](../personalization/conditions.md)

## Práticas recomendadas de design de emails {#best-practices}

Ao enviar emails, considere que os recipients podem encaminhá-los, o que às vezes pode causar problemas na renderização do email. Isso é particularmente verdadeiro ao usar classes CSS que podem não ser suportadas pelo provedor de email usado para encaminhamento. Por exemplo, se você usar a classe CSS &quot;is-desktop-hidden&quot; para ocultar uma imagem em dispositivos móveis, ela pode não ser renderizada corretamente.

Para minimizar esses problemas de renderização, mantenha sua estrutura de design de email a mais simples possível. Use um único design que funcione bem para dispositivos móveis e de desktop, e evite usar classes CSS complexas ou outros elementos de design que podem não ser totalmente compatíveis com todos os clientes de email. Ao seguir essas práticas recomendadas, você ajuda a garantir que seus emails sejam renderizados de forma consistente, independentemente de como são visualizados ou encaminhados pelos destinatários.

## Comece a criar seu conteúdo {#start-authoring}

No painel de entrega de email, passe pela tela [Editar conteúdo](edit-content.md) para abrir a página inicial do Designer de email. A partir daí, escolha como deseja criar seu email a partir das seguintes opções:

* **Criar o email do zero** por meio da interface do Designer de email. Saiba como criar seu conteúdo de email [nesta seção](create-email-content.md).

* **Desenvolver ou colar código HTML** diretamente no Designer de email. Saiba como desenvolver o código de seu próprio conteúdo [nesta seção](code-content.md).

* **Importar conteúdo HTML já existente** de um arquivo ou de uma pasta ZIP. Saiba como importar conteúdo de email [nesta seção](existing-content.md).

* **Selecionar um conteúdo já existente** de uma lista de modelos integrados ou personalizados. Saiba como trabalhar com modelos de email [nesta seção](create-email-templates.md).

  ![Opções disponíveis na interface do Email Designer para criar conteúdo de email](assets/email_designer_create_options.png){zoomable="yes"}
