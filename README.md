# Como a Internet Chega na Minha Casa?

# 1. Como surgiu a internet?

- A internet surgiu durante a Guerra Fria.

## 1.1 DARPA e ARPANET

### 1.1.1 DARPA

- A **Defense Advanced Research Projects Agency** (DARPA) realizou investimentos iniciais ao desenvolvimento de tecnologias como a criação da ARPANET.

### 1.1.2 ARPANET

- Primeira rede de computadores.
- Criada para transmitir dados militares e interligar departamentos de pesquisa nos Estados Unidos.
- Incluía 4 tipos diferentes de computadores: SDS 90, SDS Sigma 7, IBM 370/75 e DEC PDP-10.
- Cada computador tinha uma linguagem própria, dificultando a comunicação.

## 1.2 NCP

- **Network Control Protocol**.
- Permitia a comunicação entre diferentes redes de computadores.
- Necessitava parar a rede para poder se comunicar.

## 1.3 TCP/IP

- **TCP** (Transmission Control Protocol) e **IP** (Internet Protocol).
- Resolveu o problema de parar a rede para comunicação.
- Atualmente, é o protocolo utilizado.

## 1.4 Como funciona a internet?

- Relacionamento cliente e servidor.
- O cliente faz uma solicitação (request).
- O servidor entrega o que foi solicitado como resposta (response).

## 1.5 Como era a internet?

- Utilizava o protocolo **GOPHER**.
- Navegação era feita apenas pelo teclado.

## 1.6 Surgimento da WWW

### 1.6.1 Tim Berners-Lee

- Criou o protocolo **HTTP** (Hypertext Transfer Protocol), **HTML** (Hypertext Markup Language) e a **WWW** (World Wide Web).

### 1.6.2 Marc Andreessen

- Criou o **Mosaic**, o primeiro navegador compatível com HTTP.

## 1.7 WWW não é a internet?

- A WWW é apenas mais uma sub-rede da internet, especializada em **HTTP**.

### 1.7.1 A internet é composta por outros protocolos:

- **FTP**, **GOPHER**, **SMTP**, **POP3**, **IMAP**.

---

# 2. Como a Internet Funciona?

## 2.1 O que é bit e byte?

- **Bit** é representado por 0 ou 1.
- 0 representa ausência de sinal.
- 1 representa presença de sinal.
- A sequência de 8 bits forma 1 byte.

## 2.2 Servidor DNS

- Converte nomes de domínio em endereços IP, definindo qual servidor o usuário alcançará ao digitar um domínio no navegador.

---

# 3. Domínio e Hospedagem

## 3.1 Domínio

- É o endereço do site.
- Deve ser único.
- Existem vários **TLDs** (Top-Level Domain).

## 3.2 Hospedagem

- Espaço utilizado para armazenar os arquivos do site.

---

# 4. HTML, CSS e JavaScript

## 4.1 HTML (HyperText Markup Language)

- Define o conteúdo do site (texto, imagens, tabelas, vídeos, etc.).
![Tag HTML](../html/img/tagP.png)
![Estrutura HTML](../html/img/estrutura.png)

## 4.2 CSS (Cascading Style Sheets)

- Define o design e o estilo visual (cores, sombras, tamanhos, posicionamento, etc.).
![Estilo CSS](../html//img/estilo.png)

## 4.3 JavaScript (Linguagem de Programação)

- Responsável pelas interações, como menus, animações, popups e validações de formulários.
- 
---

# 5. Parágrafo e Quebra de Linha no HTML5

## 5.1 Parágrafos

- Em HTML, os parágrafos são definidos com a tag `<p>`.
- A tag `<p>` cria um bloco de texto com margens automáticas ao redor.
- É usada para agrupar blocos de texto de forma semanticamente correta.
- A tag `<br> `é usada para inserir uma quebra de linha simples dentro do texto.
- Diferente da tag `<p>`, a tag `<br>` não cria um novo bloco, mas sim uma quebra dentro do mesmo bloco de texto.

### Exemplo de Uso:

```html
    <p>Este é um exemplo de parágrafo em HTML.</p>
    <p>Este é um parágrafo com uma quebra de linha<br>no meio do texto.</p>
```
---

# 6. HTML Entities

- Tags podem aparecer no navegador usando entidades HTML (códigos especiais).
- Exemplo: `<` (menor que) é representado por `&lt;`.
- Exemplo: `>` (maior que) é representado por `&gt;`.
![Outros HTML Entities](../html/img/entities.png)

### Exemplo de Uso:

```html
<p>Para exibir o caractere menor que, use &lt;. Para o caractere maior que, use &gt;.</p>
```
---


# 7. Uso da Tag `<img>`

- A tag `<img>` é usada para exibir imagens em uma página web. Ela é uma tag auto-contida e não possui uma tag de fechamento.

## 7.1 Atributos Principais

- **`src`**: Define o caminho para o arquivo da imagem. Este atributo é obrigatório.
- **`alt`**: Fornece uma descrição alternativa da imagem, útil para acessibilidade e quando a imagem não pode ser carregada. Este atributo é recomendado.
- **`title`**: Exibe um texto quando o usuário passa o mouse sobre a imagem. Este atributo é opcional.
- **`width`** e **`height`**: Definem a largura e altura da imagem. Estes atributos são opcionais, mas é importante manter a proporção para evitar distorções.

## 7.2 Formatos de Imagem

- **JPEG (`.jpg`, `.jpeg`)**: Ideal para fotografias e imagens com muitos detalhes. Suporta compressão com perda, o que reduz o tamanho do arquivo.
- **PNG (`.png`)**: Ideal para imagens com fundo transparente e gráficos com cores sólidas. Suporta compressão sem perda.
- **GIF (`.gif`)**: Ideal para imagens animadas e gráficos simples com um número limitado de cores. Suporta animação e transparência, mas com menos qualidade do que o PNG.
- **SVG (`.svg`)**: Ideal para gráficos vetoriais e ícones. Pode ser escalado sem perda de qualidade, pois é baseado em vetores.

## Exemplo de Uso:

```html
<img src="caminho/para/imagem.jpg" alt="Descrição da Imagem" title="Texto de Dica" width="300" height="200">
<img src="caminho/para/imagem.jpg" alt="Fotografia de um parque" title="Imagem JPG">
<img src="caminho/para/imagem.png" alt="Logo da empresa" title="Imagem PNG">
<img src="caminho/para/imagem.gif" alt="Animação divertida" title="Imagem GIF">
<img src="caminho/para/imagem.svg" alt="Ícone de usuário" title="Imagem SVG">

```
---

# 8. Favicon de um Site

- Um favicon é um pequeno ícone que aparece na aba do navegador ao lado do título da página. Ele ajuda a identificar visualmente o site e melhora a experiência do usuário.

## 8.1 Como Adicionar um Favicon

**Adicione o link para o favicon no `<head>` do seu HTML**: Use a tag `<link>` para referenciar o favicon. Aqui estão os exemplos para diferentes formatos de imagem:

## Exemplos de Código:

### Para um arquivo `.ico`:

```html
<head>
    <link rel="icon" type="image/x-icon" href="/caminho/para/favicon.ico">
</head>
```

### Para um arquivo `.png`:

```html

<head>
    <link rel="icon" type="image/png" href="/caminho/para/favicon.png">
</head>

```

### Para um arquivo `.svg`:

```html

<head>
    <link rel="icon" type="image/svg+xml" href="/caminho/para/favicon.svg">
</head>

```
---

# 9. Hierarquia de Títulos

- Títulos em HTML são chamados de **headings**.
- Existem seis níveis de headings.
- Usados para organizar o conteúdo da página.
- Somente um `<h1>` deve ser utilizado por página; os demais são subtítulos.

### Exemplo de Uso:

```html

<h1>Este é o título principal (H1)</h1>
<h2>Este é um subtítulo de segundo nível (H2)</h2>
<h3>Este é um subtítulo de terceiro nível (H3)</h3>
<h4>Este é um subtítulo de quarto nível (H4)</h4>
<h5>Este é um subtítulo de quinto nível (H5)</h5>
<h6>Este é um subtítulo de sexto nível (H6)</h6>

```
---

# 10. Semântica no HTML5 é Importante

- Semântica refere-se ao significado dos elementos, em vez de apenas sua forma.
- O significado tem mais importância do que a aparência.

## 10.1 HTML4 e HTML5
- No HTML4, o comportamento das tags era suficiente.
- No HTML5, o foco está em tags semânticas, priorizando o significado.

## 10.2 O Uso do CSS
- **CSS** cuida do estilo e da forma.
- O HTML não é mais responsável por alterar o design visual, como cores de texto ou o background; para isso, usa-se o CSS.

---

# 11. Negrito e Itálico em HTML

## 11.1 Negrito

- Para aplicar negrito ao texto em HTML, você pode usar a tag `<strong>` ou a tag `<b>`.
- A tag `<strong>` não só aplica o estilo de negrito, mas também dá ênfase semântica ao texto, indicando que ele é importante.
- A tag `<b>` aplica o estilo de negrito, mas não possui significado semântico.

## 11.2 Itálico
- Para aplicar itálico ao texto em HTML, você pode usar a tag` <em> `ou a tag `<i>`.
- A tag `<em>` não só aplica o estilo de itálico, mas também dá ênfase semântica ao texto, indicando que ele deve ser lido com ênfase.
- A tag `<i>` aplica o estilo de itálico, mas não possui significado semântico.

### Exemplo de Uso:

```html

<p>Este é um texto com <strong>ênfase importante</strong> usando a tag <code>&lt;strong&gt;</code>.</p>
<p>Este é um texto com <b>negrito simples</b></p>
<p>Este é um texto com <em>ênfase importante</em></p>
<p>Este é um texto com <i>itálico simples</i></p>

``` 
---

# 12. Outras Formatações Adicionais em HTML

Além de negrito e itálico, HTML oferece várias outras opções de formatação para enriquecer o conteúdo da sua página web.

## 12.1 Sublinhado

- Para sublinhar texto, use a tag `<u>`.
- A tag `<u>` aplica um estilo de sublinhado ao texto, mas não possui significado semântico.

### Exemplo de Uso:

```html 

<p>Este é um texto com <u>sublinhado</u> usando a tag <code>&lt;u&gt;</code>.</p>

```

## 12.2 Riscar

- Para riscar texto, use a tag `<s>` ou `<del>`.
- A tag `<s>` aplica um estilo de riscar ao texto, mas não possui significado semântico.
- A tag `<del>` é usada para marcar texto que foi removido e é exibida com uma linha atravessada, indicando alterações no conteúdo.

### Exemplo de Uso:

```html

<p>Este é um texto com <s>texto riscado</s></p>
<p>Este é um texto com <del>texto deletado</del></p>

```

## 12.3. Superscrito e Subscrito

- Para aplicar o estilo de superscrito, use a tag `<sup>`.
- Para aplicar o estilo de subscrito, use a tag `<sub>`.

### Exemplo de Uso:

```html

<p>Este é um texto com <sup>superscrito</sup></p>
<p>Este é um texto com <sub>subscrito</sub></p>

```
## 12.4. Citações e Blocos de Citação
- Para citações em linha, use a tag `<q>`.
- Para blocos de citação, use a tag ``<blockquote>``.
- A tag `<q>` é usada para citações curtas e adiciona aspas automaticamente.
- A tag `<blockquote>` é usada para citações longas e é formatada com uma margem.

### Exemplo de Uso:

```html
<p>Esta é uma citação em linha usando a tag <q>como exemplo</q>.</p>
<blockquote>
    <p>Esta é uma citação em bloco. Ela é usada para exibir um bloco de texto em citação.</p>
    <footer> — Autor</footer>
</blockquote>

```

## 12.5. Código e Pré-formatado

- Para exibir código, use a tag `<code>`.
- Para exibir texto pré-formatado, use a tag `<pre>`.
- A tag `<code>` é usada para marcar trechos de código ou comandos.
- A tag `<pre>` é usada para preservar espaços e quebras de linha no texto, mantendo o formato original.

### Exemplo de Uso:

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

---

# 13. Listas Ordenadas e Desordenadas em HTML

Listas são uma maneira eficaz de organizar informações em HTML. Existem dois tipos principais de listas: ordenadas e desordenadas.

## 13.1 Listas Ordenadas

- Listas ordenadas são usadas quando a ordem dos itens é importante.
- São definidas com a tag `<ol>`, e cada item é marcado com a tag `<li>`.
- Os itens da lista são automaticamente numerados pelo navegador.
- É possível especificar o tipo de numeração usando o atributo `type`.

### 13.1.1 Tipos de Numeração:

- **`type="1"`**: Números (1, 2, 3, …). Este é o padrão.
- **`type="A"`**: Letras maiúsculas (A, B, C, …).
- **`type="a"`**: Letras minúsculas (a, b, c, …).
- **`type="I"`**: Números romanos maiúsculos (I, II, III, …).
- **`type="i"`**: Números romanos minúsculos (i, ii, iii, …).


#### Exemplo de Uso:

```html 
<ol>
    <li>Primeiro item</li>
    <li>Segundo item</li>
    <li>Terceiro item</li>
</ol>
```

## 13.2 Listas Desordenadas
- Listas desordenadas são usadas quando a ordem dos itens não é importante.
- São definidas com a tag `<ul>`, e cada item é marcado com a tag `<li>`.
- Os itens da lista são precedidos por marcadores (geralmente pontos).

### 13.1.1 Tipos de Marcadores:
- **`type="disc"`**: Marcador sólido (•). Este é o padrão.
- **`type="circle"`**: Marcador vazio (◯).
- **`type="square"`**: Marcador quadrado (▪).

#### Exemplo de Uso:

```html 
<ul>
    <li>Item um</li>
    <li>Item dois</li>
    <li>Item três</li>
</ul>

```

## 13.3 Listas Aninhadas
- Listas podem ser aninhadas dentro de outras listas para criar sublistas.
- Isso pode ser feito usando uma `<ul>` ou `<ol>` dentro de um item `<li>` de outra lista.

### Exemplo de Uso:

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
---

# 14. Links e Âncoras em HTML

- Links e âncoras são essenciais para a navegação entre páginas e seções em HTML. Eles permitem criar conexões e referências dentro de um site e entre sites.

## 14.1 Links

- Links são criados usando a tag `<a>`.
- A tag `<a>` é usada para criar um link que direciona o usuário para outra página, um endereço externo, ou uma âncora dentro da mesma página.
- O atributo principal da tag `<a>` é `href`, que define o destino do link.

### Atributos Importantes:

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

### Exemplo de Uso:

```html

<a href="https://www.example.com" target="_blank" rel="noopener noreferrer">Visite o Example.com</a>

```
---

# 15. Imagens Dinâmicas em HTML

-Imagens dinâmicas são imagens que se adaptam a diferentes dispositivos e resoluções de tela, proporcionando uma experiência responsiva para os usuários. Isso é essencial no design responsivo, garantindo que as imagens sejam exibidas corretamente em diferentes tamanhos de tela.

## 15.1 O Elemento `<picture>`

-O elemento `<picture>` em HTML permite definir múltiplas versões de uma imagem para diferentes condições, como tamanhos de tela ou tipos de dispositivo. Ele funciona em conjunto com o atributo `srcset` e a tag `<source>`, permitindo que o navegador escolha a imagem mais adequada com base em uma série de critérios.

### Atributos Importantes:

- **`<picture>`**: Define um contêiner para imagens que podem mudar dependendo das condições de exibição, como a largura da tela.
- **`<source>`**: Define um ou mais recursos de imagem, cada um com sua própria condição (geralmente um `media query`).
  - **`media`**: Utiliza media queries para definir condições específicas (ex: largura máxima da tela).
  - **`srcset`**: Define o caminho da imagem que será exibida se as condições do `media` forem atendidas.
  - **`type`**: Define o tipo do arquivo de imagem, como `image/png` ou `image/jpeg`.
- **`<img>`**: Fallback padrão, utilizado caso nenhuma das condições anteriores sejam atendidas. O navegador exibirá essa imagem se as outras condições falharem.

### Exemplo de Uso:

```html
<picture>
    <source media="(max-width: 700px)" srcset="img/pequena.png" type="image/png">
    <source media="(max-width: 1050px)" srcset="img/media.png" type="image/png">
    <img src="img/grande.png" alt="Imagem responsiva">
</picture>
```
---

# 16. Áudio em HTML

- O elemento `<audio>` em HTML permite adicionar músicas ou outros arquivos de áudio diretamente em uma página da web. Ele suporta diferentes formatos e oferece uma experiência interativa ao usuário com controles nativos do navegador.

## 16.1 O Elemento `<audio>`

- O elemento `<audio>` pode ser utilizado para incorporar arquivos de áudio no HTML, e o navegador exibirá um player com controles (play, pause, volume, etc.) para o usuário. Além disso, você pode especificar diferentes versões do arquivo de áudio em formatos distintos (MP3, OGG, WAV) para maximizar a compatibilidade com todos os navegadores.

### Atributos Importantes:

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

### Exemplo de Uso:

```html

<audio preload="metadata" autoplay controls loop>
    <source src="midia/FKJ & Tom Misch - Losing My Way.mp3" type="audio/mpeg">
    <source src="midia/FKJ & Tom Misch - Losing My Way.ogg" type="audio/ogg">
    <source src="midia/FKJ & Tom Misch - Losing My Way.wav" type="audio/wav">
    <p>Infelizmente, seu navegador não pode reproduzir esse áudio! 
    <a href="midia/FKJ & Tom Misch - Losing My Way.mp3">Clique aqui para baixar o arquivo MP3</a></p>
</audio>

```   
---

# 17. Vídeos em HTML

- O elemento `<video>` permite a incorporação de vídeos diretamente em uma página da web. Além disso, também é possível incorporar vídeos hospedados em plataformas como o YouTube usando o elemento `<iframe>`.

## 17.1 Inserindo Vídeos Hospedados Localmente

- Você pode hospedar vídeos diretamente em seu servidor e exibi-los em sua página HTML usando a tag `<video>`. Esse método permite que você controle completamente o vídeo e seus formatos.

### Atributos Importantes:

- **`width`**: Define a largura do vídeo.
- **`controls`**: Exibe os controles de reprodução (play, pause, volume, etc.) no player.
- **`autoplay`**: Faz o vídeo começar a tocar automaticamente ao carregar a página.
- **`loop`**: Faz o vídeo repetir automaticamente quando termina.
- **`muted`**: Inicia o vídeo sem som (requerido por alguns navegadores ao usar `autoplay`).
- **`poster`**: Define uma imagem a ser exibida enquanto o vídeo não começa.

### Exemplo de Vídeo Hospedado Localmente:

```html

<h1>Inserindo vídeos hospedados localmente</h1>
<p>Este vídeo está hospedado no meu próprio servidor:</p>

<video width="500" poster="img/images.jpeg" muted autoplay loop controls>
    <source src="videos/meuvideo.mp4" type="video/mp4">
    <source src="videos/meuvideo1.webm" type="video/webm">
    <p>Perdão, mas seu navegador não aceita nenhum formato de vídeo.</p>
</video>

```

---

# 18. Estilos Inline em HTML

- O CSS inline é uma das maneiras de adicionar estilos diretamente aos elementos HTML. Ele é aplicado diretamente no atributo `style` de um elemento e pode ser útil para alterações rápidas ou personalizações específicas.

## 18.1 Quando Usar CSS Inline

- O CSS inline permite que você aplique estilos diretamente a um único elemento HTML sem precisar de uma folha de estilo externa ou interna. No entanto, seu uso não é recomendado para grandes projetos, pois pode dificultar a manutenção e a consistência do design.

### Vantagens:

- Útil para pequenas modificações rápidas.
- Fácil de aplicar em testes ou correções temporárias.
- Funciona diretamente no arquivo HTML sem a necessidade de um arquivo CSS separado.

### Desvantagens:

- Não é reutilizável como estilos em arquivos CSS externos.
- Pode tornar o código mais difícil de manter e escalar.
- Torna o HTML mais "poluído" com código de estilo.

## 18.2 Exemplo de Uso de CSS Inline

- Neste exemplo, o estilo é aplicado diretamente no elemento HTML usando o atributo `style`. Ele modifica a cor do texto e o espaçamento interno (padding) do parágrafo.

```html
<p style="color: blue; padding: 10px; background-color: lightgray;">
    Este parágrafo tem um estilo inline que define a cor do texto como azul, adiciona espaçamento interno e define a cor de fundo como cinza claro.
</p>

```

# 19. Estilos CSS Internos

- O CSS interno, também conhecido como **CSS embutido**, é uma forma de adicionar estilos diretamente dentro de uma página HTML, utilizando a tag `<style>` no cabeçalho (`<head>`). Este método permite que você aplique estilos a toda a página, sem a necessidade de um arquivo CSS separado.

## 19.1 Quando Usar CSS Interno

- O CSS interno é útil quando você precisa estilizar uma única página HTML e não planeja reutilizar esses estilos em outras páginas. Ele pode ser uma solução rápida para projetos pequenos ou páginas isoladas, mas, assim como o CSS inline, deve ser usado com cautela em projetos maiores.

### Vantagens:

- Fácil de usar em projetos pequenos ou em protótipos.
- Os estilos são aplicados a todos os elementos da página sem necessidade de arquivos CSS externos.
- Não requer links externos, então é ótimo para páginas autossuficientes.

### Desvantagens:

- Não é reutilizável em outras páginas, o que pode aumentar o tamanho e a complexidade do código.
- Difícil de manter em sites maiores com múltiplas páginas.
- Menos eficiente em termos de performance em comparação ao CSS externo.

## 19.2 Exemplo de Uso de CSS Interno

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

# 20. Estilos CSS Externos

- O CSS externo é uma forma de separar completamente o estilo do conteúdo HTML, usando um arquivo `.css` separado. Esse método é o mais recomendado para projetos maiores, pois facilita a reutilização de estilos e a manutenção do código.

## 20.1 Quando Usar CSS Externo

- O CSS externo é a melhor prática quando você está trabalhando em projetos com múltiplas páginas, onde o estilo precisa ser consistente. Ele permite aplicar estilos a várias páginas ao mesmo tempo, sem duplicar código, mantendo a organização e facilitando atualizações.

### Vantagens:

- **Reutilizável**: Um arquivo CSS pode ser aplicado a várias páginas ao mesmo tempo.
- **Organização**: O HTML fica mais limpo, pois o código de estilo fica em um arquivo separado.
- **Manutenção**: Facilidade em manter e atualizar o design, pois todas as páginas compartilham o mesmo arquivo de estilo.

### Desvantagens:

- Requer uma solicitação extra ao servidor para carregar o arquivo CSS, o que pode aumentar ligeiramente o tempo de carregamento da página.
- Precisa de um bom controle de versionamento para garantir que mudanças de estilo não afetem inadvertidamente outras páginas.

## 20.2 Exemplo de Uso de CSS Externo

### Arquivo HTML:

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

### Estrutura de Pastas para CSS Externo

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
# 21. Psicologia das Cores

- A **psicologia das cores** estuda como diferentes cores podem influenciar nossas emoções, comportamentos e decisões. No design, as cores desempenham um papel fundamental na experiência do usuário, afetando desde a estética até a funcionalidade.

## 21.1 Significados das Cores

- Cada cor carrega um significado psicológico que pode influenciar como as pessoas percebem um site ou um produto. Aqui estão algumas cores e seus significados comuns:

### Vermelho
- **Emoções**: Paixão, energia, urgência.
- **Uso no Design**: Chama a atenção e estimula ação. Usado em botões de chamada para ação (CTAs) ou para destacar elementos importantes.

### Azul
- **Emoções**: Confiança, serenidade, segurança.
- **Uso no Design**: Transmite tranquilidade e profissionalismo. Muito utilizado em sites corporativos e redes sociais.

### Amarelo
- **Emoções**: Alegria, otimismo, calor.
- **Uso no Design**: Atrai atenção, mas deve ser usado com moderação para não causar fadiga visual. Geralmente associado à positividade e criatividade.

### Verde
- **Emoções**: Harmonia, equilíbrio, natureza.
- **Uso no Design**: Associado à saúde, sustentabilidade e crescimento. Amplamente utilizado em projetos relacionados ao meio ambiente e bem-estar.

### Laranja
- **Emoções**: Energia, entusiasmo, calor.
- **Uso no Design**: Estimula interações e transmite acessibilidade. É uma cor usada para envolver o usuário, especialmente em marketing.

### Roxo
- **Emoções**: Criatividade, luxo, mistério.
- **Uso no Design**: Comumente associado a produtos premium e a marcas criativas.

### Preto
- **Emoções**: Sofisticação, elegância, formalidade.
- **Uso no Design**: Sinal de exclusividade e poder. Utilizado em design minimalista e em marcas de luxo.

### Branco
- **Emoções**: Pureza, simplicidade, clareza.
- **Uso no Design**: Aumenta a sensação de espaço e limpeza. Muito usado em designs minimalistas e para criar contraste com outras cores.

---

# 22. Representação de Cores

- No desenvolvimento web, as cores podem ser representadas de diferentes formas no CSS. Abaixo estão as principais maneiras de representar cores, com exemplos práticos.

## 22.1. Cores por Nome

- No CSS, você pode usar o **nome** da cor para definir o estilo. Existem 140 cores nomeadas disponíveis.

### Exemplo de Uso:

```html

<h2 style="background-color: blue; color: white;">Exemplo de uso de cores</h2>
<p>Lorem ipsum dolor sit, amet consectetur adipisicing elit...</p>

```

## 22.2. Cores por Código Hexadecimal

- O **código hexadecimal** define cores usando o formato #RRGGBB, onde RR, GG, e BB são valores de vermelho, verde e azul, respectivamente, representados por dois dígitos hexadecimais.

### Exemplo de Uso:

```html

<h2 style="background-color: #0000ff; color: white;">Exemplo de uso de cores</h2>
<p>Lorem ipsum dolor sit, amet consectetur adipisicing elit...</p>

```
## 22.3. Cores por RGB

- O modelo **RGB** (Red, Green, Blue) define uma cor misturando valores de vermelho, verde e azul. Cada componente varia de 0 a 255.

### Exemplo de Uso:

```html

<h2 style="background-color: rgb(0, 0, 255); color: white;">Exemplo de uso de cores</h2>
<p>Lorem ipsum dolor sit, amet consectetur adipisicing elit...</p>

```
## 22.4. Cores por HSL

- O modelo **HSL (Hue, Saturation, Lightness)** define uma cor em termos de:

- **Hue** (Matiz): O valor no espectro de cores (0 a 360 graus).
- **Saturation** (Saturação): A intensidade da cor (0% a 100%).
- **Lightness** (Luminosidade): O brilho da cor (0% é preto, 100% é branco).

### Exemplo de Uso:

```html

<h2 style="background-color: hsl(240, 100%, 50%); color: white;">Exemplo de uso de cores</h2>
<p>Lorem ipsum dolor sit, amet consectetur adipisicing elit...</p>

```

## 22.5 Transparência nas Cores

- A **transparência** permite que você controle o nível de opacidade de uma cor, o que é útil para criar efeitos visuais interessantes e sobreposições.

## 22.5.1. Opacidade

- A **opacidade** é a medida de quão transparente uma cor é. Um valor de opacidade de 1 significa que a cor é totalmente opaca, enquanto um valor de 0 significa que a cor é completamente transparente.

### Exemplo de Uso com RGBA

- O formato `rgba()` é usado para definir cores com opacidade. Os valores `R`, `G`, `B` variam de 0 a 255, enquanto `A` (Alpha) varia de 0 a 1.

#### Exemplo:

```html

<h2 style="background-color: rgba(0, 0, 255, 0.5); color: white;">Exemplo de cor com transparência</h2>
<p>Lorem ipsum dolor sit, amet consectetur adipisicing elit...</p>

```

## 22.6. Quando Usar Cada Modelo

- **Nomes de cor:** Útil para situações rápidas, mas limitado em opções.
- **Hexadecimal:** Popular entre desenvolvedores e amplamente suportado.
- **RGB:** Melhor para ajustes finos em intensidades de cor.
- **HSL:** Mais intuitivo para ajustes de tonalidade, saturação e brilho.

---

# 23. Harmonia de Cores

- A harmonia das cores é um princípio essencial no design que se refere ao uso de cores que combinam bem entre si. A compreensão do círculo cromático e das relações entre cores pode ajudar a criar composições visuais agradáveis e equilibradas.

## 23.1. Círculo Cromático

- O círculo cromático é uma representação visual das cores, que organiza as cores em um formato circular. Ele é dividido em três categorias principais: cores primárias, secundárias e terciárias.

### Cores Primárias

- As cores primárias são aquelas que não podem ser criadas pela mistura de outras cores. No modelo de cores aditivas (RGB), as cores primárias são:

  - **Vermelho**
  - **Verde**
  - **Azul**

- No modelo de cores subtrativas (CMY), as cores primárias são:

  - **Ciano**
  - **Magenta**
  - **Amarelo**

### Cores Secundárias

- As cores secundárias são formadas pela mistura de duas cores primárias em partes iguais. No círculo cromático, as cores secundárias são:

  - **Laranja** (vermelho + amarelo)
  - **Verde** (azul + amarelo)
  - **Roxo** (vermelho + azul)

### Cores Terciárias

- As cores terciárias são criadas pela mistura de uma cor primária com uma cor secundária adjacente. Exemplos de cores terciárias incluem:

  - **Vermelho-alaranjado**
  - **Amarelo-alaranjado**
  - **Amarelo-esverdeado**
  - **Azul-esverdeado**
  - **Azul-arroxeado**
  - **Vermelho-arroxeado**

## 23.2. Temperaturas de Cores

- As cores também podem ser classificadas em **temperaturas**: cores quentes e cores frias.

### 23.2.1. Cores Quentes
  
- Associadas a sensações de energia, calor e emoção.

  - **vermelho**
  - **laranja**
  - **amarelo**

### 23.2.2. Cores Frias

- Evocam sensações de calma, tranquilidade e serenidade

  - **azul**
  - **verde** 
  - **roxo** 
  

## 23.3. Combinações Harmoniosas

- Ao criar paletas de cores, algumas combinações são mais harmoniosas do que outras. Aqui estão algumas maneiras comuns de combinar cores:

  - **Complementares:** Cores opostas no círculo cromático. Exemplo: azul e laranja.
  - **Análogas:** Cores que estão lado a lado no círculo. Exemplo: azul, azul-esverdeado e verde.
  - **Tríades:** Três cores equidistantes no círculo cromático. Exemplo: vermelho, amarelo e azul.

---

# 24. Degradê com CSS

- Os **degradês (ou gradientes)** são uma técnica visual utilizada no design web para criar transições suaves entre duas ou mais cores. 

## 24.1. Degradê Linear

- Um **degradê linear** é uma transição de cor que se estende em uma direção reta. Para criar um degradê linear no CSS, você utiliza a propriedade `background-image` com a função `linear-gradient()`.

### 24.1.2. Direção do Degradê Linear

- A **direção do degradê** pode ser ajustada usando palavras-chave, como to right, to left, to top, ou to bottom, ou usando ângulos. Aqui estão alguns exemplos:

  - **Degradê Horizontal**: linear-gradient(to right, #f00, #0f0) (do vermelho para o verde).
  - **Degradê Diagonal**: linear-gradient(45deg, #00f, #ff0) (do azul para o amarelo em um ângulo de 45 graus).

### Exemplo de Uso:

```css

body {
    background-image: linear-gradient(to bottom, #3198E2, #6D59C0, #B93590, #E33F5F, #FDD579);
    background-attachment: fixed;
}

```
## 24.2. Degradê Radial

- Um **degradê radial** cria uma transição circular de cores a partir de um ponto central. Para criar um degradê radial no CSS, você utiliza a função `radial-gradient()`.

### 24.2.1. Formatos do Degradê Radial

- **Círculo** radial-gradient(circle, #ff0000, #0000ff) - Um degradê circular, onde a cor transita uniformemente em todas as direções a partir do centro.

- **Elipse**: radial-gradient(ellipse, #ff0000, #0000ff) - Um degradê em formato elíptico, onde a transição de cores ocorre em uma forma oval.

### Exemplo de Uso:

```css
body {
    background-image: radial-gradient(circle, red, blue);
}
```
---

# 25. Tipografia

- A **tipografia** refere-se ao estilo, arranjo e aparência do texto em um design ou documento. Ela desempenha um papel crucial na comunicação visual, influenciando não apenas a estética, mas também a legibilidade e a hierarquia de informação. 

## 25.1 Fontes

- As **fontes** são definidas em CSS utilizando a propriedade `font-family`.
  
### 25.1.1. Definindo a Fonte

- A propriedade `font-family` aceita uma lista de fontes, sendo a primeira a preferencial.
- Caso a primeira não esteja disponível, as próximas serão usadas. 
- O uso de uma família genérica é recomendado como último recurso. (`serif`, `sans-serif` ou `monospace`) 

```css

<p style="font-family: 'Arial', sans-serif;">
  Texto com a fonte Arial.
</p>

```

## 25.2 Tamanho da Fonte

- É controlado pela propriedade `font-size` . 

### 25.2.1 Tipos de Medidas

- As medidas podem ser Absolutas ou Relativas

#### 25.2.1.1 Medidas Absolutas

- **Pixels (px)**: Tamanho fixo e absoluto, que não muda com a configuração do usuário. Exemplo: 20px.

#### 25.2.1.2 Medidas Relativas

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

## 25.3 Peso da Fonte

- É controlado pela propriedade `font-weight`.

### 25.3.1 Pesos Comuns

- **Normal**: Valor padrão, equivalente a 400.
- **`Bold`**: Texto em negrito, equivalente a 700.
- **Valores numéricos**: Variação entre 100 (mais fino) e 900 (mais espesso).


## 25.4 Estilo da Fonte

- É definido pela propriedade `font-style`. 

### 25.4.1. Valores para Font Style

- **`Normal`**: Texto sem estilo adicional.
- **`Italic`**: Texto em itálico.
- **`Oblique`**: Similar ao itálico, mas com uma inclinação diferente.


## 25.5. Alinhamento do Texto

- Todo o texto é ajustado com a propriedade `text-align`. 
- O início do paragafo por ser ajustado com a propriedade `text-indent`.
  
### 25.5.1. Opções de Alinhamento com Text-Align

- **`Left`**: Alinhamento à esquerda (padrão).
- **`Right`**: Alinhamento à direita.
- **`Center`**: Texto centralizado.
- **`Justify`**: Texto justificado, preenchendo o espaço da linha.

### 25.5.2. Alinhamento com Text-Indent

- **Valor em pixels (px) ou em (em)**: Define o tamanho do recuo.
- **Valores negativos**: Criam um recuo para a esquerda (pouco usado).

## 25.6. Altura da Linha

- A propriedade `line-height` controla a altura da linha.

### 25.6.1. Definindo a Altura da Linha

- **Normal**: Valor padrão, dependendo do navegador e da fonte.
- **Numérico**: Valor maior que 1 aumenta o espaçamento.


## 25.7. Espaçamento entre Letras e Palavras

- A propriedade `letter-spacing` ajusta o espaçamento entre as letras
- A propriedade `word-spacing` controla o espaçamento entre as palavras. 

### 25.7.1. Ajustando Espaçamentos

- **`Letter-spacing`** Aumenta ou diminui o espaçamento entre as letras.
- **`Word-spacing`** Aumenta ou diminui o espaçamento entre as palavras.


## 25.8 Decoração do Texto

- A propriedade `text-decoration` adiciona efeitos visuais ao texto.

### 25.8.1 Tipos de Decoração

- **`Underline`**: Adiciona uma linha abaixo do texto.
- **`Line-through`**: Adiciona uma linha através do texto (riscado).

## 25.9. Transformação do Texto

- A transformação do texto pode ser feita usando a propriedade `text-transform`.

### 25.9.1. Modos de Transformação

- **`Uppercase`**: Transforma todas as letras em maiúsculas.
- **`Lowercase`**: Transforma todas as letras em minúsculas.
- **`Capitalize`**: Capitaliza a primeira letra de cada palavra.

## 25.10. Cor da Fonte

- A propriedade `color` é usada para definir a cor do texto. 

### 25.10.1. Formatos de Cor

- **Hexadecimal**: Especifica cores usando código hexadecimal, por exemplo, #FF5733 para laranja.
- **RGB**: Define as cores usando valores de Red, Green, Blue (RGB).
- **Nomes de cores**: Usa nomes de cores pré-definidos, como red, blue, green.


## 25.11 Fontes Externas

### 23.11.1 Google Fonts

- Uma biblioteca de fontes que permite incorporar uma grande variedade de fontes personalizadas. 

- As fontes podem ser incluídas diretamente através de:
  - links
  - importadas via CSS.

#### 23.11.1.1 Como utilizar o Google Fonts

- Acesse o site [Google Fonts](https://fonts.google.com/).
- Escolha a fonte desejada e clique em "Select this style".
- Copie o link gerado e adicione-o no `<head>` do seu HTML.
- Defina a fonte no seu CSS utilizando a propriedade `font-family`.

### 23.11.2 DaFont

- Uma plataforma popular para baixar fontes personalizadas.

  - Baixadas e instaladas localmente.
  - Incorporadas ao projeto utilizando a regra `@font-face` no CSS.

#### 23.11.2.1 Utilizando fontes do DaFont

- Acesse o site [DaFont](https://www.dafont.com/).
- Baixe o arquivo de fonte desejado (normalmente em formatos como `.otf` ou `.ttf`).
- Inclua a fonte em seu projeto utilizando a regra `@font-face`.

### 23.11.3 Tipos de Formatos de Fonte

- Ao utilizar fontes externas, é importante conhecer os diferentes formatos de fonte para garantir compatibilidade entre navegadores.

#### 23.11.3.1 Tipos de Formatos

- **OpenType (.otf)**: Formato moderno com suporte avançado para gráficos e tipografia.
- **TrueType (.ttf)**: Formato padrão utilizado tanto em Windows quanto em macOS.
- **Embedded OpenType (.eot)**: Usado principalmente para compatibilidade com versões antigas do Internet Explorer.
- **TrueType AAT (Apple Advanced Typography)**: Formato da Apple com suporte a recursos tipográficos avançados.
- **SVG**: Fonte vetorial que pode ser escalada sem perder qualidade.

---

# 26. Seletores Personalidos

- Permitem estilizar elementos específicos de maneira flexível e eficiente usando CSS. 
- Esses seletores incluem:
  - IDs 
  - Classes 
  - Pseudo-classes
  - Pseudo-elementos

## 26.1. Seletor de ID

- O seletor de ID seleciona um elemento com base no atributo id do HTML. 
- IDs são únicos, o que significa que cada ID deve ser atribuído a apenas um elemento em um documento HTML.

### 26.1.1. Como Utilizar ID
- Defina o `id` no elemento HTML.
- Use o símbolo `#` seguido do nome do ID no CSS para aplicar o estilo.

## 26.2. Seletor de Classe

- Permite aplicar o mesmo estilo a múltiplos elementos.

### 26.2.1. Como Utilizar Classe

- Defina o atributo class nos elementos HTML.
- Use o nome da classe precedido de `.` no CSS.

## 26.3. Pseudo-classes

- As pseudo-classes são usadas para definir um estado especial de um elemento.
- Quando o usuário interage com ele (por exemplo, passar o mouse ou clicar).

### 26.3.1. Principais Pseudo-classes

- **`:hover`**: Aplica o estilo quando o usuário passa o mouse sobre o elemento.
- **`:focus`**: Aplica o estilo quando o elemento está focado, geralmente em campos de formulário.
- **`:nth-child(n)`**: Seleciona o enésimo filho de um elemento pai.

#### Exemplo de Uso:

```css

a:hover { /* Ao passar o mouse o link fica verde */
  color: green;
}

li:nth-child(2) { /* Aplica a cor laranja ao segundo item de uma lista.*/
  color: orange;
}

```

## 26.4. Pseudo-elementos

- Os pseudo-elementos permitem estilizar partes específicas de um elemento, como a primeira letra ou linha de um parágrafo.

### 26.4.1. Principais Pseudo-elementos

- **`::before`**: Insere conteúdo antes do conteúdo real de um elemento.
- **`::after`**: Insere conteúdo após o conteúdo real de um elemento.
- **`::first-letter`**: Aplica o estilo à primeira letra do texto dentro de um elemento.
- **`::first-line`**: Aplica o estilo à primeira linha do texto dentro de um elemento.

#### Exemplo de Uso:

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

## 26.5. Diferenças entre Pseudo-classe e Pseudo-elemento

- Pseudo-classes (ex: `:hover`, `:focus`) se aplicam a estados ou condições especiais dos elementos.
- Pseudo-elementos (ex: `::before, `::after`) permitem acessar e estilizar partes específicas do conteúdo de um elemento.
  
## 26.6. Seletores Combinados

- Você pode combinar seletor de classe, `id`, pseudo-classe e pseudo-elemento para aplicar estilos mais precisos.

### Exemplo de Uso:

```css

#paragrafo-unico:hover::first-letter {
  color: blue;
  font-size: 150%; /*altera o estilo da primeira letra do parágrafo com o ID "paragrafo-unico" quando o mouse passa sobre ele. */
}

```

# 27. Modelos de caixas

- Em HTML, os elementos são renderizados como caixas, seguindo dois principais modelos de layout: 
  - Modelo de caixa em **nível de bloco** (box-level).
  - Modelo de caixa em **nível de linha** (inline-level). 
- Esses modelos controlam como o navegador renderiza os elementos na página e como eles se comportam no fluxo do layout.
  
## 27.1. Modelo de Caixa Box-Level (Bloco)

- O modelo de caixa de nível de bloco é aplicado a elementos que ocupam toda a largura disponível da página, iniciando em uma nova linha.
- Esses elementos empurram o conteúdo subsequente para a próxima linha.
  
### 27.1.1. Exemplos de Elementos Box-Level

- **`<div>`**
- **`<h1>`,`<h2>`,`<h3>`...**
- **`<p>`**
- **`<section>`**
  
### 27.1.2. Propriedades de Layout Box-Level

- Elementos de bloco podem ter altura, largura, margem e preenchimento definidos de forma clara.
- Eles sempre ocupam a largura total de seu contêiner pai, a menos que um valor de largura seja especificado.
  
### 27.1.3. Comportamento do Modelo Box-Level

- Quando dois elementos de bloco são colocados consecutivamente, o segundo elemento será posicionado abaixo do primeiro, respeitando as margens e o espaço entre eles.

## 27.2. Modelo de Caixa Inline-Level (Linha)

- Elementos inline são renderizados na mesma linha em que estão posicionados, ocupando apenas o espaço necessário para o seu conteúdo.
- Eles não iniciam uma nova linha, o que permite que outros elementos estejam ao lado deles.

### 27.2.1. Exemplos de Elementos Inline-Level

- **`<span>`**
- **`<a>`**
- **`<em>`, `<strong>`**
- **`<img>`**

### 27.2.2. Propriedades de Layout Inline-Level

- Elementos inline respeitam a largura do conteúdo e não permitem definir diretamente propriedades como width e height.
- No entanto, é possível definir margens, preenchimentos e outros estilos que influenciam a aparência desses elementos.

### 27.2.3. Comportamento do Modelo Inline-Level

- Elementos inline aparecem em sequência no mesmo fluxo de texto e permitem que outros elementos estejam adjacentes.
- Eles não quebram a linha do conteúdo, a menos que o contêiner atinja seu limite de largura.

## 27.3. Diferenças entre Box-Level e Inline-Level

- **Box-Level**: Elementos ocupam toda a largura disponível, iniciando uma nova linha.
- **Inline-Level**: Elementos ocupam apenas o espaço necessário, permanecendo no fluxo de linha.

## 27.4. Box Model

- O **Box Model** em CSS define como a caixa de um elemento é composta e como suas propriedades afetam o layout.
  
- Cada elemento tem uma caixa que contém quatro áreas:
  
  - **Conteúdo**: O conteúdo real do elemento.
  - **Preenchimento (Padding)**: Espaço entre o conteúdo e a borda.
  - **Borda (Border)**: A borda ao redor do conteúdo e preenchimento.
  - **Margem (Margin)**: Espaço externo ao redor da borda.

# 28. Agrupamento de Tags (Grouping Tags)

- Usadas para organizar e estruturar o conteúdo da página.
- Permite agrupar elementos relacionados em blocos semânticos.
- Ajudam a criar uma hierarquia clara e facilitam o estilo e a manipulação de conteúdo.

## 28.1. Principais Tags de Agrupamento

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


### 28.1.1. `<div>` (Division)

- A tag `<div>` é um elemento de bloco genérico utilizado para agrupar outros elementos HTML.
- Não possui um significado semântico próprio, sendo amplamente usado para aplicar estilos ou organizar o layout com CSS e JavaScript.
  
### 28.1.2. `<span>`

- A tag `<span>` é um elemento inline genérico usado para agrupar partes do conteúdo sem alterar o fluxo de texto.
- É frequentemente utilizado para aplicar estilos a partes específicas do texto.

### 28.1.3. `<section>`

- A tag `<section>` define uma seção temática dentro do conteúdo de uma página, sendo usada para agrupar elementos relacionados que compartilham um contexto comum.
- Diferente do `<div>`, o `<section>` possui significado semântico e é recomendado quando o conteúdo possui uma função específica.

### 28.1.4. `<article>`

- A tag `<article>` é usada para representar uma unidade de conteúdo independente, como uma notícia, post de blog ou artigo.
- O conteúdo dentro de um `<article>` é normalmente autocontido e pode ser distribuído de forma independente.

### 28.1.5. `<nav>`

- A tag `<nav>` é usada para agrupar links de navegação.
- É uma forma semântica de indicar que os links dentro desse elemento representam a navegação principal ou secundária de um site.

### 28.1.6. `<aside>`

- A tag `<aside>` representa conteúdo tangencial ao conteúdo principal, como uma barra lateral, uma citação ou informações complementares.

### 28.1.7. `<header>`

- A `<header>` é usada para definir o cabeçalho de uma página ou de uma seção importante. 
- Geralmente contém títulos, logotipos, ou menus de navegação.

### 28.1.8. `<main>`

- A `<main>` define o conteúdo principal de um documento. 
- Apenas deve haver um elemento `<main>` por página, e ele deve conter o conteúdo central, excluindo navegação ou barras laterais.

### 28.1.9. `<footer>`

- A `<footer>` representa o rodapé de uma página ou seção. Geralmente contém informações como direitos autorais, links adicionais ou informações de contato.

### 28.1.10. `<figure>`

- A `<figure>` é usada para agrupar conteúdo de mídia, como imagens, gráficos ou diagramas, junto com legendas relacionadas, representadas pela tag `<figcaption>`.

### 28.1.11. `<figcaption>`

- A `<figcaption>` define uma legenda ou descrição associada ao conteúdo dentro de um `<figure>`.
- É usada para explicar ou fornecer contexto adicional para uma imagem ou gráfico.

#### Exemplo de Uso:
```html
<figure>
  <img src="gráfico.png" alt="Gráfico de vendas">
  <figcaption>Gráfico de vendas do último trimestre.</figcaption>
</figure>
```

## 28.2. Importância Semântica

- O uso correto das tags de agrupamento semânticas, melhora a acessibilidade e a indexação do conteúdo pelos motores de busca (SEO).
- `<div>` e `<span>` continuam sendo úteis para agrupamentos que não exigem uma semântica específica.

# 29. Sombra e Bordas Arredondadas

- As propriedades `box-shadow` e `border-radius` são amplamente utilizadas em conjunto no CSS para criar elementos visualmente atraentes. 
- Juntas, elas oferecem a possibilidade de adicionar profundidade, suavidade e destaque a caixas, botões, cartões e outros elementos.

## 29.1. Sombra (Box Shadow)

- A propriedade `box-shadow` aplica sombras a elementos, criando um efeito tridimensional.
- É possível ajustar o tamanho, desfoque e cor da sombra, além de definir se ela será externa ou interna ao elemento.

### 29.1.1. Sintaxe

```css
box-shadow: offset-x offset-y blur-radius spread-radius color inset;
``` 
- offset-x: Deslocamento horizontal da sombra.
- offset-y: Deslocamento vertical da sombra.
- blur-radius: Grau de desfoque.
- spread-radius: Tamanho da sombra.
- color: Cor da sombra.
- inset: Aplica a sombra para dentro do elemento (opcional).

### 29.1.2. Exemplo de Uso

```css
.elemento {
  box-shadow: 5px 10px 15px rgba(0, 0, 0, 0.3);
}
```

## 29.2. Bordas Arredondadas (Border Radius)

- A propriedade `border-radius` permite criar bordas arredondadas em elementos.

### 29.2.1. Sintaxe

```css
border-radius: valor;
```

### 29.2.2. Exemplo de Uso

```css
.caixa {
  border-radius: 15px;
}
```

## 29.3. Combinação de box-shadow e border-radius

- O uso combinado de sombras e bordas arredondadas cria efeitos visuais elegantes, como cartões de destaque ou botões interativos.

### 29.3.1. Exemplo de Combinação

```css
.cartao {
  box-shadow: 4px 8px 12px rgba(0, 0, 0, 0.2);
  border-radius: 10px;
  padding: 20px;
  background-color: #fff;
}
```

# 30. Variáveis em CSS

- As variáveis CSS permitem armazenar valores que podem ser reutilizados em várias partes de um documento CSS.
- Facilitam a manutenção do código.
- Permitindo alterar valores em um único lugar sem a necessidade de modificações repetitivas em todo o arquivo.

## 30.1. Definição de Variáveis

- As variáveis são definidas utilizando a sintaxe --nome-da-variável, e acessadas através da função var().

### 30.1.1. Sintaxe Básica
  
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

## 30.2. Benefícios

- Facilita a manutenção de grandes arquivos CSS.
- Torna o código mais legível e reutilizável.

## 30.3. Exemplo Completo

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
