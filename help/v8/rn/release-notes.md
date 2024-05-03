---
title: Notas de versão mais recentes
description: Conheça o novo recurso incluído na interface do Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: f6a1ebcb5a77798f738e2a4ac0b45454d941d7c7
workflow-type: tm+mt
source-wordcount: '1137'
ht-degree: 25%

---

# Notas de versão {#latest-release}

<!--Last update: **March 19, 2024**-->

As versões da interface do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem mais escalável e em fases para a implantação de recursos. Devido a isso, essas notas de versão são atualizadas várias vezes por mês. Verifique-as regularmente.

## Notas de versão de abril {#april-24-4-release}

**Data de lançamento**: 2 de maio de 2024

### Novos recursos {#new-24-4}

Os seguintes recursos estão disponíveis para todos os usuários a partir da versão de abril.

**Novas atividades de fluxo de trabalho**

* **Atualizar dados** - Use esta atividade para executar atualizações em massa nos campos no banco de dados. Várias opções permitem personalizar a atualização de dados. [Leia mais](../workflows/activities/update-data.md)
* **Serviços de assinatura** : use essa atividade para assinar ou cancelar a assinatura de vários perfis para/de um serviço em uma única ação. [Leia mais](../workflows/activities/subscription-services.md)
* **Extrair arquivo** : use essa atividade para exportar dados do Adobe Campaign para outro sistema como um arquivo externo. [Leia mais](../workflows/activities/extract-file.md)
* **Transferir arquivo** : use essa atividade para receber ou enviar arquivos, testar a presença de arquivos ou listar arquivos em um servidor. O protocolo usado pode ser protocolo servidor a servidor ou protocolo HTTP. [Leia mais](../workflows/activities/transfer-file.md)
* **Teste** - Use esta atividade para ativar transições com base em condições especificadas. [Leia mais](../workflows/activities/test.md)
* **Código JavaScript** - Use esta atividade para executar um trecho de código JavaScript no contexto de um workflow. [Leia mais](../workflows/activities/javascript-code.md)
* **Sinal externo** : use essa atividade para acionar a execução de um workflow a partir de outro workflow ou uma chamada de API. [Leia mais](../workflows/activities/external-signal.md)
* **Query incremental** : use essa atividade para consultar o banco de dados de forma programada. Todas as vezes que essa atividade é executada, os resultados das execuções anteriores são excluídos. Isso permite direcionar somente elementos novos. [Leia mais](../workflows/activities/incremental-query.md)

**Modelos avançados de notificação por push**

Agora você pode enviar notificações por push avançadas via Android. A notificação por push avançada é uma forma aprimorada de notificação por dispositivos móveis que vai além das mensagens de texto simples, incorporando elementos multimídia, como imagens, botões interativos ou outro conteúdo de mídia avançada. [Leia mais](../push/rich-push.md)

Observe que esse recurso está em **Disponibilidade limitada** (L-A).

<!--
* **Audit Trail**

The Audit trail feature constantly records a detailed log of actions and events taking place within the Adobe Campaign instance in real-time. It offers a convenient method to access a chronological record of data, addressing queries such as: the status of workflows, the latest individuals to modify them, or the activities performed by users within the instance.
-->

### Novos recursos em disponibilidade limitada {#acs-24-4}

>[!AVAILABILITY]
>
>Os recursos a seguir estão na Disponibilidade Limitada (DL). Eles são restritos aos clientes que estão migrando **do Adobe Campaign Standard para o Adobe Campaign v8** e não podem ser implantados em nenhum outro ambiente.
>
>Consulte as seguintes páginas de documentação: [Transição de Campaign Standard para o Campaign v8](../rn/acs-migration.md) e [Recursos para usuários do Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html).

* **Marcas** - Como usuário migrado do Campaign Standard, os administradores técnicos agora podem definir uma ou várias marcas para centralizar os parâmetros que afetam a identidade de uma marca. Isso inclui o logotipo da marca, o domínio do URL de acesso da landing page ou as configurações de rastreamento de mensagens. Você pode criar essas marcas e vinculá-las a mensagens ou páginas de aterrissagem. Essa configuração é gerenciada em modelos. [Leia mais](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html)

* **Rest APIs** - Como usuário migrado do Campaign Standard, você pode usar as APIs Rest para criar integrações com o Adobe Campaign e criar seu próprio ecossistema, conectando o Adobe Campaign ao painel de tecnologias que você usa. [Leia mais](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html)

* **Relatórios dinâmicos** - Como um usuário migrado de Campaign Standard, você pode acessar o Dynamic Reporting, que fornece relatórios totalmente personalizáveis e em tempo real para medir o impacto de suas atividades de marketing. Ele adiciona acesso aos dados do perfil, permitindo a análise demográfica por dimensões de perfil, como gênero, cidade e idade, além de dados funcionais de campanha de email, como aberturas e cliques. [Leia mais](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html)

* **Landing Pages** - As seguintes melhorias nas páginas de aterrissagem só estão disponíveis para usuários que estão fazendo a transição do Campaign Standard:

   * Agora você pode fazer referência a uma landing page padrão de subscrição/unsubscription ao configurar um serviço. Ao criar um email, se você definir um link para essa página de aterrissagem, os usuários que enviam o formulário da página de aterrissagem farão a assinatura desse serviço ou a cancelarão. [Leia mais](../audience/manage-services.md#create-service)
   * Uma nova opção na configuração da landing page permite que visitantes anônimos acessem a landing page. Se você desmarcar essa opção, somente os usuários identificados poderão acessar e enviar o formulário. [Leia mais](../landing-pages/create-lp.md#create-landing-page)
   * Uma nova opção na configuração da landing page permite armazenar dados internos adicionais quando a landing page estiver sendo enviada. [Leia mais](../landing-pages/create-lp.md#create-landing-page)
   * Uma nova opção permite usar uma landing page para vários serviços, tornando-a dinâmica. Ao adicionar um link a um email, se você selecionar uma landing page dinâmica, poderá selecionar qualquer serviço. Se você selecionar uma landing page que tenha um serviço específico associado, esse serviço será usado automaticamente (não é possível selecionar outro). [Leia mais](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * O conteúdo condicional agora é compatível com landing pages. [Leia mais](../landing-pages/lp-content.md)

### Melhorias gerais {#improvements-24-4}

Os aprimoramentos abaixo estão disponíveis para todos os clientes a partir da versão de abril.
<!--**Workflow - Copy/Paste into another tab**: -->

* A variável **Carregar arquivo** A atividade de foi aprimorada com várias seções, que permitem fazer upload de um arquivo de amostra, gerenciar erros e rejeições e excluir arquivos carregados após a execução da atividade. [Leia mais](../workflows/activities/load-file.md)


* Agora você pode **atividades de copiar/colar** de um workflow para outro workflow a partir de uma guia do navegador diferente. [Leia mais](../workflows/orchestrate-activities.md#copy-activities-copy)

<!--**Workflow - Execution options**: -->

* Todas as atividades do workflow agora permitem gerenciar seus **opções de execução**. Isso permite definir o modo de execução e o comportamento da atividade em caso de erros. [Leia mais](../workflows/orchestrate-activities.md#execution-options-execution)

<!-- **Workflow - Split Activity - Support Skipping Empty Transition**: -->

* A opção &quot;Do not ativate the transition if the population is empty&quot; no **Dividir atividade** permite escolher se o workflow deve passar para a próxima atividade quando o resultado do segmento estiver vazio. [Leia mais](../workflows/activities/split.md)

<!--* **Support of custom fields**-->

* **Campos personalizados** são atributos adicionais adicionados aos esquemas prontos para uso por meio do console do Adobe Campaign. Na interface da Web do Campaign, esses campos personalizados agora estão visíveis em várias telas, por exemplo, os detalhes de um perfil ou perfil de teste. Na interface do usuário da Web, não é possível criar campos personalizados, mas agora é possível modificar a forma como eles são exibidos. [Leia mais](../administration/custom-fields.md)


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

Agora você pode usar o **Gerar todos os subconjuntos na mesma tabela** opção no **Split** atividade de workflow para agrupar todos os subconjuntos em uma única transição de output.

### Modelador de consulta {#24-3-query-modeler}

* O modelador de consultas agora está disponível para uso no Designer de email. Ele permite criar condições ao criar conteúdo condicional.
* Os valores predefinidos agora estão disponíveis para atributos de tipo de data ao criar uma condição personalizada.
* Os operadores não podem mais ser adicionados em uma nova transição no diagrama. Eles só podem ser adicionados em uma transição existente antes de filtrar componentes para agrupá-los.
