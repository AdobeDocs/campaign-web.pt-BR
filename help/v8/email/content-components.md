---
audience: end-user
title: Usar componentes de conteúdo do Designer de email
description: Saiba como usar componentes de conteúdo em seus emails
exl-id: a77e7438-4bd3-4f99-a166-b98094a1292b
badge: label="Disponibilidade limitada"
source-git-commit: 3903513d43b699416973b26755dfc4f0337dc757
workflow-type: tm+mt
source-wordcount: '1167'
ht-degree: 67%

---

# Usar componentes de conteúdo {#content-components}

>[!CONTEXTUALHELP]
>id="ac_content_components_email"
>title="Sobre conteúdos"
>abstract="Componentes de conteúdo são espaços reservados de conteúdo vazios que podem ser usados para criar o layout de um email."

>[!CONTEXTUALHELP]
>id="ac_content_components_landing_page"
>title="Sobre conteúdos"
>abstract="Componentes de conteúdo são espaços reservados de conteúdo vazios que você pode usar para criar o layout de uma landing page."

>[!CONTEXTUALHELP]
>id="ac_content_components_fragment"
>title="Sobre conteúdos"
>abstract="Os componentes de conteúdo são espaços reservados de conteúdo vazios que podem ser usados para criar o layout de um fragmento."

>[!CONTEXTUALHELP]
>id="ac_content_components_template"
>title="Sobre conteúdos"
>abstract="Componentes de conteúdo são espaços reservados de conteúdo vazios que podem ser usados para criar o layout de um modelo."

Ao criar seu conteúdo de email, **[!UICONTROL Conteúdo]** O recurso componentes permite personalizar ainda mais o email com componentes brutos e vazios que podem ser usados depois de colocados no email.

Você pode adicionar quantos **[!UICONTROL Conteúdo]** conforme necessário em um **[!UICONTROL Estrutura]**, que define o layout do email.

## Adicionar componentes de conteúdo {#add-content-components}

Para adicionar componentes de conteúdo ao seu email e ajustá-los às suas necessidades, siga as etapas abaixo.

1. No Designer de email, use uma [conteúdo existente](existing-content.md) ou arraste e solte uma **[!UICONTROL Estrutura]** no conteúdo vazio para definir o layout do email. [Saiba como](create-email-content.md)

1. Arraste e solte a **[!UICONTROL Conteúdo]** de sua escolha dentro das estruturas relevantes.

   ![](assets/email_designer_add_content_components.png)

   >[!NOTE]
   >
   >É possível adicionar vários componentes em uma única estrutura e em cada coluna de uma estrutura.

1. Ajuste as opções de cada componente usando a variável de contexto **[!UICONTROL Configurações]** guia. Por exemplo, você pode optar por exibi-lo somente em dispositivos móveis ou de desktop, ou ambos. Você também pode gerenciar opções de link nesta guia. [Saiba mais sobre como gerenciar links](message-tracking.md)

1. Ajuste os atributos de estilo de cada componente usando o **[!UICONTROL Estilo]** guia. Por exemplo, é possível alterar o estilo do texto, o preenchimento ou a margem de cada componente. [Saiba mais sobre alinhamento e preenchimento](alignment-and-padding.md)

   ![](assets/email_designer_content_components_settings.png)

1. No menu avançado do **[!UICONTROL Conteúdo]** no painel direito, é possível excluir ou duplicar facilmente qualquer componente do conteúdo, conforme necessário.

## Container {#container}

É possível adicionar um container simples dentro do qual você adiciona outro componente de conteúdo. Isso permite aplicar um estilo específico ao container, que é diferente do componente usado internamente.

Por exemplo, adicione um componente **[!UICONTROL Container]** e, em seguida, adicione um componente [Botão](#button) dentro desse container. Você pode usar um plano de fundo específico para o container e outro para o botão.

![](assets/email_designer_container_component.png)

## Botão {#buttons}

Use o componente **[!UICONTROL Botão]** para inserir um ou vários botões no email e redirecionar o público-alvo do email para outra página.

1. A partir da lista **[!UICONTROL Conteúdos]**, arraste e solte o componente **[!UICONTROL Botão]** em um componente **[!UICONTROL Estrutura]**.

   ![](assets/email_designer_13.png)

1. Clique no botão recém-adicionado para personalizar o texto e ter acesso às guias **[!UICONTROL Configurações]** e **[!UICONTROL Estilos]**.

   ![](assets/email_designer_14.png)

1. Na guia **[!UICONTROL Configurações]**, no campo **[!UICONTROL URL]**, adicione o URL para o qual deseja redirecionar ao clicar no botão.

1. Escolha como o conteúdo será exibido com a lista suspensa do **[!UICONTROL Público-alvo]**:

   * **[!UICONTROL Nenhum]**: abre o link no mesmo quadro em que foi clicado (padrão).
   * **[!UICONTROL Branco]**: abre o link em uma nova janela ou guia.
   * **[!UICONTROL Auto]**: abre o link no mesmo quadro em que foi clicado.
   * **[!UICONTROL Principal]**: abre o link no quadro principal.
   * **[!UICONTROL Superior]**: abre o link no corpo completo da janela.

   ![](assets/email_designer_15.png)

1. Você pode personalizar ainda mais seu botão alterando atributos de estilo como **[!UICONTROL Borda]**, **[!UICONTROL Tamanho]**, **[!UICONTROL Margem]** etc., do **[!UICONTROL Estilos]** guia.

## Texto {#text}

Use o componente de **[!UICONTROL Texto]** para inserir texto no email e ajustar o estilo (borda, tamanho, preenchimento etc.) usando as guias **[!UICONTROL Configurações]** e **[!UICONTROL Estilos]**.

1. No **[!UICONTROL Conteúdo]** , arraste e solte **[!UICONTROL Texto]** em um **[!UICONTROL Estrutura]** componente.

   ![](assets/email_designer_11.png)

1. Clique no componente recém-adicionado para personalizar o texto e ter acesso às guias **[!UICONTROL Configurações]** e **[!UICONTROL Estilos]**.

1. Altere o texto com as seguintes opções disponíveis na barra de ferramentas contextual:

   ![](assets/email_designer_27.png)

   * **[!UICONTROL Alterar estilo do texto]**: aplique negrito, itálico, sublinhado ou riscado ao seu texto.
   * **Alterar alinhamento**: escolha entre alinhamento esquerdo, direito, central ou justificado para o texto.
   * **[!UICONTROL Criar lista]**: adicione marcadores ou listas de números ao texto.
   * **[!UICONTROL Definir cabeçalho]**: adicione até seis níveis de cabeçalho ao texto.
   * **Tamanho da fonte**: selecione o tamanho da fonte do texto em pixels.
   * **[!UICONTROL Editar imagem]**: adicione uma imagem ou um ativo ao seu componente de texto.
   * **[!UICONTROL Mostrar o código-fonte]**: exibir o código-fonte do texto. Ele não pode ser modificado.
   * **[!UICONTROL Duplicar]**: adicione uma cópia do seu componente de texto.
   * **[!UICONTROL Excluir]**: exclua o componente de texto selecionado do seu email.
   * **[!UICONTROL Adicionar personalização]**: adicione campos de personalização para personalizar o conteúdo dos dados de seus perfis.
   * **[!UICONTROL Habilitar conteúdo condicional]**: adicione conteúdo condicional para adaptar o conteúdo do componente aos perfis segmentados.

1. Ajuste os outros atributos de estilo, como cor do texto, família da fonte, borda, preenchimento, margem etc., do **[!UICONTROL Estilos]** guia.

   ![](assets/email_designer_12.png)

## Divisor {#divider}

Use o componente **[!UICONTROL Divisor]** para inserir uma linha divisória para organizar o layout e o conteúdo do email.

É possível ajustar atributos de estilo, como cor, estilo e altura da linha no **[!UICONTROL Estilos]** guia.

![](assets/email_designer_16.png)

## HTML {#HTML}

Use o componente **[!UICONTROL HTML]** para copiar e colar as diferentes partes do HTML existente. Isso permite que você crie componentes de HTML modulares gratuitos para reutilizar algum conteúdo externo.

1. De **[!UICONTROL Componentes]**, arraste e solte o componente **[!UICONTROL HTML]** em um Componente **[!UICONTROL Estrutura]**.

   ![](assets/email_designer_22.png)

1. Clique no componente recém-adicionado e selecione **[!UICONTROL Mostrar o código-fonte]** na barra de ferramentas contextual para adicionar o HTML.

   ![](assets/email_designer_23.png)

>[!NOTE]
>
>Para simplesmente tornar um conteúdo externo compatível com o Designer de email, o Adobe recomenda [criação de uma mensagem do zero](create-email-content.md) e copie o conteúdo do email existente para os componentes.

## Imagem {#image}

Use o componente **[!UICONTROL Imagem]** para inserir um arquivo de imagem de seu computador no email.

1. A partir do menu **[!UICONTROL Conteúdo]**, arraste e solte uma **[!UICONTROL Imagem]** em um componente **[!UICONTROL Estrutura]**.

   ![](assets/email_designer_9.png)

1. Clique em **[!UICONTROL Procurar]** para escolher um arquivo de imagem de seus ativos. Você também pode optar por **[!UICONTROL Importar sua mídia]**.

   Para saber mais sobre como fazer upload e adicionar ativos no Adobe Experience Manager, consulte [Documentação do Adobe Experience Manager as a Cloud Service](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/manage/add-assets.html).

   ![](assets/email_designer_28.png)

1. Navegue pelas pastas para localizar o ativo específico necessário ou use a barra de pesquisa para localizá-lo com eficiência.

   Depois de encontrar o ativo que está procurando, clique em **[!UICONTROL Selecionar]**.

   ![](assets/email_designer_29.png)

1. Clique no componente recém-adicionado e configure as propriedades da imagem usando o **[!UICONTROL Configurações]** guia:

   * **[!UICONTROL Título da imagem]** permite definir um título para a imagem.
   * **[!UICONTROL Texto alternativo]** permite definir a legenda vinculada à imagem. Isso corresponde ao atributo HTML alternativo.

   ![](assets/email_designer_10.png)

1. É possível adicionar um link para redirecionar o público-alvo para outro conteúdo. [Saiba mais](message-tracking.md)

1. Ajuste os outros atributos de estilo, como margem, borda etc., usando o **[!UICONTROL Estilos]** guia.

## Social {#social}

Use o componente **[!UICONTROL Social]** para inserir links às páginas de redes sociais no seu conteúdo de email.

1. A partir do menu **[!UICONTROL Componentes]**, arraste e solte o componente **[!UICONTROL Social]** em um componente **[!UICONTROL Estrutura]**.

1. Clique no componente recém-adicionado.

1. No campo **[!UICONTROL Social]** da guia **[!UICONTROL Configurações]**, escolha qual rede social deseja adicionar ou remover.

   ![](assets/email_designer_20.png)

1. Escolha o tamanho dos ícones no campo **[!UICONTROL Tamanho das imagens]**.

1. Clique em cada um dos ícones de redes sociais para configurar o **[!UICONTROL URL]** para o qual o público-alvo é redirecionado.

   ![](assets/email_designer_21.png)

1. Você também pode alterar os ícones de cada uma das mídias sociais, se necessário, no **[!UICONTROL Origem]** campo.

1. Ajuste os outros atributos de estilo, como estilo, margem, borda etc., do **[!UICONTROL Estilos]** guia.
