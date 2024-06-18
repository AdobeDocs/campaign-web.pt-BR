---
title: Notas de versão da interface do Campaign Web v8
description: Conheça os novos recursos que acompanham a versão mais recente da interface do Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: f9b8c0805d816075c5ee9ea9443f50cfead371d1
workflow-type: tm+mt
source-wordcount: '1623'
ht-degree: 90%

---

# Notas de versão {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de versão"
>abstract="As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, as notas de versão do Campaign são atualizadas várias vezes por mês, com os recursos, melhorias e correções mais recentes. Recomendamos que você as verifique regularmente."

As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, essas notas de versão são atualizadas várias vezes por mês. Verifique-as regularmente.

## Notas de versão de junho {#24-6-release}

**Data de lançamento**: 18 a 19 de junho de 2024

Os seguintes recursos e melhorias estão disponíveis para todos os usuários a partir da versão de junho.
<!--
### Visual fragments {#24-6-1}

You can now author, use, and manage **visual** fragments to quickly assemble your emails and content templates. A fragment is a prebuilt reusable component that can be referenced in multiple emails across Adobe Campaign for an improved and accelerated design process.

### Seed lists {#24-6-2}

A seed list, aka. **Trap group**, is a list of seed addresses. It is used to include specific addresses in your deliveries, and then target profiles who do not match the defined target criteria. This way, recipients who are out of the delivery audience can receive the delivery, as any other target recipient would. You can use seed addresses when sending proofs, or to protect your mailing list.-->

### Alertas de entrega {#24-6-3}

O recurso de Alerta de delivery é um sistema de gerenciamento de alertas que permite que um grupo de usuários receba automaticamente notificações contendo informações sobre a execução de seus deliveries. [Leia mais](../msg/delivery-alerting.md)

### Planos e programas {#24-6-4}

Agora você pode criar planos e programas para organizar suas campanhas. Ao definir uma hierarquia de pastas, você pode organizar suas campanhas em programas e os programas em planos. [Leia mais](../msg/delivery-alerting.md)

### Aprimoramentos {#improvements-24-6}

* **Reconciliação na atividade de Enriquecimento**: a atividade Enrichment agora pode ser usada para reconciliar dados do schema de banco de dados do Campaign com dados de outro schema ou com dados provenientes de um schema temporário, como dados carregados usando uma atividade Load file. Por exemplo, você pode usar essa opção para reconciliar o país de um perfil, especificado em um arquivo carregado, com um dos países disponíveis na tabela dedicada do banco de dados do Campaign. [Leia mais](../workflows/activities/enrichment.md)

## Notas da versão de maio {#24-5-release}

**Data de lançamento**: 21 de maio de 2024

Os seguintes recursos e melhorias estão disponíveis para todos os usuários a partir da versão de maio.

### Trilha de auditoria  {#24-5-1}

O novo recurso de **Trilha de auditoria** fornece um registro detalhado e cronológico de todas as ações e eventos realizados em sua instância do Adobe Campaign em tempo real. Esse recurso oferece um método conveniente para rastrear todas as alterações nos dados do Campaign, abordando consultas como: status dos fluxos de trabalho, últimos indivíduos que os modificaram ou atividades realizadas pelos usuários na instância. [Leia mais](../reporting/audit-trail.md)

### Campos personalizados {#24-5-2}

**Os campos personalizados** são outros atributos adicionados aos esquemas prontos para uso por meio do console do Adobe Campaign. Na interface do Campaign Web, esses campos personalizados agora ficam visíveis em diversas telas. Por exemplo, os detalhes de um perfil ou de um perfil de teste. Na interface web, você não pode criar campos personalizados, mas agora pode modificar a forma como eles são exibidos. [Leia mais](../administration/custom-fields.md)

### Crie links entre tabelas {#24-5-3}

Agora você pode criar links com outra tabela na atividade de fluxo de trabalho **Enriquecimento**. Use a nova seção **Definição de link** nos parâmetros de atividade para criar um link entre os dados da tabela de trabalho e o banco de dados do Adobe Campaign. Por exemplo, ao carregar dados de um arquivo que contenha o número da conta, o país e o email dos destinatários, agora é possível criar um link para a tabela do país para atualizar essas informações em seus perfis. [Leia mais](../workflows/activities/enrichment.md#create-links)

<!--
### Content fragments {#24-5-4}

* You can now author, use, and save **visual fragments** to quickly assemble your emails and content templates. A fragment is a prebuilt reusable component that can be referenced in multiple emails across Adobe Campaign for an improved and accelerated design process. [Learn more](../email/fragments.md)

* You can now author, use, and manage **expression fragments** to quickly build personalized content. A fragment is a prebuilt reusable component that can be referenced in multiple contents across Adobe Campaign for an improved and accelerated design process.-->


### Melhorias gerais {#improvements-24-5}

* **Correspondência direta**: agora você pode aproveitar o editor de expressão para selecionar os atributos a serem exibidos nos arquivos de extração de correspondência direta. [Leia mais](../direct-mail/content-direct-mail.md)

* **Gerenciamento de pastas**: agora é possível criar uma subpasta de um tipo diferente da pasta principal. [Leia mais](../get-started/permissions.md#folders)


<!--* **Execution options for workflows** - You can now define execution options for your workflows, such as the maximum duration, the affinity, or the time zone.-->

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

* **Marca**: como usuário migrado do Campaign Standard, seus administradores técnicos agora podem definir uma ou várias marcas para centralizar os parâmetros que afetam a identidade de uma marca. Isso inclui o logotipo da marca, o domínio do URL de acesso da página de destino ou as configurações de rastreamento de mensagens. Você pode criar essas marcas e vinculá-las a mensagens ou páginas de destino. Essa configuração é gerenciada em modelos. [Leia mais](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=pt-BR)

* **APIs REST**: como um usuário migrado do Campaign Standard, você pode usar as APIs REST para criar integrações com o Adobe Campaign e criar seu próprio ecossistema, conectando o Adobe Campaign ao painel de tecnologias que você usa. [Leia mais](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=pt-BR)

* **Relatórios dinâmicos**: como um usuário migrado do Campaign Standard, você pode acessar os relatórios dinâmicos, que fornecem relatórios totalmente personalizáveis e em tempo real para medir o impacto de suas atividades de marketing. Eles adicionam acesso aos dados do perfil, permitindo análises demográficas por dimensões do perfil, como gênero, cidade e idade, além de dados funcionais de campanha de email, como aberturas e cliques. [Leia mais](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html?lang=pt-BR)

* **Páginas de destino**: as seguintes melhorias nas páginas de destino estão disponíveis apenas para usuários em transição do Campaign Standard:

   * Agora você pode fazer referência a uma página de destino de assinatura/cancelamento de assinatura padrão ao configurar um serviço. Ao criar um email, se você definir um link para essa página de destino, os usuários que enviarem o formulário da página de destino automaticamente assinarão ou cancelarão a assinatura desse serviço. [Leia mais](../audience/manage-services.md#create-service)
   * Uma nova opção na configuração da página de destino permite que visitantes anônimos acessem-na. Se você desmarcar esta opção, apenas usuários identificados poderão acessar e enviar o formulário. [Leia mais](../landing-pages/create-lp.md#create-landing-page)
   * Uma nova opção na configuração da página de destino permite armazenar dados internos adicionais quando a página de destino está sendo enviada. [Leia mais](../landing-pages/create-lp.md#create-landing-page)
   * Uma nova opção permite utilizar uma página de destino para diversos serviços, tornando-a dinâmica. Ao adicionar um link a um email, se você selecionar uma página de destino dinâmica, poderá selecionar qualquer serviço. Se você selecionar uma página de destino que tenha um serviço específico associado, esse serviço será utilizado automaticamente (não será possível selecionar outro). [Leia mais](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * O conteúdo condicional agora é compatível com páginas de destino. [Leia mais](../landing-pages/lp-content.md)

### Melhorias gerais {#improvements-24-4}

As melhorias abaixo estão disponíveis para todos os clientes a partir da versão de abril.
<!--**Workflow - Copy/Paste into another tab**: -->

* A atividade **Carregar arquivo** foi aprimorada com diversas seções que permitem fazer upload de um arquivo de amostra, gerenciar erros e rejeições e excluir arquivos enviados após a execução da atividade. [Leia mais](../workflows/activities/load-file.md)


* Agora você pode **copiar/colar atividades** de um fluxo de trabalho para outro a partir de uma guia diferente do navegador. [Leia mais](../workflows/orchestrate-activities.md#copy-activities-copy)

<!--**Workflow - Execution options**: -->

* Todas as atividades de fluxo de trabalho agora permitem gerenciar suas **opções de execução**. Isso permite definir o modo de execução e o comportamento da atividade em caso de erros. [Leia mais](../workflows/orchestrate-activities.md#execution-options-execution)

<!-- **Workflow - Split Activity - Support Skipping Empty Transition**: -->

* A opção “Não ativar a transição se a população estiver vazia” na **Atividade Divisão** permite escolher se o fluxo de trabalho deve fazer a transição para a próxima atividade quando o resultado do segmento estiver vazio. [Leia mais](../workflows/activities/split.md)



## Notas de versão de março {#24-3-release}

>[!AVAILABILITY]
>
>Esta versão está disponível para todos os usuários a partir do [Campaign (console) v8.6](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=pt-BR). Saiba mais sobre as versões e atualizações do console do cliente do Adobe Campaign na [documentação do Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=pt-BR){target="_blank"}.

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
