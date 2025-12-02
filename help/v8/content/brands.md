---
audience: end-user
title: Gerenciar marca
description: Saiba como criar e gerenciar as diretrizes da sua marca
exl-id: d4d2c6bb-7fd0-49a0-9d73-356f4a24f021
source-git-commit: 2066f29b0867f82f2130361c8ccdb15889085886
workflow-type: tm+mt
source-wordcount: '1420'
ht-degree: 1%

---

# Criar e gerenciar suas marcas {#brands}

As diretrizes da marca são um conjunto abrangente de regras e padrões que definem a identidade visual e verbal de uma marca. Eles servem como referência para garantir uma representação de marca consistente em todos os canais de marketing e comunicação.

No [!DNL Adobe Campaign Web], os usuários podem inserir e organizar manualmente informações da marca ou carregar documentos de diretrizes da marca para extração automática de dados.

## Acessar marcas {#generative-access}

Para acessar o menu **[!UICONTROL Marcas]** no [!DNL Adobe Campaign Web], os usuários devem receber os perfis de produto **[!UICONTROL Administrador (administrador)]** e **[!UICONTROL Kit de marcas]** para criar e gerenciar marcas. Para acesso somente leitura, os usuários precisam do perfil de produto [!UICONTROL Assistente de IA]. [Saiba mais](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

+++ Saiba como atribuir permissões relacionadas à marca

1. Na página inicial do [Admin Console](https://adminconsole.adobe.com/enterprise), acesse seu produto do Campaign.

   ![Página inicial do Admin Console mostrando o acesso ao produto do Campaign](assets/brands_admin_1.png)

1. Selecione o **[!DNL Product profile]** com base no nível de permissões que você deseja conceder ao usuário.

   ![Seleção do perfil de produto no Admin Console](assets/brands_admin_2.png)

1. Clique em **[!DNL Add users]** para atribuir o perfil de produto selecionado.

   ![Opção Adicionar usuários no Admin Console](assets/brands_admin_3.png)

1. Digite seu nome de usuário, grupo de usuários ou endereço de email.

1. Clique em **Salvar** para aplicar as alterações.

Os usuários já atribuídos a esta função têm suas permissões automaticamente atualizadas.

+++

## Crie sua marca {#create-brand-kit}

Para criar e gerenciar as diretrizes da sua marca, siga as etapas abaixo.

Os usuários podem inserir os detalhes manualmente ou fazer upload de um documento de diretrizes de marca para extrair as informações automaticamente:

1. No menu **[!UICONTROL Marcas]**, clique em **[!UICONTROL Criar marca]**.

   ![Menu Marcas com a opção Criar marca](assets/brands-1.png)

1. Digite um **[!UICONTROL Nome]** para sua marca.

1. Arraste e solte ou selecione seu arquivo para fazer upload das diretrizes da marca e extrair automaticamente informações relevantes sobre a marca. Clique em **[!UICONTROL Criar marca]**.

   O processo de extração de informações agora começa. Observe que pode levar vários minutos para ser concluído.

   ![Carregamento de arquivo para extração de diretrizes de marca](assets/brands-2.png)

1. Seus padrões de criação de conteúdo e visual agora são preenchidos automaticamente. Navegue pelas diferentes guias para adaptar as informações conforme necessário. [Saiba mais](#personalize)

1. No menu avançado de cada seção ou categoria, você pode adicionar referências para extrair automaticamente informações relevantes sobre a marca.

   Para remover conteúdo existente, use as opções **[!UICONTROL Limpar seção]** ou **[!UICONTROL Limpar categoria]**.

   ![](assets/brands-15.png)

1. Após a configuração, clique em **[!UICONTROL Salvar]** e em **[!UICONTROL Publicar]** para disponibilizar a diretriz de marca no Assistente de IA.

1. Para fazer modificações na sua marca publicada, clique em **[!UICONTROL Editar marca]**.

   >[!NOTE]
   >
   >Isso cria uma cópia temporária no modo de edição, substituindo a versão online depois de publicada.

   ![Opção Editar marca no menu Marcas](assets/brands-8.png)

1. No painel **[!UICONTROL Marcas]**, abra o menu avançado clicando no ícone ![](assets/do-not-localize/Smock_More_18_N.svg) para:

   * Exibir marca
   * Editar
   * Marcar como marca padrão
   * Duplicar
   * Publicação
   * Cancelar publicação
   * Excluir

   ![Opções de menu avançadas no painel Marcas](assets/brands-6.png)

As diretrizes de marca agora podem ser acessadas no menu suspenso **[!UICONTROL Marca]** do Assistente de IA. Isso permite que o Assistente de IA gere conteúdo e ativos alinhados às suas especificações. [Saiba mais sobre o Assistente de IA](../content/generative-gs.md)

![Menu do assistente de IA com o menu suspenso Marca](assets/brands_6.png)

### Definir uma marca padrão {#default-brand}

Você pode designar uma marca padrão a ser aplicada automaticamente ao gerar conteúdo e calcular pontuações de alinhamento durante a criação da campanha.

Para definir uma marca padrão, vá para o painel **[!UICONTROL Marcas]**. Abra o menu avançado clicando no ícone ![](assets/do-not-localize/Smock_More_18_N.svg) e selecione **[!UICONTROL Marcar como marca padrão]**.

![Opções de menu avançadas no painel Marcas](assets/brands-6.png)

## Personalizar sua marca {#personalize}

### Sobre a marca {#about-brand}

Use a guia **[!UICONTROL Sobre a marca]** para estabelecer a identidade principal da sua marca, descrevendo a finalidade, a personalidade, o slogan e outros atributos de definição.

1. Comece preenchendo as informações fundamentais da sua marca na categoria **[!UICONTROL Detalhes da chave]**:

   * **[!UICONTROL Nome do Kit de Marcas]**: digite o nome do kit de marcas.

   * **[!UICONTROL Quando usar]**: especifique cenários ou contextos nos quais este kit de marcas deve ser aplicado.

   * **[!UICONTROL Nome da Marca]**: insira o nome oficial da marca.

   * **[!UICONTROL Descrição da marca]**: forneça uma visão geral do que esta marca representa.

   * **[!UICONTROL Slogan padrão]**: adicione o slogan principal associado à marca.

     ![Categoria de detalhes da chave](assets/brands-about-1.png)

1. Na categoria **[!UICONTROL Princípios orientadores]**, esclareça a direção principal e a filosofia da sua marca:

   * **[!UICONTROL Missão]**: detalhe a finalidade de sua marca.

   * **[!UICONTROL Vision]**: descreva sua meta de longo prazo ou o estado futuro desejado.

   * **[!UICONTROL Posicionamento no mercado]**: explique como sua marca está posicionada no mercado.

   ![Categoria de princípios orientadores](assets/brands-about-2.png)

1. Na categoria **[!UICONTROL Valores de marca principais]**, clique em ![Texto alternativo de imagem de mergulho](assets/do-not-localize/Smock_Add_18_N.svg "Ícone Adicionar") para adicionar os valores de marca principais e preencher os detalhes:

   * **[!UICONTROL Valor]**: nomeie um valor de marca principal.

   * **[!UICONTROL Descrição]**: explique o que esse valor significa para sua marca.

   * **[!UICONTROL Comportamentos]**: descreva as ações ou atitudes que refletem este valor na prática.

   * **[!UICONTROL Manifestações]**: forneça exemplos de como esse valor é expresso em marcas reais.

     ![](assets/brands-12.png)

1. Se necessário, clique no ícone ![Texto alternativo de imagem de mergulho](assets/do-not-localize/Smock_Edit_18_N.svg "Editar")para atualizar ou excluir um de seus valores de marca principal.

   ![Editar seu valor](assets/brands-10.png)

Agora você pode personalizar ainda mais sua marca ou [publicar sua marca](#create-brand-kit).

### Estilo de escrita {#writing-style}

A seção **[!UICONTROL Estilo de escrita]** descreve os padrões para a escrita de conteúdo, detalhando como o idioma, a formatação e a estrutura devem ser usados para manter a clareza, a coerência e a consistência entre todos os materiais.

+++ Categoria disponível e exemplos

<table>
  <thead>
    <tr>
      <th>Categoria</th>
      <th>Subcategoria</th>
      <th>Exemplo de diretrizes</th>
      <th>Exemplo de exclusões</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="4">Padrões de criação de conteúdo</td>
      <td>Padrões de mensagem da marca</td>
      <td>Destaque a inovação e as mensagens direcionadas ao cliente.</td>
      <td>Não exagere nos recursos do produto.</td>
    </tr>
    <tr>
      <td>Uso do slogan</td>
      <td>Coloque o slogan abaixo do logotipo em todos os ativos de marketing digital.</td>
      <td>Não modifique ou traduza o slogan.</td>
    </tr>
    <tr>
      <td>Mensagens principais</td>
      <td>Enfatize a principal declaração de benefícios, como maior produtividade.</td>
      <td>Não use propostas de valor não relacionadas.</td>
    </tr>
    <tr>
      <td>Padrões de nomenclatura</td>
      <td>Use nomes simples e descritivos, como "ProScheduler".</td>
      <td>Não use termos complexos ou caracteres especiais.</td>
    </tr>
    <tr>
      <td rowspan="5">Estilo de comunicação da marca</td>
      <td>Características de personalidade da marca</td>
      <td>Amigável e acessível.</td>
      <td>Não seja derrotista.</td>
    </tr>
    <tr>
      <td>Mecânica de escrita</td>
      <td>Mantenha as frases curtas e impactantes.</td>
      <td>Não use jargão em excesso.</td>
    </tr>
    <tr>
      <td>Tom de situação</td>
      <td>Mantenha um tom profissional nas comunicações de crise.</td>
      <td>Não ignore as comunicações de suporte.</td>
    </tr>
    <tr>
      <td>Diretrizes de Escolha do Word</td>
      <td>Use palavras como "inovador" e "inteligente".</td>
      <td>Evite palavras como "barato" ou "hack".</td>
    </tr>
    <tr>
      <td>Padrões de Idioma</td>
      <td>Siga as convenções do inglês americano.</td>
      <td>Não misture ortografias britânicas e americanas.</td>
    </tr>
    <tr>
      <td rowspan="3">Padrões de conformidade legal</td>
      <td>Padrões de marca comercial</td>
      <td>Sempre use o símbolo ™ ou ®.</td>
      <td>Não omita símbolos legais quando necessário.</td>
    </tr>
    <tr>
      <td>Padrões de direitos autorais</td>
      <td>Inclua avisos de direitos autorais nos materiais de marketing.</td>
      <td>Não use conteúdo de terceiros sem permissão.</td>
    </tr>
    <tr>
      <td>Padrões de isenção de responsabilidade</td>
      <td>Exibir avisos de isenção de responsabilidade de forma legível em ativos digitais.</td>
      <td>Não oculte isenções de responsabilidade em áreas não visíveis.</td>
    </tr>
</table>

+++

</br>

Para personalizar seu **[!UICONTROL Estilo de Redação]**:

1. Na guia **[!UICONTROL Estilo de Escrita]**, clique em ![](assets/do-not-localize/Smock_Add_18_N.svg) para adicionar uma diretriz, exceção ou exclusão.

1. Insira sua diretriz, exceção ou exclusão. Você também pode incluir **[!UICONTROL Exemplos]** para ilustrar melhor como ele deve ser aplicado.

   ![](assets/brands-3.png)

1. Especifique o **[!UICONTROL contexto de uso]** para sua diretriz, exceção ou exclusão:

   * **[!UICONTROL Tipo de canal]**: escolha onde esta diretriz, exceção ou exclusão deve ser aplicada. Por exemplo, talvez você queira que um estilo de escrita específico apareça apenas em E-mail, Celular, Impressões ou outros canais de comunicação.

   * **[!UICONTROL Tipo de elemento]**: especifique a qual elemento de conteúdo a regra se aplica. Isso pode incluir elementos como Títulos, Botões, Links ou outros componentes no conteúdo.

   ![](assets/brands-16.png)

1. Depois de configurar sua diretriz, exceção ou exclusão, clique em **[!UICONTROL Adicionar]**.
1. Se necessário, selecione uma de suas diretrizes ou exclusões para atualizar ou excluir.

1. Clique no ![texto alternativo de imagem de mergulho](assets/do-not-localize/Smock_Edit_18_N.svg "Editar") para editar seu exemplo ou no ícone ![Texto alternativo da imagem de mergulho](assets/do-not-localize/Smock_Delete_18_N.svg "Excluir")para excluí-lo.

   ![](assets/brands-11.png)

Agora você pode personalizar ainda mais sua marca ou [publicar sua marca](#create-brand-kit).

### Conteúdo visual {#visual-content}

A seção **[!UICONTROL Conteúdo visual]** define os padrões de imagem e design, detalhando as especificações necessárias para manter uma aparência de marca unificada e consistente.

+++ Categorias e exemplos disponíveis

<table>
  <thead>
    <tr>
      <th>Categoria</th>
      <th>Exemplo de diretrizes</th>
      <th>Exemplo de exclusões</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Padrões de fotografia</td>
      <td>Use a iluminação natural para fotos ao ar livre.</td>
      <td>Evite imagens editadas ou pixeladas em excesso.</td>
    </tr>
    <tr>
      <td>Padrões de ilustração</td>
      <td>Use estilos limpos e minimalistas.</td>
      <td>Evite complexos demais.</td>
    </tr>
    <tr>
      <td>Ícone padrões</td>
      <td>Use um sistema de grade de 24px consistente.</td>
      <td>Não misture dimensões de ícone, use espessuras de traçado inconsistentes ou desvie das regras de grade.</td>
    </tr>
    <tr>
      <td>Diretrizes de uso</td>
      <td>Escolha imagens de estilo de vida que reflitam clientes reais usando o produto em ambientes profissionais.</td>
      <td>Não use imagens que estejam em contradição com o tom da marca ou que apareçam fora de contexto.</td>
    </tr>
</table>

+++

</br>

Para personalizar seu **[!UICONTROL conteúdo visual]**:

1. Na guia **[!UICONTROL Visual content]**, clique em ![](assets/do-not-localize/Smock_Add_18_N.svg) para adicionar uma diretriz, exclusão ou exemplo.

1. Insira sua diretriz, exclusão ou exemplo.

   ![Adicionar exclusão ou botão de exemplo](assets/brands-4.png)

1. Especifique o **[!UICONTROL contexto de uso]** para sua diretriz ou exclusão:

   * **[!UICONTROL Tipo de canal]**: escolha onde esta diretriz, exceção ou exclusão deve ser aplicada. Por exemplo, talvez você queira que um estilo de escrita específico apareça apenas em E-mail, Celular, Impressões ou outros canais de comunicação.

   * **[!UICONTROL Tipo de elemento]**: especifique a qual elemento de conteúdo a regra se aplica. Isso pode incluir elementos como Títulos, Botões, Links ou outros componentes no conteúdo.

     ![Adicionar conteúdo de uso](assets/brands-17.png)

1. Depois de configurar sua diretriz, exceção ou exclusão, clique em **[!UICONTROL Adicionar]**.

1. Para adicionar uma imagem mostrando o uso correto, selecione **[!UICONTROL Exemplo]** e clique em **[!UICONTROL Selecionar imagem]**. Você também pode adicionar uma imagem mostrando o uso incorreto como exemplo de exclusão.

   ![Adicionar uma imagem como exemplo](assets/brands-13.png)

1. Selecione uma de suas diretrizes ou exclusões para atualizar ou excluir.

1. Selecione uma diretriz ou exclusão para atualizá-la. Clique no ícone ![Texto alternativo de imagem de mergulho](assets/do-not-localize/Smock_Delete_18_N.svg "Excluir")para excluí-lo.

   ![Excluir exclusão ou diretriz](assets/brands-14.png)

Agora você pode personalizar ainda mais sua marca ou [publicar sua marca](#create-brand-kit).
