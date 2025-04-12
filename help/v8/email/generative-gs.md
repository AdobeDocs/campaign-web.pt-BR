---
audience: end-user
title: Introdução ao assistente de IA
description: Introdução ao Assistente de IA
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 8%

---

# Trabalhar com o assistente de IA {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Assistente de IA"
>abstract="Depois de criar e personalizar o delivery, use o Assistente de IA para aprimorar o conteúdo. Esse recurso simplifica a personalização e a melhoria do conteúdo, permitindo que você ajuste o conteúdo descrevendo o que deseja gerar."

>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definição do contexto com o assistente de IA no Campaign"
>abstract="Para usar o conteúdo selecionado como entrada para a geração de conteúdo, ative a opção **Aprimorar com conteúdo atual**. Você também pode fazer upload dos ativos da sua marca e usá-los como fonte de conteúdo. Se você não usar o conteúdo selecionado, o upload e a seleção dos ativos da marca são obrigatórios."

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Termos da IA generativa da Adobe"
>abstract="O acesso a esse recurso depende do seu acordo com as Diretrizes de usuário da IA gerativa da Adobe Experience Cloud. Revise qualquer saída desse recurso para precisão e verifique se ele é apropriado para seu caso de uso."
>additional-url="https://www.adobe.com/br/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Diretrizes do usuário da IA generativa da Adobe"

>[!INFO]
>
>Mergulhe em uma experiência prática com a [nossa visualização de recursos ao vivo](https://experienceleague.adobe.com/pt-br/apps/journey-optimizer/ai-assistant-content-accelerator), projetada para permitir que você explore seus recursos em primeira mão e entenda totalmente suas funcionalidades.

À medida que o setor de marketing se torna mais competitivo, as marcas buscam maneiras eficientes de gerar conteúdo impactante rapidamente. O Assistente de IA no Adobe Campaign Web, desenvolvido pelo Microsoft Azure OpenAI e pelo Adobe Firefly, é o recurso de geração de conteúdo de IA da Adobe que transforma a forma como os profissionais de marketing criam conteúdo profissional e consistente com a marca em canais como email, SMS e notificações por push. Com modelos avançados de GenAI e uma profunda compreensão das diretrizes da marca, o Assistente de IA gera automaticamente conteúdo personalizado, envolvente e eficaz com base no objetivo de marketing, otimizando o conteúdo para estilos, layouts, tom e muito mais.

O AI Assistant simplifica a criação e a execução de campanhas de marketing em canais como email, SMS e notificações por push, economizando tempo, melhorando a eficiência e obtendo melhores resultados.

>[!IMPORTANT]
>
>* Antes de usar esse recurso, reveja as [Medidas de Proteção e Limitações](#generative-guardrails) relacionadas.
>
>* Você deve concordar com um [contrato de usuário](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) antes de usar o Assistente de IA no Adobe Campaign Web. Para mais informações, entre em contato com o seu representante da Adobe.

## Acessar o assistente de IA {#generative-access}

O Assistente de IA para emails, notificações por push e SMS agora está em Disponibilidade Geral (GA) e disponível para todos os usuários. As permissões e as etapas necessárias para conceder acesso aos usuários são detalhadas abaixo.

+++ Saiba como atribuir permissões relacionadas à geração de conteúdo

1. **Criar Perfil de Produto** - No [Admin Console](https://stage.adminconsole.adobe.com/), crie um perfil de produto com o seguinte padrão específico:
   `Campaign - <instance-name> - AIAssistant`

1. **Adicionar usuários** - Adicione o usuário necessário a esse perfil de produto,\
   ou\
   **Criar Grupo de Usuários**, adicionar esse grupo de usuários ao perfil de produto e, em seguida, adicionar usuários a esse perfil de produto.

Saiba como definir permissões no Campaign em [esta seção](../get-started/permissions.md).

+++

## Medidas de proteção e limitações {#generative-guardrails}

As diretrizes gerais para o uso do Assistente de IA no Adobe Campaign Web para geração de email estão listadas abaixo:

* A qualidade do conteúdo gerado depende muito do objetivo de marketing ou do prompt definido. Use um prompt bem definido para que o modelo GenAI seja interpretado com precisão.
* Faça upload dos ativos da marca para garantir um conteúdo preciso sobre a marca. Caso contrário, o conteúdo será baseado em informações disponíveis publicamente. O conteúdo carregado pode estar nos seguintes formatos: arquivos PDF, JPEG, PNG ou ZIP (com formatos de arquivo compatíveis).
* O tamanho máximo para os recursos de marca carregados é de 50 MB. Arquivos maiores ou imagens numerosas podem aumentar o tempo de processamento.
* Use [modelos de email integrados](../email/create-email-templates.md), modelos específicos da marca ou modelos personalizados para criar conteúdo de email usando o Assistente de IA. São recomendados modelos de e-mail com até 8 a 10 imagens.
* Relate quaisquer saídas problemáticas usando os ícones de miniatura, miniatura ou sinalizador ao selecionar variantes.
* O uso do Assistente de IA está sujeito às Diretrizes de usuário da IA geradora da Adobe Experience Cloud. [Saiba mais](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html).
* Como parte do compromisso da Adobe com a transparência no uso de ferramentas de IA gerativa na criação de mídia, a Adobe aplica o Content Credentials quando o conteúdo ou um projeto que inclui um ativo gerado pela Firefly é baixado ou exportado. [Saiba mais](https://helpx.adobe.com/firefly/using/content-credentials.html).

As seguintes limitações se aplicam ao Assistente de IA no Adobe Campaign Web:

* No momento, o Assistente de IA no Adobe Campaign Web é compatível somente em inglês. Entradas em outros idiomas podem produzir resultados inconsistentes ou errôneos. Problemas decorrentes de respostas em outros idiomas não serão abordados ou aprimorados neste momento.
* Disponível somente para os canais de email, push e SMS.
* O conteúdo da GenAI pode nem sempre ser preciso. Compartilhe seu feedback para que os engenheiros possam refinar os modelos.
* Você pode fazer upload de vários ativos de marca, mas pode aproveitar apenas um para uma geração específica.

## Recursos de geração de conteúdo do AI Assistant {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="[Geração de email com o Assistente de IA]" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>Geração de email com o Assistente de IA</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="[Geração de SMS com o Assistente de IA]" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-sms.md"><strong>Geração de SMS com o Assistente de IA</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="[Geração de notificação por push com o Assistente de IA]" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>Geração de notificação por push com o Assistente de IA</strong></a>
</div>
<p></td>
</tr></table>