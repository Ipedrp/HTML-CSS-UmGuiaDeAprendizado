- [1. Flexbox](#1-flexbox)
  - [1.1. Direções e Eixos](#11-direções-e-eixos)
  - [1.2. Empacotamento e Fluxo](#12-empacotamento-e-fluxo)
  - [1.3. Alinhamento dos Eixos](#13-alinhamento-dos-eixos)
  - [1.4. Centralização Absoluta](#14-centralização-absoluta)
  - [1.5. Alinhamento de Conteúdo Empacotado](#15-alinhamento-de-conteúdo-empacotado)
  - [1.6. Anatomia dos Itens Flexbox](#16-anatomia-dos-itens-flexbox)
  - [1.7. Propriedade `flex-basis`](#17-propriedade-flex-basis)
  - [1.8. Controle do Tamanho de Itens Flexíveis](#18-controle-do-tamanho-de-itens-flexíveis)
  - [1.9. Propriedade `flex`](#19-propriedade-flex)
- [2. CSS Grid](#2-css-grid)
  - [2.1. Terminologias do CSS Grid](#21-terminologias-do-css-grid)
  - [2.2. CSS Grid x Flexbox](#22-css-grid-x-flexbox)
  - [2.3. Propriedades Básicas](#23-propriedades-básicas)
  - [2.4. Grid Explícita vs. Implícita](#24-grid-explícita-vs-implícita)
  - [2.5. Funções Avançadas](#25-funções-avançadas)
  - [2.6. Unidade `fr`](#26-unidade-fr)
  - [2.7. Alinhamento](#27-alinhamento)
  - [2.8. Ocupando Espaços](#28-ocupando-espaços)
  - [2.9. Sobreposição](#29-sobreposição)
  - [2.10. Áreas Nomeadas no CSS Grid](#210-áreas-nomeadas-no-css-grid)
  - [2.11. `auto-fill` e `auto-fit`](#211-auto-fill-e-auto-fit)
  - [2.12. Linhas Nomeadas](#212-linhas-nomeadas)

# 1. Flexbox

- O Flexbox **`(Flexible Box Layout)`** é um módulo de layout CSS
  
- Proporciona uma maneira eficiente de 
  - Organizar 
  - Alinhar  
  - Distribuir espaço entre elementos dentro de um contêiner.
  
- Útil para criar layouts responsivos.
  
- O Flexbox trabalha com dois eixos principais:
  
    - `Main Axis` (eixo principal): Direção primária definida pelo contêiner flex.  
  
    - `Cross Axis` (eixo transversal): Perpendicular ao eixo principal.
  
## 1.1. Direções e Eixos

- A propriedade **`flex-direction`** define o eixo principal (main-axis) do layout:

- Valores de **`flex-direction`**

    - **`row`**: Eixo principal da esquerda para a direita; eixo transversal de cima para baixo.

    - **`row-reverse`**: Eixo principal da direita para a esquerda; eixo transversal de cima para baixo.

    - **`column`**: Eixo principal de cima para baixo; eixo transversal da esquerda para a direita.

    - **`column-reverse`**: Eixo principal de baixo para cima; eixo transversal da esquerda para a direita.
  
- Eixos
  - **`main-axis`**:

      - `main-start`: Início do eixo principal.

      - `main-end`: Fim do eixo principal.

  - **`cross-axis`**:

      - `cross-start`: Início do eixo transversal.

      - `cross-end`: Fim do eixo transversal.
  
- Exemplo de Uso:
    ```css
    .container {

        display: flex;
        flex-direction: row;

    }
    ```
- Mais Exemplo:
  
    ![Direcoes e Eixos](/img/devices-direction.png)

## 1.2. Empacotamento e Fluxo

- A propriedade **`flex-wrap`** controla o comportamento de itens que ultrapassam o espaço disponível no contêiner:

- Valores de **`flex-wrap`**

  - `nowrap`: Itens permanecem em uma única linha.

  - `wrap`: Itens são quebrados em várias linhas, seguindo o eixo transversal (cross-axis).

  - `wrap-reverse`: Itens quebrados em linhas, mas invertendo o eixo transversal (cross-axis).

  - Exemplo de Uso:
      ```css
      .container {

        display: flex;
        flex-wrap: wrap-reverse;
      
      }
      ```
- Shorthands

  - A combinação de **`flex-direction`** e **`flex-wrap`** é definida com **`flex-flow`**:

  - Exemplo de Uso:
      ```css
      .container {

          display: flex;
          flex-flow: row nowrap;
      
      }
      ```
  - Mais Exemplo:
      - Antes da quebra
      ![Flex-wrap](/img/flex-wrap-before.png)
      - Depois da quebra
      ![Flex-wrap](/img/flex-wrap-after.png)

## 1.3. Alinhamento dos Eixos

- **`Main Axis`** (Eixo Principal)

- A propriedade **`justify-content`** alinha os itens ao longo do eixo principal:

    - `flex-start`: Itens próximos ao início (main-start).

    - `flex-end`: Itens próximos ao fim (main-end).

    - `center`: Itens centralizados.

    - `space-between`: Espaçamento igual entre os itens, com o primeiro próximo ao main-start e o último ao main-end.

    - `space-around`: Espaçamento igual em torno de cada item.

    - `space-evenly`: Espaçamento igual entre os itens e as bordas.
  
- Exemplo de Uso:
    ```css
    .container {

        display: flex;
        justify-content: center;

    }
    ```
- Mais Exemplo:
    - `flex-flow`: row nowrap;
    ![justify-content](/img/justify-content.png)
    -  `flex-flow`: column nowrap;
    ![justify-content](/img/justify-content-column.png)

- **`Cross Axis`** (Eixo Transversal)

- A propriedade **`align-items`** alinha os itens ao longo do eixo transversal:

    - `stretch`: Itens esticados (padrão).

    - `flex-start`: Itens alinhados ao início (cross-start).

    - `flex-end`: Itens alinhados ao final (cross-end).

    - `center`: Itens centralizados.

- Exemplo de Uso:
    ```css
    .container {

        display: flex;
        align-items: center;
    
    }
    ```
- Mais Exemplo:
    - `flex-direction`: row
    ![Flex-wrap](/img//align-itens.png)

## 1.4. Centralização Absoluta

- Combine `justify-content`: center e align-items: center para centralizar itens em ambas as direções
- Exemplo de Uso:
    ```css
    .container {

        display: flex;
        justify-content: center;
        align-items: center;
        
    }
    ```
## 1.5. Alinhamento de Conteúdo Empacotado

- A propriedade **`align-content`** alinha várias linhas no eixo transversal (cross-axis):

    - `stretch`: Estica as linhas (padrão).

    - `flex-start`: Linhas próximas ao início.

    - `flex-end`: Linhas próximas ao final.

    - `center`: Linhas centralizadas.

    - `space-between`: Espaçamento igual entre as linhas.

    - `space-around`: Espaçamento igual em torno de cada linha.

    - `space-evenly`: Espaçamento uniforme entre as linhas e as bordas.
  
    - Exemplo de Uso:
        ```css
        .container {
            display: flex;
            flex-wrap: wrap;
            align-content: space-around;
        }
        ```
## 1.6. Anatomia dos Itens Flexbox

- Propriedade **`order`**

  - Altera a ordem dos itens:{}
  - Exemplo de Uso:
    ```css
    .item1 {
        order: 2; /* Padrão é 0 */
    }

    .item2 {
        order: 0; /* Padrão é 0 */
    } 

    .item3 {
        order: -1; /* Padrão é 0 */
    } 
    ```
  - Mais Exemplo:
    - Ordem crescente
    ![Order](/img/order.png)

- Propriedade **`align-self`**

  - Alinha individualmente cada item no eixo transversal (cross-axis):

    - auto: Herda do contêiner.

    - flex-start, flex-end, center, stretch: Alinhamentos específicos.
  
  - Exemplo de Uso:
    ```css
    .item1 {
         align-self: center; /* Padrão é auto */
    } 

    .item2 {
        align-self: flex-end; /* Padrão é auto */
    } 

    .item3 {
        align-self: stretch; /* Padrão é auto */
    } 
    ```
  - Mais Exemplo:
    
    ![Align self](/img/align-self.png)

## 1.7. Propriedade `flex-basis`

- Controla o tamanho inicial de um item:

    - `auto`: Tamanho baseado no conteúdo.

    - Valor fixo: Define o tamanho inicial, mas permite flexibilidade.
  
- Exemplo de Uso:
    ```css
    .item1 {
        flex-basis: 150px; /* Padrão é auto */
    } 

    .item2 {
        flex-basis: 350px; /* Padrão é auto */
    } 

    .item3 {
        flex-basis: 550px; /* Padrão é auto */
    } 
    ```
- Mais Exemplo:
    
    ![Align self](/img/basis.png)

## 1.8. Controle do Tamanho de Itens Flexíveis

- Propriedades

    - `flex-grow`: Permite que o item cresça.
      - valor padrão: 0 - não permite crescer
      - valor: 1 - permite crescer
    
    - `flex-shrink`: Permite que o item encolha.
      - valor padão: 1 - Permite encolher
      - valor: 0 - não permite encolher

    - `flex-basis`: Define o tamanho inicial.
  
- Exemplo de Uso:
    ```css
    div#a{

        flex-shrink: 1; /*vai encolher*/
        flex-grow: 1; /*vai crescer*/

    }

    div#b{

        flex-shrink: 0;  /*não vai encolher*/
        flex-grow: 2; /*vai crescer duas vezes mais*/

    }

    div#c{

        flex-shrink: 0;  /*não vai encolher*/
        flex-grow: 0; /*não vai crescer*/

    }
    ```
## 1.9. Propriedade `flex`

- Agrupa as propriedades `flex-grow`, `flex-shrink` e `flex-basis`:
- Exemplo de Uso:
  ```css
    div#a{

        flex: 0 1 auto
        /*ou*/
        flex: initial

    }

    div#b{

        flex: 0 0 auto
        /*ou*/
        flex: none

    }

    div#c{

        flex: 1 1 auto
        /*ou*/
        flex: auto

    }

    div#d{

        flex: 3 1 auto 
        /*ou*/
        flex: 3

    }
            
  ```

# 2. CSS Grid
- CSS Grid é um sistema de layout poderoso que permite criar estruturas complexas e responsivas de forma simples e eficiente.

## 2.1. Terminologias do CSS Grid

- **Grid Container**: O elemento onde o Grid é definido. Contém os **grid-items**.
- **Grid Item**: Os elementos filhos diretos do grid container.
- **Grid Line**: Linhas de grid (horizontais e verticais) que dividem o container em áreas.
- **Grid Track**: O espaço entre duas linhas de grid consecutivas.
- **Grid Area**: Uma ou mais células do grid ocupadas por um item.
- **Grid Gap**: O espaçamento entre linhas e colunas.
- **Grid Aninhado**: Um grid dentro de outro grid.

## 2.2. CSS Grid x Flexbox

- O CSS Grid não substitui o Flexbox. Ambos têm propósitos diferentes:
  - **Flexbox**: Ideal para layouts unidimensionais (linha ou coluna).
  - **Grid**: Melhor para layouts bidimensionais (linhas e colunas).



## 2.3. Propriedades Básicas

- Definição de Colunas e Linhas
  
    - `grid-template-columns`: Define o número de colunas e a largura de cada uma no grid.

    - `grid-template-rows`: Define o número de linhas e a altura de cada uma no grid.
      - Exemplo de Uso:
          ```css
          .grid {
              display: grid;
              grid-template-columns: 50% 200px 200px; /* 3 colunas: 50% da largura, 200px, 200px */
              grid-template-rows: 200px 200px 200px; /* 3 linhas, cada uma com 200px */
          }
          ```
- Espaçamentos
  - `column-gap`: Espaçamento entre colunas.
  - `row-gap`: Espaçamento entre linhas.
  - `gap`: Espaçamento geral (colunas e linhas).
    - Exemplo de Uso:
        ```css
        .grid {
            column-gap: 30px;
            row-gap: 30px;
            gap: 40px;
        }
        ```

## 2.4. Grid Explícita vs. Implícita

- **Grid Explícita**: Linhas e colunas definidas manualmente.
  - Exemplo de Uso:
    ```css
    .grid{
        grid-template-rows: 200px 200px;/*Duas linhas com 200px de altura cada*/
        grid-template-columns: 50% 200px 200px; /* 3 colunas: 50% da largura, 200px, 200px */
    }
    ```
- **Grid Implícita**: Linhas e colunas criadas automaticamente.
  - Exemplo de Uso:
    ```css
    .grid{
        grid-auto-rows: 70px; /* Altura padrão para linhas geradas automaticamente */
        grid-auto-columns: 100px; /* Largura padrão para colunas geradas automaticamente */
    }
    ```

## 2.5. Funções Avançadas

- `repeat()` e `minmax()`

  - `repeat()`: Define múltiplas colunas/linhas com valores repetidos.
    - Exemplo de Uso:
    
      ```css
      .grid{
        grid-template-columns: repeat(4, 200px); /* 4 colunas de 200px cada */
      }
      ```

  - `minmax()`: Define limites mínimo e máximo para colunas/linhas.
    - Exemplo de Uso:
      ```css
      .grid{
        grid-template-columns: minmax(200px, 50%) 200px 200px;
      }
      ```
## 2.6. Unidade `fr`

- `fr` (fração) distribui espaço proporcionalmente.
  - Exemplo de Uso:
      ```css
      .grid{
        grid-template-columns: 1fr 2fr 1fr; /* 3 colunas, a do meio ocupa o dobro do espaço */
      }
      ```
## 2.7. Alinhamento

- No CSS Grid, o alinhamento é controlado em dois eixos principais:
  - **Eixo vertical**: alinhamento ao longo do eixo das colunas (eixo bloco no CSS moderno).  
  - **Eixo horizontal**: alinhamento ao longo do eixo das linhas (eixo inline no CSS moderno).  

- O alinhamento pode ser aplicado ao **Grid Container** (afeta todos os itens) ou ao **Grid Item** (de forma individual).

- **No Grid Container**

    - **Alinhamento Vertical (Eixo das Colunas)**:
      - Controlado com a propriedade `align-items`:
      - Exemplo de Uso:
        ```css
        .grid-container {
            align-items: start;   /* Alinha os itens no topo */
            align-items: end;     /* Alinha os itens na parte inferior */
            align-items: center;  /* Alinha os itens ao centro verticalmente */
            align-items: stretch; /* (Padrão) Estica os itens para ocupar o espaço total */
        }
        ```

    - **Alinhamento Horizontal (Eixo das Linhas)**:
  
      - Controlado com a propriedade `justify-items`:
      - Exemplo de Uso:
        ```css
        .grid-container {
              justify-items: start;   /* Alinha os itens no início */
              justify-items: end;     /* Alinha os itens no final */
              justify-items: center;  /* Alinha os itens ao centro horizontalmente */
              justify-items: stretch; /* (Padrão) Estica os itens para ocupar o espaço total */
          }
        ```

- **No Grid Item**
- Essas propriedades ajustam o alinhamento de um item específico dentro do grid.
  - **Alinhamento Vertical (Eixo das Colunas)**
    - Controlado com a propriedade `align-self`:
    - Exemplo de Uso:
        ```css
        .grid-item {
              align-self: start;   /* Alinha o item no topo */
              align-self: end;     /* Alinha o item na parte inferior */
              align-self: center;  /* Alinha o item ao centro verticalmente */
              align-self: stretch; /* (Padrão) Estica o item para ocupar o espaço total */
          }
        ```
  - **Alinhamento Horizontal (Eixo das Linhas)**
    - Controlado com a propriedade `justify-self`:
    - Exemplo de Uso:
        ```css
        .grid-item {
            justify-self: start;   /* Alinha o item no início */
            justify-self: end;     /* Alinha o item no final */
            justify-self: center;  /* Alinha o item ao centro horizontalmente */
            justify-self: stretch; /* (Padrão) Estica o item para ocupar o espaço total */
        }
        ```
## 2.8. Ocupando Espaços
- É possível definir quantas colunas ou linhas um **Grid Item** deve ocupar, utilizando propriedades específicas. 
- Essas propriedades podem ser declaradas de forma separada:
  - `grid-column-start`
  - `grid-column-end`
  - `grid-row-start`
  - `grid-row-end`
- Ou através de suas abreviações:
  - `grid-column` 
  - `grid-row`

- **Colunas**
  - **Propriedades Individuais**
    - **`grid-column-start`**: Define onde o item inicia na grade de colunas.
    - **`grid-column-end`**: Define onde o item termina na grade de colunas.

    - Exemplo de Uso:
        ```css
        .grid-item {
            grid-column-start: 1; /* Inicia na coluna 1 */
            grid-column-end: 3;   /* Termina na coluna 3 */
        }
        ```
  - **Propriedade Combinada**
    - **`grid-column`**: Combina o início e o final da ocupação em uma única declaração.
    - Sintaxe: 
      - `grid-column`: [início] / [fim].
      - `span`: Pode ser usado para definir o número de colunas que o item deve ocupar, a partir da coluna inicial.
      - Exemplo de Uso:
          ```css
          .grid-item {
              grid-column: 1 / 3;      /* Ocupa da coluna 1 até a 3 */
              grid-column: 1 / span 2; /* Ocupa 2 colunas, começando na 1 */
          }
          ```

-  **Linhas**
-  **Propriedades Individuais**
   - **`grid-row-start`**: Define onde o item inicia na grade de linhas.
   - **`grid-row-end`**: Define onde o item termina na grade de linhas.

   - Exemplo de Uso:   
       ```css
       .grid-item {
            grid-row-start: 1; /* Inicia na linha 1 */
            grid-row-end: 4;   /* Termina na linha 4 */
       }
       ```
   - Propriedade Combinada
    - **`grid-row`**: Combina o início e o final da ocupação em uma única declaração.
    - Sintaxe: 
      - `grid-row`: [início] / [fim].
      - `span`: Pode ser usado para definir o número de linhas que o item deve ocupar, a partir da linha inicial.
   - Exemplo de Uso:
        ```css
        .grid-item {
            grid-column: 1 / 3;      /* Ocupa da coluna 1 até a 3 */
            grid-column: 1 / span 2; /* Ocupa 2 colunas, começando na 1 */
        }
        ``` 

## 2.9. Sobreposição

- Itens podem se sobrepor utilizando as mesmas áreas de grid:
  - Exemplo de Uso:

    ```css
    .grid {
        display: grid;
        grid-template-columns: repeat(5, 1fr);
    }
    .item1 {
        grid-row: 1 / span 2;
        grid-column: 1 / span 2;
    }
    .item2 {
        grid-row: 2 / span 2;
        grid-column: 1 / span 3;
    }
    ```
## 2.10. Áreas Nomeadas no CSS Grid

- O CSS Grid permite criar layouts organizados e intuitivos utilizando **áreas nomeadas**. 
- Essa funcionalidade é controlada pelas propriedades `grid-template-areas` e `grid-area`.

- **Propriedades e Funções**

    - **`grid-template-areas`**
       - Declarada no **Grid Container**.
       - Define as áreas do layout com nomes atribuídos a grupos de células.
       - Cada string dentro da propriedade corresponde a uma linha da grade.
       - Nomes repetidos em células adjacentes indicam que essas células pertencem à mesma área.
       - Espaços vazios podem ser indicados com o caractere `.`.

    - **`grid-area`**
       - Declarada no **Grid Item**.
       - Relaciona o item com uma área nomeada definida no `grid-template-areas`.

    - **Exemplo de Uso**

      - **No Grid Container**
          ```css
          .grid-container {
              display: grid;
              grid-template-columns: 1fr 2fr; /* Define duas colunas, a primeira menor */
              grid-template-rows: auto auto auto; /* Três linhas automáticas */
              grid-template-areas: 
                  "header header"    /* Primeira linha: header ocupa ambas as colunas */
                  "main sidebar"     /* Segunda linha: main e sidebar dividem o espaço */
                  "footer footer";   /* Terceira linha: footer ocupa ambas as colunas */
          }
          ```
      - **No Grid Item**
          ```css
              header {
                  grid-area: header; /* Vincula este item à área 'header' */
              }

              main {
                  grid-area: main; /* Vincula este item à área 'main' */
              }

              .sidebar {
                  grid-area: sidebar; /* Vincula este item à área 'sidebar' */
              }

              footer {
                  grid-area: footer; /* Vincula este item à área 'footer' */
              }
              
          ```
- **Espaços Vazios na Grade**
  - Para deixar espaços vazios no layout, utilize o caractere `.` em vez de um nome de área.
  - Exemplo de Uso:
    ```css
    .grid-container {
          display: grid;
          grid-template-columns: 1fr 1fr 1fr;
          grid-template-rows: auto auto;
          grid-template-areas: 
              "header header header"    /* Header ocupa toda a linha */
              "main     .    sidebar"   /* Espaço vazio no meio */
              "footer footer footer";   /* Footer ocupa toda a linha */
    }
    ```

## 2.11. `auto-fill` e `auto-fit`

- `auto-fill`: Adiciona colunas extras mesmo que estejam vazias.
- `auto-fit`: Ajusta o número de colunas ao tamanho disponível.
- Exemplo de Uso:
    ```css
    .grid-container{
        grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    }
    ```

<!-- ## 2.12. Linhas Nomeadas
- Exemplo de Uso:

    ```css
    .grid-container {
        grid-template-columns: [start] 1fr [middle] 1fr [end];
    }
    .grid-item {
        grid-column: start / middle;
    }
    ``` -->
## 2.12. Linhas Nomeadas 

- O CSS Grid permite atribuir **nomes às linhas** (tanto de colunas quanto de linhas) para tornar o layout mais descritivo e facilitar o posicionamento dos itens.

- **Propriedades e Funções**

  - **Linhas Nomeadas**

     - Declaradas no **Grid Container**.
     - Os nomes das linhas são definidos entre colchetes `[]` na propriedade `grid-template-columns` ou `grid-template-rows`.
     - Esses nomes podem ser usados no posicionamento dos itens para especificar onde começar e terminar.

  - **Utilizando Nomes no Posicionamento**

     - Os itens utilizam os nomes das linhas com as propriedades `grid-column` e `grid-row`.

- **Exemplo de Uso**

  - **No Grid Container**

    ```css
    .grid-container {
        display: grid;
        grid-template-columns: [start] 1fr [middle] 1fr [end]; /* Define nomes para as linhas de coluna */
        grid-template-rows: [top] 100px [center] 200px [bottom]; /* Define nomes para as linhas de linha */
    }
    ```

  - **No Grid Item**
  
      ```css
      .grid-item {
              grid-column: start / middle; /* O item ocupa da linha "start" até a linha "middle" na grade de colunas */
              grid-row: top / center; /* O item ocupa da linha "top" até a linha "center" na grade de linhas */
          }
      ```
- **Nomes de Múltiplas Linhas**
  
  - É possível atribuir múltiplos nomes à mesma linha, separando-os por espaços.
  
  - Exemplo de Uso:
    ```css
    .grid-container {
        display: grid;
        grid-template-columns: [col-start primary] 1fr [col-middle secondary] 1fr [col-end];
    }

    .grid-item {
        grid-column: primary / secondary; /* Usa os nomes "primary" e "secondary" para posicionamento */
    }

    ```