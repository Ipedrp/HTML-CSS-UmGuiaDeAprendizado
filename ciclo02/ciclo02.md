- [1. Psicologia das Cores](#1-psicologia-das-cores)
  - [1.1. Significados das Cores](#11-significados-das-cores)
- [2. Representação de Cores](#2-representação-de-cores)
  - [2.1. Cores por Nome](#21-cores-por-nome)
  - [2.2. Cores por Código Hexadecimal](#22-cores-por-código-hexadecimal)
  - [2.3. Cores por RGB](#23-cores-por-rgb)
  - [2.4. Cores por HSL](#24-cores-por-hsl)
  - [2.5. Transparência nas Cores](#25-transparência-nas-cores)
  - [2.6. Opacidade](#26-opacidade)
  - [2.7. Quando Usar Cada Modelo](#27-quando-usar-cada-modelo)
- [3. Harmonia de Cores](#3-harmonia-de-cores)
  - [3.1. Círculo Cromático](#31-círculo-cromático)
  - [3.2. Temperaturas de Cores](#32-temperaturas-de-cores)
  - [3.3. Combinações Harmoniosas](#33-combinações-harmoniosas)
- [4. Degradê com CSS](#4-degradê-com-css)
  - [4.1. Degradê Linear](#41-degradê-linear)
  - [4.2. Degradê Radial](#42-degradê-radial)
- [5. Tipografia](#5-tipografia)
  - [5.1. Fontes](#51-fontes)
  - [5.2. Tamanho da Fonte](#52-tamanho-da-fonte)
  - [5.3. Peso da Fonte](#53-peso-da-fonte)
  - [5.4. Estilo da Font](#54-estilo-da-font)
  - [5.5. Alinhamento do Texto](#55-alinhamento-do-texto)
  - [5.6. Altura da Linha](#56-altura-da-linha)
  - [5.7. Espaçamento entre Letras e Palavras](#57-espaçamento-entre-letras-e-palavras)
  - [5.8. Decoração do Texto](#58-decoração-do-texto)
  - [5.9. Transformação do Texto](#59-transformação-do-texto)
  - [5.10. Cor da Fonte](#510-cor-da-fonte)
  - [5.11. Fontes Externas](#511-fontes-externas)
- [6. Seletores Personalidos](#6-seletores-personalidos)
  - [6.1. Seletor de ID](#61-seletor-de-id)
  - [6.2. Seletor de Classe](#62-seletor-de-classe)
  - [6.3. Pseudo-classes](#63-pseudo-classes)
  - [6.4. Pseudo-elementos](#64-pseudo-elementos)
  - [6.5. Diferenças entre Pseudo-classe e Pseudo-elemento](#65-diferenças-entre-pseudo-classe-e-pseudo-elemento)
  - [6.6. Seletores Combinados](#66-seletores-combinados)
- [7. Modelos de caixas](#7-modelos-de-caixas)
  - [7.1. Modelo de Caixa Box-Level (Bloco)](#71-modelo-de-caixa-box-level-bloco)
  - [7.2. Modelo de Caixa Inline-Level (Linha)](#72-modelo-de-caixa-inline-level-linha)
  - [7.3. Diferenças entre Box-Level e Inline-Level](#73-diferenças-entre-box-level-e-inline-level)
  - [7.4. Box Model](#74-box-model)
- [8. Agrupamento de Tags (Grouping Tags)](#8-agrupamento-de-tags-grouping-tags)
  - [8.1. Principais Tags de Agrupamento](#81-principais-tags-de-agrupamento)
  - [8.2. Importância Semântica](#82-importância-semântica)
- [9. Sombra e Bordas Arredondadas](#9-sombra-e-bordas-arredondadas)
  - [9.1. Sombra (Box Shadow)](#91-sombra-box-shadow)
  - [9.2. Bordas Arredondadas (Border Radius)](#92-bordas-arredondadas-border-radius)
  - [9.3. Combinação de box-shadow e border-radius](#93-combinação-de-box-shadow-e-border-radius)
- [10. Variáveis em CSS](#10-variáveis-em-css)
  - [10.1. Definição de Variáveis](#101-definição-de-variáveis)
  - [10.2. Benefícios](#102-benefícios)
  - [10.3. Exemplo Completo](#103-exemplo-completo)


#  1. Psicologia das Cores

- A **psicologia das cores** estuda como diferentes cores podem influenciar nossas emoções, comportamentos e decisões. No design, as cores desempenham um papel fundamental na experiência do usuário, afetando desde a estética até a funcionalidade.

##  1.1. Significados das Cores

- Cada cor carrega um significado psicológico que pode influenciar como as pessoas percebem um site ou um produto. Aqui estão algumas cores e seus significados comuns:

  - Vermelho
    - **Emoções**: Paixão, energia, urgência.
    - **Uso no Design**: Chama a atenção e estimula ação. Usado em botões de chamada para ação (CTAs) ou para destacar elementos importantes.
  - Azul
    - **Emoções**: Confiança, serenidade, segurança.
    - **Uso no Design**: Transmite tranquilidade e profissionalismo. Muito utilizado em sites corporativos e redes sociais.

  - Amarelo
    - **Emoções**: Alegria, otimismo, calor.
    - **Uso no Design**: Atrai atenção, mas deve ser usado com moderação para não causar fadiga visual. Geralmente associado à positividade e criatividade.

  - Verde
    - **Emoções**: Harmonia, equilíbrio, natureza.
    - **Uso no Design**: Associado à saúde, sustentabilidade e crescimento. Amplamente utilizado em projetos relacionados ao meio ambiente e bem-estar.

  - Laranja
    - **Emoções**: Energia, entusiasmo, calor.
    - **Uso no Design**: Estimula interações e transmite acessibilidade. É uma cor usada para envolver o usuário, especialmente em marketing.

  - Roxo
    - **Emoções**: Criatividade, luxo, mistério.
    - **Uso no Design**: Comumente associado a produtos premium e a marcas criativas.

  - Preto
    - **Emoções**: Sofisticação, elegância, formalidade.
    - **Uso no Design**: Sinal de exclusividade e poder. Utilizado em design minimalista e em marcas de luxo.

  - Branco
    - **Emoções**: Pureza, simplicidade, clareza.
    - **Uso no Design**: Aumenta a sensação de espaço e limpeza. Muito usado em designs minimalistas e para criar contraste com outras cores.

# 2. Representação de Cores

- No desenvolvimento web, as cores podem ser representadas de diferentes formas no CSS. Abaixo estão as principais maneiras de representar cores, com exemplos práticos.

##  2.1. Cores por Nome

- No CSS, você pode usar o **nome** da cor para definir o estilo. Existem 140 cores nomeadas disponíveis.

  - Exemplo de Uso:

    ```html

    <h2 style="background-color: blue; color: white;">Exemplo de uso de cores</h2>
    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit...</p>

    ```

##  2.2. Cores por Código Hexadecimal

- O **código hexadecimal** define cores usando o formato #RRGGBB, onde RR, GG, e BB são valores de vermelho, verde e azul, respectivamente, representados por dois dígitos hexadecimais.

  - Exemplo de Uso:

    ```html

    <h2 style="background-color: #0000ff; color: white;">Exemplo de uso de cores</h2>
    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit...</p>

    ```

##  2.3. Cores por RGB

- O modelo **RGB** (Red, Green, Blue) define uma cor misturando valores de vermelho, verde e azul. Cada componente varia de 0 a 255.

  - Exemplo de Uso:

    ```html

    <h2 style="background-color: rgb(0, 0, 255); color: white;">Exemplo de uso de cores</h2>
    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit...</p>

    ```

##  2.4. Cores por HSL

- O modelo **HSL (Hue, Saturation, Lightness)** define uma cor em termos de:

  - **Hue** (Matiz): O valor no espectro de cores (0 a 360 graus).
  - **Saturation** (Saturação): A intensidade da cor (0% a 100%).
  - **Lightness** (Luminosidade): O brilho da cor (0% é preto, 100% é branco).

  - Exemplo de Uso:

    ```html

    <h2 style="background-color: hsl(240, 100%, 50%); color: white;">Exemplo de uso de cores</h2>
    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit...</p>

    ```

##  2.5. Transparência nas Cores

- A **transparência** permite que você controle o nível de opacidade de uma cor, o que é útil para criar efeitos visuais interessantes e sobreposições.

##  2.6. Opacidade

- A **opacidade** é a medida de quão transparente uma cor é. Um valor de opacidade de 1 significa que a cor é totalmente opaca, enquanto um valor de 0 significa que a cor é completamente transparente.

  - Exemplo de Uso com RGBA

    - O formato `rgba()` é usado para definir cores com opacidade. Os valores `R`, `G`, `B` variam de 0 a 255, enquanto `A` (Alpha) varia de 0 a 1.

  - Exemplo:

    ```html

    <h2 style="background-color: rgba(0, 0, 255, 0.5); color: white;">Exemplo de cor com transparência</h2>
    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit...</p>

    ```

##  2.7. Quando Usar Cada Modelo

- **Nomes de cor:** Útil para situações rápidas, mas limitado em opções.
- **Hexadecimal:** Popular entre desenvolvedores e amplamente suportado.
- **RGB:** Melhor para ajustes finos em intensidades de cor.
- **HSL:** Mais intuitivo para ajustes de tonalidade, saturação e brilho.


#  3. Harmonia de Cores

- A harmonia das cores é um princípio essencial no design que se refere ao uso de cores que combinam bem entre si. A compreensão do círculo cromático e das relações entre cores pode ajudar a criar composições visuais agradáveis e equilibradas.

##  3.1. Círculo Cromático

- O círculo cromático é uma representação visual das cores, que organiza as cores em um formato circular. Ele é dividido em três categorias principais: cores primárias, secundárias e terciárias.

  - Cores Primárias
    - As cores primárias são aquelas que não podem ser criadas pela mistura de outras cores. No modelo de cores aditivas (RGB), as cores primárias são:
      - **Vermelho**
      - **Verde**
      - **Azul**
    - No modelo de cores subtrativas (CMY), as cores primárias são:
      - **Ciano**
      - **Magenta**
      - **Amarelo**
    - Cores Secundárias
      - As cores secundárias são formadas pela mistura de duas cores primárias em partes iguais. No círculo cromático, as cores secundárias são:
        - **Laranja** (vermelho + amarelo)
        - **Verde** (azul + amarelo)
        - **Roxo** (vermelho + azul)
    - Cores Terciárias
      - As cores terciárias são criadas pela mistura de uma cor primária com uma cor secundária adjacente. Exemplos de cores terciárias incluem:
        - **Vermelho-alaranjado**
        - **Amarelo-alaranjado**
        - **Amarelo-esverdeado**
        - **Azul-esverdeado**
        - **Azul-arroxeado**
        - **Vermelho-arroxeado**

## 3.2. Temperaturas de Cores

- As cores também podem ser classificadas em **temperaturas**: cores quentes e cores frias.
  - Cores Quentes
    - Associadas a sensações de energia, calor e emoção.
      - **vermelho**
      - **laranja**
      - **amarelo**
  - Cores Frias
    - Evocam sensações de calma, tranquilidade e serenidade
      - **azul**
      - **verde** 
      - **roxo** 
##  3.3. Combinações Harmoniosas

- Ao criar paletas de cores, algumas combinações são mais harmoniosas do que outras. Aqui estão algumas maneiras comuns de combinar cores:

  - **Complementares:** Cores opostas no círculo cromático. Exemplo: azul e laranja.
  - **Análogas:** Cores que estão lado a lado no círculo. Exemplo: azul, azul-esverdeado e verde.
  - **Tríades:** Três cores equidistantes no círculo cromático. Exemplo: vermelho, amarelo e azul.

#  4. Degradê com CSS
- Os **degradês (ou gradientes)** são uma técnica visual utilizada no design web para criar transições suaves entre duas ou mais cores. 
##  4.1. Degradê Linear
- Um **degradê linear** é uma transição de cor que se estende em uma direção reta. Para criar um degradê linear no CSS, você utiliza a propriedade `background-image` com a função `linear-gradient()`.
  
  - Direção do Degradê Linear
    - A **direção do degradê** pode ser ajustada usando palavras-chave, como to right, to left, to top, ou to bottom, ou usando ângulos. Aqui estão alguns exemplos:
      - **Degradê Horizontal**: linear-gradient(to right, #f00, #0f0) (do vermelho para o verde).
      - **Degradê Diagonal**: linear-gradient(45deg, #00f, #ff0) (do azul para o amarelo em um ângulo de 45 graus).
    
      - Exemplo de Uso:

      ```css

      body {
          background-image: linear-gradient(to bottom, #3198E2, #6D59C0, #B93590, #E33F5F, #FDD579);
          background-attachment: fixed;
      }

      ```
##  4.2. Degradê Radial
- Um **degradê radial** cria uma transição circular de cores a partir de um ponto central. Para criar um degradê radial no CSS, você utiliza a função `radial-gradient()`.

  - Formatos do Degradê Radial

    - **Círculo** radial-gradient(circle, #ff0000, #0000ff) - Um degradê circular, onde a cor transita uniformemente em todas as direções a partir do centro.

    - **Elipse**: radial-gradient(ellipse, #ff0000, #0000ff) - Um degradê em formato elíptico, onde a transição de cores ocorre em uma forma oval.

    - Exemplo de Uso:

      ```css
      body {
          background-image: radial-gradient(circle, red, blue);
      }
      ```

#  5. Tipografia

- A **tipografia** refere-se ao estilo, arranjo e aparência do texto em um design ou documento. Ela desempenha um papel crucial na comunicação visual, influenciando não apenas a estética, mas também a legibilidade e a hierarquia de informação. 

##  5.1. Fontes

- As **fontes** são definidas em CSS utilizando a propriedade `font-family`.
  
  - Definindo a Fonte

    - A propriedade `font-family` aceita uma lista de fontes, sendo a primeira a preferencial.
    - Caso a primeira não esteja disponível, as próximas serão usadas. 
    - O uso de uma família genérica é recomendado como último recurso. (`serif`, `sans-serif` ou `monospace`) 

      ```css

      <p style="font-family: 'Arial', sans-serif;">
        Texto com a fonte Arial.
      </p>

      ```

##  5.2. Tamanho da Fonte

- É controlado pela propriedade `font-size` . 

  - Tipos de Medidas

    - As medidas podem ser Absolutas ou Relativas

  - Medidas Absolutas

    - **Pixels (px)**: Tamanho fixo e absoluto, que não muda com a configuração do usuário. Exemplo: 20px.
  
  - Medidas Relativas

    - **Em**: Unidade relativa, com base no tamanho da fonte do elemento pai. Se o tamanho da fonte do elemento pai for 16px, 0.5em será igual a 8px.
    - **Rem**: Unidade relativa ao tamanho da raiz do documento. Por padrão, 1rem é igual a 16px, independentemente do tamanho da fonte do elemento pai.
    - **Porcetagem (%)**: Também relativa ao tamanho da fonte do elemento pai. Por exemplo, se o elemento pai tiver um tamanho de 16px, 150% será igual a 24px.
  
      ```css

      <p style="font-size: 20px;">
        Texto com tamanho de 20px.
      </p>

      <p style="font-size: 1.5em;">
        Texto com tamanho relativo de 1.5 vezes o tamanho base da fonte.
      </p>

      ```
##  5.3. Peso da Fonte
- É controlado pela propriedade `font-weight`.

  - Pesos Comuns
    - **Normal**: Valor padrão, equivalente a 400.
    - **`Bold`**: Texto em negrito, equivalente a 700.
    - **Valores numéricos**: Variação entre 100 (mais fino) e 900 (mais espesso).

##  5.4. Estilo da Font
- É definido pela propriedade `font-style`. 
- 
  - Valores para Font Style
    - **`Normal`**: Texto sem estilo adicional.
    - **`Italic`**: Texto em itálico.
    - **`Oblique`**: Similar ao itálico, mas com uma inclinação diferente.
  
##  5.5. Alinhamento do Texto
- Todo o texto é ajustado com a propriedade `text-align`. 
- O início do paragafo por ser ajustado com a propriedade `text-indent`.
  
  - Opções de Alinhamento com Text-Align

    - **`Left`**: Alinhamento à esquerda (padrão).
    - **`Right`**: Alinhamento à direita.
    - **`Center`**: Texto centralizado.
    - **`Justify`**: Texto justificado, preenchendo o espaço da linha.

  - Alinhamento com Text-Indent

    - **Valor em pixels (px) ou em (em)**: Define o tamanho do recuo.
    - **Valores negativos**: Criam um recuo para a esquerda (pouco usado).

##  5.6. Altura da Linha

- A propriedade `line-height` controla a altura da linha.

  - Definindo a Altura da Linha

    - **Normal**: Valor padrão, dependendo do navegador e da fonte.
    - **Numérico**: Valor maior que 1 aumenta o espaçamento.


##  5.7. Espaçamento entre Letras e Palavras
- A propriedade `letter-spacing` ajusta o espaçamento entre as letras
- A propriedade `word-spacing` controla o espaçamento entre as palavras. 

  - Ajustando Espaçamentos

    - **`Letter-spacing`** Aumenta ou diminui o espaçamento entre as letras.
    - **`Word-spacing`** Aumenta ou diminui o espaçamento entre as palavras.


##  5.8. Decoração do Texto
- A propriedade `text-decoration` adiciona efeitos visuais ao texto.

  - Tipos de Decoração

    - **`Underline`**: Adiciona uma linha abaixo do texto.
    - **`Line-through`**: Adiciona uma linha através do texto (riscado).

##  5.9. Transformação do Texto
- A transformação do texto pode ser feita usando a propriedade `text-transform`.

- Modos de Transformação

  - **`Uppercase`**: Transforma todas as letras em maiúsculas.
  - **`Lowercase`**: Transforma todas as letras em minúsculas.
  - **`Capitalize`**: Capitaliza a primeira letra de cada palavra.

##  5.10. Cor da Fonte

- A propriedade `color` é usada para definir a cor do texto. 

  - Formatos de Cor

    - **Hexadecimal**: Especifica cores usando código hexadecimal, por exemplo, #FF5733 para laranja.
    - **RGB**: Define as cores usando valores de Red, Green, Blue (RGB).
    - **Nomes de cores**: Usa nomes de cores pré-definidos, como red, blue, green.

##  5.11. Fontes Externas

- **Google Fonts**
  - Uma biblioteca de fontes que permite incorporar uma grande variedade de fontes personalizadas. 

  - As fontes podem ser incluídas diretamente através de:
    - links
    - importadas via CSS.

- Como utilizar o Google Fonts

  - Acesse o site [Google Fonts](https://fonts.google.com/).
  - Escolha a fonte desejada e clique em "Select this style".
  - Copie o link gerado e adicione-o no `<head>` do seu HTML.
  - Defina a fonte no seu CSS utilizando a propriedade `font-family`.

- **DaFont**

  - Uma plataforma popular para baixar fontes personalizadas.

    - Baixadas e instaladas localmente.
    - Incorporadas ao projeto utilizando a regra `@font-face` no CSS.

  - Utilizando fontes do DaFont

    - Acesse o site [DaFont](https://www.dafont.com/).
    - Baixe o arquivo de fonte desejado (normalmente em formatos como `.otf` ou `.ttf`).
    - Inclua a fonte em seu projeto utilizando a regra `@font-face`.

- Tipos de Formatos de Fonte

  - Ao utilizar fontes externas, é importante conhecer os diferentes formatos de fonte para garantir compatibilidade entre navegadores.

- Tipos de Formatos

  - **OpenType (.otf)**: Formato moderno com suporte avançado para gráficos e tipografia.
  - **TrueType (.ttf)**: Formato padrão utilizado tanto em Windows quanto em macOS.
  - **Embedded OpenType (.eot)**: Usado principalmente para compatibilidade com versões antigas do Internet Explorer.
  - **TrueType AAT (Apple Advanced Typography)**: Formato da Apple com suporte a recursos tipográficos avançados.
  - **SVG**: Fonte vetorial que pode ser escalada sem perder qualidade.

#  6. Seletores Personalidos

- Permitem estilizar elementos específicos de maneira flexível e eficiente usando CSS. 
- Esses seletores incluem:
  - IDs 
  - Classes 
  - Pseudo-classes
  - Pseudo-elementos

## 6.1. Seletor de ID

- O seletor de ID seleciona um elemento com base no atributo id do HTML. 
- IDs são únicos, o que significa que cada ID deve ser atribuído a apenas um elemento em um documento HTML.

- Como Utilizar ID
  - Defina o `id` no elemento HTML.
  - Use o símbolo `#` seguido do nome do ID no CSS para aplicar o estilo.

## 6.2. Seletor de Classe
- Permite aplicar o mesmo estilo a múltiplos elementos.

- Como Utilizar Classe

  - Defina o atributo class nos elementos HTML.
  - Use o nome da classe precedido de `.` no CSS.

## 6.3. Pseudo-classes

- As pseudo-classes são usadas para definir um estado especial de um elemento.
- Quando o usuário interage com ele (por exemplo, passar o mouse ou clicar).

  - Principais Pseudo-classes

    - **`:hover`**: Aplica o estilo quando o usuário passa o mouse sobre o elemento.
    - **`:focus`**: Aplica o estilo quando o elemento está focado, geralmente em campos de formulário.
    - **`:nth-child(n)`**: Seleciona o enésimo filho de um elemento pai.
  
    - Exemplo de Uso:

      ```css

      a:hover { /* Ao passar o mouse o link fica verde */
        color: green;
      }

      li:nth-child(2) { /* Aplica a cor laranja ao segundo item de uma lista.*/
        color: orange;
      }

      ```

## 6.4. Pseudo-elementos

- Os pseudo-elementos permitem estilizar partes específicas de um elemento, como a primeira letra ou linha de um parágrafo.

- Principais Pseudo-elementos

  - **`::before`**: Insere conteúdo antes do conteúdo real de um elemento.
  - **`::after`**: Insere conteúdo após o conteúdo real de um elemento.
  - **`::first-letter`**: Aplica o estilo à primeira letra do texto dentro de um elemento.
  - **`::first-line`**: Aplica o estilo à primeira linha do texto dentro de um elemento.

  - Exemplo de Uso:

    ```css

    p::before { /*Coloca um conteudo antes da tag p*/
      content: "Prefixo: ";
      font-weight: bold;
    }

    p::after { /*Coloca um conteudo depois da tag p*/
      content: " [sufixo]"; 
      color: gray;
    }
    p::first-letter { /*Coloca a primeira letra da tag p com essas propriedades abaixo*/
      font-size: 200%;
      color: red;
    }

    ```

## 6.5. Diferenças entre Pseudo-classe e Pseudo-elemento

- Pseudo-classes (ex: `:hover`, `:focus`) se aplicam a estados ou condições especiais dos elementos.
- Pseudo-elementos (ex: `::before, `::after`) permitem acessar e estilizar partes específicas do conteúdo de um elemento.
  
## 6.6. Seletores Combinados

- Você pode combinar seletor de classe, `id`, pseudo-classe e pseudo-elemento para aplicar estilos mais precisos.

  - Exemplo de Uso:

    ```css

    #paragrafo-unico:hover::first-letter {
      color: blue;
      font-size: 150%; /*altera o estilo da primeira letra do parágrafo com o ID "paragrafo-unico" quando o mouse passa sobre ele. */
    }

    ```

#  7. Modelos de caixas

- Em HTML, os elementos são renderizados como caixas, seguindo dois principais modelos de layout: 
  - Modelo de caixa em **nível de bloco** (box-level).
  - Modelo de caixa em **nível de linha** (inline-level). 
- Esses modelos controlam como o navegador renderiza os elementos na página e como eles se comportam no fluxo do layout.
  
## 7.1. Modelo de Caixa Box-Level (Bloco)

- O modelo de caixa de nível de bloco é aplicado a elementos que ocupam toda a largura disponível da página, iniciando em uma nova linha.
- Esses elementos empurram o conteúdo subsequente para a próxima linha.
  
  - Exemplos de Elementos Box-Level

    - **`<div>`**
    - **`<h1>`,`<h2>`,`<h3>`...**
    - **`<p>`**
    - **`<section>`**
  
  - Propriedades de Layout Box-Level

    - Elementos de bloco podem ter altura, largura, margem e preenchimento definidos de forma clara.
    - Eles sempre ocupam a largura total de seu contêiner pai, a menos que um valor de largura seja especificado.
  
  - Comportamento do Modelo Box-Level

    - Quando dois elementos de bloco são colocados consecutivamente, o segundo elemento será posicionado abaixo do primeiro, respeitando as margens e o espaço entre eles.

## 7.2. Modelo de Caixa Inline-Level (Linha)

- Elementos inline são renderizados na mesma linha em que estão posicionados, ocupando apenas o espaço necessário para o seu conteúdo.
- Eles não iniciam uma nova linha, o que permite que outros elementos estejam ao lado deles.

  - Exemplos de Elementos Inline-Level

    - **`<span>`**
    - **`<a>`**
    - **`<em>`, `<strong>`**
    - **`<img>`**

  - Propriedades de Layout Inline-Level

    - Elementos inline respeitam a largura do conteúdo e não permitem definir diretamente propriedades como width e height.
    - No entanto, é possível definir margens, preenchimentos e outros estilos que influenciam a aparência desses elementos.

  -Comportamento do Modelo Inline-Level

    - Elementos inline aparecem em sequência no mesmo fluxo de texto e permitem que outros elementos estejam adjacentes.
    - Eles não quebram a linha do conteúdo, a menos que o contêiner atinja seu limite de largura.

## 7.3. Diferenças entre Box-Level e Inline-Level

- **Box-Level**: Elementos ocupam toda a largura disponível, iniciando uma nova linha.
- **Inline-Level**: Elementos ocupam apenas o espaço necessário, permanecendo no fluxo de linha.

## 7.4. Box Model

- O **Box Model** em CSS define como a caixa de um elemento é composta e como suas propriedades afetam o layout.
  
- Cada elemento tem uma caixa que contém quatro áreas:
  
  - **Conteúdo**: O conteúdo real do elemento.
  - **Preenchimento (Padding)**: Espaço entre o conteúdo e a borda.
  - **Borda (Border)**: A borda ao redor do conteúdo e preenchimento.
  - **Margem (Margin)**: Espaço externo ao redor da borda.

# 8. Agrupamento de Tags (Grouping Tags)

- Usadas para organizar e estruturar o conteúdo da página.
- Permite agrupar elementos relacionados em blocos semânticos.
- Ajudam a criar uma hierarquia clara e facilitam o estilo e a manipulação de conteúdo.

## 8.1. Principais Tags de Agrupamento

- Utilizadas para definir a estrutura do layout.

  - **`<div>`**.
  - **`<span>`**.
  - **`<section>`**.
  - **`<article>`**.
  - **`<nav>`**.
  - **`<aside>`**.
  - **`<header>`**. 
  - **`<footer>`**.
  - **`<main>`**.
  - **`<figure>`**.
  - **`<figcaption>`**.


  - `<div>` (Division)

    - A tag `<div>` é um elemento de bloco genérico utilizado para agrupar outros elementos HTML.
    - Não possui um significado semântico próprio, sendo amplamente usado para aplicar estilos ou organizar o layout com CSS e JavaScript.
  
  - `<span>`

    - A tag `<span>` é um elemento inline genérico usado para agrupar partes do conteúdo sem alterar o fluxo de texto.
    - É frequentemente utilizado para aplicar estilos a partes específicas do texto.

  - `<section>`

    - A tag `<section>` define uma seção temática dentro do conteúdo de uma página, sendo usada para agrupar elementos relacionados que compartilham um contexto comum.
    - Diferente do `<div>`, o `<section>` possui significado semântico e é recomendado quando o conteúdo possui uma função específica.

  - `<article>`

    - A tag `<article>` é usada para representar uma unidade de conteúdo independente, como uma notícia, post de blog ou artigo.
    - O conteúdo dentro de um `<article>` é normalmente autocontido e pode ser distribuído de forma independente.

  - `<nav>`

    - A tag `<nav>` é usada para agrupar links de navegação.
    - É uma forma semântica de indicar que os links dentro desse elemento representam a navegação principal ou secundária de um site.
  
  - `<aside>`

    - A tag `<aside>` representa conteúdo tangencial ao conteúdo principal, como uma barra lateral, uma citação ou informações complementares.

  - `<header>`

    - A `<header>` é usada para definir o cabeçalho de uma página ou de uma seção importante. 
    - Geralmente contém títulos, logotipos, ou menus de navegação.

  - `<main>`

    - A `<main>` define o conteúdo principal de um documento. 
    - Apenas deve haver um elemento `<main>` por página, e ele deve conter o conteúdo central, excluindo navegação ou barras laterais.
  
  - `<footer>`

    - A `<footer>` representa o rodapé de uma página ou seção. Geralmente contém informações como direitos autorais, links adicionais ou informações de contato.

  - `<figure>`

    - A `<figure>` é usada para agrupar conteúdo de mídia, como imagens, gráficos ou diagramas, junto com legendas relacionadas, representadas pela tag `<figcaption>`.

  - `<figcaption>`

    - A `<figcaption>` define uma legenda ou descrição associada ao conteúdo dentro de um `<figure>`.
    - É usada para explicar ou fornecer contexto adicional para uma imagem ou gráfico.

  -Exemplo de Uso:

    ```html
    <figure>
      <img src="gráfico.png" alt="Gráfico de vendas">
      <figcaption>Gráfico de vendas do último trimestre.</figcaption>
    </figure>
    ```

##  8.2. Importância Semântica

- O uso correto das tags de agrupamento semânticas, melhora a acessibilidade e a indexação do conteúdo pelos motores de busca (SEO).
  
- `<div>` e `<span>` continuam sendo úteis para agrupamentos que não exigem uma semântica específica.

#  9. Sombra e Bordas Arredondadas

- As propriedades `box-shadow` e `border-radius` são amplamente utilizadas em conjunto no CSS para criar elementos visualmente atraentes. 
- Juntas, elas oferecem a possibilidade de adicionar profundidade, suavidade e destaque a caixas, botões, cartões e outros elementos.

##  9.1. Sombra (Box Shadow)

- A propriedade `box-shadow` aplica sombras a elementos, criando um efeito tridimensional.
- É possível ajustar o tamanho, desfoque e cor da sombra, além de definir se ela será externa ou interna ao elemento.

  - Sintaxe

    ```css
    box-shadow: offset-x offset-y blur-radius spread-radius color inset;
    ``` 
  - offset-x: Deslocamento horizontal da sombra.
  - offset-y: Deslocamento vertical da sombra.
  - blur-radius: Grau de desfoque.
  - spread-radius: Tamanho da sombra.
  - color: Cor da sombra.
  - inset: Aplica a sombra para dentro do elemento (opcional).

  - Exemplo de Uso

    ```css
    .elemento {
      box-shadow: 5px 10px 15px rgba(0, 0, 0, 0.3);
    }
    ```

##  9.2. Bordas Arredondadas (Border Radius)
- A propriedade `border-radius` permite criar bordas arredondadas em elementos.

- Sintaxe

  ```css
  border-radius: valor;
  ```

  - Exemplo de Uso

    ```css
    .caixa {
      border-radius: 15px;
    }
    ```

##  9.3. Combinação de box-shadow e border-radius

- O uso combinado de sombras e bordas arredondadas cria efeitos visuais elegantes, como cartões de destaque ou botões interativos.

- Exemplo de Combinação

  ```css
  .cartao {
    box-shadow: 4px 8px 12px rgba(0, 0, 0, 0.2);
    border-radius: 10px;
    padding: 20px;
    background-color: #fff;
  }
  ```

#  10. Variáveis em CSS

- As variáveis CSS permitem armazenar valores que podem ser reutilizados em várias partes de um documento CSS.
- Facilitam a manutenção do código.
- Permitindo alterar valores em um único lugar sem a necessidade de modificações repetitivas em todo o arquivo.

##  10.1. Definição de Variáveis

- As variáveis são definidas utilizando a sintaxe **`--nome-da-variável`**, e acessadas através da função var().

  - Sintaxe Básica
  
    - **`:root:`** É um pseudo-seletor que representa o nível mais alto do documento, permitindo que as variáveis definidas sejam globais.

    ```css
    /*Declarando as variáveis*/
    :root {
      --cor-principal: #3498db;
      --tamanho-fonte: 16px;
    }

    /* Usando as variáveis */
    .elemento {
      background-color: var(--cor-principal);
      font-size: var(--tamanho-fonte);
    }

    ```

##  10.2. Benefícios

- Facilita a manutenção de grandes arquivos CSS.
- Torna o código mais legível e reutilizável.

##  10.3. Exemplo Completo

  ```css

  :root {
    --cor-de-fundo: #f4f4f4;
    --cor-texto: #333;
    --padding-geral: 20px;
  }

  .caixa {
    background-color: var(--cor-de-fundo);
    color: var(--cor-texto);
    padding: var(--padding-geral);
  }

  ```
