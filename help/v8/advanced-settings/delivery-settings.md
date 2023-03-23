---
audience: end-user
title: Configurações de entrega de email
description: Saiba mais sobre as configurações de delivery de email na interface do usuário da Web do Campaign
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: c92e6c1455266fe3430720117d61114ba027b187
workflow-type: tm+mt
source-wordcount: '1471'
ht-degree: 49%

---

# Configurações de delivery de email {#email-del-settings}

![Versão alfa](../assets/do-not-localize/badge.png)

Essas configurações são **parâmetros técnicos do delivery** que são definidas no template de email. Eles estão disponíveis no **Definir configurações de delivery** ícone disponível ao editar um delivery de email.

## Configurações de delivery de email {#email-delivery-settings}

>[!CAUTION]
>
> Essas configurações são descritas somente para suas informações. Alguns deles dependem da sua configuração e permissões. Eles não devem ser modificados nesta versão do produto.

## Tipologia {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Tipologia"
>abstract="A tipologia permite controlar, filtrar e monitorar o envio de entregas."

Tipologias são conjuntos de **regras de tipologia**, que são executadas durante a fase de análise da mensagem. Elas possibilitam garantir que seus emails sempre contenham determinados elementos (como um link de cancelamento de assinatura ou uma linha de assunto) ou regras de filtragem para excluir grupos do público-alvo desejado (como clientes que não assinam, concorrentes ou clientes não fidelizados).

Ao associar uma tipologia a uma mensagem ou a um template de mensagem, as regras de tipologia incluídas na tipologia são executadas para verificar a validade da mensagem durante a preparação da mensagem.

![](assets/delivery-settings-1.png)


### Parâmetros de pressão {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="Peso da entrega"
>abstract="Os pesos das entregas permitem identificar entregas de alta prioridade dentro da estrutura do gerenciamento de pressão. As mensagens com o peso mais alto têm prioridade."

Nesta seção, os parâmetros de pressão permitem definir uma **limite**. Esse é o número máximo de mensagens que podem ser enviadas para um perfil em um determinado período. Depois que esse limite for atingido, não poderá ocorrer mais deliveries até o final do período considerado. Esse processo permite excluir automaticamente um perfil de um delivery, caso uma mensagem exceder o limite definido, evitando assim um excesso de solicitações.

Os valores do limite podem ser constantes ou variáveis. Isso significa que, para um determinado período, os limites podem variar de um perfil para o outro, ou até mesmo para o mesmo perfil.

No **Tipo de peso** , três opções estão disponíveis:

* **Constante**
* **Depende do recipient**
* **Definido em cada regra**

Use o **Peso do delivery** para definir a prioridade do delivery. Cada delivery tem um peso que representa seu nível de prioridade. Por padrão, o peso de um delivery é definido como 5. As regras de pressão permitem definir o peso dos deliveries aos quais são aplicados. Os pesos podem ser definidos ou calculados por meio de uma fórmula para se adequar aos recipients. Por exemplo, você pode definir o peso de um delivery com base nos interesses do recipient.


Use o **Modo de entrega** para selecionar o modo de avaliação do target. Três modos estão disponíveis:

* **Estimativa do público-alvo e personalização de mensagens**
* **Estimativa e aprovação do público alvo provisório**
* **Avaliação de público alvo**

O gerenciamento de fadiga vem com o **Otimização de campanha** complemento. Saiba mais sobre as regras de pressão e como configurar o gerenciamento de fadiga no [Documentação do Campaign v8](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=pt-BR){target="_blank"}.

### Configurações de capacidade {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="Importância do recipient"
>abstract="A importância do recipient é uma fórmula usada para determinar quais recipients são mantidos quando as regras de tipologia de capacidade são excedidas."

Nesta seção, você pode selecionar uma regra de capacidade definida no Console do Adobe Campaign v8. Essa regra está associada ao canal de email.

O **importância do destinatário** é uma fórmula usada para determinar quais recipients são mantidos quando as regras de tipologia de capacidade são excedidas.

Saiba mais sobre regras de consistência e capacidade e como configurá-las em [Documentação do Campaign v8](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html){target="_blank"}.


## Público-alvo {#audience}

Nesta seção, você pode selecionar uma **target mapping** entre as disponíveis. Os mapeamentos do Target são definidos no console do Adobe Campaign v8.

Saiba mais sobre target mappings no [Documentação do Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html){target="_blank"}.

## Entrega {#delivery}

Os parâmetros de delivery são configurações técnicas que se aplicam ao seu delivery.

* **Roteamento**: a conta externa integrada de roteamento de email é fornecida por padrão. Ela contém os parâmetros técnicos que permitem ao aplicativo enviar emails.

* **Teste do delivery SMTP**: essa opção é usada para testar o envio via SMTP. A entrega é processada até a conexão com o servidor SMTP, mas não é enviada: para cada destinatário do delivery, o Campaign se conecta ao servidor do provedor SMTP, executa o comando SMTP RCPT TO e encerra a conexão antes do comando SMTP DATA.

* **Email Cco**: essa opção é usada para armazenar emails em um sistema externo por meio do CCO simplesmente adicionando um endereço de email de CCO ao target da sua mensagem. Saiba mais sobre email Cco em [Documentação do Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.



### Tentativas {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="Número máximo de tentativas"
>abstract="Se uma mensagem falhar devido a um erro temporário, as tentativas serão executadas até o fim da duração da entrega."

<!--Temporarily undelivered messages due to a Soft or Ignored error are subject to an automatic retry. By default, five retries are scheduled for the first day of the delivery with a minimum interval of one hour spread out over the 24 hours of the day. -->

Saiba mais sobre o gerenciamento de tentativas no [Documentação do Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.

## Aprovação {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Modo de aprovação"
>abstract="Cada etapa de uma entrega pode estar sujeita à aprovação para garantir o monitoramento e o controle totais dos vários processos."

Se os avisos forem gerados durante a preparação do delivery, você poderá configurar o delivery para definir se ele ainda deverá ou não ser executado. Por padrão, o usuário deverá confirmar o envio de mensagens no final da fase de análise: essa é a validação **manual**.

Você pode selecionar outro modo de aprovação no campo apropriado. Os modos disponíveis são:

* **Manual**: no final da fase de análise, o usuário deverá confirmar o delivery para começar a enviar.

* **Semiautomático**: O envio começa automaticamente se a fase de análise não gerar mensagens de aviso.

* **Automático**: O envio começa automaticamente no final da fase de análise, independentemente do resultado.


## Validade {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="Duração da entrega"
>abstract="O campo Duração da entrega permite inserir o limite de novas tentativas de entrega globais. Isso significa que o Adobe Campaign envia as mensagens começando na data de início e, em seguida, para mensagens que retornam somente um erro, tentativas regulares e configuráveis são executadas até que o limite de validade seja atingido."

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Limite da validade de recursos"
>abstract="O campo Limite da validade é usado para recursos carregados, principalmente para a mirror page e imagens. Os recursos desta página são válidos por um tempo limitado."


O campo **Delivery duration** permite inserir o limite de novas tentativas de delivery globais. Isso significa que o Adobe Campaign envia as mensagens começando na data de início e, em seguida, para mensagens que retornam somente um erro, tentativas regulares e configuráveis são executadas até que o limite de validade seja atingido.

Você também poderá optar por especificar datas. Para fazer isso, selecione **Explicitly set validity dates**. Nesse caso, as datas de delivery e limite de validade também permitem especificar o tempo. O tempo atual é usado por padrão, mas você poderá modificar isso diretamente no campo de entrada.

**Limite da validade dos recursos** é usada para recursos carregados, principalmente para mirror page e imagens. Os recursos desta página são válidos por um tempo limitado (para economizar espaço em disco).

![](assets/delivery-settings-2.png)


Saiba mais sobre o período de validade do delivery em [Documentação do Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html#validity-period){target="_blank"}.

### Gerenciamento de mirror page {#mirror}

A mirror page é uma página HTML acessível online através de um navegador da Web. Seu conteúdo é idêntico ao email. Por padrão, a mirror page é gerada se o link for inserido no conteúdo do email.

Além do modo padrão, as seguintes opções também estão disponíveis:

* **[!UICONTROL Forçar a geração da mirror page]**: mesmo se nenhum link para a mirror page for inserido no delivery, ela será criada.
* **[!UICONTROL Do not generate the mirror page]**: nenhuma mirror page é gerada, mesmo se o link estiver presente no delivery.
* **[!UICONTROL Generates a mirror page accessible using only the message identifier]**: essa opção permite acessar o conteúdo da mirror page, com informações de personalização, na janela de log do delivery. Para fazer isso, após o fim do delivery, clique na guia **[!UICONTROL Delivery]** e selecione a linha do recipient cuja mirror page você deseja exibir. Clique no link **[!UICONTROL Display the mirror page for this message...]**.


### Rastreamento {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Período de validade"
>abstract="Essa opção define a duração para a qual o rastreamento é ativado nos URLs."

Os parâmetros de rastreamento são definidos na seção relacionada. As opções possíveis são:

**Limite de validade do rastreamento**: use esta opção para alterar a duração para a qual o rastreamento é ativado nos URLs.

**URL de substituição para URLs expirados**: use esta opção para inserir um URL para uma página da Web de fallback: é exibido assim que o rastreamento expira.

## Configurações de teste {#test-setttings}

Você pode definir os parâmetros de exclusão nesta seção. As opções disponíveis são:

* **Manter duplo** permite autorizar vários deliveries a recipients que atendem a vários critérios de definição do target.

* **Manter endereços incluir na lista de bloqueios** permite manter do target os perfis que não estão mais sendo direcionados pelo delivery, como após um cancelamento de subscrição (opt-out).

* **Manter endereços em quarentena** permite manter do target qualquer perfil que não responda.

Você também pode personalizar o nome dos emails de teste.

Use o **Manter o código de delivery da prova** para associar ao email de teste o mesmo código de delivery que o definido para o delivery com o qual ele está relacionado.

Por padrão, o assunto do email de teste é prefixado em &quot;PROOF #&quot;, onde # é o número do email de teste. É possível alterar esse prefixo no campo **Label prefix**.