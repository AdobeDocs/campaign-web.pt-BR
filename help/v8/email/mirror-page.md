---
audience: end-user
title: Adicionar um link para a mirror page
description: Saiba como adicionar e gerenciar o link para a mirror page
exl-id: 0c22357f-0465-4fdc-833e-5fda5805fe42
source-git-commit: 81fa26e44739d70218b949712a41a3d520900fa0
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 96%

---

# Adicionar um link para a mirror page{#mirror-page}

A mirror page é uma versão online do seu email.

Embora a maioria dos clientes de email renderize imagens sem problemas, algumas predefinições podem evitar a exibição de imagens por motivos de segurança. Os usuários podem navegar até a mirror page de um email. Por exemplo, se estiverem enfrentando problemas de renderização ou imagens quebradas ao tentar exibi-la em sua caixa de entrada. Também é recomendável fornecer uma versão online por motivos de acessibilidade ou incentivar o compartilhamento em redes sociais.

A mirror page gerada pelo Adobe Campaign contém todos os dados de personalização.

![amostra de mirror link](assets/mirror-page-link.png){width="600" align="left"}

## Adicionar um link para a mirror page{#link-to-mirror-page}

Inserir um link para a mirror page é uma boa prática. Esse link pode ser, por exemplo, &quot;Exibir este email em seu navegador&quot; ou &quot;Leia online&quot;. Geralmente, ele está localizado no cabeçalho ou no rodapé do email.

No Adobe Campaign, você pode inserir um link para a mirror page no conteúdo do email usando o **bloco de personalização** dedicado. O bloco de personalização do **Link integrado para a mirror page** insere o seguinte código no conteúdo do email: `<%@ include view='MirrorPage' %>`.

Para adicionar um link a uma mirror page no seu email:

1. Selecione um elemento e clique em **[!UICONTROL Inserir link]** na barra de ferramentas contextual.

   ![](assets/message-tracking-mirror-page.png){zoomable="yes"}

1. Selecione o ícone de **[!UICONTROL Adicionar personalização]** para acessar o menu de personalização.

   ![](assets/message-tracking-mirror-page_2.png){zoomable="yes"}

1. No menu **[!UICONTROL Bloco de conteúdo]**, selecione o **[!UICONTROL URL da mirror page]** e clique em **[!UICONTROL Adicionar]**.

   ![](assets/message-tracking-mirror-page_3.png){zoomable="yes"}

   Para obter mais informações sobre a inserção de blocos de conteúdo personalizados, consulte [esta seção](../personalization/personalize.md#personalize-emails).

A mirror page é criada automaticamente.

>[!IMPORTANT]
>
>Os links de mirror pages são gerados automaticamente e não podem ser editados. Eles contêm todos os dados personalizados criptografados necessários para renderizar o email original. Como resultado, o uso de atributos personalizados com valores grandes pode gerar URLs de mirror pages longos, o que pode impedir que o link funcione em navegadores da Web com tamanho máximo de URLs.

Depois que o email for enviado, quando os destinatários clicarem no link da mirror page, o conteúdo do email será exibido no navegador web padrão.

>[!NOTE]
>
>Na prova enviada aos perfis de teste, o link para a mirror page não está ativo. Ele só é ativado nas mensagens finais.

Por padrão, o período de retenção de uma mirror page é de 60 dias. Após esse atraso, a mirror page não estará mais disponível.


## Geração de mirror page{#mirror-page-generation}

Por padrão, a mirror page é gerada automaticamente pelo Adobe Campaign se o conteúdo do email não estiver vazio e se contiver um link para a mirror page (também conhecida como Mirror link).

Você pode controlar o modo de geração da mirror page de email. As opções estão disponíveis nas propriedades de entrega. [Saiba mais](../advanced-settings/delivery-settings.md#mirror)
