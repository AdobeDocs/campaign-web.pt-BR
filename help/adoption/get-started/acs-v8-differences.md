---
title: Diferenças entre o Campaign Standard e o Campaign v8
description: Saiba o que muda ao fazer a transição do Campaign Standard para o Campaign v8 e onde encontrar os detalhes
hide: true
robots: noindex
googlebot: noindex
role: User, Admin, Developer
level: Beginner
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
source-git-commit: 11cf5f2a6e3e77d0747a0b88758ce3fe871e66fd
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 2%
---
# Diferenças entre o Campaign Standard e o Campaign v8 {#acs-v8-differences}

A maioria dos conceitos é a mesma no Campaign Standard e no Campaign v8. Esta página reúne as diferenças que afetam você após a transição e os links para a página que explica cada uma. Ele complementa os guias para [profissionais de marketing](marketers.md) e para [administradores e desenvolvedores](admin-developers.md).

* Para conhecer as alterações de terminologia, consulte [Principais diferenças entre o Campaign Standard e o Campaign v8](overview.md#experiences).
* Para que as verificações sejam executadas e os problemas relatados após uma transição, consulte [Verificações e solução de problemas após a transição](post-transition-checks.md).
* Para os recursos que estão disponíveis somente no console do cliente, consulte [Console do cliente do Campaign Web e do Campaign](../../v8/get-started/capability-matrix.md).

## Canais e conteúdo {#channels}

As etapas para criar e enviar mensagens são semelhantes nos dois produtos, conforme descrito no [guia para profissionais de marketing](marketers.md). As diferenças abaixo estão relacionadas à disponibilidade do canal, deliveries de teste, landing pages e workflows de mala direta.

| O que muda | Saiba mais |
|---|---|
| O canal no aplicativo não está disponível no Campaign v8. | [Canal no aplicativo](marketers.md#acs-gs-marketers-in-app) |
| Para fazer a transição de workflows e deliveries por push existentes, entre em contato com o Gerente de transição da Adobe Campaign. | [Notificações por push](marketers.md#acs-gs-marketers-push) |
| No Campaign Standard, um perfil de teste pode ser marcado como uma **Trap** para receber o envio final. No Campaign v8, habilite a opção para incluir perfis de teste no público-alvo principal do delivery. | [Testar entregas](../../v8/preview-test/test-deliveries.md) |
| As landing pages criadas na interface da Web do Campaign não são compatíveis com campos de entrada ocultos ou JavaScript personalizados. | [Páginas de destino](../../v8/landing-pages/get-started-lp.md) |
| No Campaign Standard, a transição de saída de uma atividade de correspondência direta também carregava o arquivo gerado. No Campaign v8, ele carrega somente a população direcionada. Para enviar o arquivo a um servidor, adicione uma atividade **Extração de dados** e depois uma atividade **Transferência de arquivos**. | [Correspondência direta](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |

## Públicos, fluxos de trabalho e entregas {#data-and-workflows}

Essas diferenças afetam os públicos-alvo e os fluxos de trabalho migrados do Campaign Standard, algumas opções de entregas recorrentes e da atividade **Transferência de arquivos**, além do escopo dos relatórios dinâmicos.

| O que muda | Saiba mais |
|---|---|
| Os públicos-alvo são transformados durante a transição. Por exemplo, os públicos-alvo criados com a atividade Query se tornam filtros predefinidos e os públicos-alvo do tipo file se tornam públicos-alvo do tipo List sem dimensões. | [Gerenciar públicos-alvo](marketers.md#acs-gs-marketers-audiences) |
| Os logs históricos de workflows executados no Campaign Standard não são migrados. | [Criar um fluxo de trabalho](marketers.md#acs-gs-marketers-wf) |
| No Campaign Standard, você pode selecionar o período de agregação de um email recorrente. Essa opção não está disponível no Campaign v8. | [Atividades de canal](../../v8/workflows/activities/channels.md) |
| No Campaign Standard, a atividade **Transferência de arquivos** pode classificar arquivos alfanumericamente. Essa opção não está disponível no Campaign v8. | [Transferir arquivo](../../v8/workflows/activities/transfer-file.md) |
| Os relatórios dinâmicos abrangem entregas de email, campanhas com entregas de email e mensagens transacionais. | [Relatórios](marketers.md#acs-gs-marketers-reporting) |

## Acesso e segurança {#access}

Os grupos de segurança, as funções e as unidades organizacionais do Campaign Standard são mapeados para grupos de operadores, direitos nomeados e permissões de pasta durante a transição. Analise os pontos abaixo, em especial se alguns usuários tiverem direitos mais amplos ou mais restritos do que antes.

| O que muda | Saiba mais |
|---|---|
| Os grupos de segurança, as funções e as unidades organizacionais são mapeados para grupos de operadores, direitos nomeados e permissões de pasta. As funções personalizadas não são migradas. | [Gerenciamento de acesso do usuário](user-management-acs.md) |
| Os usuários com a função de **Modelo de Dados**, mas não com a função de **Administração**, recebem acesso de **Administração**. | [Gerenciamento de acesso do usuário](user-management-acs.md#migration-approach-from-user-roles-to-named-rights) |
| Os usuários atribuídos a grupos de segurança com unidades organizacionais paralelas podem ter acesso mais amplo no Campaign v8. | [Atribuição de unidade organizacional paralela](user-management-acs.md#parallel-assignments) |
| O acesso a APIs transacionais a partir da instância de execução requer um novo perfil de produto. | [Mapeamento de perfil de produto](user-management-acs.md#product-profile-mapping-to-access-rest-apis) |
| As solicitações de privacidade podem chegar ao Campaign Standard e ao Campaign v8 durante o período em que o ambiente do Campaign Standard permanece ativo. | [Privacidade e consentimento](admin-developers.md#privacy-and-consent) |

## Administração, rastreamento e mirror pages {#admin-tracking}

Essas diferenças afetam os deliveries enviados do Campaign Standard antes da transição e as informações administrativas que não são transferidas para o Campaign v8.

| O que muda | Saiba mais |
|---|---|
| As mirror pages dos deliveries enviados do Campaign Standard antes da transição não estão disponíveis. As mirror pages dos deliveries enviados do Campaign v8 funcionam como de costume. | [Mirror pages](../../v8/email/mirror-page.md) |
| Os dados de rastreamento de deliveries transacionais em tempo real enviados do Campaign Standard antes da transição não são capturados no Campaign v8. Os links dessas mensagens ainda são redirecionados. | [Monitorar mensagens transacionais](../../v8/transactional-messaging/monitor-transactional.md) |
| As configurações de URL rastreado de deliveries de rascunho não são mantidas. Após a transição, os links de rastreamento, mirror page e subscrição seguem o padrão do Campaign v8 e os links são rastreados por padrão. | [Adicionar links e rastrear mensagens](../../v8/email/message-tracking.md) |
| As unidades geográficas não estão disponíveis. O controle de acesso com base em unidades geográficas é perdido. | [Controle de acesso](../../v8/get-started/connect-to-campaign.md#access-control) |
| As informações de entidades **Criado por** e **Modificado por** não estão disponíveis após a transição. | [Trilha de auditoria](admin-developers.md#acs-gs-admin-audit-trail) |
| Os URLs do subdomínio de marca são ajustados para o padrão do Campaign v8. As configurações de marca não padrão não são migradas e são fornecidas por meio da marca padrão. | [Identidade visual](../../v8/administration/branding/branding-gs.md) |

## APIs e integrações {#apis-and-integrations}

Essas diferenças afetam as integrações que chamam o Campaign por meio da REST API e as integrações com outras soluções e ferramentas da Adobe.

| O que muda | Saiba mais |
|---|---|
| Os valores de PKEY são alterados após a migração. Se você armazenar PKEYs fora do Campaign, siga os hrefs retornados pela API. | [REST APIs](admin-developers.md#acs-gs-admin-apis) |
| Alguns campos de perfil migrados, como fuso horário e `ccpaOptOut`, são retornados somente pela API `profileAndServicesExt/profile`. | [REST APIs](admin-developers.md#acs-gs-admin-apis) |
| As integrações do Dreamweaver e do Adobe Experience Platform Data Connector do Campaign Standard não estão disponíveis no Campaign v8. | [Trabalhar com o Campaign e outras soluções da Adobe](../../v8/integrations/integration.md) |
| O Adobe migra suas configurações do Adobe Analytics e do Audience Manager. Você deve configurar os Triggers e as integrações do Adobe Target novamente. | [Gerenciar integrações do Adobe Campaign](admin-developers.md#acs-gs-integrations) |
