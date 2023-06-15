---
audience: end-user
title: Configurações de entrega de email
description: Saiba mais sobre as configurações de entrega de email na interface do Campaign Web
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
badge: label="Alpha"
source-git-commit: a653fe4329f449a94f8056e4b5f2247bd839b87a
workflow-type: tm+mt
source-wordcount: '1475'
ht-degree: 92%

---


# Configurações de entrega de email {#email-del-settings}

Essas configurações são **parâmetros técnicos da entrega** definidas no modelo de email. Eles estão disponíveis no ícone **Definir configurações de entrega** disponível ao editar uma entrega de email.

## Configurações de entrega de email {#email-delivery-settings}

>[!CAUTION]
>
> Essas configurações estão descritas somente para suas informações. Algumas delas dependem de sua configuração e permissões. Elas não devem ser modificadas nesta versão do produto.

## Tipologia {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Tipologia"
>abstract="A tipologia permite controlar, filtrar e monitorar o envio de entregas."

Tipologias são conjuntos de **regras de tipologia**, que são executadas durante a fase de análise da mensagem. Elas possibilitam garantir que seus emails sempre contenham determinados elementos (como um link de cancelamento de assinatura ou uma linha de assunto) ou regras de filtragem para excluir grupos do público-alvo desejado (como clientes que não assinam, concorrentes ou clientes não fidelizados).

Ao associar uma tipologia a uma mensagem ou a um modelo de mensagem, as regras de tipologia incluídas na tipologia serão executadas para verificar a validade da mensagem durante a preparação da mensagem.

![](assets/delivery-settings-1.png)


### Parâmetros de pressão {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="Peso da entrega"
>abstract="Os pesos das entregas permitem identificar entregas de alta prioridade dentro da estrutura do gerenciamento de pressão. As mensagens com o peso mais alto têm prioridade."

Nesta seção, os parâmetros de pressão permitem definir um **limite**. Esse é o número máximo de mensagens que podem ser enviadas para um perfil em um dado período. Depois que esse limite for atingido, não poderá ocorrer mais entregas até o final do período considerado. Esse processo permite excluir automaticamente um perfil de uma entrega, caso uma mensagem exceder o limite definido, evitando assim um excesso de solicitações.

Os valores do limite podem ser constantes ou variáveis. Isso significa que, para um determinado período, os limites podem variar de um perfil para o outro, ou até mesmo para o mesmo perfil.

No campo **Tipo de peso**, três opções estão disponíveis:

* **Constante**
* **Depende do recipient**
* **Definido em cada regra**

Use o campo **Peso da entrega** para definir a prioridade de entrega. Cada entrega tem um peso que representa seu nível de prioridade. Por padrão, o peso de uma entrega é definido como 5. As regras de pressão permitem definir o peso das entregas às quais são aplicadas. Os pesos podem ser definidos ou calculados por meio de uma fórmula para se adequar aos recipients. Por exemplo, você pode definir o peso de uma entrega com base nos interesses do recipient.


Use o campo **Modo de entrega** para selecionar o modo de avaliação do público-alvo. Três modos estão disponíveis:

* **Estimativa do público-alvo e personalização de mensagens**
* **Estimativa e aprovação do público-alvo provisório**
* **Avaliação de público-alvo**

O gerenciamento de fadiga vem com o complemento **Otimização de campanha**. Saiba mais sobre as regras de pressão e como configurar o gerenciamento de fadiga na [Documentação do Campaign v8](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=pt-BR){target="_blank"}.

### Configurações de capacidade {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="Importância do recipient"
>abstract="A importância do recipient é uma fórmula usada para determinar quais recipients são mantidos quando as regras de tipologia de capacidade são excedidas."

Nesta seção, você pode selecionar uma regra de capacidade definida no Console do Adobe Campaign v8. Essa regra está associada ao canal de email.

O campo **importância do recipient** é uma fórmula usada para determinar quais destinatários são mantidos quando as regras de tipologia de capacidade são excedidas.

Saiba mais sobre regras de consistência e capacidade e como configurá-las em [Documentação do Campaign v8](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html?lang=pt-BR){target="_blank"}.


## Público {#audience}

Nesta seção, você pode selecionar uma **mapeamento de público-alvo** entre aquelas disponíveis. Os mapeamentos de públicos-alvo são definidos no console do Adobe Campaign v8.

Saiba mais sobre target mappings em [Documentação do Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=pt-BR){target="_blank"}.

## Entrega {#delivery}

Os parâmetros de entrega são configurações técnicas que se aplicam à sua entrega.

* **Roteamento**: a conta de email externa integrada de roteamento é fornecida por padrão. Ela contém os parâmetros técnicos que permitem ao aplicativo enviar emails.

* **Teste da entrega SMTP**: essa opção é usada para testar o envio via SMTP. A entrega é processada até a conexão com o servidor SMTP, mas não é enviada: para cada recipient da entrega, o Campaign se conecta ao servidor do provedor SMTP, executa o comando SMTP RCPT TO e encerra a conexão antes do comando SMTP DATA.

* **Email CCO**: essa opção permite armazenar emails em um sistema externo por meio do CCO, simplesmente adicionando um endereço de email CCO ao publico alvo da mensagem. Saiba mais sobre Email Cco em [Documentação do Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html?lang=pt-BR){target="_blank"}.



### Tentativas {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="Número máximo de tentativas"
>abstract="Se uma mensagem falhar devido a um erro temporário, as tentativas serão executadas até o fim da duração da entrega."

<!--Temporarily undelivered messages due to a Soft or Ignored error are subject to an automatic retry. By default, five retries are scheduled for the first day of the delivery with a minimum interval of one hour spread out over the 24 hours of the day. -->

Saiba mais sobre o gerenciamento de tentativas no [Documentação do Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html?lang=pt-BR){target="_blank"}.

## Aprovação {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Modo de aprovação"
>abstract="Cada etapa de uma entrega pode estar sujeita à aprovação para garantir o monitoramento e o controle totais dos vários processos."

Se os avisos forem gerados durante a preparação da entrega, você pode configurar a entrega para definir se ela ainda deverá ou não ser executada. Por padrão, o usuário deverá confirmar o envio de mensagens no final da fase de análise: essa é a validação **manual**.

Você pode selecionar outro modo de aprovação no campo apropriado. Os modos disponíveis são:

* **Manual**: no final da fase de análise, o usuário deverá confirmar a entrega para começar a enviar.

* **Semiautomático**: o envio começa automaticamente se a fase de análise não gerar mensagens de advertência.

* **Automático**: o envio começa automaticamente no fim da fase de análise, independentemente do resultado.


## Validade {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="Duração da entrega"
>abstract="O campo Duração da entrega permite inserir o limite de novas tentativas de entrega globais. Isso significa que o Adobe Campaign envia as mensagens começando na data de início e, em seguida, para mensagens que retornam somente um erro, tentativas regulares e configuráveis são executadas até que o limite de validade seja atingido."

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Limite da validade de recursos"
>abstract="O campo Limite da validade é usado para recursos carregados, principalmente para a mirror page ou imagens. Esses recursos são válidos por um tempo limitado: quando o limite é atingido, os recursos não estarão mais disponíveis."


O campo **Delivery duration** permite inserir o limite de novas tentativas de entrega globais. Isso significa que o Adobe Campaign envia as mensagens começando na data de início e, em seguida, para mensagens que retornam somente um erro, tentativas regulares e configuráveis são executadas até que o limite de validade seja atingido.

Você também poderá optar por especificar datas. Para fazer isso, selecione **Explicitly set validity dates**. Nesse caso, as datas de entrega e limite de validade também permitem especificar o tempo. O tempo atual é usado por padrão, mas você poderá modificar isso diretamente no campo de entrada.

O **Limite da validade de recursos** é usado para recursos carregados, principalmente para a mirror page e as imagens. Os recursos dessa página são válidos por um tempo limitado (para economizar espaço em disco). Após esse limite, esses recursos não estarão mais disponíveis.

![](assets/delivery-settings-2.png)


Saiba mais sobre o período de validade do delivery em [Documentação do Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=pt-BR#validity-period){target="_blank"}.

### Gerenciamento da mirror page {#mirror}

A mirror page é uma página HTML acessível online através de um navegador da Web. Seu conteúdo é idêntico ao email. Por padrão, a mirror page é gerada se o link for inserido no conteúdo do email.

Além do modo padrão, as seguintes opções também estão disponíveis:


* **[!UICONTROL Forçar a geração da mirror page]**: use esse modo para gerar a mirror page, mesmo que nenhum link para a mirror page for inserida na entrega,
* **[!UICONTROL Não gerar a mirror page]**: use esse modo para evitar a geração de uma mirror page, mesmo se o link estiver presente na entrega.
* **[!UICONTROL Gera uma mirror page acessível somente por meio do identificador de mensagem]**: quando o link da mirror page não estiver presente no conteúdo do email, use essa opção para ativar o acesso ao conteúdo da mirror page, na janela de log do delivery, no console do cliente.


### Rastreamento {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Período de validade"
>abstract="Essa opção define a duração do rastreamento ativado nos URLs."

Os parâmetros de rastreamento são definidos na seção relacionada. As opções possíveis são:

**Limite da validade do rastreamento**: use esta opção para alterar a duração para a qual o rastreamento é ativado nos URLs.

**URL de substituição para URLs expirados**: use esta opção para inserir um URL para uma página da Web alternativa, que é exibida assim que o rastreamento expira.

## Configurações de teste {#test-setttings}

Você pode definir os parâmetros de exclusão nesta seção. As opções disponíveis são:

* **Manter duplicada**: ela permite autorizar várias entregas a recipients que atendem a vários critérios de direcionamento.

* **Manter endereços incluídos na lista de bloqueios** permite manter do público-alvo os perfis que não estão mais sendo direcionados para entrega, como após um cancelamento de subscrição (opt-out).

* **Manter endereços na quarentena** permite excluir do público-alvo qualquer perfil com endereço que não responda.

Você também pode personalizar o nome dos emails de teste.

A opção **Guardar o código de entrega como prova** permite associar ao email de teste o mesmo código de entrega definido para a entrega ao qual está selecionado.

Por padrão, o assunto do email de teste tem o prefixo &#39;PROOF #&#39;, onde # é o número do email de teste. É possível alterar esse prefixo no campo **Rotular prefixo**.