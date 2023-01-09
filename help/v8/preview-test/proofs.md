---
audience: end-user
title: Enviar provas
description: Documentação da Web do Campaign v8
exl-id: b2677579-c95d-443d-b207-466af364c208
source-git-commit: 9c9daba092b69cc7a5c8141cd6a04cd65069fdd2
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 2%

---

# Enviar provas {#send-proofs}

>[!NOTE]
>
>Esta documentação está em construção e é atualizada com frequência. A versão final desse conteúdo estará pronta em janeiro de 2023.

O envio de emails de teste permite validar seu email e verificar vários elementos, como links, links para opção de não participação e mirror pages, imagens e detectar possíveis erros.

Provas podem ser enviadas para dois tipos de recipients:

* **Testar perfis**: enviar provas para seed addresses, que são recipients adicionais e fictícios no banco de dados,
* **Perfis de substituição**: envie provas para um endereço de email específico usando um perfil existente. Isso permite que você se posicione como os perfis e obtenha uma representação exata da mensagem que o perfil receberá.

## Selecionar os recipients das provas {#recipients}

1. Acesse a tela de criação de conteúdo de email e clique em **[!UICONTROL Simular conteúdo]**.

1. Clique no botão **[!UICONTROL Teste]** em seguida, use o **[!UICONTROL Modo]** lista suspensa para escolher o tipo de recipients que receberá as provas:

<!-- to check: by default, profiles selected in previous screen are pre-selected for proofs. Can add addtitional profiles + remove preselected?-->

### Enviar provas para perfis de teste

1. Escolha a **[!UICONTROL Usar perfis de teste]** modo.

1. Adicione os perfis de teste que receberão os emails de teste.

   <!--FOR BETA: You can also build an audience to select test profiles based on your own criteria using the **[!UICONTROL Add test audience]** button.-->

   ![](assets/test-profiles-audience.png)

### Enviar provas para perfis de substituição

1. Escolha a **[!UICONTROL Substituição do target]** modo.

1. Adicione os endereços de email que receberão as provas.

   >[!NOTE]
   >
   >Você pode especificar qualquer endereço de email. Isso permite enviar provas para qualquer usuário, mesmo que ele não seja usuário do Adobe Campaign V8.

1. Para cada endereço de email, selecione o perfil no público-alvo a ser usado. Você também pode permitir que o Adobe Campaign selecione um perfil aleatório no target.

   ![](assets/substitution.png)

Depois que os recipients de prova forem selecionados, você poderá enviar o email de teste. [Saiba como enviar provas](#send)

>[!NOTE]
>
>Se desejar enviar a mensagem de email final para os recipients das provas, habilite a opção **[!UICONTROL Incluir população de teste no target principal]** ativada.

## Enviar as provas {#send}

Para enviar as provas para os destinatários selecionados, clique em **[!UICONTROL Enviar email de teste]** em seguida, confirme o envio.

![](assets/send-proof.png)

Envie quantas provas forem necessárias até concluir o conteúdo do seu delivery. Feito isso, você pode enviar o email para o público-alvo principal. [Saiba como preparar e enviar seu email](../monitor/prepare-send.md)

## Acessar provas enviadas {#access-proofs}

Depois que as provas forem enviadas, você poderá acessar logs dedicados do **[!UICONTROL Exibir log de email de teste]** botão. Esses logs permitem acessar todas as provas enviadas para o delivery selecionado e visualizar estatísticas específicas relacionadas ao envio.

![](assets/proof-log.png)

Você também pode acessar provas da lista de deliveries, como qualquer delivery.

![](assets/delivery-list.png)
