---
audience: end-user
title: Desenvolva seu próprio conteúdo de email
description: Saiba como desenvolver seu próprio conteúdo de email
exl-id: a387bff6-3dc8-421c-9efd-043c16694ef0
TQID: 'https://experienceleague.adobe.com/PPrenfLb4utuqvAsrSitbtZzDHcCehzrOMK4R7L2EMw'
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: 7bbc2d4c383886788afc1ef83cdd27e7ec4b24ae
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 12%
---
# Desenvolva seu próprio conteúdo de email {#code-content}

Use o modo **[!UICONTROL Codifique você mesmo]** para importar HTML bruto e codificar seu conteúdo de email.

>[!CAUTION]
>
>Este método requer conhecimento do HTML.

>[!IMPORTANT]
>
>Não use a marca HTML `<base>` no seu conteúdo de email. Por motivos de segurança, essa tag não é compatível e pode impedir que o conteúdo seja carregado no editor de conteúdo. Em vez disso, use URLs absolutos para seus links e recursos externos.

1. Na página inicial do [Designer de email](get-started-email-designer.md), selecione **[!UICONTROL Codifique o seu próprio]**.

   ![Captura de tela mostrando a opção &quot;Codifique você mesmo&quot; na página inicial do Designer de email](assets/code-your-own.png){zoomable="yes"}

1. Insira ou cole seu código HTML bruto na tela principal.

1. Use o painel esquerdo para acessar os recursos de personalização. [Saiba mais](../personalization/gs-personalization.md)

   ![Captura de tela mostrando o editor de código com opções de personalização no painel esquerdo](assets/code-editor-personalization.png){zoomable="yes"}

1. Clique no botão **[!UICONTROL Simular conteúdo]** para visualizar o design da mensagem e a personalização usando perfis de teste. [Saiba mais](../preview-test/preview-test.md)

1. Quando o código estiver concluído, clique em **[!UICONTROL Salvar e fechar]** para retornar à tela de criação da mensagem e finalizar a mensagem.