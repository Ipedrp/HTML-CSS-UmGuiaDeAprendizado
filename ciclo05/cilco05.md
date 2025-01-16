# Flexbox

- O Flexbox **`(Flexible Box Layout)`** é um módulo de layout CSS
  
- Proporciona uma maneira eficiente de 
  - Organizar 
  - Alinhar  
  - Distribuir espaço entre elementos dentro de um contêiner.
  
- Útil para criar layouts responsivos.
  
- O Flexbox trabalha com dois eixos principais:
  
    - `Main Axis` (eixo principal): Direção primária definida pelo contêiner flex.  
  
    - `Cross Axis` (eixo transversal): Perpendicular ao eixo principal.
  
## Direções e Eixos

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

## Empacotamento e Fluxo

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

## Alinhamento dos Eixos

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

## Centralização Absoluta

- Combine `justify-content`: center e align-items: center para centralizar itens em ambas as direções
- Exemplo de Uso:
    ```css
    .container {

        display: flex;
        justify-content: center;
        align-items: center;
        
    }
    ```
## Alinhamento de Conteúdo Empacotado

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
## Anatomia dos Itens Flexbox

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

## Propriedade flex-basis

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

## Controle do Tamanho de Itens Flexíveis

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
## Propriedade `flex`

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

<!-- felx box, introducao, direcoes e eixos, empacotamento e fluxo, Alinhamento dos Eixos, centralização absoluta, alinhamento de conteudo empacotado, anatomia dos itens flexbox, propriedade flex-baisis, controle do tamanho de itens flexiveis, propriedade flex -->


<!-- 
    Direções e Eixos 
    flex-direction: row -> main-axis vai da esqueda para direita e o cross-axis vai de cima para baixo.
    flex-direction: row-reverse ->  main-axis vai da direita para esquerda e o cross-axis vai de cima para baixo.
    flex-direction: column -> main-axis vai de cima para baixo e o cross-axis da esquerda para direita.
    flex-direction: column-reverse -> main-axis vai de baixo para cima e o cross-axis da esquerda para direita.

    main-axis:
        main-start
        main-end
    coss-axis:
        cross-start
        cross-end
-->

<!-- 
    Empacotamento e fluxo - Quebra do elemnto pai.
    flex-wrap: nowrap -> não encpsule, nao empacote.
    flex-wrap: wrap -> Quando o elemento pai diminui, a caixa que esta dentro, vai seguir a direcao do cross-axis.
    flex-wrap: wrap-reverse -> Quando o elemento pai diminui, a caixa que esta dentro, vai vai seguir a direcao contrario do cross-axis.

    SHORTHANDS PARA FLEX-DIRECTION E FLEX-WRAP:
        flex-direction: row;
        flex-wrap: nowrap;  
        flex-flow: row nowrap;
 -->

<!--
    Alinhamento dos Eixos
    Sempre no sentido do main-axis
        justify-content: flex-start -> o primeiro item ou seja, o primeiro filho ficara grudado ao main-star, e caso exista espaco livre, ficara no final, perto do main-end.
        justify-content: flex-end o último item ou seja, o primierultimoo filho ficara grudado ao main-end, e caso exista espaco livre, ficara no inicio, perto do main-start.
        justify-content: center -> coloca todos os item no centro. no meio do main-axis. e os espacoes seram distribuidos iguais no main-start e main-end.
        justify-content: space-between - > coloca o primeiro item proximo ao main-star e o ultimo item proximo ao main-end, os itens restantes ficaram distribuindo por igual.
        justify-content: space-evenly - >  coloca o primeiro item proximo ao main-star e o ultimo item proximo ao main-end, mas nao grudam, ficam com um pequeno espaco os itens restantes ficaram distribuindo por igual.
        justify-content: space-around - >  coloca entre cada item um espaco antes e depois. Então, não fica colado no main-start e no main-end.
    Sempre no sentido do cross-axis
        align-items: stretch -> estica os items.
        align-items: flex-start -> coloca os item no inicio, colado com o cross-start.
        align-items: flex-end -> coloca os item no final, colado com o cross-end.
        align-items: center -> coloca os item no centro, distribuindo o espaco vazio par ao cross-start e cross-end.
-->

<!--
    Centralização absoluta
    justify-content: center
    align-items: center 
 -->

<!-- 
    Alinhamento de conteudo empacotado
    align-content: Alinha os elementos no eixo trasnversal (cross-axis) qunado estao empacotados
        align-content: stretch -> valor padrao, vai esticar o item
        align-content: flex-start -> coloca todos os elementos em cima, grudado com o cross-start.
        align-content: flex-end -> coloca todos os elementos embaixo, grudado com o cross-end.
        align-content: center -> coloca todos os elementos no centro, deixando espaçoes em branco no cross-start e no cross-end.
        align-content: space-between -> coloca os items em cima, no cross-start e embaixo no cross-end, deixando espaços no meio.
        align-content: space-evenly -> coloca os items proximo, ao cross-start e proximo ao cross-end, deixando espaços no antes, no meio e no final.
        align-content: space-around -> cria um caixa imaginaria e coloca os itens centalizados, com espaco em cima e embaixo.
-->

<!-- 
    Anatomia dos itens flexbox - Trabalha com o flex-itens (elemento filho).
        order: 0 (padrao). 
            Para modificar a ordem dos elementos
                sem orderm: 0 0 0 0
                com ordem: -2 0 7 9
        align-self: Alinhamento dos itens, cada um pode ter um alinhamento diferente, funciona diretamente ao cross-axis.
            align-self: auto ou inherit(herdado) -> pega o alinhamento do pai.
            align-self: flex-start -> alinha ao inicio, proximo ao cross-start.
            align-self: flex-end -> alinha ao final, proximo ao cross-end.
            align-self: center -> alinha ao centro.
            align-self: strech -> estica os elementos.
-->
<!-- 
    Propriedade flex-baisis - Trabalha com o flex-itens (elemento filho).
        flex-basis -> Controlar o tamanho
        flex-basis: auto -> o tamanho do elemento é ditado pelo tamanho do conteudo.
        flex-basis: "algum valor" -> assim determina o tamanho, mas ele pode ser diminuido, assim o conteudo do item, vai se quebrando. 
    
 -->

 <!-- 
    Controle do tamanho de itens flexiveis - Trabalha com o flex-itens (elemento filho).
        container-pai: 550px
        flex-basis: 150px
        
        flex-shrink: 1 (padrao) - significa que o elemento pode encolher
        flex-grow: 1 - significa que o elemento pode crescer

        flex-grow: 0 (padrao) - significa que o elemento não pode crescer
        flex-shrink: 0 - significa que o elemento não pode encolher

        trabalhando os tres valores: flex-basis, flex-grow e flex-shirink

        flex-basis: 150px;
        flex-grow: 0;
        flex-shrink: 1;

        flex-basis: 150px;
        flex-grow: 2;
        flex-shrink: 0;

        flex-basis: 150px;
        flex-grow: 1;
        flex-shrink: 2;
  -->

  <!-- 
    Propriedade flex - Trabalha com o flex-itens (elemento filho).

        flex = flex-grow + flex-shrink + flex-basis

        flex-basis: 150px;
        flex-grow: 0;
        flex-shrink: 1; 

            passa a ficar asssim: flex: 0 1 150px
        
        flex-basis: 150px;
        flex-grow: 2;
        flex-shrink: 0;

            passa a ficar asssim: flex: 2 0 150px

        flex-basis: 150px;
        flex-grow: 1;
        flex-shrink: 2;

            passa a ficar asssim: flex: 1 2 150px


        mais simplificações:
            flex: 0 1 auto
            flex: initial

            flex: 0 0 auto
            flex: none

            flex: 1 1 auto
            flex: auto

            flex: 3 1 auto
            flex: 3


    
   -->