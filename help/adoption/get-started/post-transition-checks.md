---
title: Verificações e solução de problemas após a transição para o Campaign v8
description: Saiba o que verificar e como corrigir problemas comuns após a transição do Campaign Standard para o Campaign v8
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
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 8b78a8494223fbcd3def29c955e6171cbb643fef
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 1%
---
# Verificações e solução de problemas após a transição {#post-transition-checks}

Após a transição do Campaign Standard para o Campaign v8, alguns deliveries, fluxos de trabalho e páginas de aterrissagem podem se comportar de forma diferente do esperado. A tabela abaixo lista os sintomas relatados pelos usuários em transição, com a causa e o que fazer. Para obter a lista completa de diferenças, consulte [Diferenças entre o Campaign Standard e o Campaign v8](acs-v8-differences.md).

| Sintoma | Causa e o que fazer | Saiba mais |
|---|---|---|
| Os links em um delivery são URLs diretos e nenhum dado de clique é coletado. | O rastreamento está desativado no delivery ou no template do delivery no qual se baseia. Verifique se **Ativar rastreamento** está habilitado, especialmente nos modelos de suas entregas recorrentes. | [Configurações de rastreamento](../../v8/advanced-settings/delivery-settings.md#tracking-tab) |
| Os recipients que cancelaram a inscrição por meio do método &quot;mailto&quot; List-Unsubscribe não estão em quarentena. | Isso é esperado. Esses recipients não são enviados para quarentena. Elas têm a subscrição cancelada do serviço associado ao delivery ou são adicionadas ao incluo na lista de bloqueios se o delivery não tiver um serviço. Para rastrear esses cancelamentos de assinatura, verifique as assinaturas do serviço ou a seção **Não contatar mais** do perfil. | [Quarentenas](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/quarantines){target="_blank"} |
| Uma landing page não salva um valor calculado por um script ou armazenado em um campo oculto. | As landing pages criadas na interface da Web do Campaign não são compatíveis com campos de entrada ocultos ou JavaScript personalizados. Em vez disso, crie o formulário como um aplicativo web no console do cliente. | [Páginas de destino](../../v8/landing-pages/get-started-lp.md) |
| **A transferência de arquivos** não encontrou o arquivo gerado por uma atividade de correspondência direta. | A transição de saída de uma atividade de correspondência direta carrega a população direcionada, não o arquivo de extração. Adicione uma atividade **Extração de dados** e depois a atividade **Transferência de arquivos**. | [Correspondência direta](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |
| Várias ondas de um delivery são enviadas juntas. | As ondas são programadas a partir da data de contato da entrega. Se a entrega começar após o tempo planejado de algumas ondas, essas ondas serão enviadas juntas, em vez de serem espaçadas. | [Enviar usando ondas](../../v8/advanced-settings/send-using-waves.md) |
| Uma máscara de arquivo com caracteres após o asterisco não encontra nenhum arquivo no Azure Blob Storage. | O Azure Blob Storage filtra os arquivos por prefixo de nome. Somente um asterisco à direita é suportado. | [Transferir conta externa](../../v8/administration/transfer-external-account.md) |
| Uma página de aterrissagem ou bloco de conteúdo que usa JavaScript personalizado se comporta de forma diferente. | O JavaScript personalizado é transformado durante a migração, mas você pode validá-lo e ajustá-lo, principalmente se ele usar `queryDef`, APIs do Campaign JavaScript, gravações de sessão, manuseio de unidade organizacional ou geração de URL personalizado. | [Páginas de destino](../../v8/landing-pages/get-started-lp.md) |
| Uma chamada à API REST retorna um valor em branco, um erro ou uma resposta inesperada. | Alguns campos do banco de dados são descartados durante a migração e retornam valores em branco. Um PATCH vazio retorna 204, e um PATCH no local retorna 500. Um POST com um recurso vinculado ignora o link ou retorna um erro. Um PKEY inválido retorna 404. | [Limitações da API REST](acs-v8-differences.md#rest-api-limitations) |
| Uma PKEY armazenada não funciona mais em chamadas de API. | Os valores de PKEY são alterados após a migração. Não os armazene fora do Campaign. De cada chamada do hrefs retornado pela chamada anterior. | [Uso da chave](acs-v8-differences.md#key-usage) |
| Fuso horário ou `ccpaOptOut` ausente em uma resposta de perfil. | Estes campos são retornados somente por `profileAndServicesExt/profile`, não por `profileAndServices/profile`. Chame o endpoint estendido. | [Fuso horário do perfil e ccpaOptOut](acs-v8-differences.md#profile-timezone) |
| Um filtro personalizado retorna um erro em uma chamada REST API. | No Campaign v8, dê ao filtro um nome no **Nome do filtro no campo API REST** e use esse nome como está na solicitação, sem o prefixo &quot;by&quot;. | [Filtragem](acs-v8-differences.md#rest-filtering) |
| Uma chamada que aciona um sinal externo de fluxo de trabalho não pode criar seu corpo de solicitação. | A API GET do workflow não retorna mais as variáveis do workflow. Crie os parâmetros do corpo da solicitação POST a partir de seu próprio conhecimento do fluxo de trabalho. | [Sinais externos do fluxo de trabalho](acs-v8-differences.md#workflow-signals) |
| O acesso às APIs transacionais é negado. | O acesso a APIs transacionais a partir da instância de execução requer um novo perfil de produto. Revise o mapeamento do perfil de produto de suas contas técnicas. | [Mapeamento de perfil de produto](user-management-acs.md#product-profile-mapping-to-access-rest-apis) |
| Um público-alvo migrado mostra somente o valor mais recente ou um público-alvo de arquivo não tem dimensões. | Isso é esperado. Um filtro predefinido assume somente o valor mais recente após a migração do público-alvo e os públicos-alvo do tipo de arquivo se tornam públicos-alvo do tipo Lista sem dimensões. | [Gerenciar públicos-alvo](marketers.md#acs-gs-marketers-audiences) |
| O histórico de fluxos de trabalho executados no Campaign Standard está vazio. | Os logs históricos de workflows executados no Campaign Standard não são migrados. Os workflows executados no Campaign v8 têm seu próprio histórico e logs. | [Criar um fluxo de trabalho](marketers.md#acs-gs-marketers-wf) |
| Alguns usuários podem ver ou fazer mais do que antes. | Os usuários com a função de **Modelo de Dados**, mas não com a função de **Administração**, têm acesso de **Administração**, e os grupos de segurança com unidades organizacionais paralelas podem ter acesso mais amplo. Revise os grupos de operadores, os direitos nomeados e as permissões de pastas. | [Gerenciamento de acesso do usuário](user-management-acs.md) |
| Um perfil de teste marcado como **Trap** não recebe o envio final. | No Campaign v8, adicione um **Grupo de interceptação** nas configurações de Público-alvo da entrega. | [Grupo de interceptação](../../v8/audience/trap-group.md) |
| Um email recorrente não tem opção de período de agregação. | Essa opção não está disponível no Campaign v8. | [Atividades de canal](../../v8/workflows/activities/channels.md) |
| Os relatórios dinâmicos não mostram dados para um delivery. | Os relatórios dinâmicos abrangem entregas de email, campanhas com entregas de email e mensagens transacionais. | [Relatórios](marketers.md#acs-gs-marketers-reporting) |
