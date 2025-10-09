---
title: Notas de versão da interface do Campaign Web v8
description: Conheça os novos recursos que acompanham a versão mais recente da interface do Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 0457e4d0150fe445ae5313377eb299cde40a51b9
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 71%

---

# Notas de versão {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de versão"
>abstract="As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, as notas de versão do Campaign são atualizadas várias vezes por mês, com os recursos, melhorias e correções mais recentes. Recomendamos que você as verifique regularmente."

As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, essas notas de versão são atualizadas várias vezes por mês. Verifique-as regularmente.

As alterações e melhorias disponíveis em versões anteriores estão listadas nas páginas de [2024](release-notes-24.md) e [2025](release-notes-25.md).

## Atualizações de outubro de 2025 {#25-9-updates}

_9 de outubro de 2025_

<table>
<thead>
<tr>
<th><strong>Recursos multilíngues para mensagens transacionais, notificações por push e SMS (DL)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Agora você pode enviar várias mensagens transacionais, notificações por push e mensagens SMS em diferentes idiomas na Interface do usuário da Web do Adobe Campaign. O recurso de entrega multilíngue permite escolher o idioma padrão da entrega, bem como os diferentes idiomas nos quais a entrega pode ser enviada. Você também pode visualizar esses deliveries nos idiomas escolhidos.</p>
<p>Observação: esse recurso só está disponível para um conjunto de organizações (disponibilidade limitada) e será implantado globalmente em uma versão futura.</p>
<p>Para obter mais informações, consulte a <a href="../msg/multilingual.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Enriquecimento de perfil em mensagens transacionais (DL)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Esse recurso permite personalizar mensagens transacionais vinculando campos do banco de dados do Adobe Campaign ao conteúdo da mensagem. Você pode selecionar target mappings, colunas de enriquecimento e uma chave de reconciliação para garantir uma personalização precisa e em tempo real, mantendo os limites de desempenho.</p>
<p>Observação: esse recurso só está disponível para um conjunto de organizações (disponibilidade limitada) e será implantado globalmente em uma versão futura. No momento, esse recurso está disponível apenas para emails.</p>
<p>Para obter mais informações, consulte a <a href="../transactional-messaging/profile-enrichment.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>


## Versão de setembro de 2025 {#25-9-release}

_23 de setembro de 2025_

Os seguintes recursos estão disponíveis a partir da versão de setembro.

<table>
<thead>
<tr>
<th><strong>Canal personalizado para entregas de API</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Agora é possível orquestrar e executar entregas com base em canais de API personalizados diretamente da interface do Adobe Campaign Web. Essas entregas podem ser autônomas ou fazer parte de um fluxo de trabalho. A configuração do canal de API personalizado é realizada no console.</p>
<p>Para obter mais informações, consulte a <a href="../call-center/gs-custom-channel.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Criação de conta externa</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Como administrador do Campaign, agora você pode configurar novas conexões com sistemas externos à partir da interface do Campaign Web. Você também pode exibir, atualizar e gerenciar contas externas existentes.</p>
<p>Para obter mais informações, consulte a <a href="../administration/create-external-account.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Bloqueio de conteúdo de email</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>O Campaign agora permite bloquear conteúdo em modelos de email ao bloquear todo o modelo ou estruturas e componentes específicos. Isso permite evitar edições ou exclusões não intencionais, dando a você maior controle sobre a personalização do modelo e melhorando a eficiência e a confiabilidade de suas campanhas de email.</p>
<p>Para obter mais informações, consulte a <a href="../content/content-locking.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>Integration with Adobe GenStudio</strong><br/></th>  LA? sort? Juliette
</tr>
</thead>
<tbody>
<tr>
<td>
<p>To enhance marketing efficiency and to maintain brand consistency, you can now seamlessly integrate GenStudio for Performance Marketing experiences with Campaign. This enables you to leverage GenStudio's AI-power content creation alongside Campaign's advanced orchestration capabilities.<p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Dark mode support in the Email designer</strong><br/></th> -> pas sept, modifier composant... -> Juliette
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The Email Designer now offers the ability to switch to dark mode view, where you can additionally define specific custom settings. Note that the final rendering depends on the recipient's email client, and not all email clients support dark mode.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>>
<thead>
<tr>
<th><strong>Multilingual capabilities for transactional messaging and push notifications (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now send multiple transactional messages and push notifications in different languages in Adobe Campaign Web User Interface. The Multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen.</p>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Profile enrichment in Transactional Messages (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>This capability allows you to personalize transactional messages (Email, SMS, Push) by linking Adobe Campaign database fields to the message content. You can select target mappings, enrichment columns, and a reconciliation key to ensure accurate, real-time personalization while maintaining performance thresholds.</p>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Dynamic reporting for transactional messaging (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->


### Melhorias {#25-9-improvements}

* Um conjunto de novos operadores foi adicionado ao configurar uma condição por meio do recurso de conteúdo condicional do designer de email.
* A dimensão de filtros agora está disponível na atividade de fluxo de trabalho **Criar público-alvo**. Para exibi-lo ou alterá-lo, clique no ícone ao lado da dimensão de direcionamento. [Saiba mais](../workflows/activities/build-audience.md#build-audience-configuration).
<!--

NEO-84915 Stop button for deliveries???? ->>> met pas, juste bouton ajouté dans webUI meme comportement que console. bleu, marche, marche pas.
NEO-90345 WebUI - Extended operators for dynamic content ->>>> deja mis
NEO-88858 WebUI - Send proof from execution recurring delivery -> bug
NEO-89777 Content locking on create email template -> juliette
NEO-90365 Multi-lingual – Identify fields editable from variants???? -> fix pour SMS
query activity -> query ds workflow fitleting dimentsion 

-->

