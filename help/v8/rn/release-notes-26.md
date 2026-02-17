---
title: Notas de versão anteriores da interface do Campaign v8 Web
description: Versões de 2026 da interface do Campaign Web
source-git-commit: abec861b2c542644b90d3385fb5cf1d785ae7b70
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 20%

---

# Notas de versão de 2026 {#2026-release}

Esta página lista todas as alterações e melhorias disponíveis com as **versões de 2026**. As notas de versão mais recentes estão disponíveis em [esta página](release-notes.md).

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
<th><strong>Atividade de delivery contínua</strong><br/></th> 
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
<th><strong>Gerenciamento de aprovação de campanha</strong><br/></th> 
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
