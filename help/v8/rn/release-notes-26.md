---
title: Notas de versão anteriores da interface do Campaign v8 Web
description: Versões de 2026 da interface do Campaign Web
exl-id: 40735c57-94ae-4646-8c3d-68197569fbd4
source-git-commit: 0cc09a983d412889f2b734a5bfb30bf422247ec0
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 22%

---

# Notas de versão de 2026 {#2026-release}

Esta página lista todas as alterações e melhorias disponíveis com as **versões de 2026**. As notas de versão mais recentes estão disponíveis em [esta página](release-notes.md).

## Versão de fevereiro de 2026 {#26-2-release}

_17 de fevereiro de 2026_

### Novos recursos {#26-2-features}

<!--table>
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
</table-->

<!--table>
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
</table-->

<table>
<thead>
<tr>
<th><strong>Exibição da linha do tempo no inventário da campanha</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>O inventário da campanha agora inclui uma visualização de Linha do tempo que permite visualizar e gerenciar campanhas ao longo do tempo: alterne entre lista e linha do tempo, navegue por semana, mês ou dia, use o botão Hoje para ir até a data atual e abra os detalhes da campanha (status, workflows, deliveries) em um painel direito, com os mesmos filtros e pesquisa como a visualização da lista.</p>
<p>Para obter mais informações, consulte a <a href="../campaigns/manage-campaigns.md#timeline">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Criação de esquema (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Agora você pode criar e gerenciar esquemas diretamente da interface do usuário da Web do Campaign. Esse recurso permite criar novas tabelas, estender esquemas existentes e criar formulários personalizados. Você pode definir estruturas de dados personalizadas para atender às suas necessidades comerciais específicas sem precisar acessar o Console do cliente.</p>
<p>Observação: esse recurso só está disponível para um conjunto de organizações (disponibilidade limitada) e será implantado globalmente em uma versão futura.</p>
<p>Para obter mais informações, consulte a <a href="../administration/schemas.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--

### Improvement {#26-2-improvements}

* Brand guidelines now include a Colors section that defines standards for your brand's color system, ensuring consistent use of primary, secondary, accent, and neutral colors across all experiences. 
[Learn more](../content/brands-personalize.md)-->

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
<p>O recurso Delivery multilíngue agora está disponível para todos os clientes (GA). Esse recurso permite enviar várias mensagens em diferentes idiomas na Interface do usuário da Web do Adobe Campaign. Você pode escolher o idioma padrão do delivery, bem como os diferentes idiomas nos quais o delivery pode ser enviado. Você também pode visualizar essas entregas nos idiomas escolhidos.  
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
<p>O recurso de enriquecimento de perfil em mensagens transacionais agora está disponível para todos os clientes (GA). Além de emails, agora também há suporte para SMS e notificações por push. Esse recurso permite personalizar mensagens transacionais vinculando campos do banco de dados do Adobe Campaign ao conteúdo da mensagem. Você pode selecionar target mappings, colunas de enriquecimento e uma chave de reconciliação para garantir uma personalização em tempo real e precisa, mantendo os limites de desempenho.</p>
<p>Para obter mais informações, consulte a <a href="../transactional-messaging/profile-enrichment.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Adobe Experience Manager live e cópias de idioma</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>A integração de conteúdo do Adobe Experience Manager permite acessar todos os idiomas e Live Copies criadas no Adobe Experience Manager diretamente no Campaign ao criar deliveries. Você pode atualizar o conteúdo em tempo real para buscar as versões mais recentes do Adobe Experience Manager. Essa integração elimina a sincronização manual de conteúdo entre o Adobe Experience Manager e o Campaign, simplificando seu fluxo de trabalho de campanha em vários idiomas.</p>
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
<p>Os experimentos de conteúdo na Adobe Campaign Web permitem definir várias variantes de delivery de teste A/B para medir qual tem o melhor desempenho para o público-alvo. Você pode variar o conteúdo do delivery, o assunto ou o remetente para testar diferentes versões e determinar qual variante produz os melhores resultados. Você pode realizar testes A/B em vários elementos de email, como linha de assunto, nome do remetente e conteúdo do corpo do email.</p>
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
<p>A atividade Continuous delivery permite adicionar novos recipients a um delivery existente. Esse tipo de delivery evita a necessidade de criar um novo delivery a cada vez, tornando-o mais eficiente para alertas de baixo volume ou notificações enviadas conforme necessário. Uma entrega contínua cria uma única instância de entrega. Todos os logs do delivery (broadLog) e logs de rastreamento fazem referência a esse delivery, simplificando o monitoramento e os relatórios.</p>
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
<p>O processo de aprovação ajuda a coordenar vários participantes e garante o controle de qualidade antes que os deliveries sejam enviados. Use aprovações quando sua organização exigir a validação de equipes diferentes, como gerentes de marketing que revisam conteúdo ou analistas de dados que validam públicos-alvo.</p>
<p>Para obter mais informações, consulte a <a href="../campaigns/campaign-approvals.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

### Aprimoramentos {#26-1-improvements}

* Os relatórios dinâmicos agora oferecem suporte a notificações por push e SMS. [Saiba mais](../reporting/dynamic-reporting/get-started-reporting.md)
* Filtros predefinidos - Uma nova opção &quot;Filtro compartilhado&quot; permite disponibilizar um filtro predefinido para outros usuários em sua organização. [Saiba mais](../get-started/predefined-filters.md#share-filter)
* Os campos de personalização criados no Adobe Experience Manager, como Nome, Email, Data e Endereço, agora estão incluídos e disponíveis ao usar o modelo de conteúdo.
* A avaliação da qualidade do conteúdo agora verifica problemas de legibilidade, coesão e eficácia independentemente das diretrizes da marca, identificando mensagens não claras, tons inconsistentes ou lacunas estruturais. [Saiba mais](../content/brands-score.md)
