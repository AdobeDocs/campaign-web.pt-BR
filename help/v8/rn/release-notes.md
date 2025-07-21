---
title: Notas de versão da interface do Campaign Web v8
description: Conheça os novos recursos que acompanham a versão mais recente da interface do Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 6f09df9a4686a56b56e837536db11a71ba5158f4
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 98%

---

# Notas de versão {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de versão"
>abstract="As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, as notas de versão do Campaign são atualizadas várias vezes por mês, com os recursos, melhorias e correções mais recentes. Recomendamos que você as verifique regularmente."

As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, essas notas de versão são atualizadas várias vezes por mês. Verifique-as regularmente.

As alterações e melhorias disponíveis em versões anteriores estão listadas nas versões de [2024](release-notes-24.md) e [2025](release-notes-25.md).

## Atualizações de julho de 2025 {#25-7-updates}

>[!AVAILABILITY]
>
>Para se beneficiar dessas atualizações, o servidor deve ser atualizado para, no mínimo, a versão 8.8.1. Consulte as [notas de versão](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=pt-BR){target="_blank"} do Console do cliente.

Anteriormente lançados em Disponibilidade limitada, os seguintes recursos agora estão disponíveis para todos os ambientes (Disponibilidade geral):

* **Criação de entrega multilíngue**: agora você pode enviar várias entregas de email em diferentes idiomas na Interface do Adobe Campaign Web. O recurso de entrega multilíngue permite escolher o idioma padrão da entrega, bem como os diferentes idiomas nos quais a entrega pode ser enviada. Você também pode visualizar essas entregas nos idiomas escolhidos. [Leia mais](../email/edit-content.md#multilingual-delivery).

<!--
* **Visual fragments** - You can now create, use and archive content fragments. Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](https://experienceleague.adobe.com/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments.html?lang=pt-BR){target="_blank"}
-->

* **Alertas de entrega**: o recurso de alertas de entrega é um sistema de gerenciamento de alertas que habilita um grupo de usuários a receber automaticamente notificações contendo informações sobre a execução de suas entregas. [Leia mais](../msg/delivery-alerting.md)

* **Melhorias nas páginas de destino**: as seguintes melhorias nas páginas de destino agora estão disponíveis:

   * Agora você pode fazer referência a uma página de destino de assinatura/cancelamento de assinatura padrão ao configurar um serviço. Ao criar um email, se você definir um link para essa página de destino, os usuários que enviarem o formulário da página de destino automaticamente assinarão ou cancelarão a assinatura desse serviço. [Leia mais](../audience/manage-services.md#create-service)
   * Uma nova opção na configuração da página de destino permite que visitantes anônimos acessem-na. Se você desmarcar esta opção, apenas usuários identificados poderão acessar e enviar o formulário. [Leia mais](../landing-pages/create-lp.md#create-landing-page)
   * Uma nova opção na configuração da página de destino permite armazenar dados internos adicionais quando a página de destino está sendo enviada. [Leia mais](../landing-pages/create-lp.md#create-landing-page)
   * Uma nova opção permite utilizar uma página de destino para diversos serviços, tornando-a dinâmica. Ao adicionar um link a um email, se você selecionar uma página de destino dinâmica, poderá selecionar qualquer serviço. Se você selecionar uma página de destino que tenha um serviço específico associado, esse serviço será utilizado automaticamente (não será possível selecionar outro). [Leia mais](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * O conteúdo condicional agora é compatível com páginas de destino. [Leia mais](../landing-pages/lp-content.md)
   * É possível vincular uma página de destino a um serviço e enviar uma mensagem de confirmação quando os usuários a validarem. [Saiba mais](../landing-pages/lp-content.md#lp-message)
   * É possível adicionar captcha para proteger a página de destino contra spam e abusos de bots. Esse mecanismo não é intrusivo para os clientes, pois não requer nenhuma interação deles e se baseia em interações com seu site. [Saiba mais](../landing-pages/create-lp.md#captcha)

Anteriormente lançados em disponibilidade limitada, os seguintes recursos agora estão disponíveis **sob demanda**:

* **Relatórios dinâmicos**: agora é possível acessar os relatórios dinâmicos, que fornecem relatórios totalmente personalizáveis e em tempo real para medir o impacto de suas atividades de marketing. Eles adicionam acesso aos dados do perfil, permitindo análises demográficas por dimensões do perfil, como gênero, cidade e idade, além de dados funcionais de campanhas de email, como aberturas e cliques. Os relatórios dinâmicos também estão disponíveis para entregas de email multilíngue e mensagens transacionais. [Leia mais](../reporting/dynamic-reporting/get-started-reporting.md)

* **Identidade visual centralizada**: admins técnicos agora podem definir uma ou várias marcas para centralizar os parâmetros que afetam a identidade de uma marca. Isso inclui o logotipo da marca, o domínio do URL de acesso da página de destino ou as configurações de rastreamento de mensagens. Você pode criar essas marcas e vinculá-las a mensagens ou páginas de destino. Essa configuração é gerenciada nos modelos. As opções de identidade visual estão disponíveis para todos os canais, incluindo SMS e correspondência direta. [Leia mais](../administration/branding/branding-gs.md){target="_blank"}

  >[!NOTE]
  >
  >Esta melhoria está disponível apenas para novas implementações.

Além dos recursos listados acima, esta versão também vem com um conjunto de funcionalidades disponíveis no Console do cliente:

* [Novo conector de envio de SMS](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=pt-BR). (Ambientes FDA)
* [Rest APIs](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=pt-BR) (sob demanda, ambientes FDA)

Consulte as [notas de versão](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=pt-BR){target="_blank"} do Console do cliente.

<!--
ACC * **Branding** - Branding options are now available for all channels, including SMS and Direct mail. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=pt-BR){target="_blank"}
web - * **Branding for Direct Mail** - Technical administrators can now define one or several brands to centralize the parameters that affect a brand's identity. This includes the brand logo, the domain of the landing pages' access URL, or message tracking settings. You can now create these brands and link them to messages or landing pages. This configuration is managed in templates. [Learn more](https://experienceleague.adobe.com/pt-br/docs/experience-cloud/campaign/branding/branding-assign)
ACC - Branding - As a Campaign Standard migrated user, your technical administrators can now define one or several brands to centralize the parameters that affect a brand’s identity. This includes the brand logo, the domain of the landing pages’ access URL, or message tracking settings. You can create these brands and link them to messages or landing pages. This configuration is managed in templates. Read more
Previously released in Limited Availability, the following capability is now available **on demand, only for [Campaign FDA deployments](../architecture/fda-deployment.md)**. To gain access, contact your Adobe representative.
Previously released in Limited Availability, the following capability is now available by default **for new implementations**, and available **on demand for existing environments**. To gain access, contact your Adobe representative.
Previously released in Limited Availability, the following capability is now available **on demand**. To gain access, contact your Adobe representative.
-->