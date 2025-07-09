---
title: Definir conteúdo específico da página de destino
description: Saiba como criar conteúdo específico de landing page no Campaign Web
feature: Landing Pages
exl-id: 6ca3c8c1-3633-4e3f-a9a1-f46ae27c5c8a
source-git-commit: e82c19df7faecbb75521bca54e32b1ba84ea1f81
workflow-type: tm+mt
source-wordcount: '1161'
ht-degree: 11%

---

# Definir conteúdo específico da página de destino {#lp-content}

>[!CONTEXTUALHELP]
>id="ac_lp_components"
>title="Usar componentes de conteúdo"
>abstract="Os componentes de conteúdo são espaços reservados de conteúdo vazios que você pode usar para criar o layout de uma página de destino. Para definir conteúdo específico que permite aos usuários selecionar e enviar suas escolhas, use o componente de formulário."

>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="Definir as configurações da página principal"
>abstract="A página principal é exibida imediatamente após os usuários clicarem no link para a página de destino, como a partir de um email ou de um site."

É possível editar o conteúdo de qualquer página da sua landing page.

A primeira página, que é exibida imediatamente aos usuários depois que eles clicam no link para a sua página de aterrissagem, já está preenchida com o [componente de formulário específico da página de aterrissagem](#use-form-component) para o modelo selecionado<!-- to enable users to select and submit their choices-->.

O conteúdo das páginas **[!UICONTROL Confirmação]**, **[!UICONTROL Erro]** e **[!UICONTROL Expiração]** também é preenchido previamente. Edite-as conforme necessário.

Você também pode definir [estilos para sua página de aterrissagem](#lp-form-styles).

Para projetar ainda mais o conteúdo da landing page:

* Use os mesmos componentes que os usados para criar um email. [Saiba mais](../email/content-components.md#add-content-components)

* Adicione conteúdo condicional às landing pages da mesma forma que para um email. [Saiba mais](../personalization/conditions.md#condition-condition-builder)

## Usar o componente de formulário {#use-form-component}

>[!CONTEXTUALHELP]
>id="ac_lp_formfield"
>title="Definir os campos do componente de formulário"
>abstract="Defina como os recipients verão a página de destino e enviarão suas opções."

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="O que acontece ao clicar no botão"
>abstract="Defina o que acontecerá depois que as pessoas enviarem o formulário da página de destino."

Para definir um conteúdo específico que permita aos usuários selecionar e enviar suas opções a partir da página de aterrissagem, edite o componente **[!UICONTROL Formulário]**. Siga as etapas abaixo.

1. O componente de Formulário **[!UICONTROL Formulário]** específico da página de aterrissagem já é exibido na tela para o modelo selecionado.

   >[!NOTE]
   >
   >O componente **[!UICONTROL Formulário]** só pode ser usado uma vez na mesma página.

1. Selecione-o. A guia **[!UICONTROL Conteúdo do formulário]** é exibida na paleta direita para permitir que você edite os diferentes campos do formulário.

   ![Componente de formulário exibido na tela](assets/lp-form-component.png){zoomable="yes"}

   >[!NOTE]
   >
   >Alterne para a guia **[!UICONTROL Estilos]** a qualquer momento para editar os estilos do conteúdo do componente de formulário. [Saiba mais](#lp-form-styles)

1. Expanda o primeiro campo de texto, se houver, ou adicione um usando o botão **[!UICONTROL Adicionar]**. Na seção **[!UICONTROL Campo de texto 1]**, edite o tipo de campo, o campo de banco de dados a ser atualizado, o rótulo e o texto exibido dentro do campo antes que os usuários insiram um valor.

   ![Configurações do campo de texto no componente de formulário](assets/lp-form-text-field.png){zoomable="yes"}

1. Marque a opção **[!UICONTROL Tornar campo de formulário obrigatório]**, se necessário. Nesse caso, a landing page só poderá ser enviada se o usuário tiver preenchido esse campo.

   >[!NOTE]
   >
   >Se um campo obrigatório não estiver preenchido, uma mensagem de erro será exibida quando o usuário enviar a página.

1. Expanda a caixa de seleção, se houver, ou adicione uma usando o botão **[!UICONTROL Adicionar]**. Selecione se essa caixa de seleção deve atualizar um serviço ou um campo do banco de dados.

   ![Configurações da caixa de seleção no componente de formulário](assets/lp-form-checkbox.png){zoomable="yes"}

   Se você selecionar **[!UICONTROL Assinatura e serviços]**, selecione um [serviço](../audience/manage-services.md) na lista e escolha entre as duas opções abaixo:

   * **[!UICONTROL Inscrever-se, se marcado]**: os usuários precisam marcar a caixa para consentir (aceitar).
   * **[!UICONTROL Cancelar inscrição se marcado]**: os usuários precisam marcar a caixa para remover seu consentimento (recusar).

   Se você selecionar **[!UICONTROL Campo]**, selecione um campo na [lista de atributos](../get-started/attributes.md) e escolha entre as duas opções abaixo:

   * **[!UICONTROL Sim, se marcado]**.
   * **[!UICONTROL Não se marcado]**.

1. Exclua e adicione quantos campos (como campos de texto, botões de opção, caixas de seleção, listas suspensas etc.) forem necessários.

1. Depois que todos os campos forem adicionados ou atualizados, clique em **[!UICONTROL Call to action]** para expandir a seção correspondente. Ela permite definir o comportamento do botão no componente **[!UICONTROL Formulário]**. [Saiba como](#define-actions-on-form-submission)

   ![Configurações do Call to action no componente de formulário](assets/lp-call-to-action.png){zoomable="yes"}

1. Salve seu conteúdo para voltar para as [propriedades da página de aterrissagem](create-lp.md#create-landing-page).

### Definir ações no envio de formulário {#define-actions-on-form-submission}

1. Defina o que acontece ao clicar no botão:

   * **[!UICONTROL Página de confirmação]**: por padrão, o usuário é redirecionado para a página **[!UICONTROL Confirmação]** definida para a página de aterrissagem atual.

   * **[!UICONTROL URL de redirecionamento]**: digite a URL da página para a qual os usuários são redirecionados.

   * **[!UICONTROL Página de aterrissagem]**: selecione outra página de aterrissagem para a qual os usuários serão redirecionados. Configure a landing page selecionada de acordo.

1. Para fazer atualizações adicionais ao enviar o formulário, selecione **[!UICONTROL Atualizações adicionais]** e selecione o item que deseja atualizar:
   * Uma assinatura [serviço](../audience/manage-services.md) - defina se você deseja aceitar ou recusar os usuários ao enviar o formulário. Ao criar um email, se você definir um link do tipo **[!UICONTROL Página de aterrissagem]** para essa página de aterrissagem, o serviço selecionado será usado automaticamente. [Saiba mais sobre como inserir links](../email/message-tracking.md)

     >[!NOTE]
     >
     >Se quiser usar vários serviços com esta página de aterrissagem, use a opção **[!UICONTROL Serviço da URL]** descrita abaixo.

   * O canal - o endereço de email usado ao preencher o formulário.
   * Todos os canais - ao enviar o formulário, os usuários optam por entrar ou sair (dependendo do modelo selecionado) de/para todas as comunicações da sua marca em todos os canais.
   * Um campo do banco de dados - selecione um campo na lista de atributos e defina se ele deve ser definido como Verdadeiro ou Falso ao enviar o formulário.

   ![Configurações de atualizações adicionais no componente de formulário](assets/lp-form-additionnal-updates.png){zoomable="yes"}

1. Selecione a opção **[!UICONTROL Serviço da URL]** para permitir que a landing page seja usada para vários serviços, tornando-a dinâmica. Defina se deseja aceitar ou recusar os usuários ao enviar o formulário.

   ![Serviço das configurações de URL no componente de formulário](assets/lp-form-service-from-url.png){zoomable="yes"}

   Ao criar um email, se você definir um link do tipo **[!UICONTROL Página de aterrissagem]** para essa página de aterrissagem, será possível selecionar qualquer serviço na lista. É possível selecionar outros serviços ao definir outros links para essa landing page. [Saiba mais sobre como inserir links](../email/message-tracking.md)

   ![Link de email para configurações da página de aterrissagem](assets/email-link-to-landing-page.png){zoomable="yes"}

1. Envie uma mensagem no envio da landing page. [Saiba mais aqui](#lp-message)

### Enviar uma mensagem após o envio {#lp-message}

Para enviar uma mensagem de confirmação automaticamente após o envio de uma landing page, siga estas etapas:

1. Na seção **[!UICONTROL CHAMADA PARA AÇÃO]**, marque a opção **[!UICONTROL Enviar email de confirmação]**.

1. Na lista suspensa associada, escolha o template de mensagem transacional que precisa ser enviado.

![Configurações de email de confirmação no componente de formulário](assets/lp-confirmation.png){zoomable="yes"}

## Definir estilos de formulário de página de destino {#lp-form-styles}

1. Para modificar os estilos do conteúdo do componente de formulário, alterne a qualquer momento para a guia **[!UICONTROL Estilos]**.

1. A seção **[!UICONTROL Campo de texto]** é expandida por padrão. Ela permite editar a aparência dos campos de texto, como a fonte do rótulo, a posição do rótulo, a cor de fundo do campo ou a borda do campo.

   ![Configurações de estilo do campo de texto](assets/lp-text-styles.png){zoomable="yes"}

1. Expanda a seção **[!UICONTROL Caixa de seleção]** para definir a aparência das caixas de seleção e o texto correspondente. Por exemplo, ajuste a família e o tamanho da fonte ou a cor da borda da caixa de seleção.

   ![Configurações de estilo da caixa de seleção](assets/lp-checkbox-style.png){zoomable="yes"}

1. Expanda e edite qualquer outra seção correspondente a outros campos que você tenha adicionado (botão de opção, lista suspensa, data e hora, etc.) ao seu formulário.

1. Expanda a seção **[!UICONTROL Call to action]** para modificar a aparência do botão no formulário do componente. Por exemplo, alterar a fonte, adicionar uma borda, editar a cor do rótulo ao passar o mouse ou ajustar o alinhamento do botão.

   ![configurações de estilo do Call to action](assets/lp-call-to-action-style.png){zoomable="yes"}

   Visualize algumas de suas configurações, como a cor do rótulo do botão ao passar o mouse, usando o botão **[!UICONTROL Simular conteúdo]**. [Saiba mais](create-lp.md#test-landing-page)

1. Salve as alterações.