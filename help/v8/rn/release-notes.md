---
title: Notas de versão da interface do Campaign Web v8
description: Conheça os novos recursos que acompanham a versão mais recente da interface do Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 127c65a466c41e1aba8408aa9cf41c2d89c93801
workflow-type: ht
source-wordcount: '900'
ht-degree: 100%

---

# Notas de versão {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de versão"
>abstract="As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, as notas de versão do Campaign são atualizadas várias vezes por mês, com os recursos, melhorias e correções mais recentes. Recomendamos que você as verifique regularmente."

As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, essas notas de versão são atualizadas várias vezes por mês. Verifique-as regularmente.

As alterações e melhorias disponíveis em versões anteriores estão listadas nas páginas de [2024](release-notes-24.md) e [2025](release-notes-25.md).

## Versão de julho de 2025 {#25-7-release}

### Novos recursos {#25-7-features}

Os seguintes recursos estão disponíveis a partir da versão de julho.

<!--table>
<thead>
<tr>
<th><strong>Multilingual email and SMS</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now send multiple email and SMS deliveries in different languages in Adobe Campaign Web UI. The multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen.
</p>
<p>For Multilingual email, your server must be upgraded to 8.8.1 minimum. Refer to the Client Console <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html" target="_blank">release notes</a>.
<p>For more information, refer to the <a href="../email/edit-content.md#multilingual-delivery">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Custom channel for API deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now, directly from Adobe Campaign Web UI, orchestrate and execute deliveries based on custom API channels. These deliveries can be standalone or part of a workflow. The configuration of the custom API channel is performed in the console.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<table>
<thead>
<tr>
<th><strong>Compatibilidade com CSS personalizado no designer de email</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ao criar emails, agora é possível adicionar o seu próprio CSS personalizado diretamente no designer de email. Esse recurso permite aplicar estilos avançados e específicos para obter mais flexibilidade e controle sobre a aparência do conteúdo.</p>
<p>Para obter mais informações, consulte a <a href="../email/custom-css.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Marcas</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Agora, você pode criar e personalizar as suas próprias marcas para definir claramente a sua identidade visual e verbal nas comunicações. Com a pontuação de alinhamento à marca, você pode receber feedback em tempo real sobre a conformidade do seu conteúdo em relação ao tom, ao estilo e às diretrizes da sua marca, o que ajuda a manter o alinhamento à marca em todas as mensagens enviadas.
</p>
<p>Para obter mais informações, consulte a <a href="../content/brands.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Alerta de entrega</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>O recurso Alerta de entrega é um sistema de gerenciamento de alertas que permite que um grupo de usuários receba automaticamente notificações sobre a execução de suas entregas.</p>
<p>Para obter mais informações, consulte a <a href="../msg/delivery-alerting.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>Landing pages improvements</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The following improvements to landing pages are now available:</p>
<ul>
    <li>You can now reference a default subscription/unsubscription landing page when configuring a service. When designing an email, if you define a link to that landing page, users submitting the landing page form are automatically subscribed to or unsubscribed from this service. <a href="../audience/manage-services.md#create-service">Read more</a></li>
    <li>A new option in the landing page configuration allows anonymous visitors to access the landing page. If you unselect this option, only identified users can access and submit the form. <a href="../landing-pages/create-lp.md#create-landing-page">Read more</a></li>
    <li>A new option in the landing page configuration allows to store additional internal data when the landing page is being submitted. <a href="../landing-pages/create-lp.md#create-landing-page">Read more</a></li>
    <li>A new option enables to use a landing page for several services, making it dynamic. When adding a link to an email, if you select a dynamic landing page, you can select any service. If you select a landing page that has a specific service associated, this service will be automatically used (you cannot select another one). <a href="../landing-pages/create-lp.md#define-actions-on-form-submission">Read more</a></li>
    <li>Conditional content is now supported in landing pages. <a href="../landing-pages/lp-content.md">Read more</a></li>
    <li>You can link a landing page to a service, and send a confirmation message when users validate it. <a href="../landing-pages/lp-content.md#lp-message">Read more</a></li>
    <li>You can add captcha to protect your landing page from spam and abuse caused by bots. This is non-intrusive for your customers since it does not require any interaction from them and is based on interactions with your site. <a href="../landing-pages/create-lp.md#captcha">Read more</a></li>
</ul>
</td>
</tr>
</tbody>
</table-->


<table>
<thead>
<tr>
<th><strong>Geração de relatórios dinâmica</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Agora é possível acessar o recurso Relatórios dinâmicos, que permite gerar relatórios totalmente personalizáveis e em tempo real para medir o impacto das suas atividades de marketing. Eles adicionam acesso aos dados do perfil, permitindo análises demográficas por dimensões do perfil, como gênero, cidade e idade, além de dados funcionais de campanhas de email, como aberturas e cliques. Os relatórios dinâmicos também estão disponíveis para entregas de email e mensagens transacionais multilíngues.</p>
<p>Este recurso só está disponível sob demanda. Para obter acesso, entre em contato com o(a) representante da Adobe. O seu servidor precisa ser atualizado para a versão 8.8.1, no mínimo. Consulte as <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=pt-BR" target="_blank">notas de versão</a> do Console do cliente.
<p>Para obter mais informações, consulte a <a href="../reporting/dynamic-reporting/get-started-reporting.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Identidade visual centralizada</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Agora, os seus administradores técnicos podem definir uma ou várias marcas para centralizar os parâmetros que afetam a identidade de uma marca. Isso inclui o logotipo da marca, o domínio do URL de acesso da página de destino ou as configurações de rastreamento de mensagens. Você pode criar essas marcas e vinculá-las a mensagens ou páginas de destino. Essa configuração é gerenciada nos modelos. As opções de identidade visual estão disponíveis para todos os canais, incluindo SMS e correspondência direta.</p>
<p>Este recurso está disponível somente sob demanda para novas implementações. Para obter acesso, entre em contato com o(a) representante da Adobe. O seu servidor precisa ser atualizado para a versão 8.8.1, no mínimo. Consulte as <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=pt-BR" target="_blank">notas de versão</a> do Console do cliente.
<p>Para obter mais informações, consulte a <a href="../administration/branding/branding-gs.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

Além dos recursos listados acima, esta versão também vem com um conjunto de funcionalidades disponíveis no Console do cliente:

* [Novo conector de envio de SMS](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=pt-BR) (ambientes FDA)
* [APIs REST](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=pt-BR) (sob demanda, ambientes FDA)

Consulte as [notas de versão](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=pt-BR){target="_blank"} do Console do cliente.

<!--

### Features previously in Limited Availability {#25-7-limited} 

>[!AVAILABILITY]
>
>To benefit from these updates, your server must be upgrated to 8.8.1 mininum. Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html){target="_blank"}.

Previously released in Limited Availability, the following capabilities are now available to all environments (General Availability):

* **Multilingual delivery creation** - You can now send multiple email deliveries in different languages in Adobe Campaign Web User Interface. The Multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen. [Read more](../email/edit-content.md#multilingual-delivery).


* **Visual fragments** - You can now create, use and archive content fragments. Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](https://experienceleague.adobe.com/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments.html){target="_blank"}

* **Delivery alerting** - The Delivery alerting feature is an alert management system that enables a group of users to automatically receive notifications containing information on the execution of their deliveries. [Read more](../msg/delivery-alerting.md)


* **Landing pages improvements** - The following improvements to landing pages are now available:

    * You can now reference a default subscription/unsubscription landing page when configuring a service. When designing an email, if you define a link to that landing page, users submitting the landing page form are automatically subscribed to or unsubscribed from this service. [Read more](../audience/manage-services.md#create-service)
    * A new option in the landing page configuration allows anonymous visitors to access the landing page. If you unselect this option, only identified users can access and submit the form. [Read more](../landing-pages/create-lp.md#create-landing-page)
    * A new option in the landing page configuration allows to store additional internal data when the landing page is being submitted. [Read more](../landing-pages/create-lp.md#create-landing-page)
    * A new option enables to use a landing page for several services, making it dynamic. When adding a link to an email, if you select a dynamic landing page, you can select any service. If you select a landing page that has a specific service associated, this service will be automatically used (you cannot select another one). [Read more](../landing-pages/create-lp.md#define-actions-on-form-submission)
    * Conditional content is now supported in landing pages. [Read more](../landing-pages/lp-content.md)
    * You can link a landing page to a service, and send a confirmation message when users validate it. [Learn more](../landing-pages/lp-content.md#lp-message)
    * You can add captcha to protect your landing page from spam and abuse caused by bots. This is non-intrusive for your customers since it does not require any interaction from them and is based on interactions with your site. [Learn more](../landing-pages/create-lp.md#captcha)

Previously released in Limited Availability, the following capabilities are now available **on demand**:

* **Dynamic Reporting** - You can now access Dynamic Reporting which provides fully customizable and real-time reports to measure the impact of your marketing activities. It adds access to profile data, enabling demographic analysis by profile dimensions such as gender, city and age in addition to functional email campaign data like opens and clicks. Dynamic reporting is also available for multilingual email deliveries and transactional messages. [Read more](../reporting/dynamic-reporting/get-started-reporting.md)

* **Centralized Branding** -  Your technical administrators can now define one or several brands to centralize the parameters that affect a brand's identity. This includes the brand logo, the domain of the landing pages' access URL, or message tracking settings. You can create these brands and link them to messages or landing pages. This configuration is managed in templates. Branding options are available for all channels, including SMS and Direct mail. [Read more](../administration/branding/branding-gs.md){target="_blank"}

    >[!NOTE]
    >
    >This feature is only available for new implementations.

In addition to the features listed above, this release also comes with a set of functionalities available in the Client Console:

* [New SMS sending connector](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html) (FDA environments)
* [Rest APIs](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html) (on demand, FDA environments)

Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html){target="_blank"}.

-->

### Melhorias {#25-7-improvements}

* Agora é possível calcular o público-alvo diretamente em cada condição e grupo no construtor de regras. Clique no número resultante para visualizar a lista detalhada de registros. [Saiba mais](../query/build-query.md#validate-query)

* Agora é possível editar ou excluir um filtro predefinido diretamente do construtor de regras. [Saiba mais](../get-started/predefined-filters.md#manage-predefined-filter)

* Ao configurar uma entrega de SMS, a seção **SMS** agora concede acesso aos **Parâmetros de SMPP opcionais (TLV)**. Esse parâmetro é igual ao do console do cliente. [Saiba mais](../advanced-settings/delivery-settings.md#sms-tab)

* Agora é possível habilitar notificações em segundo plano no iOS usando a nova opção **Conteúdo disponível**, encontrada na seção **Configurações avançadas** da tela de edição de conteúdo do iOS. Isso adiciona o sinalizador `content-available:1` no conteúdo `aps`. Saiba mais [nesta página](../push/content-push.md). Confira também [esta página](../push/rich-push-ios.md)

* As seguintes melhorias agora estão disponíveis na página de destino:

   * Agora você pode fazer referência a uma página de destino de assinatura/cancelamento de assinatura padrão ao configurar um serviço. Ao criar um email, se você definir um link para essa página de destino, os usuários que enviarem o formulário da página de destino automaticamente assinarão ou cancelarão a assinatura desse serviço. [Leia mais](../audience/manage-services.md#create-service)
   * Uma nova opção na configuração da página de destino permite que visitantes anônimos acessem-na. Se você desmarcar esta opção, apenas usuários identificados poderão acessar e enviar o formulário. [Leia mais](../landing-pages/create-lp.md#create-landing-page)
   * Uma nova opção na configuração da página de destino permite armazenar dados internos adicionais quando a página de destino está sendo enviada. [Leia mais](../landing-pages/create-lp.md#create-landing-page)
   * Uma nova opção permite utilizar uma página de destino para diversos serviços, tornando-a dinâmica. Ao adicionar um link a um email, se você selecionar uma página de destino dinâmica, poderá selecionar qualquer serviço. Se você selecionar uma página de destino que tenha um serviço específico associado, esse serviço será utilizado automaticamente (não será possível selecionar outro). [Leia mais](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * O conteúdo condicional agora é compatível com páginas de destino. [Leia mais](../landing-pages/lp-content.md)
   * É possível vincular uma página de destino a um serviço e enviar uma mensagem de confirmação quando os usuários a validarem. [Saiba mais](../landing-pages/lp-content.md#lp-message)
   * É possível adicionar captcha para proteger a página de destino contra spam e abusos de bots. Esse mecanismo não é intrusivo para os clientes, pois não requer nenhuma interação deles e se baseia em interações com seu site. [Saiba mais](../landing-pages/create-lp.md#captcha)
