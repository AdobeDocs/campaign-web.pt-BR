---
title: Criar um perfil
description: Saiba como criar um perfil no Campaign Web.
exl-id: 0680b726-8f2f-45bf-8aa0-c1d4aa1c2990
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 7%

---

# Criar um perfil {#profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_details"
>title="Detalhes básicos"
>abstract="Esta seção fornece informações sobre os detalhes básicos do perfil. Para modificar qualquer informação, faça alterações diretamente no respectivo campo e clique no botão **Salvar**, localizado no canto superior direito da tela."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="Informações de contato"
>abstract="Esta seção fornece informações de contato do perfil. Para modificar qualquer informação, faça alterações diretamente no respectivo campo e clique no botão **Salvar**, localizado no canto superior direito da tela."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title="Endereço"
>abstract="Esta seção fornece informações sobre o endereço postal do perfil e a qualidade do endereço. Para modificar qualquer informação, faça alterações diretamente no respectivo campo e clique no botão **Salvar**, localizado no canto superior direito da tela."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="Detalhes da conta"
>abstract="Esta seção fornece informações sobre os detalhes da conta do perfil. Para modificar qualquer informação, faça alterações diretamente no respectivo campo e clique no botão **Salvar**, localizado no canto superior direito da tela."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_nolongercontact"
>title="Não contatar mais"
>abstract="Esta seção fornece informações sobre as preferências de contato do perfil. Para modificar qualquer informação, faça alterações diretamente no respectivo campo e clique no botão **Salvar**, localizado no canto superior direito da tela."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="Campos personalizados"
>abstract="Os campos personalizados são atributos específicos adaptados às suas necessidades e configurados para sua instância. Para modificar qualquer informação, faça alterações diretamente no respectivo campo e clique no botão **Salvar**, localizado no canto superior direito da tela."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_othersfields"
>title="Outros"
>abstract="Esta seção fornece atributos integrados adicionais. Para modificar qualquer informação, faça alterações diretamente no respectivo campo e clique no botão **Salvar**, localizado no canto superior direito da tela."

Para criar um perfil, siga estas etapas:

1. Navegue até **[!UICONTROL Gerenciamento de clientes]** > **[!UICONTROL Perfis]** e clique no botão **[!UICONTROL Criar perfil]**, no canto superior direito da tela.

1. A lista de atributos disponíveis para o perfil é exibida, organizada em diferentes seções detalhadas na tabela abaixo.

   ![Captura de tela mostrando a lista de atributos disponíveis para o perfil, organizada em seções](assets/create-profile.png){zoomable="yes"}

   | seção Atributos | Descrição |
   |  ---  |  ---  |
   | **Detalhes básicos** | Informações básicas sobre o perfil, como nome ou data de nascimento.<br/>Por padrão, os perfis são armazenados na pasta **[!UICONTROL Recipients]**. Você pode alterá-la navegando até o local desejado. [Saiba como trabalhar com pastas](../get-started/permissions.md#folders) |
   | **Informações de contato** | As informações de contato do perfil, como endereço de email ou número de telefone. |
   | **Endereço** | O endereço postal do perfil. Esta seção também fornece uma avaliação da qualidade do endereço. O endereço de um perfil é considerado válido se os campos &quot;Sobrenome&quot;, &quot;Cidade&quot; e &quot;Código postal&quot; forem especificados. |
   | **Detalhes da conta** | Informações sobre a conta do perfil, como seu status ou número de conta. |
   | **Não contatar mais** | As preferências de contato do perfil. Quando qualquer uma dessas opções for selecionada, o perfil estará na inclui na lista de bloqueios.<br/>Por exemplo, se o recipient clicou em um link de cancelamento de assinatura em um boletim informativo, essas informações serão adicionadas aos dados de contato. Esse recipient não é mais direcionado para os canais selecionados. Saiba mais sobre o gerenciamento de quarentena na [documentação do Adobe Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html){target="_blank"} |
   | **Campos personalizados** | Se campos personalizados tiverem sido configurados, eles serão exibidos nesta seção. Campos personalizados são atributos adicionais adicionados ao esquema **[!UICONTROL Perfis]** por meio do console Adobe Campaign. Saiba mais na [documentação do Adobe Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html){target="_blank"} |
   | **Outros** | Atributos incorporados adicionais. |

1. Depois de configurar o perfil, clique em **[!UICONTROL Criar]** para salvá-lo no banco de dados.

   Depois de salvar, você pode editar o perfil a qualquer momento, abrindo-o na lista dos perfis. [Saiba como explorar os detalhes dos perfis](profile-view.md).