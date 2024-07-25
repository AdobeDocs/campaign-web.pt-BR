---
audience: end-user
title: Introdução ao assistente de IA
description: Introdução ao Assistente de IA
badge: label="Beta"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
hide: true
hidefromtoc: true
source-git-commit: 7de6d85036eac7289e7fcf3a82a7c11be12d9c6e
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 32%

---

# Introdução ao assistente de IA {#generative-gs}

>[!BEGINSHADEBOX]

**Índice**

* Introdução ao assistente de IA
* [Geração de email com o Assistente de IA](generative-content.md)
* [Geração de SMS com o Assistente de IA](generative-sms.md)
* [Geração de notificação por push com o Assistente de IA](generative-push.md)

>[!ENDSHADEBOX]

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

À medida que o setor de marketing se torna mais competitivo, as marcas buscam maneiras eficientes de gerar conteúdo impactante de maneira eficiente e rápida. O Assistente de IA no Campaign, viabilizado pelo Azure OpenAI, é um recurso de geração de conteúdo de IA de Adobe que revoluciona a maneira como os profissionais de marketing criam conteúdo profissional e consistente com a marca em canais como Email, SMS e Push. Com modelos avançados de GenAI e profunda compreensão das diretrizes da marca, o Assistente de IA gera automaticamente conteúdo personalizado, envolvente e eficaz com base no objetivo de marketing com conteúdo otimizado para estilos, layouts, tom e muito mais.

O AI Assistant torna a criação e a execução de campanhas de marketing em canais como Email, SMS e Push intuitivas, simples e sem complicações, economizando tempo, melhorando a eficiência e obtendo melhores resultados.

>[!NOTE]
>
>Esse recurso está disponível na versão para Beta e está sujeito a alterações sem aviso prévio.

## Medidas de proteção e limitações {#generative-guardrails}

As diretrizes gerais para usar o Assistente de IA no Campaign para geração de email estão listadas abaixo:

* A qualidade do conteúdo gerado é fortemente influenciada pelo objetivo/prompt de marketing definido por você. Use um prompt bem definido para que o modelo GenAI seja interpretado com precisão. 
* Faça upload do ativo da marca para ter informações precisas sobre o conteúdo da marca. Caso contrário, o conteúdo será baseado em informações disponíveis publicamente. O conteúdo carregado pode estar nos seguintes formatos: arquivos PDF, JPEG, PNG ou ZIP (com formatos de arquivo compatíveis).
* O tamanho máximo para o ativo de marca carregado é de 50 MB. Arquivos maiores ou muitas imagens podem funcionar, mas o tempo de processamento é aumentado.
* Use um modelo de email criado pela Adobe Campaign, de preferência [modelos de email integrados](../email/create-email-templates.md), um modelo específico da marca ou um modelo personalizado para criar seu conteúdo de email. Modelo de e-mail com até 8-10 imagens recomendado.
* Relate quaisquer saídas problemáticas usando os ícones de miniatura para cima, miniatura para baixo ou sinalizador ao selecionar variantes.
* O uso do assistente de IA está sujeito às Diretrizes de usuário da IA gerativa da Adobe Experience Cloud. [Saiba mais](https://www.adobe.com/br/legal/licenses-terms/adobe-gen-ai-user-guidelines.html)

As seguintes limitações se aplicam ao Assistente de IA no Campaign:

* O idioma suportado é somente em inglês.
* Disponível somente para os canais de email, push e SMS.
* O conteúdo da GenAI pode nem sempre ser preciso: compartilhe seu feedback para que nossos engenheiros possam refinar os modelos.
* Você pode fazer upload de vários ativos de marca, mas pode aproveitar apenas um para uma geração específica.

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
