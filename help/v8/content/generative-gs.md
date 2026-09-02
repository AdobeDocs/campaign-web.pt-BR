---
audience: end-user
title: Introdução à geração de conteúdo
description: Introdução à geração de conteúdo
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
TQID: https://experienceleague.adobe.com/jpw4u-Vy7M2Q9qRyQ2J3rJ-Mr8UKLUpxhw39tglbbNc
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
source-git-commit: d4e22ba88bcb6dc74d22e8a927c1640f21d75d3e
workflow-type: tm+mt
source-wordcount: 887
ht-degree: 20%

---

# Trabalhar com o recurso Gerar conteúdo {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Gerar conteúdo"
>abstract="Depois de criar e personalizar seu delivery, use a IA para aprimorar seu conteúdo. Esse recurso simplifica a personalização e o aprimoramento de conteúdo, permitindo ajustá-lo a partir da descrição do que deseja gerar."

>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definir contexto com Gerar conteúdo no Campaign"
>abstract="Para usar o conteúdo selecionado como uma entrada para a geração de conteúdo, ative a opção **Aprimorar com conteúdo atual**. Você também pode fazer upload dos ativos da sua marca e usá-los como fonte de conteúdo. Se você não usar o conteúdo selecionado, será obrigatório fazer o upload e escolher os ativos da marca."

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Termos da IA generativa da Adobe"
>abstract="O acesso a esse recurso depende de você aceitar as Diretrizes do usuário de IA generativa da Adobe Experience Cloud. Analise todos resultados deste recurso quanto à precisão e certifique-se de que sejam apropriados ao seu caso de uso."
>additional-url="https://www.adobe.com/br/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Diretrizes do usuário da IA generativa da Adobe"

>[!INFO]
>
>Mergulhe em uma experiência prática com a [nossa visualização de recursos ao vivo](https://experienceleague.adobe.com/pt-br/apps/journey-optimizer/ai-assistant-content-accelerator), projetada para permitir que você explore seus recursos em primeira mão e entenda totalmente suas funcionalidades.

À medida que o setor de marketing se torna mais competitivo, as marcas buscam maneiras eficientes de gerar conteúdo impactante rapidamente. Gerar conteúdo na Web do Adobe Campaign, viabilizado pelo Microsoft Azure OpenAI e Adobe Firefly, é o recurso de geração de conteúdo de IA da Adobe que transforma a forma como os profissionais de marketing criam conteúdo profissional e consistente com a marca em canais como email, SMS e notificações por push. Com modelos avançados de GenAI e uma profunda compreensão das diretrizes da marca, a ferramenta Gerar conteúdo gera automaticamente conteúdo personalizado, envolvente e eficaz com base no objetivo de marketing, otimizando o conteúdo para estilos, layouts, tom e muito mais.

Gerar conteúdo dá suporte à geração **em vários idiomas**, permitindo que você alcance e envolva diversos públicos globais. Gerar conteúdo está disponível nos seguintes idiomas:

<table style="table-layout:fixed; margin-top: 0px; margin-bottom: 0px;">
  <tbody>
    <tr style="border: 0;background-color: #FFFFFF;">
      <td>
        <ul>
          <li>Chinês (Hong Kong)</li>
          <li>Chinês (simplificado)</li>
          <li>Chinês (Taiwan)</li>
          <li>Holandês</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>Francês</li>
          <li>Alemão</li>
          <li>Italiano</li>
          <li>Japonês</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>Norueguês</li>
          <li>Português</li>
          <li>Espanhol</li>
          <li>Sueco</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

Gerar conteúdo simplifica a criação e a execução de campanhas de marketing em canais como email, SMS e notificações por push, economizando tempo, melhorando a eficiência e obtendo melhores resultados.

>[!IMPORTANT]
>
>* Antes de usar esse recurso, reveja as [Medidas de Proteção e Limitações](#generative-guardrails) relacionadas.
>
>* Você deve concordar com um [contrato de usuário](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) antes de usar a IA para gerar conteúdo na Adobe Campaign Web. Para mais informações, entre em contato com o seu representante da Adobe.

## Acessar Gerar Conteúdo {#generative-access}

A opção Gerar conteúdo para emails, notificações por push, página de aterrissagem e SMS agora está em Disponibilidade Geral (GA) e disponível para todos os usuários. As permissões e as etapas necessárias para conceder acesso aos usuários são detalhadas abaixo.

+++ Saiba como atribuir permissões relacionadas à geração de conteúdo

1. **Acesse o [Admin Console](https://adminconsole.adobe.com/)**, navegue até o menu **Produtos** e selecione **Adobe Campaign Managed Cloud**.

1. Acesse a instância para a qual você deseja conceder permissões e clique em **Novo perfil** para criar um novo perfil de produto com o seguinte nome de Perfil de produto específico:

   `Campaign - <instance-name> - AIAssistant`

1. Configure o perfil de produto com as permissões necessárias para o acesso Gerar conteúdo.

1. **Adicionar usuários ou grupos de usuários**. Escolha uma das seguintes opções:
   * **Adicionar usuários individuais**: adicione os usuários necessários diretamente ao perfil do produto.
   * **Adicionar grupos de usuários**: crie um grupo de usuários, adicione usuários a esse grupo e, em seguida, adicione o grupo de usuários ao perfil de produto.

Saiba como definir permissões no Campaign em [esta seção](../get-started/permissions.md).

+++

## Medidas de proteção e limitações {#generative-guardrails}

As diretrizes gerais para o uso da IA para gerar conteúdo no Adobe Campaign Web para geração de email estão listadas abaixo:

* A qualidade do conteúdo gerado depende muito do objetivo de marketing ou do prompt definido. Use um prompt bem definido para que o modelo GenAI seja interpretado com precisão.
* Faça upload dos ativos da marca para garantir um conteúdo preciso sobre a marca. Caso contrário, o conteúdo será baseado em informações disponíveis publicamente. O conteúdo carregado pode estar nos seguintes formatos: arquivos PDF, JPEG, PNG ou ZIP (com formatos de arquivo compatíveis).
* O tamanho máximo para os recursos de marca carregados é de 50 MB. Arquivos maiores ou imagens numerosas podem aumentar o tempo de processamento.
* Use [modelos de email internos](../content/create-email-templates.md), modelos específicos da marca ou modelos personalizados para criar seu conteúdo de email usando IA. São recomendados modelos de e-mail com até 8 a 10 imagens.
* Relate quaisquer saídas problemáticas usando os ícones de miniatura, miniatura ou sinalizador ao selecionar variantes.
* O uso de Gerar conteúdo está sujeito às Diretrizes de usuário da IA gerada da Adobe Experience Cloud. [Saiba mais](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html).
* Como parte do compromisso da Adobe com a transparência no uso de ferramentas de IA gerativa na criação de mídia, a Adobe aplica o Content Credentials quando o conteúdo ou um projeto que inclui um ativo gerado pela Firefly é baixado ou exportado. [Saiba mais](https://helpx.adobe.com/firefly/using/content-credentials.html).

As seguintes limitações se aplicam à Geração de conteúdo no Adobe Campaign Web:

* Gerar conteúdo no Adobe Campaign Web é atualmente suportado somente em inglês. Entradas em outros idiomas podem produzir resultados inconsistentes ou errôneos. Problemas decorrentes de respostas em outros idiomas não serão abordados ou aprimorados neste momento.
* Disponível somente para os canais de email, push e SMS.
* O conteúdo da GenAI pode nem sempre ser preciso. Compartilhe seu feedback para que os engenheiros possam refinar os modelos.
* Você pode fazer upload de vários ativos de marca, mas pode aproveitar apenas um para uma geração específica.

## Gerar recursos de conteúdo {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-full-content.md">
<img alt="[Geração de conteúdo completo com Gerar conteúdo]" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-full-content.md"><strong>Geração de conteúdo completo com Gerar conteúdo</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-text.md">
<img alt="[Geração de conteúdo de texto com Gerar conteúdo]" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-text.md"><strong>Geração de texto com Gerar conteúdo</strong>
</div>
<p>
</td>
<td>
<a href="generative-image.md">
<img alt="[Geração de imagem com Gerar conteúdo]" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-image.md"><strong>Geração de imagem com Gerar conteúdo</strong></a>
</div>
<p></td>
</tr></table>