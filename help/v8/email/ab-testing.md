---
audience: end-user
title: Criar experimentos de conteúdo
description: Saiba como criar experimentos de conteúdo no Adobe Campaign Web
source-git-commit: f772e19fd033b007680777f75b48775b6d7851b9
workflow-type: tm+mt
source-wordcount: '1154'
ht-degree: 2%

---

# Criar experimentos de conteúdo {#content-experiment}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="Experimentos de conteúdo - Teste A/B"
>abstract="Agora você pode definir várias variantes de entrega para testar qual tem melhor desempenho. Varie o conteúdo, o assunto ou o remetente entre elementos de email para determinar os resultados ideais."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=pt-BR" text="Consulte as notas de versão"

## Sobre experimentos de conteúdo {#about-content-experiment}

Os experimentos de conteúdo na Adobe Campaign Web permitem definir várias variantes de delivery de teste A/B para medir qual tem o melhor desempenho para o público-alvo. Você pode variar o conteúdo do delivery, o assunto ou o remetente para testar diferentes versões e determinar qual variante produz os melhores resultados.

Você pode realizar testes A/B em vários elementos de email, como:

* **Linha de assunto**: teste diferentes linhas de assunto de email para ver qual gera a maior taxa de abertura
* **Nome do remetente**: experimente com combinações de remetentes diferentes
* **Conteúdo do corpo do email**: crie várias versões de conteúdo para identificar quais acionam a melhor taxa de cliques

>[!NOTE]
>
>* Os experimentos de conteúdo estão disponíveis no momento somente para canal de email.
>* O teste A/B não é compatível com mensagens transacionais.
>* Máximo de 3 tratamentos (variantes) por experimento.

## Criar um experimento de conteúdo {#create-content-experiment}

Para adicionar um experimento de conteúdo ao delivery de email, siga estas etapas:

1. Criar um delivery de email ou abrir um delivery de rascunho existente. [Saiba como criar um email](create-email.md)

1. Na página de propriedades do delivery de email, clique no botão **[!UICONTROL Criar experimento]** localizado na seção **[!UICONTROL Conteúdo]**.

   ![Captura de tela mostrando o botão Criar experimento nas propriedades do email](assets/ab-testing-1.png){zoomable="yes"}

## Definir as configurações do experimento {#configure-experiment}

Configure seu experimento usando as seguintes seções:

![Captura de tela mostrando as configurações do experimento](assets/ab-testing-2.png){zoomable="yes"}

### Configurações de público-alvo {#audience-settings}

Defina a porcentagem da população do target que receberá as variantes de experimento.

Insira um valor para definir o tamanho do público. Representa a proporção de recipients que receberão uma das variantes de experimento durante a fase de teste.

* **Mínimo**: 1%
* **Máximo**: 100%
* **Padrão**: 10%

O público restante (90% por padrão) receberá a variante vencedora assim que o experimento for concluído e um vencedor for determinado.

Por exemplo, com um público-alvo de 10.000 recipients e um tamanho de público de 10%, 1.000 recipients serão aleatoriamente selecionados para participar do experimento. Os 9.000 recipients restantes receberão a variante vencedora após o término do experimento.

### Estratégia vencedora {#winning-strategy}

Selecione a métrica que será usada para determinar a variante vencedora:

* **[!UICONTROL Melhor taxa de abertura]** (padrão): a variante com a maior porcentagem de aberturas de email vence
* **[!UICONTROL Melhor taxa de cliques]**: a variante com a maior porcentagem de cliques no email vence
* **[!UICONTROL Taxa de cancelamento de assinatura mais baixa]**: a variante com a menor porcentagem de cancelamentos de assinatura vence

O sistema rastreia automaticamente essas métricas durante o experimento e calcula qual variante tem melhor desempenho de acordo com o critério selecionado.

### Método de envio do vencedor {#sending-method}

Defina por quanto tempo o experimento deve ser executado e selecione o método de envio:

1. Insira o valor da duração em horas. O experimento será executado por esse período antes de determinar a variante vencedora.

   * **Mínimo**: 3 horas
   * **Máximo**: 240 horas (10 dias)
   * **Padrão**: 24 horas

   >[!NOTE]
   >
   >Verifique se a duração do experimento é longa o suficiente para coletar dados significativos. Uma curta duração pode não fornecer significância estatística suficiente, especialmente para métricas como a taxa de cliques, que pode levar mais tempo para se acumular.

1. Escolha como a variante vencedora deve ser enviada para a população restante:

   * **[!UICONTROL Envio automático]** ativado: o sistema envia automaticamente a variante vencedora para o público restante após o término do experimento.
   * **[!UICONTROL Envio automático]** desativado: você deve clicar manualmente no botão **[!UICONTROL Enviar]** para enviar a variante vencedora depois de examinar os resultados do experimento.

Se nenhuma variante alcançar resultados significativamente melhores do que as outras até o final do experimento, o sistema envia a primeira variante para a população restante. Consulte esta [seção](#send-deliveries).

## Definir os tratamentos de conteúdo {#define-content}

Depois de salvar as configurações do experimento, um primeiro tratamento é criado por padrão. Agora é necessário adicionar outros tratamentos (até três) e definir o conteúdo específico.

1. Nas propriedades de entrega, clique em **[!UICONTROL Editar conteúdo]**. Os tratamentos são exibidos no lado esquerdo.

   ![Captura de tela mostrando o painel de experimentos de conteúdo](assets/ab-testing-3.png){zoomable="yes"}

1. Clique no botão **[!UICONTROL Adicionar tratamento]** e defina seu nome. Repita essa operação para todos os tratamentos que precisam ser adicionados. Em seguida, você pode alterar o nome, duplicá-los e removê-los.

1. Clique em cada tratamento e personalize os seguintes itens:

   * **Nome do remetente**: personalize de quem o email parece ser
   * **Linha de assunto**: escreva uma linha de assunto exclusiva para cada tratamento
   * **Corpo do email**: crie versões diferentes de conteúdo usando o Designer de email

   ![Captura de tela mostrando vários tratamentos](assets/ab-testing-4.png){zoomable="yes"}

1. Visualize cada tratamento clicando no tratamento e em **[!UICONTROL Simular conteúdo]**.

## Iniciar o experimento e monitorar os resultados {#validate-start}

Depois de definir todos os tratamentos de conteúdo, você pode validar e iniciar o experimento.

1. Nas propriedades de entrega, clique em **[!UICONTROL Revisar e enviar]** e em **[!UICONTROL Preparar]**.

1. Em seguida, clique em **[!UICONTROL Iniciar experimentação]** para iniciar o teste A/B.

   ![Captura de tela mostrando o botão Iniciar experimentação](assets/ab-testing-5.png){zoomable="yes"}

1. Depois que o experimento estiver em execução, monitore as diferentes métricas exibidas no painel do delivery.

Enquanto o experimento é executado, você pode clicar em **[!UICONTROL Parar envio]** para encerrar o experimento. Você também pode decidir enviar manualmente antes do fim do experimento clicando em **[!UICONTROL Selecionar e enviar para o vencedor]**.

>[!NOTE]
>
>Os resultados são atualizados em tempo quase real, à medida que os recipients interagem com seu email. No entanto, os resultados iniciais podem não ter significância estatística - é recomendável esperar até que a duração do experimento esteja concluída antes de tomar decisões finais.

## Enviar os deliveries {#send-deliveries}

O envio pode ser executado automática ou manualmente, de acordo com o que você escolheu nas configurações do **[!UICONTROL método de envio do vencedor]**. Consulte esta [seção](#sending-method).

### Envio automático {#automatic-sending}

Para envio automático, o sistema analisa os resultados com base em sua estratégia vencedora e determina o tratamento vencedor. O tratamento vencedor é enviado automaticamente para o público restante. Se nenhum vencedor claro surgir, a primeira variante será escolhida.

### Envio manual {#manual-sending}

Se você configurou o envio manual, analise os resultados quando o experimento terminar e clique em **[!UICONTROL Enviar]** para enviar o tratamento vencedor. Se nenhum vencedor claro emergir, o primeiro tratamento é selecionado por padrão, mas você pode escolher um diferente.

## Exibir resultados finais {#final-results}

Depois que o experimento for concluído e o delivery for totalmente enviado, você poderá acessar relatórios abrangentes:

1. No painel de entrega, clique em **[!UICONTROL Relatórios]**.

1. Navegue até a guia de relatório **[!UICONTROL Experimentos]** para exibir as principais métricas de desempenho para cada tratamento.

## Práticas recomendadas {#best-practices}

Ao criar experimentos de conteúdo, considere estas recomendações:

* **Testar um elemento de cada vez**: para obter resultados mais claros, teste variações de um único elemento (por exemplo, somente linha de assunto ou somente conteúdo) em vez de vários elementos simultaneamente.

* **Escolha a duração apropriada**: permita tempo suficiente para significância estatística:
   * Para testes de taxa aberta: 12 a 24 horas geralmente são suficientes
   * Para testes de taxa de cliques: 24 a 48 horas ou mais podem ser necessárias
   * Públicos-alvo maiores podem exigir menos tempo; públicos-alvo menores podem precisar de mais tempo

* **Dimensione seu público adequadamente**:
   * Verifique se o público-alvo do experimento (a porcentagem alocada para o teste) é grande o suficiente para produzir resultados significativos
   * Diretriz geral: Mínimo de 1.000 recipients por tratamento para resultados confiáveis

* **Testar regularmente, mas não excessivamente**: realize experimentos em campanhas importantes, mas evite testar cada envio individual para concentrar os recursos em decisões impactantes.

* **Documente seus aprendizados**: mantenha registros dos resultados dos experimentos para informar as estratégias de campanhas futuras.

## Tópicos relacionados {#related-topics}

* [Criar seu primeiro email](create-email.md)
* [Configurar conteúdo de email](edit-content.md)
* [Pré-visualizar e enviar um email](../monitor/prepare-send.md)
* [Relatórios de entrega de email](../reporting/email-report.md)
