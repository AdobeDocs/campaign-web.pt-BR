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
source-git-commit: 11cf5f2a6e3e77d0747a0b88758ce3fe871e66fd
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 1%
---
# Verificações e solução de problemas após a transição {#post-transition-checks}

Após a transição do Campaign Standard para o Campaign v8, alguns deliveries, fluxos de trabalho e páginas de aterrissagem podem se comportar de forma diferente do esperado. A tabela abaixo lista os sintomas relatados pelos usuários em transição, com a causa e o que fazer. Para obter a lista completa de diferenças, consulte [Diferenças entre o Campaign Standard e o Campaign v8](acs-v8-differences.md).

| Sintoma | Causa e o que fazer | Saiba mais |
|---|---|---|
| Os links em um delivery são URLs diretos e nenhum dado de clique é coletado. | O rastreamento está desativado no delivery ou no template do delivery no qual se baseia. Verifique se **Ativar rastreamento** está habilitado, especialmente nos modelos de suas entregas recorrentes. | [Configurações de rastreamento](../../v8/advanced-settings/delivery-settings.md#tracking-tab) |
| Os recipients que cancelaram a inscrição por meio do método &quot;mailto&quot; List-Unsubscribe não estão em quarentena. | Isso é esperado. Esses recipients não são enviados para quarentena. Elas têm a subscrição cancelada do serviço associado ao delivery ou são adicionadas ao incluo na lista de bloqueios se o delivery não tiver um serviço. Para rastrear esses cancelamentos de assinatura, verifique as assinaturas do serviço ou a seção **Não contatar mais** do perfil. | [Quarentenas](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/send/failures/quarantines){target="_blank"} |
| Uma landing page não salva um valor calculado por um script ou armazenado em um campo oculto. | As landing pages criadas na interface da Web do Campaign não são compatíveis com campos de entrada ocultos ou JavaScript personalizados. Em vez disso, crie o formulário como um aplicativo web no console do cliente. | [Páginas de destino](../../v8/landing-pages/get-started-lp.md) |
| **A transferência de arquivos** não encontrou o arquivo gerado por uma atividade de correspondência direta. | A transição de saída de uma atividade de correspondência direta carrega a população direcionada, não o arquivo de extração. Adicione uma atividade **Extração de dados** e depois a atividade **Transferência de arquivos**. | [Correspondência direta](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |
| Várias ondas de um delivery são enviadas juntas. | As ondas são programadas a partir da data de contato da entrega. Se a entrega começar após o tempo planejado de algumas ondas, essas ondas serão enviadas juntas, em vez de serem espaçadas. | [Enviar usando ondas](../../v8/advanced-settings/send-using-waves.md) |
| Uma máscara de arquivo com caracteres após o asterisco não encontra nenhum arquivo no Azure Blob Storage. | O Azure Blob Storage filtra os arquivos por prefixo de nome. Somente um asterisco à direita é suportado. | [Transferir conta externa](../../v8/administration/transfer-external-account.md) |
| Uma mirror page de um delivery enviado antes da transição não é aberta. | As mirror pages dos deliveries enviados do Campaign Standard antes da transição não estão disponíveis e não há solução alternativa. As mirror pages dos deliveries enviados do Campaign v8 funcionam como de costume. | [Mirror pages](../../v8/email/mirror-page.md) |
| Uma página de aterrissagem ou bloco de conteúdo que usa JavaScript personalizado se comporta de forma diferente. | O JavaScript personalizado é transformado durante a migração, mas você pode validá-lo e ajustá-lo, principalmente se ele usar `queryDef`, APIs do Campaign JavaScript, gravações de sessão, manuseio de unidade organizacional ou geração de URL personalizado. | [Páginas de destino](../../v8/landing-pages/get-started-lp.md) |
