---
audience: end-user
title: Introdução ao Assistente de IA
description: Introdução ao Assistente de IA
badge: label="Beta"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
hide: true
hidefromtoc: true
source-git-commit: af67094638cfc3c5c64385203340918f0f8f2482
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 33%

---

# Introdução ao Assistente de IA {#generative-gs}

>[!BEGINSHADEBOX]

**Índice**

* **[Introdução ao Assistente de IA](generative-gs.md)**
* [Geração de email com o Assistente de IA](generative-content.md)
* [Geração de SMS com o Assistente de IA](generative-sms.md)
* [Geração de notificação por push com o Assistente de IA](generative-push.md)

>[!ENDSHADEBOX]

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Assistente de IA"
>abstract="Depois de criar e personalizar o delivery, você pode usar o Assistente de IA para aprimorar o conteúdo. Esse recurso simplifica o processo de personalização e aprimoramento de conteúdo, permitindo ajustar o conteúdo, descrevendo o que deseja gerar."


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definir contexto com o Assistente de IA no Campaign"
>abstract="Para usar o conteúdo selecionado como uma entrada para a geração de conteúdo, ative a opção **Aprimorar com conteúdo atual**. Você também pode fazer upload dos ativos da sua marca e usá-los como fonte de conteúdo. Se você não usar o conteúdo selecionado, será obrigatório fazer o upload e selecionar os ativos de marca."


>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Termos da IA generativa da Adobe"
>abstract="O acesso a esse recurso está sujeito à concordância com as Diretrizes do usuário da IA generativa da Adobe Experience Cloud. Quaisquer prompts, contexto, informações complementares ou outras informações fornecidas para este recurso devem ser vinculadas a um contexto específico, que pode incluir materiais de marca, conteúdo de site, dados, esquemas para tais dados, modelos ou outros documentos confiáveis, e não devem conter nenhuma informação pessoal (as informações pessoais incluem tudo o que pode ser vinculado a um indivíduo específico). É recomendado revisar qualquer saída deste recurso para verificar a precisão e garantir que seja apropriado para seu caso de uso"
>additional-url="https://www.adobe.com/br/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Diretrizes do usuário da IA generativa da Adobe"

O Assistente de IA é uma ferramenta valiosa para melhorar o conteúdo de email. Ele simplifica a personalização e o aprimoramento de conteúdo, otimizando suas entregas de email para melhor repercutir com seu público.

Esse recurso economiza tempo e garante qualidade consistente, gerando automaticamente conteúdo completo do email. Com a IA gerativa, você pode criar emails atraentes sem esforço, melhorando a eficácia e a eficiência da sua comunicação.

>[!NOTE]
>
>Esse recurso está disponível na versão Alpha e está sujeito a alterações sem aviso prévio. Ela será ativada no início de outubro.

## Medidas de proteção e limitações {#generative-guardrails}

As diretrizes gerais para usar o Assistente de IA no Campaign para geração de email estão listadas abaixo:

* A qualidade do conteúdo gerado é fortemente influenciada pelo objetivo/prompt de marketing definido por você. Use um prompt bem definido para que o modelo GenAI seja interpretado com precisão. 
* Faça upload do ativo da marca para ter informações precisas sobre o conteúdo da marca. Caso contrário, o conteúdo será baseado em informações disponíveis publicamente. O conteúdo carregado pode estar nos seguintes formatos: arquivos PDF, JPEG, PNG ou ZIP (com formatos de arquivo compatíveis).
* O tamanho recomendado para o ativo de marca carregado é menor que 50 MB. Arquivos maiores ou muitas imagens podem funcionar, mas o tempo de processamento é aumentado.
* Use modelos de email criados no Adobe Campaign, de preferência [modelos de email incorporados](../email/create-email-templates.md), um modelo específico da marca ou um modelo personalizado para criar seu conteúdo de email. Modelo de e-mail com até 8-10 imagens recomendado.


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
