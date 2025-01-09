- [1. Imagens de Fundo em HTML E CSS](#1-imagens-de-fundo-em-html-e-css)
  - [1.1. Propriedade `background-image`](#11-propriedade-background-image)
  - [1.2. Propriedade `background-color`](#12-propriedade-background-color)
  - [1.3. Combinação de Imagens e Gradientes](#13-combinação-de-imagens-e-gradientes)
  - [1.4. Repetição de Fundo:` background-repeat`](#14-repetição-de-fundo-background-repeat)
  - [1.5. Tamanho do Fundo: `background-size`](#15-tamanho-do-fundo-background-size)
  - [1.6. Posição do Fundo: `background-position`](#16-posição-do-fundo-background-position)
  - [1.7. Fixação do Fundo:` background-attachment`](#17-fixação-do-fundo-background-attachment)
- [2. Centralização Vertical de Caíxas](#2-centralização-vertical-de-caíxas)
  - [2.1. Propriedade `position: relative`](#21-propriedade-position-relative)
  - [2.2. Propriedade `position: absolute`](#22-propriedade-position-absolute)
  - [2.3. Centralização com `transform`](#23-centralização-com-transform)
- [3. Introdução às Tabelas em HTML e CSS](#3-introdução-às-tabelas-em-html-e-css)
  - [3.1. Hierarquia de Tabelas Simples](#31-hierarquia-de-tabelas-simples)
  - [3.2. Anatomia de Tabelas Grandes](#32-anatomia-de-tabelas-grandes)
  - [3.3. Mesclagem de Células](#33-mesclagem-de-células)
  - [3.4. Estilização com CSS](#34-estilização-com-css)
  - [3.5. Usando colgroup e col](#35-usando-colgroup-e-col)
  - [3.6. Tabelas Responsivas](#36-tabelas-responsivas)


# 1. Imagens de Fundo em HTML E CSS

## 1.1. Propriedade `background-image` 
- Define uma imagem como fundo de um elemento.

- Exemplo de Uso:
  
    ```css
    body {
        background-image: url("../exercicios/ex022/imagens/wallpaper001.jpg");
    }
    ```

## 1.2. Propriedade `background-color`
- Define a cor de fundo para um elemento.
- Pode ser usada sozinha ou junto de uma imagem de fundo.

- Exemplo de Uso:

    ```css
    div {
            width: 300px;
            height: 300px;
            background-color: lightgrey;
            border: 1px solid black;
            border-radius: 10px;
        }
    ```
## 1.3. Combinação de Imagens e Gradientes
- Gradientes podem ser usados como imagens de fundo.
  
- Exemplo de Uso:

  ```css
    background-image: linear-gradient(to bottom, yellow, red);
  ```

## 1.4. Repetição de Fundo:` background-repeat`
- Define como a imagem de fundo será repetida.
- Valores comuns:
  - **no-repeat**: Não repete a imagem.
  - **repeat**: Repete a imagem em ambas as direções.
  - **repeat-x**: Repete a imagem apenas horizontalmente.
  - **repeat-y**: Repete a imagem apenas verticalmente.
  
  - Exemplo de Uso:

      ```css
      body {
        background-image: url("https://gustavoguanabara.github.io/html-css/imagens/mascote.png");
        background-repeat: no-repeat;
      }
      ```

## 1.5. Tamanho do Fundo: `background-size`
- Controla o tamanho da imagem de fundo.
- Valores comuns:
    - **cover**: Ajusta a imagem para cobrir todo o elemento.
    - **contain**: Ajusta a imagem para caber dentro do elemento.
    - Valores específicos, como ` 100px 100px`.
  
    - Exemplo de Uso:

        ```css
      body {
        background-size: 100px 100px;
      }              
        ```

## 1.6. Posição do Fundo: `background-position`
- Define a posição da imagem de fundo.
- Valores comuns:
  - Palavras-chave: `left top`,`` center center``, ``right bottom.``
- Coordenadas específicas: `50% 50%` ou `10px 20px`.
- Exemplo de Uso:

    ```css
    div {
        width: 300px;
        height: 300px;
        background-image: url("../exercicios/ex022/imagens/wallpaper002.jpg");
        background-position: center center;
    }
    ```

## 1.7. Fixação do Fundo:` background-attachment`
- Define se a imagem de fundo será fixa ou se deslocará com a rolagem.
- Valores Comuns:
    - **scroll**: O fundo se move com a página.
    - **fixed**: O fundo permanece fixo no viewport.
    - **local**: O fundo se move com o conteúdo do elemento.

- Exemplo de Uso:

    ```css
    body {
        background-image: url("../exercicios/ex022/imagens/wallpaper001.jpg");
        background-attachment: fixed;
    }
    ```
# 2. Centralização Vertical de Caíxas

## 2.1. Propriedade `position: relative`
- Define um contexto de posicionamento para os elementos filhos.

- O elemento com `position: relative` não se move, a menos que seja combinado com propriedades como `top`, `left`, `right` ou `bottom`.

- Exemplo de Uso:

  ```css
  #container {
      position: relative; /* Cria um contexto para elementos filhos */
      height: 500px;
      background-color: lightblue;
  }
  ``` 

## 2.2. Propriedade `position: absolute`
- Permite posicionar um elemento em relação ao seu elemento pai mais próximo que tenha `position: relative`, `absolute` ou `fixed`.

- É útil para mover elementos para posições específicas.

- Exemplo de Uso:

  ```css
  #conteudo {
      position: absolute; /* Faz referência ao elemento pai */
      top: 50px; /* Move o elemento 50px para baixo */
      left: 100px; /* Move o elemento 100px para a direita */
  }
  ```

## 2.3. Centralização com `transform`
- Combina-se `top: 50%` e `left: 50%` para mover o elemento para o centro do container.

- O elemento é então ajustado com` transform: translate(-50%, -50%)`, deslocando seu ponto de referência para o centro.

- Exemplo de Uso:
  
  ```css
  #conteudo {
      position: absolute;
      top: 50%; /* Centraliza verticalmente */
      left: 50%; /* Centraliza horizontalmente */
      transform: translate(-50%, -50%); /* Ajusta o ponto de referência para o centro */
      width: 200px;
      height: 100px;
      background-color: yellow;
  }
  ```
# 3. Introdução às Tabelas em HTML e CSS
- As tabelas em HTML são usadas para organizar dados em linhas e colunas. 
- Poderosa ferramenta para exibir informações estruturadas
- Podem ser personalizadas com CSS para se adequarem ao design de qualquer site.

## 3.1. Hierarquia de Tabelas Simples
- Uma tabela básica é estruturada com as seguintes tags principais:

- **`<table>: `** Define a tabela.
- **`<tr>: `** Representa uma linha da tabela.
- **`<th>: `** Define um cabeçalho de coluna (table header).
- **`<td>: `** Define uma célula de dado (table data).
- Exemplo de Uso:
  
  ```html
    <table border="1">
      <tr>
        <th>Nome</th>
        <th>Idade</th>
        <th>Cidade</th>
      </tr>
      <tr>
        <td>João</td>
        <td>25</td>
        <td>São Paulo</td>
      </tr>
      <tr>
        <td>Maria</td>
        <td>30</td>
        <td>Rio de Janeiro</td>
      </tr>
    </table>
  ```
## 3.2. Anatomia de Tabelas Grandes
- Para tabelas maiores e mais complexas, o HTML fornece as tags:
  - **`caption`**: Adiciona um título à tabela.
  - **`thead`**: Agrupa cabeçalhos de coluna.
  - **`tbody`**: Agrupa o corpo da tabela.
  - **`tfoot`**: Agrupa rodapés da tabela.
  
- Ajudam na organização semântica e estrutural.

- Exemplo de Uso:
  
  ```html
    <table border="1">
      <caption>Lista de Produtos</caption>
      <thead>
        <tr>
          <th>Produto</th>
          <th>Quantidade</th>
          <th>Preço</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Notebook</td>
          <td>10</td>
          <td>R$ 3.500,00</td>
        </tr>
        <tr>
          <td>Mouse</td>
          <td>50</td>
          <td>R$ 50,00</td>
        </tr>
      </tbody>
      <tfoot>
        <tr>
          <td colspan="2">Total</td>
          <td>R$ 3.550,00</td>
        </tr>
      </tfoot>
    </table>
  ```

## 3.3. Mesclagem de Células
- As propriedades rowspan e colspan permitem mesclar células em uma tabela.

- **`colspan`**: Mescla células horizontalmente.
- **`rowspan`**: Mescla células verticalmente.

- Exemplo de Uso:
  
  ```html
  <table border="1">
    <tr>
      <th>Item</th>
      <th>Descrição</th>
      <th>Preço</th>
    </tr>
    <tr>
      <td rowspan="2">Cadeira</td>
      <td>Ergonômica</td>
      <td>R$ 250,00</td>
    </tr>
    <tr>
      <td>De Escritório</td>
      <td>R$ 300,00</td>
    </tr>
  </table>
  ```

## 3.4. Estilização com CSS
- As tabelas podem ser estilizadas com CSS para melhorar sua aparência.
  
- Exemplo de Uso:
```html
  <style>
    table {
      width: 100%;
      border-collapse: collapse;
    }
    th, td {
      border: 1px solid #ddd;
      padding: 8px;
      text-align: left;
    }
    th {
      background-color: #f4f4f4;
    }
  </style>

  <table>
    <tr>
      <th>Nome</th>
      <th>Idade</th>
      <th>Cidade</th>
    </tr>
    <tr>
      <td>Lucas</td>
      <td>22</td>
      <td>Fortaleza</td>
    </tr>
  </table>
```


## 3.5. Usando colgroup e col

- A tag `<colgroup>` define grupos de colunas. 
- A tag `<col>` aplica estilos específicos a essas colunas.

- Exemplo de Uso:
  ```html
  <style>
    colgroup col:nth-child(1) {
      background-color: #e6f7ff;
    }
    colgroup col:nth-child(2) {
      background-color: #fff5e6;
    }
  </style>

  <table border="1">
    <colgroup>
      <col>
      <col>
    </colgroup>
    <tr>
      <th>Categoria</th>
      <th>Descrição</th>
    </tr>
    <tr>
      <td>Frutas</td>
      <td>Banana, Maçã</td>
    </tr>
  </table>
  ```

## 3.6. Tabelas Responsivas
- Tabelas podem ser adaptadas para telas menores usando CSS.

- **`overflow-x: auto;`**:

  - Faz com que, se o conteúdo da tabela for mais largo que a largura do contêiner pai, uma barra de rolagem horizontal seja exibida automaticamente.

  - Isso preserva a estrutura da tabela, evitando quebra ou ocultação de colunas.
  
- Por que usar uma **`<div>`**?

  - Envolver a tabela em uma `<div>` separa sua rolagem do restante do conteúdo, garantindo que apenas a tabela seja rolada horizontalmente quando necessário.

- Exemplo de Uso:
  
    ```html
    <style>
      .container {
        overflow-x: auto;
      }

      table {
        width: 100%;
        border-collapse: collapse;
      }

      th, td {
        border: 1px solid #ddd;
        padding: 8px;
        text-align: left;
      }

      th {
        background-color: #f4f4f4;
      }
    </style>

    <div class="container">
      <table>
        <thead>
          <tr>
            <th>Nome</th>
            <th>Email</th>
            <th>Telefone</th>
            <th>Endereço</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>João</td>
            <td>joao@email.com</td>
            <td>(11) 99999-9999</td>
            <td>Rua das Flores, 123, São Paulo</td>
          </tr>
          <tr>
            <td>Maria</td>
            <td>maria@email.com</td>
            <td>(21) 88888-8888</td>
            <td>Av. Atlântica, 456, Rio de Janeiro</td>
          </tr>
        </tbody>
      </table>
    </div>

    ```




 