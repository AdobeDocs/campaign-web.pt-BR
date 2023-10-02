---
audience: end-user
title: Introdução ao Assistente de conteúdo
description: Introdução ao Assistente de conteúdo
badge: label="Alfa"
source-git-commit: 2eea0827a1daf4af002587d09c11e2279aaf933c
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 11%

---


# Introdução ao Assistente de conteúdo {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Assistente de conteúdo"
>abstract="Depois de criar e personalizar a entrega, você pode usar o Assistente de conteúdo para aprimorar o conteúdo. Esse recurso simplifica o processo de personalização e aprimoramento de conteúdo, permitindo ajustar o conteúdo, descrevendo o que deseja gerar."


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definir contexto para geração de conteúdo"
>abstract="Para usar o conteúdo selecionado como uma entrada para a geração de conteúdo, ative o **Aprimorar com conteúdo atual** alternar. Você também pode fazer upload dos ativos da sua marca para usá-los como uma fonte. Se você não usar o conteúdo selecionado, o upload e a seleção de ativos de uma marca serão obrigatórios."

O Assistente de conteúdo, viabilizado pela IA gerativa, é uma ferramenta valiosa para melhorar o conteúdo de emails. Ele simplifica a personalização e o aprimoramento de conteúdo, otimizando suas entregas de email para melhor repercutir com seu público.

Esse recurso economiza tempo e garante qualidade consistente, gerando automaticamente conteúdo completo do email. Com a IA gerativa, você pode criar emails atraentes sem esforço, melhorando a eficácia e a eficiência da sua comunicação.


Você pode usar o Assistente de conteúdo do Campaign em seus emails para: [gerar imagens](generative-image.md), [gerar conteúdo de texto](generative-content.md), [gerar o conteúdo de HTML completo](generative-email.md).

>[!NOTE]
>
>Esse recurso está disponível na versão Alpha e está sujeito a alterações sem aviso prévio. Ela será ativada no início de outubro.

## Medidas de proteção e limitações {#generative-guardrails}

As diretrizes gerais para o uso do Assistente de conteúdo para geração de email estão listadas abaixo:

* A qualidade do conteúdo gerado é fortemente influenciada pelo objetivo/prompt de marketing definido por você. Use um prompt bem definido para que o modelo GenAI seja interpretado com precisão. 
* Faça upload do ativo da marca para ter informações precisas sobre o conteúdo da marca. Caso contrário, o conteúdo será baseado em informações disponíveis publicamente. O conteúdo carregado pode ser: arquivos PDF, documentos do Microsoft Word, arquivos JPEG, PNG ou ZIP (com formatos de arquivo compatíveis).
* O tamanho recomendado para o ativo de marca carregado é menor que 10 MB. Arquivos maiores ou muitas imagens podem funcionar, mas o tempo de processamento é aumentado.
* Use modelos de email criados pela Adobe Campaign ou, de preferência, [modelos de email incorporados](../content/email-sample-templates.md) para criar seu conteúdo de email. Modelo de e-mail com até 8-10 imagens recomendado.


As seguintes limitações se aplicam ao Assistente de conteúdo do Campaign:

* O idioma suportado é somente em inglês
* Disponível somente para o canal de email
* O conteúdo da GenAI pode nem sempre ser preciso: compartilhe seu feedback para que nossos engenheiros possam refinar os modelos
* Você pode fazer upload de vários ativos de marca, mas pode aproveitar apenas um para uma geração específica



<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="Geração de texto" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>Geração de texto com o Assistente de conteúdo</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-image.md">
<img alt="Geração de imagem" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-image.md"><strong>Geração de imagens com o Assistente de conteúdo</strong>
</div>
<p>
</td>
<td>
<a href="generative-email.md">
<img alt="Geração de email" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-email.md"><strong>Geração de email com o Assistente de conteúdo</strong></a>
</div>
<p></td>
</tr></table>

