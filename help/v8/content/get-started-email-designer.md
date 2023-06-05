---
audience: end-user
title: Editar o conteúdo do email
description: Saiba como começar a criar conteúdo usando o Designer de email na interface do usuário da Web do Campaign
badge: label="Alpha" type="Positive"
source-git-commit: 983541f5dea47102ae9ee3c5351a7149484a1fa5
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 5%

---

# Introdução ao Designer de email {#get-started-email-designer}

É possível importar um conteúdo existente para o [!DNL Journey Optimizer] ou aproveitar os recursos de design de conteúdo:

* Uso [!DNL Campaign] recursos de design de email para criar e-mails responsivos com facilidade. [Saiba mais](create-email-content.md)

* Melhorar a experiência dos clientes criando produtos personalizados com base em seus atributos de perfil. [Saiba mais](../personalization/personalize.md)

* Configure campos de conteúdo condicional para criar personalização dinâmica com base no perfil do recipient. [Saiba mais](../personalization/conditions.md)

## Práticas recomendadas de design de email {#best-practices}

Ao enviar emails, é importante considerar que os recipients podem encaminhá-los, o que às vezes pode causar problemas na renderização do email. Isso é particularmente verdadeiro ao usar classes CSS que podem não ser suportadas pelo provedor de email usado para encaminhamento, por exemplo, se você estiver usando a classe CSS &quot;is-desktop-hidden&quot; para ocultar uma imagem em dispositivos móveis.

Para minimizar esses problemas de renderização, recomendamos manter a estrutura de design de email a mais simples possível. Tente usar um único design que funcione bem para dispositivos móveis e de desktop, e evite usar classes CSS complexas ou outros elementos de design que possam não ser totalmente compatíveis com todos os clientes de email. Seguindo essas práticas recomendadas, você pode ajudar a garantir que seus emails sejam renderizados de forma consistente corretamente, independentemente de como são visualizados ou encaminhados pelos destinatários.

## Comece a criar seu conteúdo {#start-authoring}

No painel de delivery de email, passe pelo link [Editar conteúdo](edit-content.md) para abrir a página inicial do Designer de email. A partir daí, escolha como deseja criar seu email a partir das seguintes opções:

* **Projetar o email do zero** por meio da interface do designer de email. Saiba como projetar seu conteúdo de email no [nesta seção](create-email-content.md).

* **Codificar ou colar HTML bruto** diretamente no designer de email. Saiba como codificar seu próprio conteúdo no [nesta seção](code-content.md).

* **Importar conteúdo de HTML existente** de um arquivo ou de uma pasta .zip. Saiba como importar um conteúdo de email no [nesta seção](existing-content.md).

* **Selecionar um conteúdo existente** de uma lista de modelos incorporados ou personalizados. Saiba como trabalhar com modelos de email [nesta seção](email-templates.md).

   ![](assets/email_designer_create_options.png)

