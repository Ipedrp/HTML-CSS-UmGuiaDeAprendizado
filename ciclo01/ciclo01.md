- [1. Parágrafo e Quebra de Linha no HTML5](#1-parágrafo-e-quebra-de-linha-no-html5)
  - [1.1. Parágrafos](#11-parágrafos)
- [2. HTML Entities](#2-html-entities)
- [3. Uso da Tag `<img>`](#3-uso-da-tag-img)
  - [3.1. Atributos Principais](#31-atributos-principais)
  - [3.2. Formatos de Imagem](#32-formatos-de-imagem)
  - [3.3. Exemplo de Uso:](#33-exemplo-de-uso)
- [4. Favicon de um Site](#4-favicon-de-um-site)
  - [4.1. Como Adicionar um Favicon](#41-como-adicionar-um-favicon)
  - [4.2. Exemplos de Código:](#42-exemplos-de-código)
- [5. Hierarquia de Títulos](#5-hierarquia-de-títulos)
- [6. Semântica no HTML5 é Importante](#6-semântica-no-html5-é-importante)
  - [6.1. 10.1 HTML4 e HTML5](#61-101-html4-e-html5)
  - [6.2. O Uso do CSS](#62-o-uso-do-css)
- [7. Negrito e Itálico em HTML](#7-negrito-e-itálico-em-html)
  - [7.1. Negrito](#71-negrito)
  - [7.2. Itálico](#72-itálico)
    - [7.2.1. Exemplo de Uso:](#721-exemplo-de-uso)
- [8. Outras Formatações Adicionais em HTML](#8-outras-formatações-adicionais-em-html)
  - [8.1. Sublinhado](#81-sublinhado)
    - [8.1.1. Exemplo de Uso:](#811-exemplo-de-uso)
  - [8.2. Riscar](#82-riscar)
  - [8.3. Superscrito e Subscrito](#83-superscrito-e-subscrito)
  - [8.4. Citações e Blocos de Citação](#84-citações-e-blocos-de-citação)
  - [8.5. Código e Pré-formatado](#85-código-e-pré-formatado)
- [9. Listas Ordenadas e Desordenadas em HTML](#9-listas-ordenadas-e-desordenadas-em-html)
  - [9.1. Listas Ordenadas](#91-listas-ordenadas)
  - [9.2. Listas Desordenadas](#92-listas-desordenadas)
  - [9.3. Listas Aninhadas](#93-listas-aninhadas)
- [10. Links e Âncoras em HTML](#10-links-e-âncoras-em-html)
  - [10.1. Links](#101-links)
- [11. Imagens Dinâmicas em HTML](#11-imagens-dinâmicas-em-html)
  - [11.1. O Elemento `<picture>`](#111-o-elemento-picture)
- [12. Áudio em HTML](#12-áudio-em-html)
  - [12.1. O Elemento `<audio>`](#121-o-elemento-audio)
- [13. Vídeos em HTML](#13-vídeos-em-html)
  - [13.1. Inserindo Vídeos Hospedados Localmente](#131-inserindo-vídeos-hospedados-localmente)
- [14. Estilos Inline em HTML](#14-estilos-inline-em-html)
  - [14.1. Quando Usar CSS Inline](#141-quando-usar-css-inline)
    - [14.1.1. Vantagens:](#1411-vantagens)
    - [14.1.2. Desvantagens:](#1412-desvantagens)
  - [14.2. Exemplo de Uso de CSS Inline](#142-exemplo-de-uso-de-css-inline)
- [15. Estilos CSS Internos](#15-estilos-css-internos)
  - [15.1. Quando Usar CSS Interno](#151-quando-usar-css-interno)
    - [15.1.1. Vantagens:](#1511-vantagens)
    - [15.1.2. Desvantagens:](#1512-desvantagens)
  - [15.2. Exemplo de Uso de CSS Interno](#152-exemplo-de-uso-de-css-interno)
- [16. Estilos CSS Externos](#16-estilos-css-externos)
  - [16.1. Quando Usar CSS Externo](#161-quando-usar-css-externo)
  - [16.2. Exemplo de Uso de CSS Externo](#162-exemplo-de-uso-de-css-externo)



# 1. Parágrafo e Quebra de Linha no HTML5

##  1.1. Parágrafos

- Em HTML, os parágrafos são definidos com a tag `<p>`.
- A tag `<p>` cria um bloco de texto com margens automáticas ao redor.
- É usada para agrupar blocos de texto de forma semanticamente correta.
- A tag `<br> `é usada para inserir uma quebra de linha simples dentro do texto.
- Diferente da tag `<p>`, a tag `<br>` não cria um novo bloco, mas sim uma quebra dentro do mesmo bloco de texto.

  - Exemplo de Uso:

    ```html
        <p>Este é um exemplo de parágrafo em HTML.</p>
        <p>Este é um parágrafo com uma quebra de linha<br>no meio do texto.</p>
    ```

# 2. HTML Entities

- Tags podem aparecer no navegador usando entidades HTML (códigos especiais).
- Exemplo: `<` (menor que) é representado por `&lt;`.
- Exemplo: `>` (maior que) é representado por `&gt;`.

  ![Outros HTML Entities](../img/entities.png)

    - Exemplo de Uso:

      ```html
      <p>Para exibir o caractere menor que, use &lt;. Para o caractere maior que, use &gt;.</p>
      ```
# 3. Uso da Tag `<img>`

- A tag `<img>` é usada para exibir imagens em uma página web. Ela é uma tag auto-contida e não possui uma tag de fechamento.

##  3.1. Atributos Principais

- **`src`**: Define o caminho para o arquivo da imagem. Este atributo é obrigatório.
- **`alt`**: Fornece uma descrição alternativa da imagem, útil para acessibilidade e quando a imagem não pode ser carregada. Este atributo é recomendado.
- **`title`**: Exibe um texto quando o usuário passa o mouse sobre a imagem. Este atributo é opcional.
- **`width`** e **`height`**: Definem a largura e altura da imagem. Estes atributos são opcionais, mas é importante manter a proporção para evitar distorções.

##  3.2. Formatos de Imagem

- **JPEG (`.jpg`, `.jpeg`)**: Ideal para fotografias e imagens com muitos detalhes. Suporta compressão com perda, o que reduz o tamanho do arquivo.
- **PNG (`.png`)**: Ideal para imagens com fundo transparente e gráficos com cores sólidas. Suporta compressão sem perda.
- **GIF (`.gif`)**: Ideal para imagens animadas e gráficos simples com um número limitado de cores. Suporta animação e transparência, mas com menos qualidade do que o PNG.
- **SVG (`.svg`)**: Ideal para gráficos vetoriais e ícones. Pode ser escalado sem perda de qualidade, pois é baseado em vetores.

## 3.3. Exemplo de Uso:

```html
<img src="caminho/para/imagem.jpg" alt="Descrição da Imagem" title="Texto de Dica" width="300" height="200">
<img src="caminho/para/imagem.jpg" alt="Fotografia de um parque" title="Imagem JPG">
<img src="caminho/para/imagem.png" alt="Logo da empresa" title="Imagem PNG">
<img src="caminho/para/imagem.gif" alt="Animação divertida" title="Imagem GIF">
<img src="caminho/para/imagem.svg" alt="Ícone de usuário" title="Imagem SVG">

```
# 4. Favicon de um Site

- Um favicon é um pequeno ícone que aparece na aba do navegador ao lado do título da página. Ele ajuda a identificar visualmente o site e melhora a experiência do usuário.

##  4.1. Como Adicionar um Favicon

**Adicione o link para o favicon no `<head>` do seu HTML**: Use a tag `<link>` para referenciar o favicon. Aqui estão os exemplos para diferentes formatos de imagem:

## 4.2. Exemplos de Código:

  - Para um arquivo `.ico`:

    ```html
    <head>
        <link rel="icon" type="image/x-icon" href="/caminho/para/favicon.ico">
    </head>
    ```

  - Para um arquivo `.png`:

    ```html
    <head>
        <link rel="icon" type="image/png" href="/caminho/para/favicon.png">
    </head>
    ```

  - Para um arquivo `.svg`:

    ```html
    <head>
        <link rel="icon" type="image/svg+xml" href="/caminho/para/favicon.svg">
    </head>
    ```

# 5. Hierarquia de Títulos

- Títulos em HTML são chamados de **headings**.
- Existem seis níveis de headings.
- Usados para organizar o conteúdo da página.
- Somente um `<h1>` deve ser utilizado por página; os demais são subtítulos.

  - Exemplo de Uso:

    ```html

    <h1>Este é o título principal (H1)</h1>
    <h2>Este é um subtítulo de segundo nível (H2)</h2>
    <h3>Este é um subtítulo de terceiro nível (H3)</h3>
    <h4>Este é um subtítulo de quarto nível (H4)</h4>
    <h5>Este é um subtítulo de quinto nível (H5)</h5>
    <h6>Este é um subtítulo de sexto nível (H6)</h6>

    ```
# 6. Semântica no HTML5 é Importante

- Semântica refere-se ao significado dos elementos, em vez de apenas sua forma.
- O significado tem mais importância do que a aparência.

## 6.1. 10.1 HTML4 e HTML5
- No HTML4, o comportamento das tags era suficiente.
- No HTML5, o foco está em tags semânticas, priorizando o significado.

## 6.2. O Uso do CSS
- **CSS** cuida do estilo e da forma.
- O HTML não é mais responsável por alterar o design visual, como cores de texto ou o background; para isso, usa-se o CSS.

# 7. Negrito e Itálico em HTML

##  7.1. Negrito

- Para aplicar negrito ao texto em HTML, você pode usar a tag `<strong>` ou a tag `<b>`.
- A tag `<strong>` não só aplica o estilo de negrito, mas também dá ênfase semântica ao texto, indicando que ele é importante.
- A tag `<b>` aplica o estilo de negrito, mas não possui significado semântico.

##  7.2. Itálico
- Para aplicar itálico ao texto em HTML, você pode usar a tag` <em> `ou a tag `<i>`.
- A tag `<em>` não só aplica o estilo de itálico, mas também dá ênfase semântica ao texto, indicando que ele deve ser lido com ênfase.
- A tag `<i>` aplica o estilo de itálico, mas não possui significado semântico.

### 7.2.1. Exemplo de Uso:

```html

<p>Este é um texto com <strong>ênfase importante</strong> usando a tag <code>&lt;strong&gt;</code>.</p>
<p>Este é um texto com <b>negrito simples</b></p>
<p>Este é um texto com <em>ênfase importante</em></p>
<p>Este é um texto com <i>itálico simples</i></p>

``` 

# 8. Outras Formatações Adicionais em HTML

Além de negrito e itálico, HTML oferece várias outras opções de formatação para enriquecer o conteúdo da sua página web.

##  8.1. Sublinhado

- Para sublinhar texto, use a tag `<u>`.
- A tag `<u>` aplica um estilo de sublinhado ao texto, mas não possui significado semântico.

### 8.1.1. Exemplo de Uso:

```html 

<p>Este é um texto com <u>sublinhado</u> usando a tag <code>&lt;u&gt;</code>.</p>

```

##  8.2. Riscar

- Para riscar texto, use a tag `<s>` ou `<del>`.
- A tag `<s>` aplica um estilo de riscar ao texto, mas não possui significado semântico.
- A tag `<del>` é usada para marcar texto que foi removido e é exibida com uma linha atravessada, indicando alterações no conteúdo.

    - Exemplo de Uso:

      ```html

      <p>Este é um texto com <s>texto riscado</s></p>
      <p>Este é um texto com <del>texto deletado</del></p>

      ```

##  8.3. Superscrito e Subscrito

- Para aplicar o estilo de superscrito, use a tag `<sup>`.
- Para aplicar o estilo de subscrito, use a tag `<sub>`.

  - Exemplo de Uso:

  ```html

  <p>Este é um texto com <sup>superscrito</sup></p>
  <p>Este é um texto com <sub>subscrito</sub></p>

  ```

##  8.4. Citações e Blocos de Citação
- Para citações em linha, use a tag `<q>`.
- Para blocos de citação, use a tag ``<blockquote>``.
- A tag `<q>` é usada para citações curtas e adiciona aspas automaticamente.
- A tag `<blockquote>` é usada para citações longas e é formatada com uma margem.

  - Exemplo de Uso:

      ```html
      <p>Esta é uma citação em linha usando a tag <q>como exemplo</q>.</p>
      <blockquote>
          <p>Esta é uma citação em bloco. Ela é usada para exibir um bloco de texto em citação.</p>
          <footer> — Autor</footer>
      </blockquote>

      ```

##  8.5. Código e Pré-formatado

- Para exibir código, use a tag `<code>`.
- Para exibir texto pré-formatado, use a tag `<pre>`.
- A tag `<code>` é usada para marcar trechos de código ou comandos.
- A tag `<pre>` é usada para preservar espaços e quebras de linha no texto, mantendo o formato original.

  - Exemplo de Uso:

    ```html
    <p>Este é um exemplo de <code>código</code> dentro de um parágrafo.</p>
    <pre>
        <code>
    function exemplo() {
        console.log("Texto pré-formatado");
    }
        </code>
    </pre>

    ```

# 9. Listas Ordenadas e Desordenadas em HTML

Listas são uma maneira eficaz de organizar informações em HTML. Existem dois tipos principais de listas: ordenadas e desordenadas.

## 9.1. Listas Ordenadas

- Listas ordenadas são usadas quando a ordem dos itens é importante.
- São definidas com a tag `<ol>`, e cada item é marcado com a tag `<li>`.
- Os itens da lista são automaticamente numerados pelo navegador.
- É possível especificar o tipo de numeração usando o atributo `type`.

  - Tipos de Numeração:

    - **`type="1"`**: Números (1, 2, 3, …). Este é o padrão.
    - **`type="A"`**: Letras maiúsculas (A, B, C, …).
    - **`type="a"`**: Letras minúsculas (a, b, c, …).
    - **`type="I"`**: Números romanos maiúsculos (I, II, III, …).
    - **`type="i"`**: Números romanos minúsculos (i, ii, iii, …).

    - Exemplo de Uso:

        ```html 
        <ol>
            <li>Primeiro item</li>
            <li>Segundo item</li>
            <li>Terceiro item</li>
        </ol>
        ```

##  9.2. Listas Desordenadas
- Listas desordenadas são usadas quando a ordem dos itens não é importante.
- São definidas com a tag `<ul>`, e cada item é marcado com a tag `<li>`.
- Os itens da lista são precedidos por marcadores (geralmente pontos).

  - Tipos de Marcadores:
  - **`type="disc"`**: Marcador sólido (•). Este é o padrão.
  - **`type="circle"`**: Marcador vazio (◯).
  - **`type="square"`**: Marcador quadrado (▪).

  - Exemplo de Uso:

    ```html 
    <ul>
        <li>Item um</li>
        <li>Item dois</li>
        <li>Item três</li>
    </ul>

    ```

##  9.3. Listas Aninhadas
- Listas podem ser aninhadas dentro de outras listas para criar sublistas.
- Isso pode ser feito usando uma `<ul>` ou `<ol>` dentro de um item `<li>` de outra lista.

  - Exemplo de Uso:

    ```html

    <ol>
        <li>Primeiro item
            <ul>
                <li>Subitem um</li>
                <li>Subitem dois</li>
            </ul>
        </li>
        <li>Segundo item</li>
    </ol>

    ```
# 10. Links e Âncoras em HTML

- Links e âncoras são essenciais para a navegação entre páginas e seções em HTML. Eles permitem criar conexões e referências dentro de um site e entre sites.

## 10.1. Links

- Links são criados usando a tag `<a>`.
- A tag `<a>` é usada para criar um link que direciona o usuário para outra página, um endereço externo, ou uma âncora dentro da mesma página.
- O atributo principal da tag `<a>` é `href`, que define o destino do link.

  - Atributos Importantes:

    - **`href`**: Define o destino do link. Pode ser um URL, um caminho relativo para uma página no mesmo site, ou uma âncora dentro da mesma página.
    - **`target`**: Define como o link será aberto. Pode ter os seguintes valores:
      - **`_self`**: Abre o link na mesma janela/aba (padrão).
      - **`_blank`**: Abre o link em uma nova janela/aba.
      - **`_parent`**: Abre o link na janela/aba pai, se houver um `<iframe>` envolvido.
      - **`_top`**: Abre o link na janela/aba principal, substituindo qualquer `<iframe>`.
    - **`rel`**: Define a relação entre a página atual e o link. Usado principalmente para melhorar a segurança e SEO. Exemplos:
      - **`nofollow`**: Indica que os motores de busca não devem seguir o link.
      - **`noopener`**: Melhora a segurança ao abrir links em novas abas, evitando que a nova página possa acessar a página original.
      - **`noreferrer`**: Impede o envio de informações sobre a origem do link ao site de destino.
      
      - Exemplo de Uso:

        ```html

        <a href="https://www.example.com" target="_blank" rel="noopener noreferrer">Visite o Example.com</a>

        ```
# 11. Imagens Dinâmicas em HTML

- Imagens dinâmicas são imagens que se adaptam a diferentes dispositivos e resoluções de tela, proporcionando uma experiência responsiva para os usuários. Isso é essencial no design responsivo, garantindo que as imagens sejam exibidas corretamente em diferentes tamanhos de tela.

##  11.1. O Elemento `<picture>`

- O elemento `<picture>` em HTML permite definir múltiplas versões de uma imagem para diferentes condições, como tamanhos de tela ou tipos de dispositivo. Ele funciona em conjunto com o atributo `srcset` e a tag `<source>`, permitindo que o navegador escolha a imagem mais adequada com base em uma série de critérios.

  - Atributos Importantes:

    - **`<picture>`**: Define um contêiner para imagens que podem mudar dependendo das condições de exibição, como a largura da tela.
    - **`<source>`**: Define um ou mais recursos de imagem, cada um com sua própria condição (geralmente um `media query`).
      - **`media`**: Utiliza media queries para definir condições específicas (ex: largura máxima da tela).
      - **`srcset`**: Define o caminho da imagem que será exibida se as condições do `media` forem atendidas.
      - **`type`**: Define o tipo do arquivo de imagem, como `image/png` ou `image/jpeg`.
    - **`<img>`**: Fallback padrão, utilizado caso nenhuma das condições anteriores sejam atendidas. O navegador exibirá essa imagem se as outras condições falharem.

    - Exemplo de Uso:

      ```html
      <picture>
          <source media="(max-width: 700px)" srcset="img/pequena.png" type="image/png">
          <source media="(max-width: 1050px)" srcset="img/media.png" type="image/png">
          <img src="img/grande.png" alt="Imagem responsiva">
      </picture>
      ```

# 12. Áudio em HTML

- O elemento `<audio>` em HTML permite adicionar músicas ou outros arquivos de áudio diretamente em uma página da web. Ele suporta diferentes formatos e oferece uma experiência interativa ao usuário com controles nativos do navegador.

##  12.1. O Elemento `<audio>`

- O elemento `<audio>` pode ser utilizado para incorporar arquivos de áudio no HTML, e o navegador exibirá um player com controles (play, pause, volume, etc.) para o usuário. Além disso, você pode especificar diferentes versões do arquivo de áudio em formatos distintos (MP3, OGG, WAV) para maximizar a compatibilidade com todos os navegadores.

  - Atributos Importantes:

    - **`controls`**: Exibe os controles padrão do navegador para o áudio (play, pause, volume, etc.).
    - **`autoplay`**: Faz o áudio começar a tocar automaticamente assim que a página carrega. 
      - **Atenção**: Muitos navegadores bloqueiam a reprodução automática sem interação do usuário, especialmente quando o áudio não está silenciado.
    - **`preload`**: Informa ao navegador como ele deve lidar com o carregamento do áudio.
      - **Valores**:
        - `none`: Não carrega o áudio até que o usuário clique em play.
        - `metadata`: Carrega apenas os metadados (duração, etc.) do áudio.
        - `auto`: Carrega o áudio assim que a página é carregada.
    - **`loop`**: Faz o áudio repetir automaticamente quando chega ao final.
    - **`<source>`**: Especifica o caminho do arquivo de áudio e seu formato. Vários `<source>` podem ser utilizados para oferecer compatibilidade com diferentes navegadores.
    - **Fallback (texto dentro da tag `<audio>`)**: Exibido quando o navegador não suporta a reprodução de áudio. Pode incluir um link para download do arquivo.

    - Exemplo de Uso:

      ```html

      <audio preload="metadata" autoplay controls loop>
          <source src="midia/FKJ & Tom Misch - Losing My Way.mp3" type="audio/mpeg">
          <source src="midia/FKJ & Tom Misch - Losing My Way.ogg" type="audio/ogg">
          <source src="midia/FKJ & Tom Misch - Losing My Way.wav" type="audio/wav">
          <p>Infelizmente, seu navegador não pode reproduzir esse áudio! 
          <a href="midia/FKJ & Tom Misch - Losing My Way.mp3">Clique aqui para baixar o arquivo MP3</a></p>
      </audio>

      ```   
# 13. Vídeos em HTML

- O elemento `<video>` permite a incorporação de vídeos diretamente em uma página da web. Além disso, também é possível incorporar vídeos hospedados em plataformas como o YouTube usando o elemento `<iframe>`.

##  13.1. Inserindo Vídeos Hospedados Localmente

- Você pode hospedar vídeos diretamente em seu servidor e exibi-los em sua página HTML usando a tag `<video>`. Esse método permite que você controle completamente o vídeo e seus formatos.

  - Atributos Importantes:

    - **`width`**: Define a largura do vídeo.
    - **`controls`**: Exibe os controles de reprodução (play, pause, volume, etc.) no player.
    - **`autoplay`**: Faz o vídeo começar a tocar automaticamente ao carregar a página.
    - **`loop`**: Faz o vídeo repetir automaticamente quando termina.
    - **`muted`**: Inicia o vídeo sem som (requerido por alguns navegadores ao usar `autoplay`).
    - **`poster`**: Define uma imagem a ser exibida enquanto o vídeo não começa.
  
    - Exemplo de Vídeo Hospedado Localmente:

        ```html

        <h1>Inserindo vídeos hospedados localmente</h1>
        <p>Este vídeo está hospedado no meu próprio servidor:</p>

        <video width="500" poster="img/images.jpeg" muted autoplay loop controls>
            <source src="videos/meuvideo.mp4" type="video/mp4">
            <source src="videos/meuvideo1.webm" type="video/webm">
            <p>Perdão, mas seu navegador não aceita nenhum formato de vídeo.</p>
        </video>

        ```
# 14. Estilos Inline em HTML

- O CSS inline é uma das maneiras de adicionar estilos diretamente aos elementos HTML. Ele é aplicado diretamente no atributo `style` de um elemento e pode ser útil para alterações rápidas ou personalizações específicas.

##  14.1. Quando Usar CSS Inline

- O CSS inline permite que você aplique estilos diretamente a um único elemento HTML sem precisar de uma folha de estilo externa ou interna. No entanto, seu uso não é recomendado para grandes projetos, pois pode dificultar a manutenção e a consistência do design.

### 14.1.1. Vantagens:

- Útil para pequenas modificações rápidas.
- Fácil de aplicar em testes ou correções temporárias.
- Funciona diretamente no arquivo HTML sem a necessidade de um arquivo CSS separado.

### 14.1.2. Desvantagens:

- Não é reutilizável como estilos em arquivos CSS externos.
- Pode tornar o código mais difícil de manter e escalar.
- Torna o HTML mais "poluído" com código de estilo.

##  14.2. Exemplo de Uso de CSS Inline

- Neste exemplo, o estilo é aplicado diretamente no elemento HTML usando o atributo `style`. Ele modifica a cor do texto e o espaçamento interno (padding) do parágrafo.

  ```html
  <p style="color: blue; padding: 10px; background-color: lightgray;">
      Este parágrafo tem um estilo inline que define a cor do texto como azul, adiciona espaçamento interno e define a cor de fundo como cinza claro.
  </p>

  ```

# 15. Estilos CSS Internos

- O CSS interno, também conhecido como **CSS embutido**, é uma forma de adicionar estilos diretamente dentro de uma página HTML, utilizando a tag `<style>` no cabeçalho (`<head>`). Este método permite que você aplique estilos a toda a página, sem a necessidade de um arquivo CSS separado.

##  15.1. Quando Usar CSS Interno

- O CSS interno é útil quando você precisa estilizar uma única página HTML e não planeja reutilizar esses estilos em outras páginas. Ele pode ser uma solução rápida para projetos pequenos ou páginas isoladas, mas, assim como o CSS inline, deve ser usado com cautela em projetos maiores.

### 15.1.1. Vantagens:

- Fácil de usar em projetos pequenos ou em protótipos.
- Os estilos são aplicados a todos os elementos da página sem necessidade de arquivos CSS externos.
- Não requer links externos, então é ótimo para páginas autossuficientes.

### 15.1.2. Desvantagens:

- Não é reutilizável em outras páginas, o que pode aumentar o tamanho e a complexidade do código.
- Difícil de manter em sites maiores com múltiplas páginas.
- Menos eficiente em termos de performance em comparação ao CSS externo.

##  15.2. Exemplo de Uso de CSS Interno

```html

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Exemplo de CSS Interno</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            color: #333;
            padding: 20px;
        }
        p {
            background-color: #fff;
            padding: 10px;
            border-radius: 5px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }
    </style>
</head>
<body>
    <p>Este parágrafo está sendo estilizado usando CSS interno. A cor do texto, o espaçamento interno, a sombra e o arredondamento dos cantos são aplicados com o uso de CSS na tag <style> no cabeçalho da página.</p>
</body>
</html>

```
---

# 16. Estilos CSS Externos

- O CSS externo é uma forma de separar completamente o estilo do conteúdo HTML, usando um arquivo `.css` separado. Esse método é o mais recomendado para projetos maiores, pois facilita a reutilização de estilos e a manutenção do código.

##  16.1. Quando Usar CSS Externo

- O CSS externo é a melhor prática quando você está trabalhando em projetos com múltiplas páginas, onde o estilo precisa ser consistente. Ele permite aplicar estilos a várias páginas ao mesmo tempo, sem duplicar código, mantendo a organização e facilitando atualizações.

  - Vantagens:

    - **Reutilizável**: Um arquivo CSS pode ser aplicado a várias páginas ao mesmo tempo.
    - **Organização**: O HTML fica mais limpo, pois o código de estilo fica em um arquivo separado.
    - **Manutenção**: Facilidade em manter e atualizar o design, pois todas as páginas compartilham o mesmo arquivo de estilo.

  - Desvantagens:

    - Requer uma solicitação extra ao servidor para carregar o arquivo CSS, o que pode aumentar ligeiramente o tempo de carregamento da página.
    - Precisa de um bom controle de versionamento para garantir que mudanças de estilo não afetem inadvertidamente outras páginas.

##  16.2. Exemplo de Uso de CSS Externo

  - Arquivo HTML:

    ```html

    <!DOCTYPE html>
    <html lang="pt-br">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Exemplo de CSS Externo</title>
        <link rel="stylesheet" href="styles.css">
    </head>
    <body>
        <h1>Estilos CSS Externos</h1>
        <p>Este parágrafo está sendo estilizado usando um arquivo CSS externo. A vantagem do CSS externo é que ele pode ser reutilizado em várias páginas do site.</p>
    </body>
    </html>

    ```

  - Estrutura de Pastas para CSS Externo

    ```bash

    meu-projeto/
    │
    ├── index.html           # Arquivo HTML principal
    │
    ├── css/                 # Diretório para arquivos CSS
    │   ├── styles.css       # Arquivo de estilos CSS principal
    │          
    │
    ├── js/                  # Diretório para arquivos JavaScript
    │   └── script.js        # Arquivo de scripts JavaScript
    │
    ├── img/                 # Diretório para imagens
    │   ├── logo.png         # Exemplo de imagem do projeto
    │   └── banner.jpg       # Exemplo de imagem do projeto
    │
    └── assets/              # Diretório para outros recursos, como fontes e ícones
        ├── fonts/           # Subdiretório para fontes
        │   └── custom-font.ttf
        └── icons/           # Subdiretório para ícones SVG ou outros formatos
    ```