---
audience: end-user
title: Conteúdo gerativo
description: Saiba como gerar imagens com o Assistente de IA
source-git-commit: 2066f29b0867f82f2130361c8ccdb15889085886
workflow-type: tm+mt
source-wordcount: '1098'
ht-degree: 2%

---

# Gerar imagens com o Assistente de IA {#generative-image}

>[!IMPORTANT]
>
>Antes de começar a usar este recurso, leia as [Medidas de Proteção e Limitações](generative-gs.md#generative-guardrails) relacionadas.
></br>
>
>Você deve concordar com um [contrato de usuário](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"} antes de usar o Assistente de IA no Adobe Campaign Web. Para mais informações, entre em contato com o seu representante da Adobe.

Use o Assistente de IA no Adobe Campaign Web para criar conteúdo visual atraente que aprimore suas mensagens de email, páginas de aterrissagem e notificações por push. O Assistente de IA ajuda você a gerar e otimizar imagens, garantindo que seu conteúdo seja visualmente envolvente e alinhado com sua marca.

## Para emails e landing pages {#email-web-channels}

O AI Assistant pode gerar experiências visuais completas para seus deliveries de email e landing pages. Esse recurso permite produzir imagens atraentes na marca que repercutem com seu público em pontos de contato digitais.

### Acessar e configurar {#access-configure}

Para começar a gerar imagens com o Assistente de IA, primeiro configure seu delivery e abra o editor de conteúdo. Siga as etapas abaixo para preparar seu espaço de trabalho e acessar o painel Assistente de IA.

1. Criar e configurar o delivery:

   * **Email**: depois de criar e configurar sua entrega de email, clique em **[!UICONTROL Editar conteúdo]**. [Saiba mais](../email/create-email-content.md)
   * **Página de aterrissagem**: depois de criar e configurar sua página de aterrissagem, clique em **[!UICONTROL Editar conteúdo]**. [Saiba mais](../landing-pages/create-lp.md)

1. Selecione o ativo que você deseja alterar com o Assistente de IA e acesse o menu **[!UICONTROL Assistente de IA]**.

   ![Captura de tela mostrando a seleção do componente de texto na Adobe Campaign Web](assets/image-genai-1.png){zoomable="yes"}

### Gerar conteúdo {#generate-content}

1. Habilite a opção **[!UICONTROL Estilo de referência]** para que o Assistente de IA personalize o novo conteúdo com base no conteúdo selecionado.

1. Selecione sua **[!UICONTROL Marca]** para garantir que o conteúdo gerado por IA esteja alinhado às especificações da sua marca. [Saiba mais](brands.md) sobre marcas.

1. Ajuste o conteúdo descrevendo o que você deseja gerar no campo **[!UICONTROL Prompt]**.

   Se precisar de ajuda para criar seu prompt, acesse a **[!UICONTROL Biblioteca de Prompts]**, que fornece diversas ideias de prompt para melhorar suas entregas. [Saiba mais sobre as práticas recomendadas do prompt](ai-assistant-prompting-guide.md)

   ![Captura de tela mostrando a biblioteca de prompts para geração de imagens na Adobe Campaign Web](assets/image-genai-2.png){zoomable="yes"}

1. Personalize seu prompt usando a opção **[!UICONTROL Configurações de imagem]**:

   * **[!UICONTROL Taxa de proporção]**: determine a largura e a altura do ativo. Escolha entre taxas comuns, como 16:9, 4:3, 3:2 ou 1:1, ou insira um tamanho personalizado.
   * **[!UICONTROL Tipo de conteúdo]**: categorize a natureza do elemento visual, distinguindo entre diferentes formas de representação visual, como fotos, gráficos ou arte.
   * **[!UICONTROL Intensidade visual]**: controle o impacto da imagem ajustando sua intensidade. Uma configuração mais baixa (2) cria uma aparência mais suave, enquanto uma configuração mais alta (10) torna a imagem mais vibrante.
   * **[!UICONTROL Cor e tom]**: ajuste a aparência geral das cores e o humor ou atmosfera transmitidos.
   * **[!UICONTROL Iluminação]**: modifique a iluminação na imagem para moldar sua atmosfera e destacar elementos específicos.
   * **[!UICONTROL Composição]**: organizar elementos dentro do quadro da imagem.

     ![Captura de tela mostrando as opções de configuração de imagem na Adobe Campaign Web](assets/image-genai-4.png){zoomable="yes"}

1. No menu **[!UICONTROL Conteúdo de referência]**, clique em **[!UICONTROL Carregar arquivo]** para adicionar qualquer ativo de marca que contenha conteúdo que possa fornecer o Assistente de IA de contexto adicional ou selecione um que tenha sido carregado anteriormente.

   Os arquivos carregados anteriormente estão disponíveis no menu suspenso **[!UICONTROL Conteúdo de referência carregado]**. Basta alternar os ativos que deseja incluir na geração.

1. Quando estiver satisfeito com a configuração do prompt, clique em **[!UICONTROL Gerar]**.

### Refinar e finalizar {#refine-finalize}

Depois de gerar variações de imagem, você pode revisar os resultados, verificar o alinhamento da marca e selecionar a melhor opção para o seu conteúdo.

1. Navegue pelas **[!UICONTROL Variações]** geradas.

1. Clique no ícone de porcentagem para exibir sua **[!UICONTROL Pontuação de alinhamento da marca]** e identificar quaisquer desalinhamentos com sua marca.

   Saiba mais sobre [Pontuação de alinhamento da marca](../content/brands-score.md).

   ![](assets/image-genai-3.png){zoomable="yes"}

1. Clique em **[!UICONTROL Visualizar]** para exibir uma versão em tela inteira da variação selecionada ou em **[!UICONTROL Aplicar]** para substituir o conteúdo atual.

1. Escolha **[!UICONTROL Gerar Semelhante]** se desejar exibir imagens relacionadas a essa variante.

1. Abra a guia **[!UICONTROL Alinhamento da marca]** para ver como o seu conteúdo se alinha às suas [diretrizes da marca](../content/brands.md).

1. Clique em **[!UICONTROL Selecionar]** depois de encontrar o conteúdo apropriado.

1. Após definir o conteúdo da mensagem, clique no botão **[!UICONTROL Simular conteúdo]** para controlar a renderização e verificar as configurações de personalização com perfis de teste. [Saiba mais](../preview-test/preview-content.md)

1. Revise e ative o conteúdo:
   * **Email**: quando tiver definido seu conteúdo, público-alvo e agendamento, você estará pronto para preparar sua entrega de email. [Saiba mais](../monitor/prepare-send.md)
   * **Página de aterrissagem**: quando a página de aterrissagem estiver pronta, você poderá publicá-la para disponibilizá-la para uso em uma mensagem. [Saiba mais](../landing-pages/create-lp.md)

## Para canais móveis {#mobile-channels}

O Assistente de IA permite gerar imagens envolventes para notificações por push, ajudando você a criar comunicações móveis visualmente atraentes que captam atenção e repercutem no seu público-alvo.

### Acessar e configurar {#mobile-access-configure}

Para começar a gerar imagens para notificações por push com o AI Assistant, primeiro configure seu delivery e abra o AI Assistant.

1. Depois de criar e configurar a entrega de notificação por push, clique em **[!UICONTROL Editar conteúdo]**. [Saiba mais](../push/create-push.md)

1. Acesse o menu **[!UICONTROL Mostrar assistente de IA]**.

   ![Captura de tela mostrando o menu Mostrar Assistente de IA](assets/push-img-1.png){zoomable="yes"}

### Gerar conteúdo {#mobile-generate-content}

Depois de acessar o Assistente de IA, você pode ajustar as configurações de geração para criar imagens que se alinhem à sua marca e sejam compatíveis com seus objetivos.

1. Selecione sua **[!UICONTROL Marca]** para garantir que o conteúdo gerado por IA esteja alinhado às especificações da sua marca. [Saiba mais](brands.md) sobre marcas.

1. Ajuste o conteúdo descrevendo o que você deseja gerar no campo **[!UICONTROL Prompt]**.

   Se você estiver procurando ajuda para criar seu prompt, acesse a **[!UICONTROL Biblioteca de Prompts]**, que fornece diversas ideias de prompt para melhorar suas campanhas. [Saiba mais sobre as práticas recomendadas do prompt](ai-assistant-prompting-guide.md)

   ![Assistente de IA com campo de prompt e opções](assets/push-img-2.png){zoomable="yes"}

1. Selecione **[!UICONTROL Imagem]** para gerar apenas ativos.

1. Escolha suas **[!UICONTROL configurações de imagem]**:

   * **[!UICONTROL Tipo de conteúdo]**: categorize a natureza do elemento visual, distinguindo entre diferentes formas de representação visual, como fotos, gráficos ou arte.
   * **[!UICONTROL Intensidade visual]**: controle o impacto da imagem ajustando sua intensidade. Uma configuração mais baixa (2) cria uma aparência mais suave e mais restrita, enquanto uma configuração mais alta (10) torna a imagem mais vibrante e visualmente poderosa.
   * **[!UICONTROL Iluminação]**: Ajuste a iluminação na imagem para moldar sua atmosfera e destacar elementos específicos.
   * **[!UICONTROL Composição]**: organizar elementos dentro do quadro da imagem.

     ![Captura de tela mostrando as opções de configuração de imagem](assets/push-img-3.png){zoomable="yes"}

1. No menu **[!UICONTROL Conteúdo de referência]**, clique em **[!UICONTROL Carregar arquivo]** para adicionar qualquer ativo de marca que contenha conteúdo que possa fornecer o Assistente de IA de contexto adicional ou selecione um que tenha sido carregado anteriormente.

   Os arquivos carregados anteriormente estão disponíveis no menu suspenso **[!UICONTROL Conteúdo de referência carregado]**. Basta alternar os ativos que deseja incluir na geração.

1. Quando o prompt estiver pronto, clique em **[!UICONTROL Gerar]**.

### Refinar e finalizar {#mobile-refine-finalize}

Depois de gerar variações de imagem para suas mensagens móveis, você pode ajustar os resultados para garantir que eles atendam aos seus requisitos exatos.

1. Após a geração, navegue pelas **[!UICONTROL Variações]**.

1. Clique no ícone de porcentagem para exibir sua **[!UICONTROL Pontuação de alinhamento da marca]** e identificar quaisquer desalinhamentos com sua marca.

   Saiba mais sobre [Pontuação de alinhamento da marca](../content/brands-score.md).

   ![](assets/push-img-4.png){zoomable="yes"}

1. Clique em **[!UICONTROL Visualizar]** para navegar pelas **[!UICONTROL Variações]**.

1. Abra a guia **[!UICONTROL Alinhamento da marca]** para ver como o seu conteúdo se alinha às suas [diretrizes da marca](brands.md).

1. Clique em **[!UICONTROL Selecionar]** depois de encontrar o conteúdo apropriado.

Depois de definir o conteúdo, o público-alvo e o cronograma, prepare a entrega por push. [Saiba mais](../monitor/prepare-send.md)
