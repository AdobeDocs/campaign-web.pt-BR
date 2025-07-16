---
title: Notas de versão anteriores da interface do Campaign v8 Web
description: Versões de 2024 da interface do usuário do Campaign Web
exl-id: 430dc1ba-dfa9-4d51-b4ed-f3f048da6ec0
source-git-commit: 4f32adbbe360b76d227c431281ef10a47e6a37ba
workflow-type: ht
source-wordcount: '2532'
ht-degree: 100%

---

# Notas de versão de 2024 {#2024-release}

Esta página lista todas as alterações e melhorias disponíveis com as **versões de 2024**. As notas de versão mais recentes estão disponíveis [nesta página](release-notes.md).


## Versão de outubro de 2024 {#24-10-release}

**Data de lançamento**: 29 de outubro de 2024

Os seguintes recursos e melhorias estão disponíveis a partir da versão de outubro.

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
<p>Agora é possível configurar e gerenciar contas externas diretamente na interface do Adobe Campaign Web. Esse novo recurso facilita a configuração de diferentes tipos de contas externas, como emails de rejeição (POP3) ou instâncias de execução.</p>
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
<p>As mensagens transacionais (Centro de mensagens) agora estão disponíveis na interface do Campaign Web. Este complemento foi desenvolvido para Acionar mensagens geradas de eventos disparados por sistemas de informação, podendo ser: fatura, confirmação de pedido, confirmação de envio, alteração de senha, notificação de indisponibilidade de produto, extrato de conta, criação de conta em site etc.</p>
<p>Para obter mais informações, consulte a <a href="../transactional-messaging/transactional.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>


### Melhorias

* **Atividades do fluxo de trabalho**: agora é possível mover uma atividade e todos os seus nós filhos de uma transição para outra dentro de um fluxo de trabalho. Um botão **Mover** dedicado está disponível no painel de propriedades da atividade para realizar isso. [Saiba mais](../workflows/orchestrate-activities.md#move)

* **Atividade de enriquecimento de fluxo de trabalho**

   * Agora é possível definir um alias e um rótulo ao criar um novo campo na atividade **Enriquecimento**. [Saiba mais](../workflows/activities/enrichment.md#collection-settings)
   * Agora você pode adicionar ofertas para cada perfil na atividade **Enriquecimento**. [Saiba mais](../workflows/activities/enrichment.md##add-offers)

* **Distribuição de valores**: ao acessar a lista de campos para personalização, agora é possível verificar como os valores estão distribuídos para cada campo. Uma janela pop-up exclusiva mostra o número e a porcentagem para cada valor. [Saiba mais](../query/build-query.md#distribution-values-query)

* **Informações de versão e sistema**: agora você pode acessar detalhes das versões da sua instância, tanto para o console do cliente quanto para a Interface da Web. Esta nova seção também lista todos os pacotes integrados instalados no seu ambiente. [Saiba mais](../get-started/user-interface.md#user-interface-about)

* **Listas**: agora é possível reordenar facilmente os valores de uma lista. [Saiba mais](../get-started/work-with-folders.md)

* **Entrega**: a variável Entrega agora pode ser acessada em campos de personalização. [Saiba mais](../personalization/conditions.md#use-variables-for-conditional-content-variables-conditional)


## Atualizações de setembro {#9-2024}

<table>
<thead>
<tr>
<th><strong>Assistente de IA</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Depois de criar e personalizar sua mensagem, melhore-a ainda mais com o Assistente de IA no Adobe Campaign Web. Essa ferramenta avançada permite otimizar o impacto do conteúdo gerando uma variedade de textos envolventes, títulos principais e imagens visualmente atraentes.</p>
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
>Consulte as seguintes páginas de documentação: [Transição do Campaign Standard para o Campaign v8](../rn/acs-migration.md) e [Recursos para usuários do Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=pt-BR){target="_blank"}.

* **Identidade visual para correspondência direta**: os administradores técnicos agora podem definir uma ou várias marcas para centralizar os parâmetros que afetam a identidade de uma marca. Isso inclui o logotipo da marca, o domínio do URL de acesso da página de destino ou as configurações de rastreamento de mensagens. Você pode criar essas marcas e vinculá-las a mensagens ou páginas de destino. Essa configuração é gerenciada nos modelos. [Saiba mais](../administration/branding/branding-assign.md)

* **Assinaturas com páginas de destino**: agora, você pode vincular uma página de destino a um serviço e enviar uma mensagem de confirmação quando os usuários a validarem. [Saiba mais](../landing-pages/lp-content.md#lp-message){target="_blank"}.

* **Fragmentos visuais**: agora, você pode arquivar fragmentos de conteúdo visuais. [Saiba mais](../content/create-fragment.md#archive)

* **Captcha em páginas de destino**: agora, você pode adicionar um captcha para proteger a sua página de destino contra spam e abusos causados por bots. Esse mecanismo não é intrusivo para os clientes, pois não requer nenhuma interação deles e se baseia em interações com seu site. [Saiba mais](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html){target="_blank"}.-->


## Notas de versão de julho {#24-7-release}

**Data de lançamento**: 30 a 31 de julho de 2024

Os seguintes recursos e melhorias estão disponíveis a partir da versão de julho.

### Fragmentos de conteúdo {#24-7-1}

Agora você pode criar e usar fragmentos de conteúdo. Um fragmento de conteúdo é um componente reutilizável que pode ser referenciado em uma ou mais mensagens. Ao modificar um fragmento, todos os conteúdos que o usam serão atualizados. Essa funcionalidade permite pré-construir vários blocos de conteúdo personalizados que podem ser usados por usuários de marketing para montar rapidamente o conteúdo de mensagens em um processo de design aprimorado.

Dois tipos de fragmentos estão disponíveis:

* **Fragmentos de expressão** são expressões predefinidas disponíveis em uma entrada dedicada no editor de expressão.
* **Fragmentos visuais** são blocos visuais predefinidos que podem ser reutilizados em várias entregas de email ou em modelos de conteúdo. [Saiba mais](../content/fragments.md)

  >[!AVAILABILITY]
  >
  >**Fragmentos visuais** estão em disponibilidade limitada (LA). Esse recurso é restrito a clientes que estão migrando **do Adobe Campaign Standard para o Adobe Campaign v8** e não pode ser implantado em nenhum outro ambiente.

### Grupo de interceptação {#24-7-2}

Um **grupo de interceptação** contém vários seed addresses. Ela é usada para incluir endereços específicos em suas entregas e direcionar perfis que não correspondem aos critérios de destino definidos. Dessa forma, os destinatários que não pertencem ao público-alvo da entrega podem recebê-la, assim como qualquer outro destinatário. É possível usar seed addresses ao enviar provas ou para proteger a lista de mala direta. [Saiba mais](../audience/trap-group.md)

### Modelos de notificação por push avançada {#24-7-3}

Agora é possível enviar notificações por push avançadas. Uma notificação por push avançada é uma forma aprimorada de notificação em dispositivos móveis que vai além das mensagens de texto simples, incorporando elementos multimídia, como imagens, botões interativos ou outros conteúdos de mídia avançada. Com esta versão, um conjunto de modelos para notificações por push avançadas agora está disponível para seus aplicativos iOS e Android.

[Saiba mais](../push/rich-push.md)

>[!AVAILABILITY]
>
>Esse recurso exige a atualização para o Campaign v8.6.3 <!--or v8.7.2-->. Saiba mais nas [notas de versão](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/releases/release-notes){target="_blank"} do console do cliente do Campaign v8.

### Melhorias {#improvements-24-7}

**Gerenciamento de pastas**: agora é possível gerenciar permissões e restrições em pastas.

## Notas de versão de junho {#24-6-release}

**Data de lançamento**: 18 a 19 de junho de 2024

Os seguintes recursos e melhorias estão disponíveis para todos os usuários a partir da versão de junho.


### Planos e programas {#24-6-4}

Agora é possível criar planos e programas para organizar suas campanhas. Ao definir uma hierarquia de pastas, você pode organizar suas campanhas em programas e os programas em planos. [Leia mais](../administration/plans-programs.md)

### Melhorias {#improvements-24-6}

* **Reconciliação na atividade de enriquecimento**: a atividade de **enriquecimento** agora pode ser usada para reconciliar dados do esquema do banco de dados do Campaign com dados de outro esquema ou de um esquema temporário, como dados carregados usando uma atividade Carregar arquivo. Por exemplo, é possível usar essa opção para reconciliar o país de um perfil, que é especificado em um arquivo carregado, com um dos países disponíveis na tabela dedicada do banco de dados do Campaign. [Leia mais](../workflows/activities/enrichment.md)


### Novo recurso em disponibilidade limitada {#acs-24-6}

>[!AVAILABILITY]
>
>Os seguintes recursos estão em disponibilidade limitada. Eles são restritos a clientes que estão migrando **do Adobe Campaign Standard para o Adobe Campaign v8** e não podem ser implantados em nenhum outro ambiente.

* **Alerta de entrega**

O recurso Alerta de entrega é um sistema de gerenciamento de alertas que permite que um grupo de usuários receba automaticamente notificações sobre a execução de suas entregas. [Leia mais](../msg/delivery-alerting.md)


## Notas da versão de maio {#24-5-release}

**Data de lançamento**: 21 de maio de 2024

Os seguintes recursos e melhorias estão disponíveis para todos os usuários a partir da versão de maio.

### Trilha de auditoria  {#24-5-1}

O novo recurso de **Trilha de auditoria** fornece um registro detalhado e cronológico de todas as ações e eventos realizados em sua instância do Adobe Campaign em tempo real. Esse recurso oferece um método conveniente para rastrear todas as alterações nos dados do Campaign, abordando consultas como: status dos fluxos de trabalho, últimas pessoas que os modificaram ou atividades realizadas pelos usuários na instância. [Leia mais](../reporting/audit-trail.md)

### Campos personalizados {#24-5-2}

**Os campos personalizados** são outros atributos adicionados aos esquemas prontos para uso por meio do console do Adobe Campaign. Na interface do Campaign Web, esses campos personalizados agora ficam visíveis em diversas telas. Por exemplo, os detalhes de um perfil ou de um perfil de teste. Na interface web, você não pode criar campos personalizados, mas agora pode modificar a forma como eles são exibidos. [Leia mais](../administration/custom-fields.md)

### Crie links entre tabelas {#24-5-3}

Agora você pode criar links com outra tabela na atividade de fluxo de trabalho **Enriquecimento**. Use a nova seção **Definição de link** nos parâmetros de atividade para criar um link entre os dados da tabela de trabalho e o banco de dados do Adobe Campaign. Por exemplo, ao carregar dados de um arquivo que contenha o número da conta, o país e o email dos destinatários, agora é possível criar um link para a tabela do país para atualizar essas informações em seus perfis. [Leia mais](../workflows/activities/enrichment.md#create-links)

### Melhorias gerais {#improvements-24-5}

* **Correspondência direta**: agora você pode aproveitar o editor de expressão para selecionar os atributos a serem exibidos nos arquivos de extração de correspondência direta. [Leia mais](../direct-mail/content-direct-mail.md)

* **Gerenciamento de pastas**: agora é possível criar uma subpasta de um tipo diferente da pasta principal. [Leia mais](../get-started/permissions.md#folders)

* **Globalização**: como parte de nosso esforço contínuo para oferecer uma experiência de usuário unificada, harmonizamos a terminologia usada nos produtos e aplicativos da Adobe Experience Cloud. Isto afeta o termo alemão “Titel” que é alterado para “Label” quando se refere ao nome de um objeto. As mudanças serão implementadas progressivamente na interface e na documentação.


## Notas da versão de abril {#april-24-4-release}

**Data de lançamento**: 2 de maio de 2024

### Novos recursos {#new-24-4}

Os seguintes recursos estão disponíveis para todos os usuários a partir da versão de abril.

**Novas atividades de fluxo de trabalho**

* **Atualizar dados**: use esta atividade para realizar atualizações em massa nos campos do banco de dados. Várias opções permitem personalizar a atualização dos dados. [Leia mais](../workflows/activities/update-data.md)
* **Serviços de assinatura**: use esta atividade para assinar ou cancelar inscrição de vários perfis de/para um serviço em uma única ação. [Leia mais](../workflows/activities/subscription-services.md)
* **Extrair arquivo**: use esta atividade para exportar dados do Adobe Campaign para outro sistema como um arquivo externo. [Leia mais](../workflows/activities/extract-file.md)
* **Transferir arquivo**: use esta atividade para receber ou enviar arquivos, testar a presença de arquivos ou listar arquivos em um servidor. O protocolo usado pode ser o protocolo servidor para servidor ou o protocolo HTTP. [Leia mais](../workflows/activities/transfer-file.md)
* **Teste**: use esta atividade para permitir transições com base em condições especificadas. [Leia mais](../workflows/activities/test.md)
* **Código JavaScript**: use esta atividade para executar um trecho de código JavaScript no contexto de um fluxo de trabalho. [Leia mais](../workflows/activities/javascript-code.md)
* **Sinal externo**: use esta atividade para acionar a execução de um fluxo de trabalho a partir de outro fluxo de trabalho ou de uma chamada de API. [Leia mais](../workflows/activities/external-signal.md)
* **Consulta incremental**: use esta atividade para consultar o banco de dados de forma programada. Todas as vezes que essa atividade é executada, os resultados das execuções anteriores são excluídos. Isso permite direcionar somente elementos novos. [Leia mais](../workflows/activities/incremental-query.md)

**Modelos de notificação por push avançada**

Agora é possível enviar notificações por push avançadas via Android. A notificação por push avançada é uma forma aprimorada de notificação em dispositivos móveis que vai além de simples mensagens de texto, incorporando elementos multimídia, como imagens, botões interativos ou outros conteúdos de mídia avançada. [Leia mais](../push/rich-push.md)

Observe que esse recurso está em **Disponibilidade limitada** (LA).


### Novos recursos em Disponibilidade limitada {#acs-24-4}

>[!AVAILABILITY]
>
>Os seguintes recursos estão em Disponibilidade limitada (LA). Eles estão restritos a clientes que estão migrando **do Adobe Campaign Standard para o Adobe Campaign v8** e não podem ser implantados em nenhum outro ambiente.
>
>Consulte as seguintes páginas de documentação: [Transição do Campaign Standard para o Campaign v8](../rn/acs-migration.md) e [Recursos para usuários do Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=pt-BR).

* **Marca**: como usuário migrado do Campaign Standard, seus administradores técnicos agora podem definir uma ou várias marcas para centralizar os parâmetros que afetam a identidade de uma marca. Isso inclui o logotipo da marca, o domínio do URL de acesso da página de destino ou as configurações de rastreamento de mensagens. Você pode criar essas marcas e vinculá-las a mensagens ou páginas de destino. Essa configuração é gerenciada nos modelos. [Leia mais](../administration/branding/branding-gs.md)

* **APIs REST**: como um usuário migrado do Campaign Standard, você pode usar as APIs REST para criar integrações com o Adobe Campaign e criar seu próprio ecossistema, conectando o Adobe Campaign ao painel de tecnologias que você usa. [Leia mais](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=pt-BR)

* **Relatórios dinâmicos**: como um usuário migrado do Campaign Standard, você pode acessar os relatórios dinâmicos, que fornecem relatórios totalmente personalizáveis e em tempo real para medir o impacto de suas atividades de marketing. Eles adicionam acesso aos dados do perfil, permitindo análises demográficas por dimensões do perfil, como gênero, cidade e idade, além de dados funcionais de campanhas de email, como aberturas e cliques. [Leia mais](../reporting/dynamic-reporting/get-started-reporting.md)

* **Páginas de destino**: as seguintes melhorias nas páginas de destino estão disponíveis apenas para usuários em transição do Campaign Standard:

   * Agora você pode fazer referência a uma página de destino de assinatura/cancelamento de assinatura padrão ao configurar um serviço. Ao criar um email, se você definir um link para essa página de destino, os usuários que enviarem o formulário da página de destino automaticamente assinarão ou cancelarão a assinatura desse serviço. [Leia mais](../audience/manage-services.md#create-service)
   * Uma nova opção na configuração da página de destino permite que visitantes anônimos acessem-na. Se você desmarcar esta opção, apenas usuários identificados poderão acessar e enviar o formulário. [Leia mais](../landing-pages/create-lp.md#create-landing-page)
   * Uma nova opção na configuração da página de destino permite armazenar dados internos adicionais quando a página de destino está sendo enviada. [Leia mais](../landing-pages/create-lp.md#create-landing-page)
   * Uma nova opção permite utilizar uma página de destino para diversos serviços, tornando-a dinâmica. Ao adicionar um link a um email, se você selecionar uma página de destino dinâmica, poderá selecionar qualquer serviço. Se você selecionar uma página de destino que tenha um serviço específico associado, esse serviço será utilizado automaticamente (não será possível selecionar outro). [Leia mais](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * O conteúdo condicional agora é compatível com páginas de destino. [Leia mais](../landing-pages/lp-content.md)

### Melhorias gerais {#improvements-24-4}

As melhorias abaixo estão disponíveis para todos os clientes a partir da versão de abril.

* A atividade **Carregar arquivo** foi aprimorada com diversas seções que permitem fazer upload de um arquivo de amostra, gerenciar erros e rejeições e excluir arquivos enviados após a execução da atividade. [Leia mais](../workflows/activities/load-file.md)


* Agora você pode **copiar/colar atividades** de um fluxo de trabalho para outro a partir de uma guia diferente do navegador. [Leia mais](../workflows/orchestrate-activities.md#copy-activities-copy)

* Todas as atividades de fluxo de trabalho agora permitem gerenciar suas **opções de execução**. Isso permite definir o modo de execução e o comportamento da atividade em caso de erros. [Leia mais](../workflows/orchestrate-activities.md#execution-options-execution)

* A opção “Não ativar a transição se a população estiver vazia” na **Atividade Divisão** permite escolher se o fluxo de trabalho deve fazer a transição para a próxima atividade quando o resultado do segmento estiver vazio. [Leia mais](../workflows/activities/split.md)

## Notas de versão de março {#24-3-release}

>[!AVAILABILITY]
>
>Esta versão está disponível para todos os usuários a partir do [Campaign (console) v8.6](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=pt-BR). Saiba mais sobre lançamentos e atualizações do console do cliente do Adobe Campaign na [documentação do Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=pt-BR){target="_blank"}.

**Data de lançamento**: 19 a 20 de março de 2024

### Canal de correspondência direta {#24-3-dm}

O canal de **Correspondência direta** agora está disponível para uso em fluxos de trabalho e como entregas independentes. A correspondência direta é um canal offline que permite criar, personalizar e gerar arquivos de extração e compartilhá-los com seus provedores de correspondência direta para enviar emails a seus clientes.

### Nova atividade de fluxo de trabalho Alterar fonte de dados {#24-3-change-data-source}

A atividade de direcionamento **Alterar fonte de dados** permite alterar a fonte de dados de uma tabela de trabalho do fluxo de trabalho. Essa atividade oferece mais flexibilidade, permitindo gerenciar dados em seus diferentes bancos de dados e melhorar o desempenho.

### Melhoria da atividade do fluxo de trabalho Divisão {#24-3-split}

Agora é possível usar a opção **Gerar todos os subconjuntos na mesma tabela** na atividade de fluxo de trabalho **Divisão** para agrupar todos os subconjuntos em uma única transição de saída.

### Modelador de consulta {#24-3-query-modeler}

* O modelador de consultas agora está disponível para uso no Designer de email. Isso permite criar condições ao criar conteúdo condicional. 
* Os valores predefinidos agora estão disponíveis para atributos do tipo de data ao criar uma condição personalizada. 
* Os operadores não podem mais ser adicionados em uma nova transição no diagrama. Eles só podem ser adicionados a uma transição já existente antes de filtrar os componentes para agrupá-los. 