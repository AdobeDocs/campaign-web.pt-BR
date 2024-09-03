---
title: Notas de versão da interface do Campaign Web v8
description: Conheça os novos recursos que acompanham a versão mais recente da interface do Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: e9022e53ff8733ecdfcca1aec2ba31ca6c79c3ad
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 52%

---

# Notas de versão {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de versão"
>abstract="As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, as notas de versão do Campaign são atualizadas várias vezes por mês, com os recursos, melhorias e correções mais recentes. Recomendamos que você as verifique regularmente."

As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, essas notas de versão são atualizadas várias vezes por mês. Verifique-as regularmente.

## Notas de versão de agosto {#24-8-release}

**Data de lançamento**: 3 de setembro de 2024

Os seguintes recursos e melhorias estão disponíveis a partir da versão de agosto.

* **Distribuição de valores** - Ao acessar a lista de campos para personalização, agora é possível verificar como os valores são distribuídos para cada campo. Uma janela pop-up dedicada mostra o número e a porcentagem para cada valor. [Saiba mais](../query/build-query.md#distribution-values-query)

* **Parâmetros SMTP** - As configurações SMTP agora estão disponíveis nas configurações de entrega de email. [Saiba mais](../advanced-settings/delivery-settings.md#smtp)

* **Variáveis globais** - Agora é possível definir variáveis globais para definir valores para seus deliveries. [Saiba mais](../advanced-settings/delivery-settings.md#variables-delivery)

### Novos recursos em Disponibilidade limitada {#acs-24-8}

>[!AVAILABILITY]
>
>Os seguintes recursos estão em Disponibilidade limitada (LA). Eles estão restritos a clientes que estão migrando **do Adobe Campaign Standard para o Adobe Campaign v8** e não podem ser implantados em nenhum outro ambiente.
>
>Consulte as seguintes páginas de documentação: [Transição de Campaign Standard para o Campaign v8](../rn/acs-migration.md) e [Recursos para usuários de Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=pt-BR){target="_blank"}.

* **Marcas para correspondência direta** - Os administradores técnicos agora podem definir uma ou várias marcas para centralizar os parâmetros que afetam a identidade de uma marca. Isso inclui o logotipo da marca, o domínio do URL de acesso da página de destino ou as configurações de rastreamento de mensagens. Agora você pode criar essas marcas e vinculá-las a mensagens ou páginas de aterrissagem. Essa configuração é gerenciada em modelos. [Saiba mais](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-assign)

* **Assinaturas com páginas de aterrissagem** - Agora é possível vincular uma página de aterrissagem a um serviço e enviar uma mensagem de confirmação quando os usuários a validarem. [Saiba mais](../landing-pages/lp-content.md#lp-message){target="_blank"}.

* **Fragmentos visuais** - Agora você pode arquivar fragmentos de conteúdo visual. [Saiba mais](../content/create-fragment.md#archive)

* **Captcha nas páginas de aterrissagem** - Agora é possível adicionar captcha para proteger sua página de aterrissagem contra spam e abuso causado por bots. Esse mecanismo não é intrusivo para os clientes, pois não requer nenhuma interação deles e se baseia em interações com seu site. [Saiba mais](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.-->
