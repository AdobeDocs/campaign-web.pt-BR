---
title: Notas de versão anteriores da interface do Campaign v8 Web
description: Versões de 2026 da interface do Campaign Web
exl-id: 40735c57-94ae-4646-8c3d-68197569fbd4
source-git-commit: be38a0d27ae805ac64f0c951e5ea470cd1feb859
workflow-type: ht
source-wordcount: '753'
ht-degree: 100%

---

# Notas de versão de 2026 {#2026-release}

Esta página lista todas as alterações e melhorias disponíveis nas **versões de 2026**. As notas de versão mais recentes estão disponíveis [nesta página](release-notes.md).

## Versão de fevereiro de 2026 {#26-2-release}

_17 de fevereiro de 2026_

### Novos recursos {#26-2-features}

<!--
table>
<thead>
<tr>
<th><strong>Delivery scheduling compute process</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now use a delivery scheduling compute process similar to the one available in Adobe Campaign Standard. This feature allows you to calculate sending dates based on recipient timezones, enabling you to send communications at the optimal time for each recipient. This is particularly useful for organizations operating across multiple timezones, as it allows you to target regions with different timezones using a single delivery configuration.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table
-->

<!--
table>
<thead>
<tr>
<th><strong>Themes in the Email Designer (Beta)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Themes provide an improved authoring experience for emails by allowing you to define reusable theme styles that fit your brand guidelines. You can now use theme variables in fragments, ensuring consistent styling across your email templates. This feature enables you to build emails faster with predefined modules that abstract content elements such as titles, descriptions, images, and links, while maintaining brand consistency.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table
-->

<table>
<thead>
<tr>
<th><strong>Visualização de linha do tempo no inventário da campanha</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>O inventário da campanha agora inclui uma visualização de Linha do tempo que permite visualizar e gerenciar campanhas ao longo do tempo: alterne entre a lista e a linha do tempo, navegue por semana, mês ou dia, use o botão Hoje para ir até a data atual e abra os detalhes da campanha (status, fluxos de trabalho, entregas) no painel à direita, com os mesmos filtros e opções de pesquisa da visualização em lista.</p>
<p>Para obter mais informações, consulte a <a href="../campaigns/manage-campaigns.md#timeline">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Criação de esquema (Disponibilidade limitada ou LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Agora você pode criar e gerenciar esquemas diretamente da interface do Campaign Web. Esse recurso permite criar novas tabelas, estender esquemas existentes e criar formulários personalizados. Você pode definir estruturas de dados personalizadas para atender às suas necessidades comerciais específicas sem precisar acessar o Console do cliente.</p>
<p>Observação: esse recurso só está disponível para um conjunto de organizações (disponibilidade limitada) e será implantado globalmente em uma versão futura.</p>
<p>Para obter mais informações, consulte a <a href="../administration/schemas.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--

### Improvement {#26-2-improvements}

* Brand guidelines now include a Colors section that defines standards for your brand's color system, ensuring consistent use of primary, secondary, accent, and neutral colors across all experiences. 
[Learn more](../content/brands-personalize.md)
-->

## Versão de janeiro de 2026 {#26-1-release}

_27 de janeiro de 2026_

### Novos recursos {#26-1-features}

<table>
<thead>
<tr>
<th><strong>Recursos de entrega multilíngue (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>O recurso entrega multilíngue agora está disponível para todos os clientes (Disponibilidade geral ou GA). Esse recurso permite enviar várias mensagens em diferentes idiomas na interface do Adobe Campaign Web. Você pode escolher o idioma padrão da sua entrega, bem como os diferentes idiomas nos quais a entrega pode ser enviada. Você também pode visualizar essas entregas nos idiomas escolhidos. 
<p>Para obter mais informações, consulte a <a href="../msg/multilingual.md">documentação detalhada</a>.</p>
<p>As seguintes melhorias foram realizadas nas notificações por push multilíngues:</p>
<ul>
<li>Agora é possível preencher rapidamente todas as variantes de idioma fazendo upload de um arquivo CSV com seu conteúdo multilíngue. <a href="../msg/multilingual.md#csv-upload">Leia mais</a>
</li>
<li>Agora há suporte para notificações por push avançadas.</li>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Enriquecimento de perfil em mensagens transacionais (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>O recurso de enriquecimento de perfil em mensagens transacionais agora está disponível para todos os clientes (GA). Além de emails, agora também há suporte para SMS e notificações por push. Esse recurso permite personalizar mensagens transacionais vinculando campos do banco de dados do Adobe Campaign ao conteúdo da mensagem. Você pode selecionar mapeamentos de destino, colunas de enriquecimento e uma chave de reconciliação para garantir uma personalização precisa e em tempo real, mantendo os limites de desempenho.</p>
<p>Para obter mais informações, consulte a <a href="../transactional-messaging/profile-enrichment.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Cópias online e de idioma do Adobe Experience Manager</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>A integração de conteúdo do Adobe Experience Manager permite acessar diretamente no Campaign todas as cópias de idioma e cópias online criadas no Adobe Experience Manager ao gerar entregas. Você pode atualizar o conteúdo em tempo real para obter as versões mais recentes do Adobe Experience Manager. Essa integração elimina a sincronização manual de conteúdo entre o Adobe Experience Manager e o Campaign, simplificando o fluxo de trabalho das suas campanhas multilíngues.</p>
<p>Para obter mais informações, consulte a <a href="../integrations/aem-multilingual.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Experimentos de conteúdo - Teste A/B</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Os experimentos de conteúdo no Adobe Campaign Web permitem definir diversas variantes de entrega para testes A/B, a fim de avaliar qual delas apresenta melhor desempenho para o seu público-alvo. Você pode variar o conteúdo da entrega, o assunto ou o remetente para testar diferentes versões e determinar qual variante produz os melhores resultados. Você pode realizar testes A/B em vários elementos de email, como linha de assunto, nome do remetente e conteúdo do corpo do email.</p>
<p>Para obter mais informações, consulte a <a href="../email/ab-testing.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Atividade de entrega contínua</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>A atividade de entrega contínua permite adicionar novos destinatários a uma entrega já existente. Esse tipo de entrega evita a necessidade de criar uma nova entrega a cada vez, tornando o processo mais eficiente para alertas ou notificações de baixo volume que são enviados conforme necessário. Uma entrega contínua cria uma única instância de entrega. Todos os logs de entrega (broadLog) e logs de rastreamento fazem referência a esta única entrega, simplificando o monitoramento e os relatórios.</p>
<p>Para obter mais informações, consulte a <a href="../workflows/activities/continuous-delivery.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Gerenciamento de aprovação da campanha</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>O processo de aprovação ajuda a coordenar as diversas partes interessadas e garante o controle de qualidade antes do envio das entregas. Utilize o processo de aprovação quando sua organização precisar da validação de diferentes equipes, como gerentes de marketing que precisam revisar conteúdo ou analistas de dados que precisam validar públicos-alvo.</p>
<p>Para obter mais informações, consulte a <a href="../campaigns/campaign-approvals.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

### Aprimoramentos {#26-1-improvements}

* Os relatórios dinâmicos agora oferecem suporte a notificações por push e SMS. [Saiba mais](../reporting/dynamic-reporting/get-started-reporting.md)
* Filtros predefinidos - Uma nova opção chamada “Filtro compartilhado” permite disponibilizar um filtro predefinido para outros usuários da sua organização. [Saiba mais](../get-started/predefined-filters.md#share-filter)
* Os campos de personalização criados no Adobe Experience Manager, como Nome, Email, Data e Endereço, agora estão incluídos e disponíveis ao usar modelos de conteúdo.
* A avaliação da qualidade do conteúdo agora verifica questões relacionadas à legibilidade, coesão e eficácia, independentemente das diretrizes da marca, identificando mensagens pouco claras, tom inconsistente ou lacunas estruturais. [Saiba mais](../content/brands-score.md)
