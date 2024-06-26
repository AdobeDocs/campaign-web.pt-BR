---
title: Definir conteúdo específico da página de destino
description: Saiba como criar conteúdo específico de landing page no Campaign Web
feature: Landing Pages
exl-id: 6ca3c8c1-3633-4e3f-a9a1-f46ae27c5c8a
source-git-commit: 4dee53676949282b7c0e7664405b7d5a35ef64d2
workflow-type: tm+mt
source-wordcount: '1153'
ht-degree: 13%

---

# Definir conteúdo específico da página de destino {#lp-content}

>[!CONTEXTUALHELP]
>id="ac_lp_components"
>title="Usar componentes de conteúdo"
>abstract="Os componentes de conteúdo são espaços reservados de conteúdo vazios que você pode usar para criar o layout de uma página de destino. Para definir um conteúdo específico que permitirá aos usuários selecionar e enviar suas opções, use o componente de formulário."

>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="Definir as configurações da página principal"
>abstract="A página principal é exibida imediatamente depois que os usuários clicam no link da landing page que consta em um email ou site."

É possível editar o conteúdo de qualquer página da sua landing page.

A primeira página, que é imediatamente exibida aos usuários depois que eles clicam no link para a página de aterrissagem, já está pré-preenchida com o [componente de formulário específico da página de destino](#use-form-component) para o modelo selecionado<!-- to enable users to select and submit their choices-->.

O conteúdo do **[!UICONTROL Confirmação]**, **[!UICONTROL Erro]** e **[!UICONTROL Expiração]** também é pré-preenchido. Edite-as conforme necessário.

Você também pode definir [estilos para sua página de aterrissagem](#lp-form-styles).

Para projetar ainda mais o conteúdo da landing page:

* Você pode usar os mesmos componentes que os usados para criar um email. [Saiba mais](../email/content-components.md#add-content-components)

* Você pode adicionar conteúdo condicional às suas landing pages, da mesma forma que faria para um email. [Saiba mais](../personalization/conditions.md#condition-condition-builder)

  >[!AVAILABILITY]
  >
  >Esse recurso está na disponibilidade limitada (DL). É restrito aos clientes que estão migrando **do Adobe Campaign Standard para o Adobe Campaign v8** e não podem ser implantados em nenhum outro ambiente.

## Usar o componente de formulário {#use-form-component}

>[!CONTEXTUALHELP]
>id="ac_lp_formfield"
>title="Definir os campos do componente de formulário"
>abstract="Defina como os recipients verão a página de destino e enviarão suas opções."

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="O que acontece ao clicar no botão"
>abstract="Defina o que acontecerá depois que as pessoas enviarem o formulário da página de destino."

Para definir um conteúdo específico que permita aos usuários selecionar e enviar suas opções a partir da página de aterrissagem, edite o **[!UICONTROL Formulário]** componente. Para fazer isso, siga as etapas abaixo.

1. A página de aterrissagem específica **[!UICONTROL Formulário]** já é exibido na tela para o modelo selecionado.

   >[!NOTE]
   >
   >A variável **[!UICONTROL Formulário]** O componente só pode ser usado uma vez na mesma página.

1. Selecione-o. A variável **[!UICONTROL Conteúdo do formulário]** é exibida na paleta direita para permitir a edição dos diferentes campos do formulário.

   ![](assets/lp-form-component.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Alterne para a **[!UICONTROL Estilos]** a qualquer momento para editar os estilos do conteúdo do componente de formulário. [Saiba mais](#lp-form-styles)

1. Expanda o primeiro campo de texto, se houver, ou adicione um usando o **[!UICONTROL Adicionar]** botão. No **[!UICONTROL Campo de texto 1]** você pode editar o tipo de campo, o campo do banco de dados a ser atualizado, o rótulo e o texto que será exibido dentro do campo antes que os usuários insiram um valor.

   ![](assets/lp-form-text-field.png){zoomable=&quot;yes&quot;}

1. Verifique a **[!UICONTROL Tornar campo de formulário obrigatório]** opção, se necessário. Nesse caso, a landing page só poderá ser enviada se o usuário tiver preenchido esse campo.

   >[!NOTE]
   >
   >Se um campo obrigatório não estiver preenchido, uma mensagem de erro será exibida quando o usuário enviar a página.

1. Expanda a caixa de seleção, se houver, ou adicione uma usando o **[!UICONTROL Adicionar]** botão. Selecione se essa caixa de seleção deve atualizar um serviço ou um campo do banco de dados.

   ![](assets/lp-form-checkbox.png){zoomable=&quot;yes&quot;}

   Se você selecionar **[!UICONTROL Assinatura e serviços]**, selecione um [serviço](../audience/manage-services.md) na lista e escolha entre as duas opções abaixo:

   * **[!UICONTROL Inscrever-se se marcado]**: os usuários precisam marcar a caixa para consentir (aceitar).
   * **[!UICONTROL Cancelar inscrição se marcado]**: os usuários precisam marcar a caixa para remover seu consentimento (recusa).

   Se você selecionar **[!UICONTROL Campo]**, selecione um campo na lista de atributos e escolha entre as duas opções abaixo:

   * **[!UICONTROL Sim, se marcado]**.<!--TBC-->

   * **[!UICONTROL Não se estiver marcado]**.<!--TBC-->

1. É possível excluir e adicionar quantos campos (como campos de texto, botões de opção, caixas de seleção, lista suspensa etc.) conforme necessário.

1. Após adicionar ou atualizar todos os campos, clique em **[!UICONTROL Chamada para ação]** para expandir a seção correspondente. Ela permite definir o comportamento do botão na variável **[!UICONTROL Formulário]** componente. [Saiba como](#define-actions-on-form-submission)

   ![](assets/lp-call-to-action.png){zoomable=&quot;yes&quot;}

1. Salve o conteúdo para voltar para o [propriedades da landing page](create-lp.md#create-landing-page).

### Definir ações no envio de formulário {#define-actions-on-form-submission}

1. Defina o que acontecerá ao clicar no botão:

   * **[!UICONTROL Página de confirmação]**: por padrão, o usuário será redirecionado para o **[!UICONTROL Confirmação]** página definida para a página inicial atual.

   * **[!UICONTROL URL de redirecionamento]**: digite o URL da página para a qual os usuários serão redirecionados.

   * **[!UICONTROL Landing page]**: é possível selecionar outra página de aterrissagem para a qual os usuários serão redirecionados. Configure a landing page selecionada de acordo.

1. Se quiser fazer atualizações adicionais ao enviar o formulário, selecione **[!UICONTROL Atualizações adicionais]** e selecione o item que deseja atualizar:
   * Uma assinatura [serviço](../audience/manage-services.md) - nesse caso, defina se deseja aceitar ou recusar os usuários ao enviar o formulário. Ao criar um email, se você definir uma variável **[!UICONTROL Landing page]** para essa página de aterrissagem, o serviço selecionado será usado automaticamente. [Saiba mais sobre inserção de links](../email/message-tracking.md)

     >[!NOTE]
     >
     >Se quiser usar vários serviços com essa landing page, use o **[!UICONTROL Serviço do URL]** descrita abaixo.

   * O canal - o email endereçado usado ao preencher o formulário.
   * Todos os canais - ao enviar o formulário, os usuários entrarão ou não (dependendo do modelo selecionado) em/de todas as comunicações da sua marca em todos os canais.
   * Um campo do banco de dados - selecione um campo na lista de atributos e defina se ele deve ser definido como Verdadeiro ou Falso ao enviar o formulário.

   ![](assets/lp-form-additionnal-updates.png){zoomable=&quot;yes&quot;}

1. Selecione o **[!UICONTROL Serviço do URL]** opção para permitir que a landing page seja usada para vários serviços, tornando-a dinâmica. Defina se deseja aceitar ou recusar os usuários ao enviar o formulário.

   >[!AVAILABILITY]
   >
   >Esse recurso está na disponibilidade limitada (DL). É restrito aos clientes que estão migrando **do Adobe Campaign Standard para o Adobe Campaign v8** e não podem ser implantados em nenhum outro ambiente.

   ![](assets/lp-form-service-from-url.png){zoomable=&quot;yes&quot;}

   Ao criar um email, se você definir uma variável **[!UICONTROL Landing page]** para essa landing page, você poderá selecionar qualquer serviço na lista. É possível selecionar outros serviços ao definir outros links para essa landing page. [Saiba mais sobre inserção de links](../email/message-tracking.md)

   ![](assets/email-link-to-landing-page.png){zoomable=&quot;yes&quot;}

## Definir estilos de formulário de página de destino {#lp-form-styles}

1. Para modificar os estilos do conteúdo do componente de formulário, alterne a qualquer momento para o **[!UICONTROL Estilos]** guia.

1. A variável **[!UICONTROL Campo de texto]** é expandida por padrão. Ela permite editar a aparência dos campos de texto, como a fonte do rótulo, a posição do rótulo, a cor de fundo do campo ou a borda do campo.

   ![](assets/lp-text-styles.png){zoomable=&quot;yes&quot;}

1. Expanda a **[!UICONTROL Caixa de seleção]** para definir a aparência das caixas de seleção e o texto correspondente. Por exemplo, é possível ajustar a família e o tamanho da fonte ou a cor da borda da caixa de seleção.

   ![](assets/lp-checkbox-style.png){zoomable=&quot;yes&quot;}

1. Expanda e edite qualquer outra seção correspondente a outros campos que você possa ter adicionado (botão de opção, lista suspensa, data e hora etc.) ao seu formulário.

1. Expanda a **[!UICONTROL Chamada para ação]** para modificar a aparência do botão no formulário do componente. Por exemplo, você pode alterar a fonte, adicionar uma borda, editar a cor do rótulo ao passar o mouse ou ajustar o alinhamento do botão.

   ![](assets/lp-call-to-action-style.png){zoomable=&quot;yes&quot;}

   Você pode visualizar algumas de suas configurações, como a cor do rótulo do botão ao passar o mouse, usando o **[!UICONTROL Simular conteúdo]** botão. [Saiba mais](create-lp.md#test-landing-page)

1. Salve as alterações.
