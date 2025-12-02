---
audience: end-user
title: Conteúdo gerativo
description: Saiba como gerar experiências de conteúdo de texto com o Assistente de IA
source-git-commit: 2066f29b0867f82f2130361c8ccdb15889085886
workflow-type: tm+mt
source-wordcount: '1441'
ht-degree: 1%

---

# Gerar texto com o Assistente de IA {#generative-text}

>[!IMPORTANT]
>
>Antes de começar a usar este recurso, leia as [Medidas de Proteção e Limitações](generative-gs.md#generative-guardrails) relacionadas.
></br>
>
>Você deve concordar com um [contrato de usuário](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"} antes de usar o Assistente de IA no Adobe Campaign Web. Para mais informações, entre em contato com o seu representante da Adobe.

Use o Assistente de IA na Web do Adobe Campaign para gerar um texto envolvente que repercuta em seu público-alvo. Quer você esteja aprimorando a cópia de emails, criando conteúdo persuasivo de página de aterrissagem, escrevendo mensagens de notificação por push ou compondo texto SMS, o Assistente de IA ajuda a fornecer comunicação clara e impactante.

## Para emails e landing pages {#email-web-channels}

O AI Assistant pode gerar conteúdo de texto de alta qualidade para seus deliveries de email e landing pages. Esse recurso permite criar mensagens atraentes na marca que se conectam com seu público-alvo em pontos de contato digitais.

### Acessar e configurar {#access-configure}

Antes de começar a gerar conteúdo de texto com o AI Assistant, você precisará configurar o delivery e acessar o editor de conteúdo. Siga estas etapas para preparar seu espaço de trabalho e abrir o painel Assistente de IA.

1. Criar e configurar o delivery:

   * **Email**: depois de criar e configurar sua entrega de email, clique em **[!UICONTROL Editar conteúdo]**. [Saiba mais](../email/create-email-content.md)
   * **Página de aterrissagem**: depois de criar e configurar sua página de aterrissagem, clique em **[!UICONTROL Editar conteúdo]**. [Saiba mais](../landing-pages/create-lp.md)

1. Selecione um **[!UICONTROL Componente de texto]** para direcionar conteúdo específico e acesse o menu **[!UICONTROL Assistente de IA]**.

   ![Captura de tela mostrando a seleção do componente de texto na Adobe Campaign Web](assets/text-genai-1.png){zoomable="yes"}

### Gerar conteúdo {#generate-content}

Saiba como criar solicitações claras, configurações de ajuste e gerar texto personalizado usando o Assistente de IA, garantindo que suas mensagens se alinhem às suas metas de marca e comunicação.

1. Selecione sua **[!UICONTROL Marca]** para garantir que o conteúdo gerado por IA esteja alinhado às especificações da sua marca. [Saiba mais](brands.md) sobre marcas.

1. Ajuste o conteúdo descrevendo o que você deseja gerar no campo **[!UICONTROL Prompt]**.

   Se precisar de ajuda para criar seu prompt, acesse a **[!UICONTROL Biblioteca de Prompts]**, que fornece diversas ideias de prompt para melhorar suas entregas. [Saiba mais sobre as práticas recomendadas do prompt](ai-assistant-prompting-guide.md)

   ![Captura de tela mostrando a biblioteca de prompts na Adobe Campaign Web](assets/text-genai-2.png){zoomable="yes"}

1. Personalize seu prompt usando a opção **[!UICONTROL Configurações de texto]**:

   * **[!UICONTROL Estratégia de comunicação]**: escolha o estilo de comunicação mais adequado para o texto gerado.
   * **[!UICONTROL Idiomas]**: escolha o idioma do conteúdo gerado.
   * **[!UICONTROL Tone]**: verifique se o tom do seu email está de acordo com o seu público-alvo. Se você quiser soar informativo, divertido ou persuasivo, o Assistente de IA adapta a mensagem de acordo.
   * **Comprimento do texto**: use o controle deslizante para selecionar o comprimento desejado do texto.

     ![Captura de tela mostrando as opções de configurações de texto na Adobe Campaign Web](assets/text-genai-4.png){zoomable="yes"}

1. No menu **[!UICONTROL Conteúdo de referência]**, clique em **[!UICONTROL Carregar arquivo]** para adicionar qualquer ativo de marca que contenha conteúdo que possa fornecer o Assistente de IA de contexto adicional ou selecione um que tenha sido carregado anteriormente.

   Os arquivos carregados anteriormente estão disponíveis no menu suspenso **[!UICONTROL Conteúdo de referência carregado]**. Basta alternar os ativos que deseja incluir na geração.

1. Quando o prompt estiver pronto, clique em **[!UICONTROL Gerar]**.

### Refinar e finalizar {#refine-finalize}

Saiba como revisar o texto gerado, fazer refinamentos e aplicar personalização para finalizar seu conteúdo, criando mensagens sofisticadas e envolventes prontas para entrega.

1. Navegue pelas **[!UICONTROL Variações]** geradas.

1. Clique no ícone de porcentagem para exibir sua **[!UICONTROL Pontuação de alinhamento da marca]** e identificar quaisquer desalinhamentos com sua marca.

   Saiba mais sobre [Pontuação de alinhamento da marca](brands-score.md).

   ![](assets/text-genai-6.png){zoomable="yes"}

1. Clique em **[!UICONTROL Visualizar]** para exibir uma versão em tela inteira da variação selecionada ou em **[!UICONTROL Aplicar]** para substituir o conteúdo atual.

1. Navegue até a opção **[!UICONTROL Refinar]** na janela **[!UICONTROL Visualizar]** para acessar recursos de personalização adicionais:

   * **[!UICONTROL Usar como conteúdo de referência]**: a variante escolhida serve como conteúdo de referência para gerar outros resultados.
   * **[!UICONTROL Elaborar]**: aprofunde-se em tópicos específicos, fornecendo detalhes adicionais para compreender e participar melhor.
   * **[!UICONTROL Resumir]**: condensa os pontos-chave em resumos claros e concisos para chamar a atenção e incentivar mais leituras.
   * **[!UICONTROL Refrase]**: reformule sua mensagem de maneiras diferentes, mantendo sua escrita atualizada e engajando públicos diversos.
   * **[!UICONTROL Usar linguagem mais simples]**: simplifique sua linguagem para garantir clareza e acessibilidade para um público-alvo maior.
   * **[!UICONTROL Traduzir]**: simplifique seu idioma para garantir clareza e acessibilidade para um público-alvo maior.

   Você também pode alterar o **[!UICONTROL Tom]** e a **[!UICONTROL estratégia de comunicação]** do seu texto.

   ![Captura de tela mostrando as opções de refinamento na Adobe Campaign Web](assets/text-genai-5.png){zoomable="yes"}

1. Abra a guia **[!UICONTROL Alinhamento da marca]** para ver como o seu conteúdo se alinha às suas [diretrizes da marca](../content/brands.md).

1. Clique em **[!UICONTROL Selecionar]** depois de encontrar o conteúdo apropriado.

1. Insira campos de personalização para personalizar seu conteúdo com base nos dados do perfil. Em seguida, clique no botão **[!UICONTROL Simular conteúdo]** para controlar a renderização e verificar as configurações de personalização com perfis de teste. [Saiba mais](../preview-test/preview-content.md)

1. Revise e ative o conteúdo:
   * **Email**: quando tiver definido seu conteúdo, público-alvo e agendamento, você estará pronto para preparar sua entrega de email. [Saiba mais](../monitor/prepare-send.md)
   * **Página de aterrissagem**: quando a página de aterrissagem estiver pronta, você poderá publicá-la para disponibilizá-la para uso em uma mensagem. [Saiba mais](../landing-pages/create-lp.md)

## Para canais móveis {#mobile-channels}

O Assistente de IA pode gerar conteúdo de texto atraente para suas notificações por push e mensagens SMS, ajudando você a criar comunicações móveis envolventes que se conectam com seu público-alvo em todos os pontos de contato móveis.

### Acessar e configurar {#mobile-access-configure}

Antes de começar a gerar texto com o Assistente de IA para canais móveis, você deve configurar o delivery e acessar o Assistente de IA.

1. Criar e configurar o delivery móvel:
   * **Notificações por push**: depois de criar e configurar sua entrega de notificação por push, clique em **[!UICONTROL Editar conteúdo]**. [Saiba mais](../push/create-push.md)
   * **SMS**: depois de criar e configurar sua entrega de SMS, clique em **[!UICONTROL Editar conteúdo]**. [Saiba mais](../sms/create-sms.md)

1. Personalize a mensagem conforme necessário:
   * **Notificações por push**: [Saiba mais](../push/content-push.md)
   * **SMS**: [Saiba mais](../sms/content-sms.md)

1. Acesse o menu **[!UICONTROL Mostrar assistente de IA]**.

   ![Captura de tela mostrando o menu Mostrar Assistente de IA](assets/sms-genai-1.png){zoomable="yes"}

### Gerar conteúdo {#mobile-generate-content}

Depois de acessar o Assistente de IA, você pode definir as configurações de geração para criar conteúdo móvel que corresponda à sua marca e metas de entrega. Personalize parâmetros de texto, adicione ativos de marca e forneça prompts para orientar a IA na geração de variações relevantes.

1. Selecione sua **[!UICONTROL Marca]** para garantir que o conteúdo gerado por IA esteja alinhado às especificações da sua marca. [Saiba mais](brands.md) sobre marcas.

1. Ajuste o conteúdo descrevendo o que você deseja gerar no campo **[!UICONTROL Prompt]**.

   Se você estiver procurando ajuda para criar seu prompt, acesse a **[!UICONTROL Biblioteca de Prompts]**, que fornece diversas ideias de prompt para melhorar sua entrega. [Saiba mais sobre as práticas recomendadas do prompt](ai-assistant-prompting-guide.md)

   ![Assistente de IA com campo de prompt e opções](assets/sms-genai-2.png){zoomable="yes"}

1. **Para notificações por push**, escolha o campo de texto que deseja gerar: **[!UICONTROL Título]**, **[!UICONTROL Subtítulo]** e/ou **[!UICONTROL Mensagem]**.

1. Personalize seu prompt com a opção **[!UICONTROL Configurações de texto]**:

   * **[!UICONTROL Estratégia de comunicação]**: escolha o estilo de comunicação mais adequado para o texto gerado.
   * **[!UICONTROL Idiomas]**: escolha o idioma do conteúdo gerado.
   * **[!UICONTROL Tone]**: o tom deve repercutir na audiência. Se você deseja parecer informativo, divertido ou persuasivo, o Assistente de IA pode adaptar a mensagem de acordo.
   * **[!UICONTROL Comprimento]**: selecione o comprimento do conteúdo usando o controle deslizante de intervalo.

     ![Painel de configurações de texto](assets/sms-genai-3.png){zoomable="yes"}

1. No menu **[!UICONTROL Conteúdo de referência]**, clique em **[!UICONTROL Carregar arquivo]** para adicionar qualquer ativo de marca que contenha conteúdo que possa fornecer o Assistente de IA de contexto adicional ou selecione um que tenha sido carregado anteriormente.

   Os arquivos carregados anteriormente estão disponíveis no menu suspenso **[!UICONTROL Conteúdo de referência carregado]**. Basta alternar os ativos que deseja incluir na geração.

1. Quando o prompt estiver pronto, clique em **[!UICONTROL Gerar]**.

### Refinar e finalizar {#mobile-refine-finalize}

Depois de gerar variações de texto para suas mensagens móveis, você pode ajustar os resultados para garantir que eles atendam aos seus requisitos exatos. Revise o alinhamento da marca, ajuste o tom e o idioma e prepare o conteúdo para ativação.

1. Após a geração, navegue pelas **[!UICONTROL Variações]**.

1. Clique no ícone de porcentagem para exibir sua **[!UICONTROL Pontuação de alinhamento da marca]** e identificar quaisquer desalinhamentos com sua marca.

   Saiba mais sobre [Pontuação de alinhamento da marca](brands-score.md).

   ![Refinar menu](assets/sms-genai-4.png){zoomable="yes"}

1. Clique em **[!UICONTROL Visualizar]** para exibir uma versão em tela inteira da variação selecionada ou clique em **[!UICONTROL Aplicar]** para substituir o conteúdo atual.

1. Navegue até a opção **[!UICONTROL Refinar]** na janela **[!UICONTROL Visualizar]** para acessar recursos de personalização adicionais:

   * **[!UICONTROL Usar como conteúdo de referência]**: a variante escolhida servirá como conteúdo de referência para gerar outros resultados.

   * **[!UICONTROL Refrase]**: reescreva a mensagem preservando seu significado. Essa opção ajuda a gerar texto alternativo, melhorar o fluxo ou ajustar o estilo sem alterar a mensagem principal.

   * **[!UICONTROL Usar linguagem mais simples]**: use o AI Assistant para simplificar sua linguagem, garantindo clareza e acessibilidade para um público-alvo maior.

   * **[!UICONTROL Traduzir]**: simplifique seu idioma para garantir clareza e acessibilidade para um público-alvo maior.

   * **[!UICONTROL Alterar tom]**: ajuste o tom da mensagem para corresponder melhor ao seu estilo de comunicação, ou seja, tornando-a mais amigável, profissional, urgente ou inspiradora.

   * **[!UICONTROL Alterar estratégia de comunicação]**: modifique a abordagem de mensagens com base em seus objetivos, como criar urgência ou enfatizar o apelo interessante.

     ![Variações de texto geradas com a Pontuação de alinhamento da marca](assets/sms-genai-5.png){zoomable="yes"}

1. Abra a guia **[!UICONTROL Alinhamento da marca]** para ver como o seu conteúdo se alinha às suas [diretrizes da marca](brands.md).

1. Clique em **[!UICONTROL Selecionar]** depois de encontrar o conteúdo apropriado.

1. Insira campos de personalização para personalizar seu conteúdo com base nos dados de perfis. Em seguida, clique no botão **[!UICONTROL Simular conteúdo]** para controlar a renderização e verificar as configurações de personalização com perfis de teste. [Saiba mais](../personalization/personalize.md)

1. Revise e ative o conteúdo:
   * **Notificação por push**: quando tiver definido seu conteúdo, público-alvo e agendamento, você estará pronto para preparar sua entrega de notificação por push. [Saiba mais](../push/send-push.md)
   * **SMS**: quando o SMS estiver pronto, você poderá publicá-lo para disponibilizá-lo para uso em uma mensagem. [Saiba mais](../sms/send-sms.md)
