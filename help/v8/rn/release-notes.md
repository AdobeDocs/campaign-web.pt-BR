---
title: Notas de versão da interface do Campaign Web v8
description: Conheça os novos recursos que acompanham a versão mais recente da interface do Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: ef040ec079961771b734208ecf8ac9e510b38104
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 69%

---

# Notas de versão {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de versão"
>abstract="As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, as notas de versão do Campaign são atualizadas várias vezes por mês, com os recursos, melhorias e correções mais recentes. Recomendamos que você as verifique regularmente."

As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, essas notas de versão são atualizadas várias vezes por mês. Verifique-as regularmente.

## Versão de outubro {#24-10-release}

**Data de lançamento**: 29 de outubro de 2024

Os seguintes recursos e melhorias estarão disponíveis a partir da versão de outubro.

### Recursos

<table>
<thead>
<tr>
<th><strong>Contas externas</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Agora é possível configurar e gerenciar contas externas diretamente por meio da interface da Web do Adobe Campaign. Esse novo recurso facilita a configuração de diferentes tipos de contas externas, como emails de devolução (POP3) ou instâncias de execução.</p>
<p>Para obter mais informações, consulte a <a href="../administration/external-account.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Mensagens transacionais</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Agora você pode criar e monitorar mensagens transacionais na interface do usuário da Web do Campaign. As mensagens transacionais são um módulo especializado no Adobe Campaign criado para lidar com mensagens acionadas. Essas mensagens são geradas automaticamente em resposta a eventos provenientes de sistemas de informações. Exemplos comuns de tais eventos incluem clicar em botões ou links, abandono de carrinho, solicitação de alertas de disponibilidade de produto, criação ou modificação de conta etc.</p>
<p>Para obter mais informações, consulte a <a href="../transactional-messaging/transactional.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>External deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now define External deliveries, and External delivery templates, in Campaign web user interface. With this mode, messages are generated in an input file which can be shared with your external provider. The External delivery mode is the default mode for the direct mail channel.</p>
</td>
</tr>
</tbody>
</table-->


### Melhorias

* **Atividades do fluxo de trabalho** - Agora é possível mover uma atividade e todos os seus nós filhos de uma transição para outra dentro de um fluxo de trabalho. Um botão **Mover** dedicado está disponível no painel de propriedades da atividade para realizar isso. [Saiba mais](../workflows/orchestrate-activities.md#move)

* **Atividade de enriquecimento do fluxo de trabalho**

   * Agora você pode definir um Alias e um Label ao criar um novo campo na atividade **Enriquecimento**. [Saiba mais](../workflows/activities/enrichment.md#collection-settings)
   * Agora você pode adicionar ofertas para cada perfil na atividade **Enriquecimento**. [Saiba mais](../workflows/activities/enrichment.md##add-offers)

* **Distribuição de valores**: ao acessar a lista de campos para personalização, agora é possível verificar como os valores estão distribuídos para cada campo. Uma janela pop-up exclusiva mostra o número e a porcentagem para cada valor. [Saiba mais](../query/build-query.md#distribution-values-query)


## Atualizações de setembro {#9-2024}

<table>
<thead>
<tr>
<th><strong>Acelerador de conteúdo do Assistente de IA</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Depois de criar e adaptar sua mensagem, leve-a para o próximo nível com o Acelerador de conteúdo do assistente de IA na Web do Adobe Campaign. Essa ferramenta avançada permite otimizar o impacto do conteúdo gerando uma variedade de textos envolventes, títulos principais e imagens visualmente atraentes.</p>
<p>Mergulhe em uma experiência prática com a <a href="https://experienceleague.adobe.com/pt-br/apps/journey-optimizer/ai-assistant-content-accelerator">nossa visualização de recursos ao vivo</a>, projetada para permitir que você explore seus recursos em primeira mão e entenda totalmente suas funcionalidades.</a>.</p>
<p>Para obter mais informações, consulte a <a href="../email/generative-gs.md">documentação detalhada</a>.</p>
<img src="assets/do-not-localize/ai-content-webui.gif"/>
<p>Data de disponibilidade: 12 de setembro</p>
</td>
</tr>
</tbody>
</table>

## Versão de agosto {#24-8-release}

**Data de lançamento**: 3 de setembro de 2024

Os seguintes recursos e melhorias estão disponíveis a partir da versão de agosto.

* **Parâmetros SMTP**: as configurações de SMTP agora estão disponíveis nas configurações de entrega de email. [Saiba mais](../advanced-settings/delivery-settings.md#smtp)

* **Variáveis globais**: agora, você pode definir variáveis globais para estipular valores para as suas entregas. [Saiba mais](../advanced-settings/delivery-settings.md#variables-delivery)

### Novos recursos em Disponibilidade limitada {#acs-24-8}

>[!AVAILABILITY]
>
>Os seguintes recursos estão em Disponibilidade limitada (LA). Eles estão restritos a clientes que estão migrando **do Adobe Campaign Standard para o Adobe Campaign v8** e não podem ser implantados em nenhum outro ambiente.
>
>Consulte as seguintes páginas de documentação: [Transição do Campaign Standard para o Campaign v8](../rn/acs-migration.md) e [Recursos para usuários do Campaign Standard](https://experienceleague.adobe.comdocs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=pt-BR){target="_blank"}.

* **Identidade visual para correspondência direta**: os administradores técnicos agora podem definir uma ou várias marcas para centralizar os parâmetros que afetam a identidade de uma marca. Isso inclui o logotipo da marca, o domínio do URL de acesso da página de destino ou as configurações de rastreamento de mensagens. Você pode criar essas marcas e vinculá-las a mensagens ou páginas de destino. Essa configuração é gerenciada nos modelos. [Saiba mais](https://experienceleague.adobe.com/pt-br/docs/experience-cloud/campaign/branding/branding-assign)

* **Assinaturas com páginas de destino**: agora, você pode vincular uma página de destino a um serviço e enviar uma mensagem de confirmação quando os usuários a validarem. [Saiba mais](../landing-pages/lp-content.md#lp-message){target="_blank"}.

* **Fragmentos visuais**: agora, você pode arquivar fragmentos de conteúdo visuais. [Saiba mais](../content/create-fragment.md#archive)

* **Captcha em páginas de destino**: agora, você pode adicionar um captcha para proteger a sua página de destino contra spam e abusos causados por bots. Esse mecanismo não é intrusivo para os clientes, pois não requer nenhuma interação deles e se baseia em interações com seu site. [Saiba mais](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.-->
