---
audience: end-user
title: Notificação por push com o Assistente de IA no Campaign
description: Introdução ao Assistente de IA no Campaign
badge: label="Beta"
hide: true
hidefromtoc: true
exl-id: a361f75d-63c2-4fdc-993c-f8414b18e13e
source-git-commit: f249a73e25857e65e200f3cbd9516206aab918f9
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 9%

---

# Geração de notificação por push com o Assistente de IA {#generative-push}

>[!BEGINSHADEBOX]

**Índice**

* [Introdução ao assistente de IA](generative-gs.md)
* [Geração de email com o Assistente de IA](generative-content.md)
* [Geração de SMS com o Assistente de IA](generative-sms.md)
* **[Geração de notificação por push com o Assistente de IA](generative-push.md)**

>[!ENDSHADEBOX]


O Assistente de IA pode ajudá-lo a otimizar o impacto de suas entregas, sugerindo conteúdo diferente que tenha mais probabilidade de repercutir com seu público-alvo.

Com o Assistente de IA, seu conteúdo pode ser elevado a novos patamares. Por exemplo, ela pode ser usada para:

* **Resuma**: concentre conteúdo longo em resumos sucintos para notificações por push. Vá direto ao ponto e certifique-se de que os recipients entendam a mensagem principal instantaneamente.
* **Elaborar**: expanda os tópicos em suas notificações por push, fornecendo detalhes adicionais e contexto para compreender melhor.
* **Simplificar idioma**: torne suas notificações por push acessíveis a um público-alvo maior usando uma linguagem clara e concisa.
* **Refrase**: Evite a repetição fazendo com que o Assistente de IA reformule a mensagem de maneiras diferentes
* **Alterar Tom**: altere o tom emocional das notificações por push. Se você deseja parecer informativo, divertido ou urgente, o Assistente de IA pode adaptar a mensagem de acordo.

>[!NOTE]
>
>Antes de começar a usar esse recurso, leia as informações relacionadas [Medidas de proteção e limitações](generative-gs.md#guardrails-and-limitations).

No exemplo a seguir, aproveitaremos o assistente de IA para criar mensagens atraentes e criar uma experiência do cliente mais envolvente.

1. Depois de criar e configurar o delivery de notificação por push, clique em **[!UICONTROL Editar conteúdo]**.

   Para obter mais informações sobre como configurar o delivery por push, consulte [esta página](../push/create-push.md).

1. Preencha o **[!UICONTROL Detalhes básicos]** para o seu delivery. Depois de concluído, clique em **[!UICONTROL Editar conteúdo]**.

1. Personalize sua notificação por push conforme necessário. [Saiba mais](../push/content-push.md)

1. Acesse o **[!UICONTROL Mostrar assistente de IA]** menu.

   ![](assets/push-genai-1.png){zoomable=&quot;yes&quot;}

1. Ajuste o conteúdo descrevendo o que você deseja gerar na variável **[!UICONTROL Aviso]** campo.

   Se você estiver procurando ajuda para elaborar seu prompt, acesse o **[!UICONTROL Biblioteca de Prompts]** que fornece uma variedade diversa de ideias rápidas para melhorar seus deliveries.

   ![](assets/push-genai-2.png){zoomable=&quot;yes&quot;}

1. Ativar o **[!UICONTROL Aprimorar com o contexto atual]** opção do Assistente de IA para personalizar novo conteúdo com base na entrega, nome da entrega e público-alvo selecionado.

   >[!IMPORTANT]
   >
   > Seu prompt deve estar sempre vinculado a um contexto específico, carregando um ativo de marca ou habilitando o **[!UICONTROL Melhorar conteúdo atual]** opção.

   ![](assets/push-genai-3.png){zoomable=&quot;yes&quot;}

1. Selecionar **[!UICONTROL Fazer upload do ativo da marca]** para adicionar qualquer ativo de marca com conteúdo que possa fornecer contexto adicional ao Assistente de IA.

1. Escolha qual campo você deseja gerar: **[!UICONTROL Título]**, **[!UICONTROL Legenda]** ou **[!UICONTROL Mensagem]**.

1. Selecione o **[!UICONTROL Estratégia de comunicação]** que melhor atenda às suas necessidades. Isso afetará o tom e o estilo do texto gerado.

1. Escolha o **[!UICONTROL Idioma]** e **[!UICONTROL Tom]** que você deseja que o texto gerado tenha. Isso garantirá que o texto seja adequado ao seu público-alvo e propósito.

   ![](assets/push-genai-4.png){zoomable=&quot;yes&quot;}

1. Quando o prompt estiver pronto, clique em **[!UICONTROL Gerar]**.

1. Navegue pelo arquivo gerado **[!UICONTROL Variações]** e clique em **[!UICONTROL Aplicar]** depois de encontrar o conteúdo apropriado.

   Clique em **[!UICONTROL Visualizar]** para exibir uma versão em tela cheia da variação selecionada.

   ![](assets/push-genai-5.png){zoomable=&quot;yes&quot;}

1. Insira campos de personalização para personalizar o conteúdo de push com base nos dados de perfis. [Saiba mais sobre a personalização de conteúdo](../personalization/personalize.md)

   ![](assets/push-genai-6.png){zoomable=&quot;yes&quot;}

1. Depois de definir o conteúdo da mensagem, clique no link **[!UICONTROL Simular conteúdo]** botão para controlar a renderização e verificar as configurações de personalização com perfis de teste. [Saiba mais](../preview-test/preview-content.md)

   ![](assets/push-genai-7.png){zoomable=&quot;yes&quot;}

1. Depois de definir seu conteúdo, público-alvo e programação, você estará pronto para preparar sua entrega por push. [Saiba mais](../monitor/prepare-send.md)
