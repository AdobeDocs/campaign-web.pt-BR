---
audience: end-user
title: Introdução ao acelerador de conteúdo do Assistente de IA
description: Introdução ao Acelerador de conteúdo do Assistente de IA
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: 9d022ad4ce9d001d6f5154d2778a538aae560d52
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 29%

---

# Trabalho com o acelerador de conteúdo do Assistente de IA  {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="Acelerador de conteúdo do Assistente de IA"
>abstract="O Assistente de IA facilita a criação e a execução de campanhas de marketing em canais como Email, SMS e Push, tornando-as intuitivas, economizando tempo, melhorando a eficiência e proporcionando melhores resultados."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=pt-BR" text="Consulte as notas de versão"


>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Assistente de IA"
>abstract="Depois de criar e personalizar a entrega, use o assistente de IA para aprimorar o conteúdo. Esse recurso simplifica o processo de personalização e aprimoramento de conteúdo, permitindo ajustar o conteúdo, descrevendo o que deseja gerar."


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definição do contexto com o assistente de IA no Campaign"
>abstract="Para usar o conteúdo selecionado como uma entrada para a geração de conteúdo, ative a opção **Aprimorar com conteúdo atual**. Você também pode fazer upload dos ativos da sua marca e usá-los como fonte de conteúdo. Se você não usar o conteúdo selecionado, será obrigatório fazer o upload e selecionar os ativos de marca."

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Termos da IA generativa da Adobe"
>abstract="O acesso a esse recurso está sujeito à concordância com as Diretrizes do usuário da IA generativa da Adobe Experience Cloud. Analise os resultados deste recurso quanto à precisão e certifique-se de que sejam apropriados ao seu caso de uso."
>additional-url="https://www.adobe.com/br/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Diretrizes do usuário da IA generativa da Adobe"

>[!INFO]
>
>Mergulhe em uma experiência prática com a [nossa visualização de recursos ao vivo](https://experienceleague.adobe.com/pt-br/apps/journey-optimizer/ai-assistant-content-accelerator), projetada para permitir que você explore seus recursos em primeira mão e entenda totalmente suas funcionalidades.


À medida que o setor de marketing se torna mais competitivo, as marcas buscam maneiras eficientes de gerar conteúdo impactante de maneira eficiente e rápida. O Acelerador de conteúdo do assistente de IA no Adobe Campaign Web, viabilizado pelo Microsoft Azure OpenAI e Adobe Firefly, é o recurso de geração de conteúdo de IA de Adobe que revoluciona a forma como os profissionais de marketing criam conteúdo profissional e consistente com a marca em canais como Email, SMS e Push. Com modelos avançados de GenAI e profunda compreensão das diretrizes da marca, o Assistente de IA gera automaticamente conteúdo personalizado, envolvente e eficaz com base no objetivo de marketing com conteúdo otimizado para estilos, layouts, tom e muito mais.

O Assistente de IA facilita a criação e a execução de campanhas de marketing em canais como Email, SMS e Push, tornando-as intuitivas, economizando tempo, melhorando a eficiência e proporcionando melhores resultados.

>[!IMPORTANT]
>
>* Antes de começar a usar esse recurso, leia as [Medidas de Proteção e Limitações](#generative-guardrails) relacionadas.
>
>* Você deve concordar com um [contrato de usuário](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) antes de usar o Acelerador de Conteúdo do Assistente de IA na Web do Adobe Campaign. Para mais informações, entre em contato com o seu representante da Adobe.

## Acesse o Acelerador de conteúdo do assistente de IA {#generative-access}

O Acelerador de conteúdo do assistente de IA para emails, notificações por push e SMS está agora em Disponibilidade geral (GA) e disponível para todos os usuários. As permissões e as etapas necessárias para conceder acesso aos usuários são detalhadas abaixo.

+++  Saiba como atribuir permissões relacionadas à geração de conteúdo

1. **Criar Perfil de Produto** - Em [Admin Console](https://stage.adminconsole.adobe.com/), crie um perfil de produto com o seguinte padrão específico:
   `Campaign - <instance-name> - AIAssistant`

1. **Adicionar usuários** - Adicione o usuário necessário a esse perfil de produto,
ou
   **Criar Grupo de Usuários** e adicionar esse grupo de usuários ao perfil de produto e adicionar usuários a esse perfil de produto.

Saiba como definir permissões no Campaign em [esta seção](../get-started/permissions.md).

+++

## Medidas de proteção e limitações {#generative-guardrails}

As diretrizes gerais para usar o Acelerador de conteúdo do Assistente de IA no Adobe Campaign Web para geração de email estão listadas abaixo:

* A qualidade do conteúdo gerado é fortemente influenciada pelo objetivo/prompt de marketing definido por você. Use um prompt bem definido para que o modelo GenAI seja interpretado com precisão. 
* Faça upload do ativo da marca para ter informações precisas sobre o conteúdo da marca. Caso contrário, o conteúdo será baseado em informações disponíveis publicamente. O conteúdo carregado pode estar nos seguintes formatos: arquivos PDF, JPEG, PNG ou ZIP (com formatos de arquivo compatíveis).
* O tamanho máximo para o ativo de marca carregado é de 50 MB. Arquivos maiores ou muitas imagens podem funcionar, mas o tempo de processamento é aumentado.
* Use [modelos de email internos](../email/create-email-templates.md), modelo específico da marca ou modelo personalizado para criar seu conteúdo de email usando o Acelerador de Conteúdo. Modelos de e-mail com até 8-10 imagens são recomendados.
* Relate quaisquer saídas problemáticas usando os ícones de miniatura para cima, miniatura para baixo ou sinalizador ao selecionar variantes.
* O uso do assistente de IA está sujeito às Diretrizes de usuário da IA gerativa da Adobe Experience Cloud. [Saiba mais](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)
* Adobe Como parte do compromisso de promover a transparência no uso de ferramentas de IA gerativa na criação de mídia, o Adobe aplicará Contents credentials quando o conteúdo ou um projeto que inclui um ativo gerado por Firefly for baixado ou exportado. [Saiba mais](https://helpx.adobe.com/firefly/using/content-credentials.html)

As seguintes limitações se aplicam ao Acelerador de conteúdo do assistente de IA no Adobe Campaign Web:

* O Acelerador de conteúdo do assistente de IA na Web do Adobe Campaign é atualmente suportado somente em inglês. Entradas em outros idiomas podem produzir resultados inconsistentes ou errôneos. Questões decorrentes de respostas em outros idiomas não serão tratadas ou melhoradas no momento.
* Disponível somente para os canais de email, push e SMS.
* O conteúdo da GenAI pode nem sempre ser preciso: compartilhe seu feedback para que nossos engenheiros possam refinar os modelos.
* Você pode fazer upload de vários ativos de marca, mas pode aproveitar apenas um para uma geração específica.

## Recursos de geração de conteúdo do AI Assistant {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="Geração de email" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>Geração de email com o Assistente de IA</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="Geração de SMS" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-sms.md"><strong>Geração de SMS com o Assistente de IA</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="Geração de push" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>Geração de notificação por push com o Assistente de IA</strong></a>
</div>
<p></td>
</tr></table>
