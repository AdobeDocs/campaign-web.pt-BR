---
audience: end-user
title: Configurações avançadas
description: Documentação da Web do Campaign v8
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: 60bd1b795a44019929eae2267304e45b1fd570a9
workflow-type: tm+mt
source-wordcount: '1241'
ht-degree: 49%

---

# Configurações avançadas {#advanced-settings}

>[!NOTE]
>
>Esta documentação está em construção e é atualizada com frequência. A versão final desse conteúdo estará pronta em janeiro de 2023.

Essas configurações são **parâmetros técnicos do delivery** que são definidas no template de email. Se quiser modificar qualquer um deles para um delivery específico, continue com cautela.

## Configurações de delivery de email {#email-delivery-settings}

>[!NOTE]
>
> Modificar somente configurações, nenhuma nova criação é permitida. Sujeito a direitos de acesso.

## Tipologia {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Tipologia"
>abstract="A tipologia permite controlar, filtrar e monitorar o envio de deliveries."

Tipologias são conjuntos de **regras de tipologia**, que são executadas durante a fase de análise da mensagem. Elas possibilitam garantir que seus emails sempre contenham determinados elementos (como um link de cancelamento de assinatura ou uma linha de assunto) ou regras de filtragem para excluir grupos do público-alvo desejado (como clientes que não assinam, concorrentes ou clientes não fidelizados).

Ao associar uma tipologia a uma mensagem ou a um template de mensagem, as regras de tipologia incluídas na tipologia serão executadas para verificar a validade da mensagem.

### Parâmetros de pressão {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="Peso da entrega"
>abstract="Os pesos do delivery permitem identificar deliveries de alta prioridade dentro da estrutura do gerenciamento de pressão. As mensagens com o peso mais alto têm prioridade."

Nesta seção, os parâmetros de pressão permitem definir uma **limite**. Esse é o número máximo de mensagens que podem ser enviadas para um perfil em um determinado período. Depois que esse limite for atingido, não poderá ocorrer mais deliveries até o final do período considerado. Esse processo permite excluir automaticamente um perfil de um delivery, caso uma mensagem exceder o limite definido, evitando assim um excesso de solicitações.

Os valores do limite podem ser constantes ou variáveis. Isso significa que, para um determinado período, os limites podem variar de um perfil para o outro, ou até mesmo para o mesmo perfil.

No **Tipo de peso** , três opções estão disponíveis: (fórmula ausente, dependendo da opção..)

* **Constante**
* **Depende do recipient**
* **Definido em cada regra**

O **Peso do delivery** campo : Cada delivery tem um peso que representa seu nível de prioridade. Por padrão, o peso de um delivery é definido como 5. As regras de pressão permitem definir o peso dos deliveries aos quais serão aplicados.Os pesos podem ser definidos ou calculados por meio de uma fórmula para se adequar aos recipients. Por exemplo, você pode definir o peso de um delivery com base nos interesses do recipient.

O **Modo de entrega** campo.. ??

* **Estimativa do público-alvo e personalização de mensagens**
* **Estimativa e aprovação do público alvo provisório**
* **Avaliação de público alvo**

### Configurações de capacidade {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="Importância do destinatário"
>abstract="A importância do recipient é uma fórmula usada para determinar quais recipients são mantidos quando as regras de tipologia de capacidade são excedidas."

Nesta seção, você pode selecionar uma regra de capacidade definida no Console do Adobe Campaign v8. Essa regra está associada ao canal de email.

O **importância do destinatário** é uma fórmula usada para determinar quais recipients são mantidos quando as regras de tipologia de capacidade são excedidas.

## Público-alvo {#audience}

Nesta seção, você pode escolher uma **target mapping** definido no console do Adobe Campaign v8. A criação do target mapping é necessária no caso de usar uma tabela de recipients diferente da fornecida pelo Adobe Campaign.

## Entrega {#delivery}

**Roteamento** seleção: A conta externa de roteamento de email integrado é fornecida por padrão. Ela contém os parâmetros técnicos que permitem ao aplicativo enviar emails.

**Teste do delivery SMTP**: use essa opção para testar o envio via SMTP. A entrega é processada até a conexão com o servidor SMTP, mas não é enviada: para cada destinatário do delivery, o Campaign se conecta ao servidor do provedor SMTP, executa o comando SMTP RCPT TO e encerra a conexão antes do comando SMTP DATA.

**Email Cco**: use essa opção para armazenar emails em um sistema externo por meio do CCO simplesmente adicionando um endereço de email de CCO ao target da sua mensagem.

### Tentativas {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="Número máximo de tentativas"
>abstract="Se uma mensagem falhar devido a um erro temporário, novas tentativas serão executadas durante a duração do delivery."

As mensagens temporariamente não entregues devido a um erro Suave ou Ignorado estão sujeitas a uma repetição automática. Por padrão, cinco tentativas são agendadas para o primeiro dia do delivery, com um intervalo mínimo de uma hora distribuído pelas 24 horas do dia. Uma nova tentativa por dia é programada depois disso e até o prazo do delivery, que é definido na guia Validity .

## Aprovação {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Aprovação modo"
>abstract="Cada etapa de um delivery pode ser sujeita a aprovação para garantir o monitoramento e o controle totais dos vários processos."

**Manual**: no final da fase de análise, o usuário deverá confirmar o delivery para começar a enviar.

**Semiautomático**: O envio começa automaticamente se a fase de análise não gerar mensagens de aviso.

**Automatic**: o envio começa automaticamente no fim da fase de análise, independentemente do resultado.


## Validade {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="Duração da entrega"
>abstract="O campo Delivery duration permite inserir o limite de novas tentativas de delivery globais. Isso significa que o Adobe Campaign envia as mensagens começando na data de início e, em seguida, para mensagens que retornam somente um erro, tentativas regulares e configuráveis são executadas até que o limite de validade seja atingido."

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Limite da validade de recursos"
>abstract="O campo Validity limit é usado para recursos carregados, principalmente para a mirror page e imagens. Os recursos desta página são válidos por um tempo limitado."


O campo **Delivery duration** permite inserir o limite de novas tentativas de delivery globais. Isso significa que o Adobe Campaign envia as mensagens começando na data de início e, em seguida, para mensagens que retornam somente um erro, tentativas regulares e configuráveis são executadas até que o limite de validade seja atingido.

Você também poderá optar por especificar datas. Para fazer isso, selecione **Explicitly set validity dates**. Nesse caso, as datas de delivery e limite de validade também permitem especificar o tempo. O tempo atual é usado por padrão, mas você poderá modificar isso diretamente no campo de entrada.

**Limite da validade dos recursos** é usada para recursos carregados, principalmente para mirror page e imagens. Os recursos desta página são válidos por um tempo limitado (para economizar espaço em disco).

### Gerenciamento de mirror page {#mirror}

**Gerenciamento de mirror pages** contém quatro opções :

* **Gerar a mirror page se um link for exibido no conteúdo do email**: a mirror page é gerada se o link for inserido no conteúdo do email.
* **Forçar a geração da mirror page**: mesmo se nenhum link para a mirror page for inserido nas mensagens, a mirror page será criada.
* **Não gerar a mirror page**: nenhuma mirror page é gerada, mesmo se o link estiver presente nas mensagens.
* **Generates a mirror page accessible using only the message identifier**: essa opção permite acessar o conteúdo da mirror page, com informações de personalização, na janela de log do delivery.


### Rastreamento {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Período de validade"
>abstract="Essa opção define a duração para a qual o rastreamento será ativado nos URLs."

**Limite de validade do rastreamento**: Essa opção define a duração para a qual o rastreamento será ativado nos URLs.

**URL de substituição para URLs expirados**: use esta opção para inserir um URL para uma página da Web de fallback: é exibido assim que o rastreamento expira.


## Configurações de teste {#test-setttings}

**Manter duplo** permite autorizar vários deliveries a recipients que atendem a vários critérios de definição do target.

**Manter endereços incluir na lista de bloqueios** permite manter do target os perfis que não estão mais sendo direcionados pelo delivery, como após um cancelamento de subscrição (opt-out).

**Manter endereços em quarentena** permite manter do target qualquer perfil que não responda.

**Manter o código de delivery da prova** permite que você forneça o mesmo código de delivery que o definido para o delivery com o qual ele está relacionado.

Por padrão, o assunto da prova tem o prefixo &quot;Proof #&quot;, onde # é o número da prova. É possível alterar esse prefixo no campo **Label prefix**.