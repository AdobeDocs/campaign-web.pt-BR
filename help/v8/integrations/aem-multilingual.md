---
audience: end-user
title: Criar emails multilíngues com o Adobe Experience Manager
description: Saiba como criar entregas de email multilíngues usando cópias de idioma do Adobe Experience Manager no Campaign Web.
feature: Email
topic: Content Management
role: User
level: Intermediate
source-git-commit: f238fde4a79d3303f2b5c9a2d26b11ffad8ac54e
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 1%

---


# Criar emails multilíngues com o Adobe Experience Manager {#aem-multilingual}

A integração do Adobe Experience Manager permite criar deliveries de email multilíngues usando cópias de idioma do Adobe Experience Manager. Isso permite gerenciar variantes de conteúdo em diferentes idiomas e enviar emails personalizados com base nas preferências de idioma do recipient.

## Pré-requisitos {#prerequisites}

Antes de criar um delivery de email multilíngue, verifique se você tem:

* Acesso a uma instância do Adobe Experience Manager configurada para integração com a interface da Web do Adobe Campaign.
* Conteúdo do Adobe Experience Manager com cópias de idioma já criado e aprovado. Saiba mais sobre o Assistente de Cópia de Idioma na [documentação do Adobe Experience Manager](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/sites/administering/reusing-content/translation/wizard)
* Modelo de entrega de email configurado para receber conteúdo do Adobe Experience Manager. Consulte as etapas detalhadas na seção [Habilitar modo multilíngue](#enable-multilingual).

## Criar seu delivery multilíngue

Para criar um delivery de email multilíngue, primeiro é necessário habilitar a opção multilíngue nas configurações do delivery. O sistema detecta automaticamente as cópias de idioma disponíveis e permite que você escolha as que serão adicionadas.

### Ativar modo multilíngue {#enable-multilingual}

Crie um novo delivery e ative a opção multilíngue nas configurações avançadas.

1. No menu **[!UICONTROL Entregas]**, clique em **[!UICONTROL Criar entrega]**.

   ![](assets/lg-copy-1.png)

1. Selecione o modelo de **[!UICONTROL Entrega de email com conteúdo do AEM]** e clique em **[!UICONTROL Criar entrega]**.

   ![](assets/lg-copy-2.png)

1. Insira um rótulo para o delivery e configure seu público. [Saiba mais](../email/create-email.md)

1. Acesse as **[!UICONTROL Configurações]** da sua entrega e navegue até a seção **[!UICONTROL Avançadas]**.

1. Habilite a opção **[!UICONTROL Habilitar AEM multilíngue]**.

   ![](assets/lg-copy-3.png)

1. Verifique se:

   * **[!UICONTROL Modo de edição de conteúdo]** definido como **[!UICONTROL AEM]**.
   * A **[!UICONTROL Conta externa]** correta do Adobe Experience Manager está selecionada.

1. Clique em **[!UICONTROL Salvar e fechar]**.

### Criar variantes de conteúdo {#create-variants}

Selecione o conteúdo do Adobe Experience Manager e escolha quais variantes de idioma incluir no delivery.

1. Clique em **[!UICONTROL Editar conteúdo]**.

1. Selecione **[!UICONTROL Criar variante de conteúdo]**.

   ![](assets/lg-copy-4.png)

1. Selecione o conteúdo do Adobe Experience Manager na lista.

   ![](assets/lg-copy-5.png)

1. O sistema detecta todas as cópias de idioma associadas ao conteúdo selecionado (relacionamento pai-filho). Por exemplo, se o conteúdo do Adobe Experience Manager tiver variantes em francês, alemão e italiano, todas as variantes estarão disponíveis para seleção.

   Selecione as variantes de idioma que deseja incluir no delivery.

   ![](assets/lg-copy-6.png)

1. Clique em **[!UICONTROL Save]**.

1. Revise suas variantes de idioma no editor de conteúdo. Agora você pode [gerenciar cada variante individualmente](#manage-variants) ou prosseguir com [envio da entrega](../monitor/prepare-send.md).

   ![](assets/lg-copy-7.png)

## Gerenciar variantes de idioma {#manage-variants}

Depois de criar variantes de conteúdo, é possível gerenciá-las diretamente no delivery:

1. Para definir um idioma padrão, acesse o menu avançado da variante escolhida e selecione **[!UICONTROL Definir como padrão]**. O idioma padrão é usado quando a preferência de idioma de um perfil não está definida ou não corresponde a nenhuma variante disponível.

   Clique em **[!UICONTROL Excluir]** para remover qualquer variante da entrega.

   ![](assets/lg-copy-8.png)

1. No menu avançado Variantes de conteúdo, clique em **[!UICONTROL Gerenciar localidades]** para adicionar outras localidades à entrega.

   ![](assets/lg-copy-9.png)

1. Selecione cópias de idioma adicionais para incluir mais variantes e clique em **[!UICONTROL Salvar]**.

   ![](assets/lg-copy-11.png)

1. Se o conteúdo for atualizado no Adobe Experience Manager, clique em **[!UICONTROL Atualizar conteúdo do AEM]** para sincronizar todas as variantes com a versão mais recente.

   ![](assets/lg-copy-10.png)

1. Clique em **[!UICONTROL Desvincular conteúdo do AEM]** se quiser editar o conteúdo diretamente no Campaign ou romper o vínculo com o Adobe Experience Manager.

   >[!CAUTION]
   >
   >Depois da desvinculação, não é possível atualizar o conteúdo do Adobe Experience Manager ou criar novas variantes. O conteúdo se torna independente do Adobe Experience Manager.


