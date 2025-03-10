---
audience: end-user
title: Adicionar um link para a mirror page
description: Saiba como adicionar e gerenciar o link para a mirror page
exl-id: 0c22357f-0465-4fdc-833e-5fda5805fe42
source-git-commit: 00a612513bcb649d23b2c5b4d5ed05b06a6a80ef
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 73%

---

# Mirror page {#mirror-page}

A mirror page é uma versão online do email. Adicionar um link para a mirror page é uma prática recomendada de marketing por email. Os usuários podem navegar até a mirror page de um email. Por exemplo, se estiverem enfrentando problemas de renderização ou imagens quebradas ao tentar exibi-la em sua caixa de entrada. Também é recomendável fornecer uma versão online por motivos de acessibilidade ou incentivar o compartilhamento em redes sociais.

A mirror page gerada pelo Adobe Campaign contém todos os dados de personalização.

![amostra de mirror link](assets/mirror-page-link.png){width="600" align="left"}

## Adicionar um link para a mirror page{#link-to-mirror-page}

No Adobe Campaign, você pode inserir um link para a mirror page no conteúdo do email usando o **bloco de personalização** dedicado. O bloco de personalização do **Link integrado para a mirror page** insere o seguinte código no conteúdo do email: `<%@ include view='MirrorPage' %>`.

Para adicionar um link a uma mirror page no seu email, siga estas etapas:

1. Selecione um elemento (texto ou imagem) e clique em **[!UICONTROL Inserir link]** na barra de ferramentas contextual.

   ![](assets/message-tracking-mirror-page.png){zoomable="yes"}

1. Selecione o ícone de **[!UICONTROL Adicionar personalização]** para acessar o menu de personalização.

   ![](assets/message-tracking-mirror-page_2.png){zoomable="yes"}

1. No menu **[!UICONTROL Fragmentos]**, selecione **[!UICONTROL URL da mirror page]** e clique em **[!UICONTROL Adicionar]**. [Saiba como usar fragmentos de expressão](../content/use-expression-fragments.md)

   ![](assets/message-tracking-mirror-page_3.png){zoomable="yes"}

A mirror page é criada automaticamente.

Depois que o email for enviado, quando os destinatários clicarem no link da mirror page, o conteúdo do email será exibido no navegador web padrão.

Por padrão, o período de retenção de uma mirror page é de **60 dias**. Após esse atraso, a mirror page não estará mais disponível.

>[!CAUTION]
>
>* Os links de mirror pages são gerados automaticamente e não podem ser editados. Eles contêm todos os dados personalizados criptografados necessários para renderizar o email original. Como resultado, o uso de atributos personalizados com valores grandes pode gerar URLs de mirror pages longos, o que pode impedir que o link funcione em navegadores da Web com tamanho máximo de URLs.
>
>* Na prova enviada aos perfis de teste, o link para a mirror page não está ativo. Ela só estará ativa nas mensagens finais.


## Geração de mirror page {#mirror-page-generation}

Por padrão, a mirror page é gerada automaticamente pelo Adobe Campaign se o conteúdo do email não estiver vazio e se contiver um link para a mirror page (também conhecida como Mirror link).

Você pode controlar o modo de geração da mirror page de email. As opções estão disponíveis nas propriedades de entrega. [Saiba mais](../advanced-settings/delivery-settings.md#mirror)
