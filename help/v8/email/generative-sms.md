---
audience: end-user
title: SMS com o Assistente de IA no Campaign
description: Introdução ao Assistente de IA no Campaign
badge: label="Beta"
hide: true
hidefromtoc: true
exl-id: db0459e5-8759-42d9-8945-8c9667450527
source-git-commit: fe687647b0a3d4969373ced400c49b364e878acd
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 9%

---

# Geração de SMS com o Assistente de IA {#generative-sms}

>[!BEGINSHADEBOX]

**Índice**

* [Introdução ao assistente de IA](generative-gs.md)
* [Geração de email com o Assistente de IA](generative-content.md)
* Geração de SMS com o Assistente de IA
* [Geração de notificação por push com o Assistente de IA](generative-push.md)

>[!ENDSHADEBOX]

Depois de criar e personalizar suas mensagens SMS para atender ao seu público-alvo, leve sua comunicação para o próximo nível com a ajuda do Assistente de IA do Campaign, viabilizada pela tecnologia inovadora de IA.

Essa ferramenta útil fornece sugestões inteligentes para refinar seu conteúdo, garantindo que suas mensagens repercutam com eficiência e maximizem o engajamento.

>[!NOTE]
>
>Antes de começar a usar esse recurso, leia as [Medidas de Proteção e Limitações](generative-gs.md#generative-guardrails) relacionadas.

1. Depois de criar e configurar a entrega de SMS, clique em **[!UICONTROL Editar conteúdo]**.

   Para obter mais informações sobre como configurar a entrega de SMS, consulte [esta página](../sms/create-sms.md).

1. Preencha os **[!UICONTROL detalhes Básicos]** da sua entrega. Depois de concluído, clique em **[!UICONTROL Editar conteúdo]**.

1. Personalize a mensagem SMS conforme necessário. [Saiba mais](../sms/content-sms.md)

1. Acesse o menu **[!UICONTROL Mostrar assistente de IA]**.

   ![](assets/sms-genai-1.png){zoomable="yes"}

1. Habilite a opção **[!UICONTROL Usar conteúdo original]** para que o Assistente de IA personalize novo conteúdo com base na sua entrega, nome de entrega e público selecionado.

   >[!IMPORTANT]
   >
   > Seu prompt deve estar sempre vinculado ao conteúdo atual.

1. Ajuste o conteúdo descrevendo o que você deseja gerar no campo **[!UICONTROL Prompt]**.

   Se você estiver procurando ajuda para criar seu prompt, acesse a **[!UICONTROL Biblioteca de Prompts]**, que fornece diversas ideias de prompt para melhorar suas entregas.

   ![](assets/sms-genai-2.png){zoomable="yes"}

1. Selecione **[!UICONTROL Carregar ativo de marca]** para adicionar qualquer ativo de marca que contenha conteúdo que possa fornecer contexto adicional ao Assistente de IA.

1. Personalize seu prompt com as diferentes opções:

   * **[!UICONTROL Estratégia de comunicação]**: selecione a abordagem de comunicação desejada para o texto gerado.
   * **[!UICONTROL Idioma]**: escolha o idioma para o conteúdo da variante.
   * **[!UICONTROL Tone]**: certifique-se de que o texto é apropriado para seu público-alvo e sua finalidade.
   * **[!UICONTROL Comprimento]**: selecione o comprimento do conteúdo usando o controle deslizante de intervalo.

   ![](assets/sms-genai-3.png){zoomable="yes"}

1. Quando o prompt estiver pronto, clique em **[!UICONTROL Gerar]**.

1. Navegue pelas **[!UICONTROL Variações]** geradas e clique em **[!UICONTROL Visualizar]** para exibir uma versão em tela inteira da variação selecionada.

1. Navegue até a opção **[!UICONTROL Refinar]** na janela **[!UICONTROL Visualizar]** para acessar recursos de personalização adicionais e ajustar a variação de acordo com suas preferências:

   * **[!UICONTROL Usar como conteúdo de referência]**: a variante escolhida servirá como conteúdo de referência para gerar outros resultados.

   * **[!UICONTROL Usar linguagem mais simples]**: o assistente de IA ajuda você a escrever mensagens claras e concisas que todos possam entender.

   * **[!UICONTROL Refrase]**: o Assistente de IA reformula sua mensagem para manter as coisas atraentes para públicos diferentes.

   ![](assets/sms-genai-4.png){zoomable="yes"}

1. Clique em **[!UICONTROL Selecionar]** depois de encontrar o conteúdo apropriado.

1. Insira campos de personalização para personalizar o conteúdo de SMS com base nos dados de perfis. [Saiba mais sobre a personalização de conteúdo](../personalization/personalize.md)

   ![](assets/sms-genai-5.png){zoomable="yes"}

1. Após definir o conteúdo da mensagem, clique no botão **[!UICONTROL Simular conteúdo]** para controlar a renderização e verificar as configurações de personalização com perfis de teste. [Saiba mais](../preview-test/preview-content.md)

   ![](assets/sms-genai-6.png){zoomable="yes"}

Depois de definir seu conteúdo, público-alvo e programação, você estará pronto para preparar sua entrega de SMS. [Saiba mais](../monitor/prepare-send.md)
