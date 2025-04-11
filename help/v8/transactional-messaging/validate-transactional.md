---
audience: end-user
title: Validar mensagens transacionais
description: Saiba como validar uma mensagem transacional na interface da Web do Campaign
exl-id: 4a24792f-b9f4-4224-b3a8-75f6969b64da
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 1%

---

# Validar mensagens transacionais

Durante ou depois de criar a mensagem transacional, talvez você queira validar o conteúdo usando uma amostra de dados.

## Simular conteúdo {#simulate-content}

Siga estas etapas para simular o conteúdo da mensagem:

* Verifique se o caminho de personalização no conteúdo da mensagem corresponde à sua amostra de contexto. No exemplo abaixo, para exibir o nome do perfil de teste, use o caminho *rtEvent.ctx.basicDetails.firstName*.

  Você pode modificar o conteúdo da mensagem ou a amostra de contexto para alinhá-los.

  ![Captura de tela mostrando a verificação dos caminhos de personalização no conteúdo da mensagem](assets/validate-verification.png){zoomable="yes"}

* Clique no botão **[!UICONTROL Simular conteúdo]** para visualizar sua mensagem transacional com os dados inseridos na amostra de contexto.

  ![Captura de tela mostrando o botão Simular conteúdo e a funcionalidade de visualização](assets/validate-simulate.png){zoomable="yes"}

  Depois de revisar o conteúdo, clique no botão **[!UICONTROL Fechar]**.

* Clique no botão **[!UICONTROL Republicar]** se tiver feito alterações no conteúdo.

## Enviar prova

Para testar e experimentar a mensagem transacional como ela seria entregue por meio do canal escolhido, como email, SMS ou notificação por push, use o recurso de prova.

Na [janela de conteúdo da simulação](#simulate-content), clique no botão **[!UICONTROL Enviar prova]**.

![Captura de tela mostrando o botão Enviar prova na janela de conteúdo da simulação](assets/transactional-proof.png){zoomable="yes"}

Na nova janela exibida, digite o endereço de email ou o número de telefone, dependendo do canal, onde você deseja receber a prova. Depois de inserir o endereço desejado, clique nos botões **[!UICONTROL Enviar prova]** e **[!UICONTROL Confirmar]**. Essa ação envia um exemplo da mensagem transacional, garantindo que todas as personalizações, o conteúdo dinâmico e a formatação sejam exibidos corretamente para os usuários finais.

![Captura de tela mostrando a funcionalidade Enviar prova e o processo de confirmação](assets/transactional-sendproof.png){zoomable="yes"}

Essa etapa é essencial para identificar possíveis problemas antes de publicar sua mensagem transacional.