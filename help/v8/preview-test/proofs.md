---
audience: end-user
title: Enviar emails de teste
description: Saiba como definir e enviar emails de teste
exl-id: b2677579-c95d-443d-b207-466af364c208
badge: label="Alpha" type="Positive"
source-git-commit: b5af5099d62e0e424fffdd8eb74d67f12777b0f2
workflow-type: ht
source-wordcount: '541'
ht-degree: 100%

---

# Enviar emails de teste {#send-proofs}

O envio de emails de teste é uma etapa importante na validação da campanha de email e na identificação de possíveis problemas. Ao enviar emails de teste, você pode verificar vários elementos, como links, opções de não participação, imagens e mirror pages, bem como detectar quaisquer erros.

Os emails de teste podem ser enviados para dois tipos de recipients:

* **Perfis de teste**: envia emails de teste para os seed addresses, que são recipients adicionais e fictícios no banco de dados. Eles podem ser criados no console do Adobe Campaign, na pasta **[!UICONTROL Recursos]** / **[!UICONTROL Gerenciamento de campanhas]** / **[!UICONTROL Seed addresses]**.

* **Substituição do público alvo principal**: envia emails de teste para um endereço de email específico como a representação de um perfil existente. Isso permite visualizar a experiência de email dos recipients, fornecendo uma representação precisa da mensagem que o perfil recebe.

## Selecione os recipients de teste {#recipients}

1. Acesse a tela de simulação de conteúdo de email e clique no botão **[!UICONTROL Teste]**.

   ![](assets/test-button.png)

1. Use a lista suspensa **[!UICONTROL Modo]** para escolher o tipo de recipients que receberão o email de teste:

   * **Perfis de teste**: envia o email de teste para os seed addresses, que são recipients adicionais e fictícios no banco de dados,

   * **Substituição do público alvo principal**: envia o email de teste para um endereço de email específico como a representação de um perfil existente. Isso permite visualizar a experiência de email dos recipients, fornecendo uma representação precisa da mensagem que o perfil recebe.

   ![](assets/test-mode.png)

   >[!NOTE]
   >
   >O modo **[!UICONTROL Perfis de teste]** está selecionado por padrão. Se já tiver selecionado perfis para visualizar o email na tela de simulação de conteúdo, esses perfis serão pré-selecionados como recipients de teste. Você pode limpar a seleção e/ou adicionar outros recipients.

1. Para enviar emails de teste para perfis de substituição, escolha **[!UICONTROL Substituição do público alvo]** e, em seguida, siga estas etapas:

   1. Clique no botão **[!UICONTROL Adicionar endereço]** e especifique o endereço de email que receberá o email de teste.

      Você pode inserir qualquer endereço de email. Isso permite enviar emails de teste para qualquer usuário, mesmo que ele não utilize o Adobe Campaign V8.

   1. Selecione o perfil do público alvo a ser usado para enviar o email de teste. Você também pode permitir que o Adobe Campaign selecione um perfil aleatório do público alvo.

   1. Confirme o recipient e repita a operação para adicionar quantos endereços forem necessários.

      ![](assets/substitution.png)

1. Após selecionar os recipients do teste, você pode enviar o email de teste. [Saiba como enviar emails de teste](#send)

   >[!NOTE]
   >
   >Se deseja enviar a mensagem de email final para os recipients do email de teste, habilite a opção **[!UICONTROL Incluir população de teste no público alvo principal]**.

## Enviar o email de teste {#send}

Para enviar o email de teste para os recipients selecionados, clique em **[!UICONTROL Enviar email de teste]** e, em seguida, confirme o envio.

![](assets/send-proof.png)

Envie quantos emails de teste forem necessários até concluir o conteúdo da sua entrega. Feito isso, você poderá enviar o email para o público alvo principal. [Saiba como preparar e enviar seu email](../monitor/prepare-send.md)

## Acessar emails de teste enviados {#access-proofs}

Depois que os emails de teste forem enviados, você poderá acessar os logs dedicados por meio do botão **[!UICONTROL Exibir log de email de teste]**.

Esses logs permitem acessar todos os emails de teste enviados para a entrega selecionada e visualizar estatísticas específicas relacionadas ao envio. [Saiba como monitorar os logs de entrega](../monitor/delivery-logs.md)

![](assets/proof-log.png)

Você também pode acessar os emails de teste enviados por meio da lista de entregas, como em qualquer entrega.

![](assets/delivery-list.png)
