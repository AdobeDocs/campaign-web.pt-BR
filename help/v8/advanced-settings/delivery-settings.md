---
audience: end-user
title: Definir configurações de entrega
description: Saiba como definir as configurações de entrega no Campaign Web
feature: Email, Push, SMS, Direct Mail, Cross Channel Orchestration
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '2420'
ht-degree: 55%

---


# Definir configurações de entrega {#del-settings}

As configurações de entrega são **parâmetros técnicos de entrega** que são definidas no template do delivery. Eles podem ser sobrecarregados para cada delivery. Essas configurações estão disponíveis no **Configurações** botão disponível ao editar um delivery ou um template do delivery.

>[!CAUTION]
>
>Essas configurações estão descritas somente para suas informações. Algumas delas dependem de sua configuração e permissões. Elas não devem ser modificadas nesta versão do produto.

## Configurações de tipologia {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Tipologia"
>abstract="As regras de tipologia permitem que os profissionais de marketing padronizem práticas comerciais em todas as entregas. Uma tipologia é uma coleção de regras de tipologia que permitem controlar, filtrar e priorizar o envio de entregas. Os perfis que correspondem aos critérios em uma regra de tipologia são excluídos dos públicos-alvo da entrega na fase de preparação. As tipologias e regras de tipologia são criadas no Console do cliente do Campaign."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_typology"
>title="Configurações de tipologia para a entrega"
>abstract="As regras de tipologia permitem que os profissionais de marketing padronizem práticas comerciais em todas as entregas. Uma tipologia é uma coleção de regras de tipologia que permitem controlar, filtrar e priorizar o envio de entregas. Os perfis que correspondem aos critérios em uma regra de tipologia são excluídos dos públicos-alvo da entrega na fase de preparação. As tipologias e regras de tipologia são criadas no Console do cliente do Campaign."

Tipologias são conjuntos de **regras de tipologia** que são executados durante a fase de preparação para aplicar facilmente várias regras de filtragem a uma entrega de uma vez. Elas permitem que os profissionais de marketing padronizem práticas comerciais em todas as entregas, pois possibilitam controlar, filtrar e priorizar o envio de entregas.

Ao associar uma tipologia a uma mensagem ou a um template de mensagem, as regras de tipologia incluídas na tipologia são executadas para verificar a validade do delivery durante a preparação da mensagem. Os perfis que correspondem aos critérios em uma regra de tipologia são excluídos dos públicos-alvo do delivery.

As tipologias permitem que você garanta que seus deliveries sempre contenham determinados elementos (como um link de unsubscription ou uma linha de assunto) ou regras de filtragem para excluir grupos do target pretendido (como unsubscribers, concorrentes ou clientes não fidelizados).

![](assets/delivery-settings-typology.png){zoomable=&quot;yes&quot;}

>[!NOTE]
>
>As tipologias e regras de tipologia são criadas no console do cliente do Campaign. Saiba mais sobre regras de pressão e como configurar o gerenciamento de fadiga no [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-typologies.html?lang=pt-BR){target="_blank"}.

### Parâmetros de pressão {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_pressure_parameters"
>title="Parâmetros de pressão da entrega"
>abstract="Os pesos das entregas permitem identificar entregas de alta prioridade dentro da estrutura do gerenciamento de fadiga. As mensagens com o peso mais alto têm prioridade."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_weight"
>title="Peso da entrega"
>abstract="Os pesos das entregas permitem identificar entregas de alta prioridade dentro da estrutura do gerenciamento de pressão. As mensagens com o peso mais alto têm prioridade."

Nesta seção, os parâmetros de pressão permitem definir um **limite** para configurar regras de gerenciamento de fadiga, que é o número máximo de mensagens que podem ser enviadas para um perfil em um determinado período.

Depois que esse limite for atingido, não poderá ocorrer mais entregas até o final do período considerado. Esse processo permite excluir automaticamente um perfil de uma entrega, caso uma mensagem exceder o limite definido, evitando assim um excesso de solicitações.

Os valores do limite podem ser constantes ou variáveis. Isso significa que, para um determinado período, os limites podem variar de um perfil para o outro, ou até mesmo para o mesmo perfil.

No campo **[!UICONTROL Tipo de peso]**, três opções estão disponíveis:

* **[!UICONTROL Constante]**
* **[!UICONTROL Depende do destinatário]**
* **[!UICONTROL Definido em cada regra]**

Use o campo **[!UICONTROL Peso da entrega]** para definir a prioridade de entrega. Cada entrega tem um peso que representa seu nível de prioridade. Por padrão, o peso de uma entrega é definido como 5. As regras de pressão permitem definir o peso das entregas às quais são aplicadas. Os pesos podem ser definidos ou calculados por meio de uma fórmula para se adequar aos destinatários. Por exemplo, você pode definir o peso de uma entrega com base nos interesses do destinatário.

Use o **[!UICONTROL Modo de entrega]** para selecionar o modo de avaliação de target.

Três modos estão disponíveis:

* **[!UICONTROL Estimativa do público-alvo e personalização de mensagens]**
* **[!UICONTROL Estimativa e aprovação do público-alvo provisório]**
* **[!UICONTROL Avaliação de público-alvo]**

>[!NOTE]
>
>O gerenciamento de fadiga e as regras de pressão são configurados no console do cliente do Campaign. Saiba mais em [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=pt-BR){target="_blank"}.

### Configurações de capacidade {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_capacity_settings"
>title="Configurações de capacidade da entrega"
>abstract="Antes de enviar mensagens, use regras de capacidade para garantir que sua organização possa processar a entrega, as mensagens de entrada que a entrega pode gerar e o número de chamadas a serem feitas para entrar em contato com assinantes, por exemplo. As regras de capacidade são definidas no Console do Adobe Campaign v8. Nesta tela, selecione uma regra associada ao canal."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_recipient_importance"
>title="Importância do destinatário"
>abstract="A importância do recipient é uma fórmula usada para determinar quais perfis são mantidos quando as regras de tipologia de capacidade são excedidas."

Nesta seção, você pode selecionar uma regra de capacidade definida no console do Adobe Campaign v8. Essa regra está associada ao canal.

A variável **[!UICONTROL Importância do destinatário]** field é uma fórmula usada para determinar quais perfis são mantidos quando as regras de tipologia de capacidade são excedidas.

>[!NOTE]
>
>As regras de tipologia são configuradas no console do cliente do Campaign. Saiba mais em [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html?lang=pt-BR){target="_blank"}.

## Configurações de público-alvo {#audience}

>[!CONTEXTUALHELP]
>id="acw_email_settings_audience"
>title="Configurações do público-alvo da entrega"
>abstract="Selecione um **target mapping** entre os disponíveis. Os target mappings são definidos no console do Adobe Campaign v8. Também é possível definir os parâmetros de exclusão da entrega."

Nesta seção, você pode selecionar uma **mapeamento de público-alvo** entre aquelas disponíveis. Os target mappings são definidos no console do Adobe Campaign v8. O target mapping é o tipo de dados que uma operação está tratando. Ele permite definir a população direcionada: recipients, beneficiários de contrato, operadores, assinantes etc. [Saiba mais sobre target mappings](../audience/targeting-dimensions.md).

No **[!UICONTROL Exclusão]** , você pode optar por excluir os perfis que não desejam mais ser contatados ou que estão em quarentena. [Saiba mais](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html){target="_blank"}

## Entrega {#delivery}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery"
>title="Configurações da entrega"
>abstract="Os parâmetros de entrega são configurações técnicas que se aplicam à sua entrega. Você pode alterar os modos de entrega e rotina, ativar a cópia oculta (CCO) de email, enviar por meio de ondas, bem como escolher o formato das mensagens de email enviadas. Essas opções são restritas apenas a usuários especialistas."

**[!UICONTROL Entrega]** parâmetros são configurações técnicas que se aplicam ao seu delivery.

![](assets/delivery-settings-delivery.png){zoomable=&quot;yes&quot;}

O sistema integrado de **[!UICONTROL Roteamento]** a conta externa de é fornecida por padrão. Ela contém os parâmetros técnicos que permitem ao aplicativo enviar deliveries.

Você pode definir a variável **[!UICONTROL Enviando]** abaixo.

* **[!UICONTROL Prioridade de entrega]**: use essa opção para alterar a ordem de envio dos deliveries, definindo o nível de prioridade (normal, alto ou baixo).

* **[!UICONTROL Quantidade do lote de mensagens]**: use essa opção para definir o número de mensagens agrupadas no mesmo pacote do delivery XML. Se o parâmetro for definido como 0, as mensagens serão automaticamente agrupadas. O tamanho do pacote é definido pelo cálculo `<delivery size>/1024`, com no mínimo 8 e no máximo 256 mensagens por pacote.

  >[!IMPORTANT]
  >
  >Quando a entrega é criada duplicando uma existente, esse parâmetro é redefinido.

* **[!UICONTROL Testar entrega SMTP]** (canal de email): essa opção é usada para testar o envio via SMTP. O email é processado até a conexão com o servidor SMTP, mas não é enviado: para cada recipient do email, o Campaign se conecta ao servidor do provedor SMTP, executa o comando SMTP RCPT TO e fecha a conexão antes do comando SMTP DATA.

* **[!UICONTROL Email Cco]** (canal de email): essa opção é usada para armazenar emails em um sistema externo por meio do CCO simplesmente adicionando um endereço de email de CCO ao target da sua mensagem. Saiba mais em [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/emails/email-bcc.html){target="_blank"}.

No **[!UICONTROL Definição da onda]** , selecione a **[!UICONTROL Enviar usando várias ondas]** opção para aumentar progressivamente o volume enviado usando ondas. Esse aumento evitará que sua mensagem seja marcada como spam ou pode ser usado quando você quiser restringir o número de mensagens diárias. Ao usar ondas, você pode dividir as entregas em vários lotes, em vez de enviar grandes volumes de mensagens ao mesmo tempo. [Saiba mais](send-using-waves.md)

Para emails, você também pode alterar a variável **[!UICONTROL Formatos de email]** das mensagens enviadas conforme detalhado abaixo.

* **[!UICONTROL Usar preferências do recipient]** (modo padrão): o formato do email é definido de acordo com os dados armazenados no perfil do recipient. Se um recipient desejar receber emails em um determinado formato, esse será o formato enviado. Se o campo não estiver preenchido, um email multipart-alternative será enviado (veja abaixo).

* **[!UICONTROL Permitir que o cliente de correio do recipient escolha o formato mais apropriado]**: O email contém ambos os formatos: texto e HTML. O formato exibido no recebimento depende da configuração do software de email do destinatário (multipart-alternative).

  >[!IMPORTANT]
  >
  >Essa opção inclui ambas as versões do documento. Portanto, isso afeta a taxa de delivery, pois o tamanho do email é maior.

* **[!UICONTROL Enviar todas as mensagens no formato de texto]**: o email é enviado em formato de texto. O formato HTML não será enviado, mas usado somente para a mirror page quando o recipient clicar no email.

## Análise da web {#web-analytics}

>[!CONTEXTUALHELP]
>id="acw_email_settings_webanalytics"
>title="Configurações de análise da web da entrega"
>abstract="Selecione uma conta de análise da web. Essa conta é configurada no Console do cliente do Campaign. Também é possível definir as tags compartilhadas com a ferramenta de análise utilizada."

Nesta seção, você pode selecionar uma conta do Web Analytics. Essa conta é configurada no console do cliente do Campaign.

Também é possível definir as tags compartilhadas com a ferramenta de análise utilizada.

>[!NOTE]
>
>Os recursos do Web Analytics são configurados no console do Campaign Client. Saiba mais em [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html#external-account-ac){target="_blank"}.

## Tentativas {#retries}

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_retries"
>title="Número máximo de tentativas"
>abstract="Se uma mensagem falhar devido a um erro temporário, as tentativas serão executadas até o fim da duração da entrega."

<!--Currently not visible in UI > ??-->

As mensagens temporariamente não entregues devido a um erro Suave ou Ignorado estão sujeitas a uma repetição automática. Por padrão, cinco tentativas são agendadas para o primeiro dia do delivery com um intervalo mínimo de uma hora distribuída pelas 24 horas do dia.

## Aprovação (canal de email) {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Modo de aprovação da entrega"
>abstract="Selecione o modo de aprovação. Se os avisos forem gerados durante a preparação da entrega, você pode configurar a entrega para definir se ela ainda deverá ou não ser executada."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_approval"
>title="Modo de aprovação das entregas"
>abstract="Selecione o modo de aprovação para entregas com base neste modelo. Se os avisos forem gerados durante a preparação da entrega, você pode configurar a entrega para definir se ela ainda deverá ou não ser executada."

Se os avisos forem gerados durante uma preparação de delivery de email, você poderá configurar o delivery para definir se ele ainda deverá ou não ser executado. Por padrão, o usuário deverá confirmar o envio de emails no final da fase de análise: isso é **manual** validação.

Você pode selecionar outro modo de aprovação no campo apropriado. Os modos disponíveis são:

* **[!UICONTROL Manual]**: no final da fase de análise, o usuário deverá confirmar a entrega para começar a enviar.
* **[!UICONTROL Semiautomático]**: o envio começa automaticamente se a fase de análise não gerar mensagens de advertência.
* **[!UICONTROL Automático]**: o envio começa automaticamente no fim da fase de análise, independentemente do resultado.

## Validade {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_validity"
>title="Validade das configurações"
>abstract="O campo **Delivery duration** permite inserir o limite de novas tentativas de entrega globais. Isso significa que o Adobe Campaign envia as mensagens começando na data de início e, em seguida, para mensagens que retornam somente um erro, tentativas regulares e configuráveis são executadas até que o limite de validade seja atingido.<br>O campo **Limite da validade dos recursos** é usado para recursos enviados por upload, como mirror page ou imagens. Quando o limite for atingido, os recursos não estarão mais disponíveis."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_resources_validity"
>title="Limite da validade de recursos"
>abstract="O campo **Limite da validade dos recursos** é usado para recursos enviados por upload, como a mirror page ou imagens. Esses recursos são válidos por um tempo limitado: quando o limite é atingido, os recursos não estarão mais disponíveis."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_duration"
>title="Duração da entrega"
>abstract="O campo **Delivery duration** permite inserir o limite de novas tentativas de entrega globais. Isso significa que o Adobe Campaign envia as mensagens começando na data de início e, em seguida, para mensagens que retornam somente um erro, tentativas regulares e configuráveis são executadas até que o limite de validade seja atingido."

<!--
>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Resources validity limit"
>abstract="The Validity limit field is used for uploaded resources, such as the mirror page or images. These resources are valid for a limited time: once the limit is reached, resources are no longer available."
-->

### Período de validade {#validity-period}

O campo **[!UICONTROL Delivery duration]** permite inserir o limite de novas tentativas de entrega globais. Isso significa que o Adobe Campaign envia as mensagens começando na data de início e, em seguida, para mensagens que retornam somente um erro, tentativas regulares e configuráveis são executadas até que o limite de validade seja atingido.

Você também poderá optar por especificar datas. Para fazer isso, selecione **[!UICONTROL Explicitly set validity dates]**. Nesse caso, as datas de entrega e limite de validade também permitem especificar o tempo. O tempo atual é usado por padrão, mas você poderá modificar isso diretamente no campo de entrada.

**[!UICONTROL Limite da validade de recursos]** é usado para recursos dos quais foram feitos upload, principalmente para mirror pages e imagens. Os recursos dessa página são válidos por um tempo limitado (para economizar espaço em disco). Após esse limite, esses recursos não estarão mais disponíveis.

![](assets/delivery-settings-validity.png){zoomable=&quot;yes&quot;}

<!--Change screenshot to be consistent with prod > not sure which version is correct-->

Saiba mais sobre o período de validade do delivery em [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=pt-BR#validity-period){target="_blank"}.

### Gerenciamento de mirror page (canal de email) {#mirror}

A mirror page é uma página HTML acessível online através de um navegador da Web. Seu conteúdo é idêntico ao email. Por padrão, a mirror page é gerada se o link for inserido no conteúdo do email.

Além do modo padrão, as seguintes opções também estão disponíveis:

* **[!UICONTROL Forçar a geração da mirror page]**: use esse modo para gerar a mirror page mesmo se nenhum link para a mirror page for inserido no email.
* **[!UICONTROL Não gerar a mirror page]**: use esse modo para evitar gerar uma mirror page, mesmo se o link estiver presente no email.
* **[!UICONTROL Gera uma mirror page acessível somente por meio do identificador de mensagem]**: quando o link da mirror page não estiver presente no conteúdo do email, use essa opção para habilitar o acesso ao conteúdo da mirror page, na janela de log do delivery, no console do cliente.

### Rastreamento {#tracking}

<!--
>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Validity period"
>abstract="This option defines the duration for which the tracking is activated on the URLs."
-->

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_tracking_validity"
>title="Período de validade"
>abstract="O período de validade define a duração para a qual o rastreamento estará ativado nos URLs da mensagem."

**[!UICONTROL Rastreamento]** Os parâmetros do são definidos na seção relacionada. As opções possíveis são:

* **[!UICONTROL Limite da validade de rastreamento]**: use essa opção para alterar a duração da ativação do rastreamento nos URLs.
* **[!UICONTROL URL substituto para URLs expirados]**: use essa opção para inserir um URL para uma página da Web de fallback: ele é exibido depois que o rastreamento expira.

## Configurações de prova {#test-setttings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_testsettings"
>title="Definir as configurações de prova para a entrega"
>abstract="Selecione os parâmetros de exclusão e personalize o rótulo das provas."

<!--Test to be replaced with Proof everywhere - currently not consistent within UI > changed to Proof to reflect UI here but not consistent in documentation either-->

Você pode definir os parâmetros de exclusão nesta seção. As opções disponíveis são:

* **[!UICONTROL Manter duplicatas]** permite autorizar vários deliveries a perfis que atendem a vários critérios de definição do target.
* **[!UICONTROL Manter endereços incluídos na lista de bloqueios]** permite manter do público-alvo os perfis que não estão mais sendo direcionados para entrega, como após um cancelamento de subscrição (opt-out).
* **[!UICONTROL Manter endereços na quarentena]** permite excluir do público-alvo qualquer perfil com endereço que não responda.

Você também pode personalizar o rótulo das provas:

* Use o **[!UICONTROL Manter o código de entrega para a prova]** para associar à prova o mesmo código de delivery que o definido para o delivery com o qual ele está relacionado.
* Por padrão, o assunto da prova tem o prefixo &#39;PROOF #&#39;, onde # é o número da prova. É possível alterar esse prefixo no campo **[!UICONTROL Rotular prefixo]**.
