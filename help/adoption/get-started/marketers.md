---
title: Introdução ao Adobe Campaign v8 para profissionais de marketing
description: Descubra a principal funcionalidade do Campaign v8. Ele é para profissionais de marketing que migram do Campaign Standard para o Campaign v8.
role: User
level: Beginner, Experienced
exl-id: 514da15d-325b-4d28-9a58-50c1ae2e4925
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '2453'
ht-degree: 19%

---

# Introdução para profissionais de marketing {#acs-gs-marketers}

Este guia fornece uma visão geral das principais funcionalidades do Campaign v8 para profissionais de marketing que estão fazendo a transição do Campaign Standard para o Campaign v8.

Você pode acessar o Adobe Campaign v8 por meio do console do cliente ou da interface da Web. A interface da Web permite criar, gerenciar e executar as principais ações de marketing. A nova interface do Adobe Campaign Web oferece uma experiência de usuário moderna e intuitiva para simplificar o design e a entrega da campanha de marketing. [Saiba mais](../../v8/get-started/user-interface.md).

Com a migração, todos os seus dados do Campaign Standard são importados para o Campaign v8, garantindo uma transição tranquila com o mínimo de interrupção nas operações em andamento.

Você pode continuar a usar suas credenciais existentes para fazer logon e se conectar à nova instância do Adobe Campaign v8. Depois de conectado, você pode encontrar todos os perfis e workflows que estão sendo migrados, permitindo que continue trabalhando nas campanhas.

A principal diferença está na interface do usuário. Abaixo, uma comparação do mesmo workflow nas 2 interfaces:

![](assets/transition_workflow.png){zoomable="yes"}


>[!NOTE]
> As versões da interface do usuário da Web do Adobe Campaign operam em um modelo de entrega contínua, que permite uma abordagem mais escalável e em fases para a implantação de recursos. Verifique regularmente as [Notas de versão](../../v8/rn/release-notes.md) para obter as atualizações mais recentes.

## Conheça a interface da Web do Campaign {#acs-gs-marketers-ui}

No vídeo abaixo, aprenda a acessar e navegar na interface da Web do Campaign e personalizar as listas de inventário.

>[!VIDEO](https://video.tv.adobe.com/v/3427278?quality=12&learn=on){transcript=true}

Para obter mais detalhes, consulte a documentação abaixo:

1. [Conheça a interface da Web do Campaign](../../v8/get-started/user-interface.md)

1. [Procurar e filtrar listas](../../v8/get-started/list-filters.md)


## Criar e gerenciar perfis e públicos {#acs-gs-marketers-profiles-and-audiences}

Os conceitos gerais para criar e gerenciar perfis e públicos no Campaign v8 são os mesmos do Adobe Campaign Standard. Saiba como começar com perfis e públicos-alvo [nesta seção](../../v8/audience/gs-audiences-recipients.md).

Você pode encontrar abaixo alguns links úteis para começar.

### Gerenciar perfis {#acs-gs-marketers-profiles}

No Adobe Campaign, um perfil é um registro armazenado no banco de dados, que serve como um componente principal para criar públicos-alvo para deliveries e adicionar dados de personalização ao seu conteúdo.

1. Saiba como acessar, gerenciar e explorar perfis usando a interface da Web do Campaign neste vídeo:

   >[!VIDEO](https://video.tv.adobe.com/v/3427293?quality=12&learn=on){transcript=true}

   Saiba mais na documentação [Introdução aos perfis](../../v8/audience/about-recipients.md).

1. Saiba como [criar e gerenciar perfis de teste](../../v8/audience/test-profiles.md) no Campaign v8.

### Gerenciar públicos {#acs-gs-marketers-audiences}

Públicos são conjuntos de perfis que compartilham comportamentos e/ou características semelhantes. Essa coleção de pessoas pode ser gerada, selecionada ou carregada.  Depois de criados, os públicos-alvo podem ser usados como a população de público-alvo das suas entregas.

Saiba como criar e gerenciar públicos-alvo, como selecionar públicos-alvo para um delivery e definir grupos de controle neste vídeo:

>[!VIDEO](https://video.tv.adobe.com/v/3425861?quality=12&learn=on){transcript=true}

Consulte [Introdução aos públicos-alvo](../../v8/audience/manage-audience.md){target="_blank"} para obter mais informações.

Como no Campaign Standard, você pode adicionar um grupo de controle ao seu delivery. Você pode definir um grupo de controle para evitar o envio de mensagens para uma parte do público-alvo e comparar o comportamento após o delivery com o público-alvo principal. Essa opção ajuda a medir o impacto da campanha.
Saiba como [definir um grupo de controle](../../v8/audience/control-group.md){target="_blank"}.

>[!AVAILABILITY]
>
>* Todos os públicos-alvo criados por meio da atividade Campaign Standard Query são transformados em filtro predefinido no Campaign v8 durante a transição. O Campaign v8 também oferece suporte à atividade Query.
>
>* O público de leitura é transformado em uma atividade de Consulta com [filtro predefinido](../../v8/query/build-query.md)
>
>* O filtro predefinido só assume o valor mais recente após a migração de público para o Campaign v8.
>
>* Os públicos-alvo do tipo de arquivo no Campaign Standard são migrados como do tipo Lista sem dimensões.

### Gerenciar assinaturas {#acs-gs-marketers-sub}

É possível gerenciar e criar serviços, como boletins informativos, e verificar as assinaturas ou cancelamentos de assinaturas desses serviços. Globalmente, as principais etapas são as mesmas do Campaign Standard. Saiba mais nas páginas abaixo:

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/audiences/work-with-services/manage-services">
<img alt="Pouco frequente" src="assets/lp-list.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/audiences/work-with-services/manage-services"><strong>Criar serviços de assinatura</strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/audiences/work-with-services/manage-subscribers">
<img alt="Pouco frequente" src="assets/workflow-activities.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/audiences/work-with-services/manage-subscribers"><strong>Gerenciar assinantes<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/msg/send-to-subscribers">
<img alt="Validação" src="assets/workflow-create.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/msg/send-to-subscribers"><strong>Enviar mensagens aos assinantes de um serviço</strong></a>
</div>
<p>
</td>
</tr>
</table>

## Usar planos, programas e campanhas {#acs-gs-marketers-plans}

O Adobe Campaign v8 permite configurar a hierarquia de pastas para planos de marketing e programas. Os recursos de planos, programas e campanhas são semelhantes ao Campaign Standard e ao Campaign v8.

Saiba mais na [documentação de planos e programas](../../v8/administration/plans-programs.md).

Você pode encontrar abaixo links úteis para começar. As alterações que podem afetar a experiência do usuário são destacadas nas Notas de disponibilidade.


### Criar uma campanha {#acs-gs-marketers-campaign}

O Adobe Campaign permite orquestrar facilmente suas iniciativas de marketing direcionadas, usando o recurso integrado de gerenciamento de campanhas. Com a capacidade de definir um cronograma, é possível planejar a duração e o tempo de suas campanhas para se alinharem aos objetivos estratégicos e maximizar o engajamento do público-alvo.

![Fluxo de campanha](assets/campaign-flow.png)

Siga a documentação abaixo para saber mais sobre campanhas:

1. [Introdução às campanhas](../../v8/campaigns/gs-campaigns.md)
1. [Acesso e gerenciamento de suas campanhas](../../v8/campaigns/manage-campaigns.md)
1. [Criar sua primeira campanha](../../v8/campaigns/create-campaigns.md)


### Criar um fluxo de trabalho {#acs-gs-marketers-wf}

A interface do usuário do workflow foi totalmente reimaginada na interface do usuário da Web do Campaign para facilitar o uso, a configuração, a execução e a solução de problemas. Como você já experienciou no Campaign Standard, com workflows você pode orquestrar a gama completa de processos e tarefas, melhorar a velocidade e a escala de cada aspecto de suas campanhas de marketing, desde a criação de segmentos e preparação de mensagens até a entrega. Além disso, você pode sincronizar seus canais com uma interface única e fácil de usar para a orquestração de campanhas.

Entenda como os fluxos de trabalho funcionam e como criar um fluxo de trabalho de direcionamento neste vídeo:

>[!VIDEO](https://video.tv.adobe.com/v/3425873?quality=12&learn=on){transcript=true}

Obtenha mais detalhes com a [Documentação de fluxo de trabalho](../../v8/workflows/gs-workflows.md).

A interface de usuário da Web do Adobe Campaign apresenta um modelador de consultas em workflows que simplifica o processo de filtragem do banco de dados com base em vários critérios. [Saiba mais sobre o modelador de consultas](../../v8/query/query-modeler-overview.md)

Para entender a finalidade e a funcionalidade de cada atividade no seu fluxo de trabalho, explore as informações detalhadas disponíveis em [atividades do fluxo de trabalho](../../v8/workflows/activities/about-activities.md)

Maximize a eficiência do seu fluxo de trabalho revisando as [Medidas de proteção e limitações para fluxos de trabalho](../../v8/get-started/guardrails.md).

>[!AVAILABILITY]
>
>* O [histórico e os logs](../../v8/workflows/start-monitor-workflows.md#logs-tasks) de execução de fluxo de trabalho estão disponíveis no Adobe Campaign v8.
>
>* Os logs históricos de workflows executados na instância do Campaign Standard não são migrados para o Campaign v8.
>
>* As Unidades organizacionais são mapeadas de acordo com o conceito de pasta para mapear e garantir um controle de acesso semelhante.
>

## Criar e gerenciar deliveries {#acs-gs-marketers-deliveries}

Com a Interface do usuário da Web do Campaign, como profissional de marketing, você pode criar entregas independentes a partir do menu esquerdo **Entregas** ou criar entregas no contexto de um fluxo de trabalho, incluído ou não em uma campanha. As principais etapas estão alinhadas com sua experiência anterior no Campaign Standard. Saiba como criar uma entrega na seguinte seção: [Documentação de criação e gerenciamento da entrega](../../v8/msg/gs-deliveries.md).

Links úteis:

* **Modelos de entrega** - Para um processo de design acelerado e aprimorado, você pode criar modelos de entrega para reutilizar facilmente o conteúdo e as configurações personalizadas em suas campanhas. Essa funcionalidade permite padronizar a aparência criativa para agilizar a execução e a inicialização de campanhas. Saiba mais na página [Modelo de entrega](../../v8/msg/delivery-template.md).

* **Configurações de entrega** - As configurações de entrega são parâmetros técnicos de entrega definidos no modelo de entrega. Eles podem ser sobrecarregados para cada delivery. Essas configurações estão disponíveis no botão Configurações, disponível ao editar um delivery ou um template de delivery. Saiba mais na seção [Configurações de entrega](../../v8/advanced-settings/delivery-settings.md).

* **Conteúdo dinâmico** - Os recursos de conteúdo dinâmico da Web do Adobe Campaign permitem personalizar o conteúdo com base nas informações coletadas sobre os destinatários. Ao utilizar o conteúdo dinâmico, você garante que seus esforços de marketing sejam mais relevantes, evitando o anúncio de produtos ou serviços indesejados ou desnecessários. Saiba mais na seção [Conteúdo dinâmico](../../v8/personalization/gs-personalization.md).

* **Testes e provas** - Depois que o conteúdo da entrega for definido, você poderá usar perfis e perfis de teste para pré-visualizá-lo e testá-lo antes de enviar a mensagem. Essa etapa é essencial para garantir que seja precisa, mas também esteja livre de erros nas configurações de conteúdo e personalização. Consulte [Pré-visualização e teste](../../v8/preview-test/preview-test.md).

* **Agendando** - Você pode definir a data e a hora exata para enviar suas mensagens. Ao escolher o horário mais apropriado para sua mensagem de marketing, você pode maximizar as taxas de abertura.

   * Saiba como [agendar uma entrega independente](../../v8/msg/gs-deliveries.md#gs-schedule)
   * Saiba como [agendar uma entrega em um fluxo de trabalho](../../v8/monitor/schedule-sending.md#schedule-a-delivery-in-a-campaign-workflow)

* **Adicionar ofertas** - Você pode adicionar ofertas às suas entregas na interface de usuário da Web do Adobe Campaign. Essas ofertas estão disponíveis no menu Offers à esquerda, que permite acessar a lista de ofertas.  Saiba como [adicionar ofertas às suas mensagens](../../v8/msg/offers.md)

>[!AVAILABILITY]
>
>* Os deliveries no estado de rascunho ou concluído foram migrados.
>
>* Os deliveries que estão em um dos seguintes status foram migrados para o Adobe Campaign v8, mas devem ser preparados novamente: In transition / In progress / Cancelled / Retry in progress / Preparation error.
>
>* Os deliveries que estão em um dos seguintes status foram migrados como deliveries cancelados: Para Cancelados / Nova tentativa em andamento.
>
>* Os links de rastreamento, links de URL de mirror page, links de subscrição/cancelamento de subscrição funcionam como no Campaign Standard.
>
>Consulte também as seguintes seções: [Rastreamento e monitoramento](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/analytics/tracking){target="_blank"}, [Identidade visual](https://experienceleague.adobe.com/pt-br/docs/experience-cloud/campaign/branding/branding-gs){target="_blank"} no Adobe Campaign.

### Entrega por email {#acs-gs-marketers-email}

Saiba como criar uma entrega de email do zero, definir o público-alvo, criar o conteúdo, simular a pré-visualização e enviar uma prova neste vídeo:

>[!VIDEO](https://video.tv.adobe.com/v/3425866?quality=12&learn=on){transcript=true}

Saiba como criar seu primeiro email direcionado na [Criar sua primeira documentação de email](../../v8/email/create-email.md)

No Campaign v8, as etapas detalhadas para criar, testar e enviar um delivery de email são semelhantes ao Campaign Standard.

1. **Projetar e definir conteúdo**

   O Designer de email do Campaign v8 é semelhante ao disponível no Campaign Standard. Lembrando que o [editor de email herdado do Campaign Standard foi descontinuado](https://experienceleague.adobe.com/pt-br/docs/campaign-standard/using/release-notes/deprecated-features#deprecated-features){target="_blank"} há alguns anos. Você já deve ter feito a transição para o Campaign Email Designer para criar e personalizar seu conteúdo de email.

   Saiba como navegar no Designer de email. Saiba como estruturar e projetar um email do zero, personalizar e testar seu email no vídeo a seguir:

   >[!VIDEO](https://video.tv.adobe.com/v/3425867?quality=12&learn=on){transcript=true}

   O Designer de email permite criar emails atrativos e personalizados por meio de uma interface intuitiva de arrastar e soltar. Saiba mais na [documentação do Email Designer](../../v8/email/get-started-email-designer.md)

   Saiba como criar um email carregando o HTML, como torná-lo compatível com o Designer de email e como convertê-lo em um modelo neste vídeo:

   >[!VIDEO](https://video.tv.adobe.com/v/3427633?quality=12&learn=on){transcript=true}

   Um fragmento de conteúdo é um componente reutilizável que pode ser referenciado em uma ou mais mensagens. Saiba mais sobre [Fragmentos de conteúdo](../../v8/content/fragments.md) para simplificar a criação de sua entrega de email.

   Para um processo de design acelerado e aprimorado, é possível criar modelos independentes para reutilizar facilmente o conteúdo personalizado no Adobe Campaign. Consulte [Criar modelos de email](../../v8/content/create-email-templates.md)

1. **Visualizar e testar**

   Saiba como pré-visualizar o conteúdo e a personalização da mensagem de email, enviar deliveries de teste (provas) e verificar a renderização de email em clientes populares de desktop, móveis e baseados na Web, neste vídeo:

   >[!VIDEO](https://video.tv.adobe.com/v/3425862?quality=12&learn=on){transcript=true}

1. **Enviar email e verificar logs**

   Após definir o conteúdo, o público-alvo e o agendamento, você estará pronto para preparar o delivery de email. Saiba mais nas seguintes seções:

   * [Preparar e enviar um email](../../v8/monitor/prepare-send.md)
   * [Monitorar logs de entrega](../../v8/monitor/delivery-logs.md)


### Entrega por SMS {#acs-gs-marketers-sms}

As entregas de SMS fornecem uma maneira prática e eficiente de enviar mensagens de texto para os dispositivos móveis de clientes. Com esse recurso, é possível criar, personalizar e visualizar mensagens baseadas em texto para uma comunicação eficiente.

No Campaign v8, as etapas detalhadas para criar, testar e enviar um delivery de SMS são semelhantes ao Campaign Standard.


<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/msg/sms/create-sms">
<img alt="Lead" src="assets/create_sms.png">
</a>
<div><a href="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/msg/sms/create-sms"><strong>Criar uma entrega de SMS</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/msg/sms/content-sms">
<img alt="Pouco frequente" src="assets/design_sms.png">
</a>
<div>
<a href="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/msg/sms/content-sms"><strong>Criar uma entrega de SMS<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/msg/sms/send-sms">
<img alt="Validação" src="assets/send_sms.png">
</a>
<div>
<a href="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/msg/sms/send-sms"><strong>Pré-visualizar e enviar uma entrega de SMS</strong></a>
</div>
<p>
</td>
</tr></table>

### Notificações por push {#acs-gs-marketers-push}

As notificações por push são essenciais para se comunicar com usuários de aplicativos móveis, mesmo que não estejam usando ativamente seu aplicativo. Elas atendem a vários propósitos, como fornecer atualizações, orientar ações específicas e notificar sobre ofertas.

No Campaign v8, as etapas detalhadas para criar, testar e enviar um delivery de notificação por push são semelhantes ao Campaign Standard.


<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/msg/push/create-push">
<img alt="Lead" src="assets/push_create.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/msg/push/create-push"><strong>Criação de uma entrega por push</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/msg/push/content-push">
<img alt="Pouco frequente" src="assets/push_design.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/msg/push/content-push"><strong>Criar uma entrega por push<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/msg/push/send-push">
<img alt="Validação" src="assets/push_send.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/msg/push/send-push"><strong>Visualizar e enviar uma entrega por push</strong></a>
</div>
<p>
</tr></table>

>[!AVAILABILITY]
>
>* O Adobe Campaign v8 é compatível com o Android e o iOS Push Channel. Para a transição de fluxos de trabalho e entregas existentes usando o Canal por push, conecte-se com seu Gerente de transição do Adobe Campaign. Saiba mais sobre a [Configuração de canal](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/send/push/push-data-collection){target="_blank"}.
>
>* Observe que o SDK V4 para aplicativos móveis foi [descontinuado no Campaign Standard](https://experienceleague.adobe.com/pt-br/docs/campaign-standard/using/release-notes/deprecated-features#deprecated-features){target="_blank"} há alguns anos. Você já deve ter feito a transição para o Adobe Experience Platform SDK, que é o mesmo usado no Campaign v8.
> 

### Correspondência direta {#acs-gs-marketers-direct-mail}

A correspondência direta é um canal offline que permite produzir arquivos para entregar cartas personalizadas em massa aos clientes, como cartões-postais, panfletos ou catálogos. Ao criar uma entrega de correspondência direta, o Adobe Campaign gera automaticamente um arquivo de extração contendo todos os perfis direcionados e dados selecionados, como endereços postais e atributos de perfil.

No Campaign v8, as etapas detalhadas para criar, testar e enviar um delivery de correspondência direta são semelhantes ao Campaign Standard.


1. [Criar entrega de correspondência direta](../../v8/direct-mail/create-direct-mail.md)
1. [Definir o arquivo de extração](../../v8/direct-mail/content-direct-mail.md)
1. [Visualizar e enviar](../../v8/direct-mail/send-direct-mail.md)

### Canal no aplicativo {#acs-gs-marketers-in-app}

Observe que o canal No aplicativo não está disponível no Campaign v8. Se precisar enviar notificações no aplicativo, entre em contato com o representante da Adobe.

## Criar e gerenciar landing pages {#acs-gs-marketers-lp}

A interface do usuário da Web do Adobe Campaign v8 vem com uma experiência de usuário recriada para landing pages. O Campaign permite criar, projetar e compartilhar landing pages. As páginas de destino permitem direcionar usuários para formulários online onde é possível atualizar dados, aceitar ou recusar o recebimento de comunicações ou assinar um serviço específico, como um informativo.

Como usuário do Campaign Standard que está fazendo a transição para o Campaign v8, suas páginas de aterrissagem existentes foram migradas para a interface do usuário da Web do Campaign. Você pode acessar a mesma variedade de recursos.

Saiba mais sobre landing pages nas seguintes seções:

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/landing-pages/create-lp">
<img alt="Lead" src="assets/lp-subscription.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/landing-pages/create-lp"><strong>Criar páginas de destino</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/landing-pages/lp-content">
<img alt="Validação" src="assets/lp-design.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/landing-pages/lp-content"><strong>Design de páginas de destino</strong></a>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/landing-pages/lp-templates">
<img alt="Validação" src="assets/lp-reporting.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/landing-pages/lp-templates"><strong>Trabalhar com modelos de página de aterrissagem</strong></a>
</div>
<p>
</td>
</tr></table>


## Relatórios {#acs-gs-marketers-reporting}

A Adobe Campaign fornece um conjunto de [ferramentas de relatório](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/analytics/reports/gs-reporting){target="_blank"}. Como administrador, você pode criar e configurar relatórios para compartilhar com outros usuários do Campaign.

O conjunto de ferramentas de relatórios do Adobe Campaign fornece insights valiosos sobre a eficácia de seus esforços de marketing, permitindo otimizar suas campanhas para obter o máximo impacto. Saiba mais na [documentação sobre relatórios](../../v8/reporting/gs-reports.md).

Além disso, alinhado à experiência do Adobe Campaign Standard, o Dynamic Reporting está disponível no Campaign v8 para seus deliveries de email. Ele fornece relatórios totalmente personalizáveis e em tempo real para medir o impacto de suas atividades de marketing. Eles adicionam acesso aos dados do perfil, permitindo análises demográficas por dimensões do perfil, como gênero, cidade e idade, além de dados funcionais de campanhas de email, como aberturas e cliques. Saiba mais na [documentação do Dynamic Reporting](https://experienceleague.adobe.com/pt-br/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"}

>[!AVAILABILITY]
>
>* [Relatórios dinâmicos](https://experienceleague.adobe.com/pt-br/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"} podem ser usados para relatórios de entregas de email, campanhas com entregas de email e mensagens transacionais. A análise demográfica por dimensão de Perfil também está disponível.
>
> * O [relatório da interface da Web do Adobe Campaign](../../v8/reporting/campaign-reports.md) também está disponível para todos os usuários na transição do Adobe Campaign Standard para o Adobe Campaign v8.

O Adobe Campaign oferece três relatórios diferentes:

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/campaign-report/campaign-reports">
<img alt="Validação" src="./assets/campaign_report.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/campaign-report/campaign-reports"><strong>Relatórios de campanha</strong></a>
</div>
<p>
<div>
<p>Forneça informações detalhadas sobre o desempenho, a eficácia e os resultados de seus deliveries individuais, fornecendo uma visão geral abrangente.</p>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/delivery-report/delivery-reports">
<img alt="Lead" src="assets/email_report.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/delivery-report/delivery-reports"><strong>Relatórios de entrega</strong>
</div>
<p>
<div>
<p>Ofereça uma análise completa do desempenho de cada delivery, por canal: taxas de sucesso, envolvimento do público-alvo e outras métricas essenciais. Por isso, eles permitem avaliar a eficácia geral e o impacto da campanha.</p>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/global-report/global-reports">
<img alt="Relatórios globais" src="assets/push_report.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/global-report/global-reports"><strong> Relatórios globais</strong></a>
</div>
<p>
<div>
<p>Ofereça um resumo geral consolidado das métricas de tráfego e engajamento para cada canal na instância do Campaign. Esses relatórios consistem em vários dispositivos, cada um oferecendo uma perspectiva distinta sobre sua campanha ou desempenho de entrega.</p>
</div>
<p>
</td>
</tr>
</table>
