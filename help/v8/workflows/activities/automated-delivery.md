---
audience: end-user
title: Atividade do fluxo de trabalho de delivery automatizado
description: Saiba como usar a atividade de workflow de entrega automatizada
exl-id: a9c485f1-0369-414d-9e43-bedb0390a2f5
source-git-commit: 65031741dc7c667ef74469d75b8ea60a5fc20aaf
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 20%

---

# Entrega automatizada {#automated-delivery}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="Atividade de entrega automatizada"
>abstract="A atividade de fluxo de trabalho Entrega automatizada agora está disponível na paleta do fluxo de trabalho. Você pode usá-la para criar ou executar ações de entrega (preparar, enviar uma prova, preparar e iniciar etc.) diretamente do seu fluxo de trabalho."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=pt-BR" text="Consulte as notas de versão"

>[!CONTEXTUALHELP]
>id="acw_orchestration_automated-delivery"
>title="Atividade de entrega automatizada"
>abstract="A atividade **Entrega Automatizada** é usada para automação: crie ou reutilize uma entrega no fluxo de trabalho e, em seguida, escolha uma ação para executar (preparar, preparar e iniciar, enviar prova, etc.). É possível selecionar uma entrega explícita já existente criada fora do fluxo de trabalho ou criar uma nova entrega a partir de um modelo sempre que a atividade for executada."

A atividade de **Entrega automatizada** permite criar, configurar e executar ações de entrega diretamente no fluxo de trabalho. Use-a quando quiser executar um delivery predefinido em uma programação ou como parte de um fluxo automatizado, ou quando quiser gerar um novo delivery a partir de um modelo sempre que a atividade for executada.

<!--
**[Continuous delivery](continuous-delivery.md)** always uses a template. The first run creates one delivery; later runs send to new recipients through that same delivery. **Automated delivery** is different: you either reuse one existing delivery every run, or you create a new delivery from a template each time—so each run can be its own delivery if you want. 
-->

Para configurar essa atividade, siga estas etapas:

1. Definir as configurações de entrega, [leia mais](#delivery-settings)
1. Selecione a ação a ser executada, [leia mais](#action-to-execute)
1. Configure a transição, [leia mais](#transition-to-execute)
1. Definir um script de modificação, [leia mais](#script)

## Definir as configurações de entrega {#delivery-settings}

Ao configurar a atividade, você escolhe de onde o delivery vem. Duas opções estão disponíveis nesta seção:

![Captura de tela mostrando a entrega automatizada](../assets/automated-delivery.png){zoomable="yes"}

* Selecione **Entrega explícita** quando quiser atuar em uma entrega existente, por exemplo, uma entrega independente ou uma entrega criada a partir de uma campanha. Escolha a entrega usando o botão **Selecionar entrega**. Cada vez que o fluxo de trabalho é executado e atinge esta atividade, ele age na entrega **igual**. Nenhum novo delivery é criado por execução. A atividade reutiliza o mesmo delivery. Isso é útil quando você tem um único delivery que deseja preparar ou enviar repetidamente, por exemplo, em uma programação ou após uma etapa de aprovação.

<!-- by default, the list shows unfinished deliveries in the Deliveries folder. You can browse other folders to select a delivery from another campaign. You choose the action to perform (prepare, prepare and start, send a proof, and so on).-->

* Selecione **Novo, criado a partir de um modelo** quando quiser que uma entrega **novo** seja criada toda vez que a atividade for executada. Escolha o modelo de entrega usando o botão **Selecionar modelo**. Cada execução gera um novo delivery com base nesse template. Use isso quando cada execução de workflow deve resultar em seu próprio delivery distinto (por exemplo, um email por execução).

<!-- Unlike the Continuous delivery activity, there is no “append” to a previous execution—each run produces a separate delivery. -->

>[!NOTE]
>
>As opções **Especificado na transição** e **Calculado por script**, usadas para casos de uso avançados, só podem ser configuradas no Console do Cliente. Consulte a [documentação do Campaign v8](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/wf-activities/action-activities/delivery){target="_blank"}.

## Selecionar a ação a ser executada {#action-to-execute}

Nesta seção, escolha o que a atividade faz com o delivery. As seguintes opções estão disponíveis:

![Captura de tela mostrando as ações a serem executadas na entrega automatizada](../assets/automated-delivery2.png){zoomable="yes"}

* **Salvar**: cria e salva a entrega sem analisá-la ou enviá-la.
* **Estimar o destino**: calcula o destino de entrega para avaliar seu potencial (primeira fase de análise).
* **Prepare**: executa a análise completa (cálculo de destino e preparação de conteúdo). O delivery não é enviado.
* **Enviar uma prova**: envia uma prova da entrega.
* **Preparar e iniciar**: executa a análise completa (cálculo de destino e preparação de conteúdo) e envia a entrega.

## Configurar a transição {#transition-to-execute}

Esta seção permite escolher se deseja gerar transições após a atividade. As seguintes opções estão disponíveis:

![Captura de tela mostrando as transições na entrega automatizada](../assets/automated-delivery3.png){zoomable="yes"}

* **Gerar uma transição de saída**: gera uma transição de saída quando a atividade é concluída.
* **Rótulo de transição**: permite personalizar o rótulo exibido na transição na tela.
* **Processar erros**: adiciona uma transição adicional para manipular erros.

## Definir um script de modificação {#script}

Você pode usar um script para alterar o comportamento da atividade, por exemplo, parâmetros de delivery como o rótulo da atividade. Use isso quando precisar de lógica personalizada para essa atividade.

Clique em **Criar script** e escreva a lógica de modificação no editor.

## Tópicos relacionados {#related}

* [Sobre atividades de fluxo de trabalho](about-activities.md)
* [Entrega contínua](continuous-delivery.md)
* [Atividades de email, SMS, Push, Correspondência direta](channels.md)
* [Modelos de entrega](../../msg/delivery-template.md)
