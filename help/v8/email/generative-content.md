---
audience: end-user
title: Texto com o Assistente de IA
description: Introdução ao Assistente de IA no Campaign
badge: label="Beta"
exl-id: d9d35c1d-13db-4d2c-82f8-1629fd1e5848
hide: true
hidefromtoc: true
source-git-commit: 23c43fad6076fc1dd1eaec2aee1664773ac7ce09
workflow-type: tm+mt
source-wordcount: '1097'
ht-degree: 5%

---

# Geração de email com o Assistente de IA {#generative-content}

>[!BEGINSHADEBOX]

**Índice**

* [Introdução ao assistente de IA](generative-gs.md)
* **[Geração de email com o Assistente de IA](generative-content.md)**
* [Geração de SMS com o Assistente de IA](generative-sms.md)
* [Geração de notificação por push com o Assistente de IA](generative-push.md)

>[!ENDSHADEBOX]

Depois de criar e personalizar seus emails, use o Assistente de IA do Journey Optimizer no Campaign viabilizado pela IA gerativa para elevar seu conteúdo ao próximo nível.

O Assistente de IA pode ajudá-lo a otimizar o impacto de suas entregas, sugerindo conteúdo diferente que tenha mais probabilidade de repercutir com seu público-alvo.

>[!NOTE]
>
>Antes de começar a usar esse recurso, leia as informações relacionadas [Medidas de proteção e limitações](generative-gs.md#guardrails-and-limitations).

## Geração de conteúdo com o Assistente de IA {#generative-text}

Veja como o Assistente de IA pode ajudar você a escrever emails atraentes:

* **Resuma**: informações longas podem sobrecarregar os recipients de email. Use o Assistente de IA para condensar os pontos principais em resumos claros e concisos que chamem a atenção e os incentivem a ler mais.

* **Elaborar**: O Assistente de IA pode ajudá-lo a abordar tópicos específicos, fornecendo detalhes adicionais para melhorar a compreensão e o engajamento.

* **Simplificar idioma**: use o Assistente de IA para simplificar o seu idioma, garantindo clareza e acessibilidade para um público-alvo maior.

* **Refrase**: O Assistente de IA pode reformular sua mensagem de maneiras diferentes, mantendo sua escrita atualizada e atraente para públicos-alvo diversos.

* **Alterar Tom**: o tom do seu email deve refletir no seu público-alvo. Se você quiser soar informativo, divertido ou persuasivo, o Assistente de IA poderá adaptar a mensagem de acordo.

No exemplo a seguir, aproveitaremos o assistente de IA para aprimorar o conteúdo de nosso convite por email para o evento futuro.

1. Depois de criar e configurar o delivery de email, clique em **[!UICONTROL Editar conteúdo]**.

   Para obter mais informações sobre como configurar o delivery de email, consulte [esta página](../email/create-email-content.md).

1. Personalize seu email conforme necessário e acesse o **[!UICONTROL Assistente de IA]** menu.

   Você também pode selecionar um **[!UICONTROL Componente de texto]** para direcionar somente a um conteúdo específico.

   ![](assets/text-genai-1.png){zoomable=&quot;yes&quot;}

1. Ativar o **[!UICONTROL Usar conteúdo original]** opção do Assistente de IA para personalizar novo conteúdo com base na entrega, nome da entrega e público-alvo selecionado.

   >[!IMPORTANT]
   >
   > Seu prompt deve estar sempre vinculado a um contexto específico, carregando um ativo de marca ou habilitando o **[!UICONTROL Melhorar conteúdo atual]** opção.

1. Ajuste o conteúdo descrevendo o que você deseja gerar na variável **[!UICONTROL Aviso]** campo.

   Se você estiver procurando ajuda para elaborar seu prompt, acesse o **[!UICONTROL Biblioteca de Prompts]** que fornece uma variedade diversa de ideias rápidas para melhorar seus deliveries.

   ![](assets/text-genai-2.png){zoomable=&quot;yes&quot;}

1. É possível alternar a variável **[!UICONTROL Linha de assunto]** ou **[!UICONTROL Pré-cabeçalho]** para incluí-los na geração da variante.

   Observe que isso estará disponível se você não tiver selecionado um componente de Texto específico.

1. Clique em **[!UICONTROL Fazer upload do ativo da marca]** para adicionar qualquer ativo de marca com conteúdo que possa fornecer contexto adicional ao Assistente de IA.

   ![](assets/text-genai-3.png){zoomable=&quot;yes&quot;}

1. Personalize seu prompt com as diferentes opções:

   * **[!UICONTROL Estratégia de comunicação]**: selecione a abordagem de comunicação desejada para o texto gerado.
   * **[!UICONTROL Idioma]**: escolha o idioma para o conteúdo da variante.
   * **[!UICONTROL Tom]**: verifique se o texto é apropriado para seu público-alvo e sua finalidade.
   * **[!UICONTROL Comprimento]**: selecione o comprimento do conteúdo usando o controle deslizante de intervalo. Disponível somente se você tiver selecionado um componente Texto específico.

   ![](assets/text-genai-4.png){zoomable=&quot;yes&quot;}

1. Quando o prompt estiver pronto, clique em **[!UICONTROL Gerar]**.

1. Navegue pelo arquivo gerado **[!UICONTROL Variações]** e clique em **[!UICONTROL Visualizar]** para exibir uma versão em tela cheia da variação selecionada.

1. Navegue até a **[!UICONTROL Refinar]** opção no campo **[!UICONTROL Visualizar]** para acessar recursos de personalização adicionais e ajustar a variação de acordo com suas preferências.

   Clique em **[!UICONTROL Selecionar]** depois de encontrar o conteúdo apropriado.

   ![](assets/text-genai-5.png){zoomable=&quot;yes&quot;}

1. Insira campos de personalização para personalizar seu conteúdo de email com base nos dados de perfis. Em seguida, clique no link **[!UICONTROL Simular conteúdo]** botão para controlar a renderização e verificar as configurações de personalização com perfis de teste. [Saiba mais](../preview-test/preview-content.md)

   ![](assets/text-genai-7.png){zoomable=&quot;yes&quot;}

Depois de definir seu conteúdo, público-alvo e agendamento, você estará pronto para preparar seu delivery de email. [Saiba mais](../monitor/prepare-send.md)

## Geração de imagens com o Assistente de IA {#generative-image}

Aproveite o Assistente de IA para gerar visuais diversificados e personalizados para suas campanhas de email. Por exemplo, ela pode ser usada para:

* **Gerar**: gere uma variedade diversa de imagens atraentes especificamente projetadas para suas campanhas de email. O controle granular sobre configurações como paleta de cores, raio e composição permite que você repercuta com segmentos de público distintos e atinja seus objetivos exclusivos de campanha.

* **Gerar semelhante**: use o Assistente de IA para gerar imagens semelhantes de uma variante selecionada.

* **Ativo da marca**: otimize a seleção de imagens para campanhas de email aproveitando os ativos de marca internos e fontes externas, como o Adobe Firefly.

No exemplo abaixo, aprenda a usar o Assistente de IA para otimizar e melhorar o conteúdo, garantindo uma experiência mais fácil de usar. Siga estas etapas:

1. Depois de criar e configurar o delivery de email, clique em **[!UICONTROL Editar conteúdo]**.

   Para obter mais informações sobre como configurar o delivery de email, consulte [esta página](../email/create-email-content.md).

1. Preencha o **[!UICONTROL Detalhes básicos]** para o seu delivery. Depois de concluído, clique em **[!UICONTROL Editar conteúdo de email]**.

1. Selecione o ativo que deseja alterar com o Assistente de IA.

1. No menu à direita, selecione **[!UICONTROL Assistente de IA]**.

   ![](assets/image-genai-1.png){zoomable=&quot;yes&quot;}

1. Ajuste o conteúdo descrevendo o que você deseja gerar na variável **[!UICONTROL Aviso]** campo.

   Se você estiver procurando ajuda para elaborar seu prompt, acesse o **[!UICONTROL Biblioteca de Prompts]** que fornece uma variedade diversa de ideias rápidas para melhorar seus deliveries.

   ![](assets/image-genai-2.png){zoomable=&quot;yes&quot;}

1. Clique em **[!UICONTROL Fazer upload do ativo da marca]** para adicionar qualquer ativo de marca com conteúdo que possa fornecer contexto adicional ao Assistente de IA.

   >[!IMPORTANT]
   >
   > Seu prompt deve estar sempre vinculado a um contexto específico.

1. Personalize seu prompt com as diferentes opções:

   * **[!UICONTROL Taxa de proporção]**: determina a largura e a altura do ativo. Você tem a opção de escolher entre taxas comuns, como 16:9, 4:3, 3:2 ou 1:1, ou pode inserir um tamanho personalizado.
   * **[!UICONTROL Cor e tom]**: a aparência geral das cores em uma imagem e o humor ou atmosfera transmitidos.
   * **[!UICONTROL Tipo de conteúdo]**: categoriza a natureza do elemento visual, distinguindo entre diferentes formas de representação visual, como fotos, gráficos ou arte.
   * **[!UICONTROL Iluminação]**: refere-se aos relâmpagos presentes em uma imagem, que molda sua atmosfera e destaca elementos específicos.
   * **[!UICONTROL Composição]**: refere-se à disposição dos elementos dentro do quadro de uma imagem

   ![](assets/image-genai-3.png){zoomable=&quot;yes&quot;}

1. Quando estiver satisfeito com a configuração do prompt, clique em **[!UICONTROL Gerar]**.

1. Navegue pelo **[!UICONTROL Sugestões de variação]** para encontrar o ativo desejado.

   Clique em **[!UICONTROL Visualizar]** para exibir uma versão em tela cheia da variação selecionada.

   ![](assets/image-genai-5.png){zoomable=&quot;yes&quot;}

1. Escolher **[!UICONTROL Mostrar semelhante]** se você quiser exibir imagens relacionadas a essa variante.

1. Clique em **[!UICONTROL Selecionar]** depois de encontrar o conteúdo apropriado.

   ![](assets/image-genai-6.png){zoomable=&quot;yes&quot;}

1. Depois de definir o conteúdo da mensagem, clique no link **[!UICONTROL Simular conteúdo]** botão para controlar a renderização e verificar as configurações de personalização com perfis de teste.  [Saiba mais](../preview-test/preview-content.md)

   ![](assets/image-genai-7.png){zoomable=&quot;yes&quot;}

1. Depois de definir seu conteúdo, público-alvo e agendamento, você estará pronto para preparar seu delivery de email. [Saiba mais](../monitor/prepare-send.md)
