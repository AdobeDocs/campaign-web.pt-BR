---
audience: end-user
title: Notificação por push com o Assistente de IA
description: Introdução ao Assistente de IA
exl-id: a361f75d-63c2-4fdc-993c-f8414b18e13e
source-git-commit: 127c65a466c41e1aba8408aa9cf41c2d89c93801
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 2%

---

# Geração de notificação por push com o Assistente de IA {#generative-push}

>[!IMPORTANT]
>
>Antes de começar a usar este recurso, leia as [Medidas de Proteção e Limitações](generative-gs.md#generative-guardrails) relacionadas.
>></br>
>
>Você deve concordar com um [contrato de usuário](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) antes de usar o Assistente de IA no Adobe Campaign Web. Para mais informações, entre em contato com o seu representante da Adobe.

O Assistente de IA ajuda a otimizar o impacto de suas entregas, sugerindo conteúdo diferente que repercuta com seu público-alvo.

No exemplo a seguir, o Assistente de IA é aproveitado para criar mensagens atraentes e proporcionar uma experiência do cliente mais envolvente.

1. Depois de criar e configurar a entrega de notificação por push, clique em **[!UICONTROL Editar conteúdo]**.

   Para obter mais informações sobre como configurar a entrega por push, consulte [esta página](../push/create-push.md).

1. Acesse o menu **[!UICONTROL Mostrar assistente de IA]**.

   ![Captura de tela mostrando o menu Mostrar Assistente de IA](assets/push-genai-1.png){zoomable="yes"}

1. Habilite a opção **[!UICONTROL Usar conteúdo original]** para que o Assistente de IA personalize o novo conteúdo com base no conteúdo selecionado.

1. Ajuste o conteúdo descrevendo o que você deseja gerar no campo **[!UICONTROL Prompt]**.

   Se precisar de ajuda para criar seu prompt, acesse a **[!UICONTROL Biblioteca de Prompts]**, que fornece diversas ideias de prompt para melhorar suas entregas.

   ![Captura de tela mostrando a interface da Biblioteca de Prompts](assets/push-genai-2.png){zoomable="yes"}

1. Escolha o campo que deseja gerar: **[!UICONTROL Título]**, **[!UICONTROL Subtítulo]**, **[!UICONTROL Mensagem]** e/ou **[!UICONTROL Imagem]**.

1. Personalize seu prompt usando a opção **[!UICONTROL Configurações de texto]**:

   * **[!UICONTROL Estratégia de comunicação]**: escolha o estilo de comunicação mais adequado para o texto gerado.
   * **[!UICONTROL Tom]**: ajuste o tom do seu email para refletir com o seu público-alvo. Se você quiser soar informativo, divertido ou persuasivo, o Assistente de IA adapta a mensagem de acordo.

   ![Captura de tela mostrando as opções de configuração de texto](assets/push-genai-3.png){zoomable="yes"}

1. Escolha suas **[!UICONTROL configurações de imagem]**:

   * **[!UICONTROL Tipo de conteúdo]**: categorize a natureza do elemento visual, distinguindo entre diferentes formas de representação visual, como fotos, gráficos ou arte.
   * **[!UICONTROL Intensidade visual]**: controle o impacto da imagem ajustando sua intensidade. Uma configuração mais baixa (2) cria uma aparência mais suave e mais restrita, enquanto uma configuração mais alta (10) torna a imagem mais vibrante e visualmente poderosa.
   * **[!UICONTROL Iluminação]**: Ajuste a iluminação na imagem para moldar sua atmosfera e destacar elementos específicos.
   * **[!UICONTROL Composição]**: organizar elementos dentro do quadro da imagem.

   ![Captura de tela mostrando as opções de configuração de imagem](assets/push-genai-4.png){zoomable="yes"}

1. No menu **[!UICONTROL Ativos de marca]**, clique em **[!UICONTROL Carregar ativo de marca]** para adicionar qualquer ativo de marca que contenha conteúdo que forneça contexto adicional ao Assistente de IA ou selecione um ativo carregado anteriormente.

   Os arquivos carregados anteriormente estão disponíveis no menu suspenso **[!UICONTROL Ativos de marca carregados]**. Alterne os ativos que deseja incluir na geração.

1. Quando o prompt estiver pronto, clique em **[!UICONTROL Gerar]**.

1. Navegue pelas **[!UICONTROL Variações]** geradas e clique em **[!UICONTROL Visualizar]** para exibir uma versão em tela inteira da variação selecionada ou **[!UICONTROL Aplicar]** para substituir o conteúdo atual.

1. Clique no ícone de porcentagem para exibir sua **[!UICONTROL Pontuação de alinhamento da marca]** e identificar quaisquer desalinhamentos com sua marca.

   Saiba mais sobre [Pontuação de alinhamento da marca](../content/brands-score.md).

   ![](assets/push-genai-6.png){zoomable="yes"}

1. Navegue até a opção **[!UICONTROL Refinar]** na janela **[!UICONTROL Visualizar]** para acessar recursos de personalização adicionais:

   * **[!UICONTROL Usar como conteúdo de referência]**: usar a variante escolhida como conteúdo de referência para gerar outros resultados.
   * **[!UICONTROL Refrase]**: reformule sua mensagem de diferentes maneiras para manter sua escrita atualizada e envolvente para públicos diversos.
   * **[!UICONTROL Usar linguagem mais simples]**: simplifique sua linguagem para garantir clareza e acessibilidade para um público-alvo maior.

   Você também pode alterar o **[!UICONTROL Tom]** e a **[!UICONTROL estratégia de comunicação]** do seu texto.

   ![Captura de tela mostrando as opções de Refinar](assets/push-genai-5.png){zoomable="yes"}

1. Abra a guia **[!UICONTROL Alinhamento da marca]** para ver como o seu conteúdo se alinha às suas [diretrizes da marca](../content/brands.md).

1. Clique em **[!UICONTROL Selecionar]** depois de encontrar o conteúdo apropriado.

1. Insira campos de personalização para personalizar seu conteúdo de email com base nos dados do perfil. Em seguida, clique no botão **[!UICONTROL Simular conteúdo]** para controlar a renderização e verificar as configurações de personalização com perfis de teste. [Saiba mais](../preview-test/preview-content.md)

Ao definir seu conteúdo, público-alvo e agendamento, prepare sua entrega por push. [Saiba mais](../monitor/prepare-send.md)