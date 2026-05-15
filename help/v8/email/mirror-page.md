---
audience: end-user
title: Adicionar um link para a mirror page
description: Saiba como adicionar e gerenciar o link para a mirror page
exl-id: 0c22357f-0465-4fdc-833e-5fda5805fe42
TQID: https://experienceleague.adobe.com/iigr3vwibRH-qRbWaTXszxTuJqgdFJG6QEC1T9Z487s
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: beb7a3c1-66ab-4786-b879-7621375b3c40
  - id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 5a231f1dc49379d1be5d36e1732660111f851649
workflow-type: tm+mt
source-wordcount: 397
ht-degree: 19%

---

# Mirror page {#mirror-page}

A mirror page é uma versão online do seu email. Adicionar um link para a mirror page é uma boa prática no marketing por email. Os usuários podem acessar a mirror page de um email, por exemplo, se tiverem problemas de renderização ou imagens corrompidas ao visualizá-lo na caixa de entrada. O fornecimento de uma versão online também é recomendado por motivos de acessibilidade ou para incentivar o compartilhamento em redes sociais.

A mirror page gerada pelo Adobe Campaign inclui todos os dados de personalização.

![Exemplo de um mirror link em um email](assets/mirror-page-link.png){width="600" align="left"}

## Adicionar um link para a mirror page {#link-to-mirror-page}

No Adobe Campaign, insira um link para a mirror page do conteúdo do email usando o **bloco de personalização** dedicado. O bloco de personalização do **Link integrado para a mirror page** insere o seguinte código no conteúdo do email: `<%@ include view='MirrorPage' %>`.

Para adicionar um link a uma mirror page no seu email, siga estas etapas:

1. Selecione um elemento (texto ou imagem) e clique em **[!UICONTROL Inserir link]** na barra de ferramentas contextual.

   ![Barra de ferramentas contextual que mostra a opção Inserir link](assets/message-tracking-mirror-page.png){zoomable="yes"}

1. Selecione o ícone de **[!UICONTROL Adicionar personalização]** para acessar o menu de personalização.

   ![Menu Personalization no Adobe Campaign](assets/message-tracking-mirror-page_2.png){zoomable="yes"}

1. No menu **[!UICONTROL Fragmentos]**, selecione **[!UICONTROL URL da mirror page]** e clique em **[!UICONTROL Adicionar]**. [Saiba como usar fragmentos de expressão](../content/use-expression-fragments.md)

   ![Opção de URL da mirror page no menu Fragmentos](assets/message-tracking-mirror-page_3.png){zoomable="yes"}

A mirror page é criada automaticamente.

Quando o email é enviado, os recipients que clicam no link da mirror page veem o conteúdo do email exibido em seu navegador da Web padrão.

Por padrão, o período de retenção de uma mirror page é de **60 dias**. Após esse período, a mirror page não estará mais disponível.

>[!CAUTION]
>
>* Os links da mirror page são gerados automaticamente e não podem ser editados. Eles incluem todos os dados personalizados criptografados necessários para renderizar o email original. Usar atributos personalizados com valores grandes pode gerar URLs de mirror page longos, o que pode impedir que o link funcione em navegadores da Web com um comprimento máximo de URL.
>
>* Na prova enviada para perfis de teste, o link para a mirror page não está ativo. Ela só estará ativa nas mensagens finais.

## Geração de mirror page {#mirror-page-generation}

Por padrão, o Adobe Campaign gera automaticamente a mirror page se o conteúdo do email não estiver vazio e contiver um link para a mirror page (também conhecido como Mirror link).

Controle o modo de geração da mirror page do email por meio das opções disponíveis nas propriedades de delivery. [Saiba mais](../advanced-settings/delivery-settings.md#mirror)