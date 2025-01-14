
- [1. Uso de **`iframe`**](#1-uso-de-iframe)
  - [1.1. Estrutura Básica do **`iframe`**](#11-estrutura-básica-do-iframe)
  - [1.2. Propriedades do **`iframe`**](#12-propriedades-do-iframe)
- [2. Formulários - `form`](#2-formulários---form)
  - [2.1. Estrutura Básica do Formulário](#21-estrutura-básica-do-formulário)
  - [2.2. Tipos de Campos com `<input>`](#22-tipos-de-campos-com-input)
  - [2.3. Atributos Comuns dos Campos](#23-atributos-comuns-dos-campos)
- [3. Media Queries](#3-media-queries)
  - [3.1. Media Types](#31-media-types)
  - [3.2. Media Features](#32-media-features)
  - [3.3. Mobile First](#33-mobile-first)
  - [3.4. Device Breakpoints](#34-device-breakpoints)
  - [3.5. Propriedades e Atributos em Media Queries](#35-propriedades-e-atributos-em-media-queries)

# 1. Uso de **`iframe`** 
- O elemento `<iframe>` é utilizado para incorporar documentos externos em uma página da web. 
- Permite que conteúdos como:
  - Páginas HTML
  - Vídeos,
  - Mapas ou outros elementos sejam integrados diretamente em uma página.

## 1.1. Estrutura Básica do **`iframe`**
- Exemplo de Uso:
  
    ```html
        <iframe 
            src="paginasExtras/pag004.html" 
            frameborder="1" 
            width="500px" 
            height="300px" 
            sandbox="allow-same-origin allow-forms allow-scripts" 
            referrerpolicy="no-referrer">
        </iframe>

    ```

## 1.2. Propriedades do **`iframe`**

- **`src`**
- **`frameborder`**
- **`width e height`**
- **`sandbox`**
- **`referrerpolicy`**
- **`allow`**
- **`loading`**


- Um pouco sobre cada uma:

  - **`src`**

    - Especifica a URL do conteúdo a ser exibido no iframe.
    - Exemplo de Uso:

        ```html
        <iframe src="https://www.example.com"></iframe>
        ```

  - **`frameborder`**

    - Define se o contorno do iframe será exibido.
    - Valores:

      - 1 (padrão): exibe o contorno.
      - 0: remove o contorno.
    
  - **`width`** e **`height`**
    - Define a largura e altura do iframe. É possível utilizar
    - Valores absolutos (px) ou relativos (%).
    - Exemplo de Uso:

        ```html
        <iframe width="100%" height="400px"></iframe>
        ```
  - **`sandbox`**
    - Aplica restrições ao conteúdo do iframe por questões de segurança.
    - Possíveis valores:
      - **`sandbox`**: bloquei toda ação
      - **`allow-same-origin`**: permite acesso ao mesmo domínio.
      - **`allow-forms`**: permite envio de formulários.
      - **`allow-scripts`**: permite execução de scripts (não em contexto de origem).
      - **`allow-popups`**: permite abertura de janelas popup.
      - **`allow-modals`**: permite exibição de modais
  
      - Exemplo de Uso com Múltiplos Valores:
        ```html
        <iframe sandbox="allow-same-origin allow-forms"></iframe>
        ```
  - **`referrerpolicy`**
    - Controla como o cabeçalho Referer é enviado ao carregar o conteúdo do iframe.
    - Possíveis valores:

      - **`no-referrer`**: nenhum cabeçalho Referer será enviado.
      - **`origin`**: apenas a origem será enviada.
      - **`same-origin`**: informações de Referer são enviadas apenas se a origem for a mesma.
  
  - **`allow`**: Especifica permissões como uso de câmera ou microfone.
  - Exemplo de Uso:
    ```html
    <iframe allow="camera; microphone"></iframe>
    ```
  - **`loading`**: Define o comportamento de carregamento.
    - **`lazy`**: carrega sob demanda (ao entrar no viewport).
    - **`eager`**: carrega imediatamente.
  
    - Exemplo de Uso:
        ```html
        <iframe loading="lazy"></iframe>
        ```



# 2. Formulários - `form`
- São usados para coletar e enviar informações do usuário para um servidor. 

## 2.1. Estrutura Básica do Formulário
- O tag **`<form>`** serve como um contêiner para os campos de entrada e inclui atributos essenciais para controlar o envio.

  - Atributos Importantes:
    - **`action`**: Define o URL para onde os dados do formulário serão enviados.
    - **`method`**: Especifica o método HTTP usado para enviar os dados:     
      - `GET`: Dados são enviados como parte da URL. 
        - Melhor para buscas ou operações que não alteram o estado do servidor.
        - Limitação no tamanho dos dados ( 3000 Bytes ). 
      - `POST`: Dados são enviados no corpo da requisição.
        - Ideal para envio de informações sensíveis ou que alterem o estado no servidor.
        - Sem limite significativo de tamanho.
  
## 2.2. Tipos de Campos com `<input>`
- O elemento **`<input>`** é usado para criar diferentes tipos de campos de entrada. O tipo do campo é especificado pelo atributo type.

- Principais Tipos de **`<input>`** e Seus Usos:
  - `text`: Campo de texto simples para entrada de uma linha. 
    - Uso: 	Nome, sobrenome...
  - `email`: Valida entrada de um endereço de e-mail.	
    - Uso: Cadastro de e-mail.
  - `password`: Entrada de texto oculto (usado para senhas).		
    - Uso: Senhas.
  - `number`: Aceita somente números, com incrementadores opcionais.		
    - Uso: Idade, quantidade...
  - `tel`: Valida entrada de números de telefone.		
    - Uso: Contato telefônico.
  - `url`: 	Valida entrada de um URL válido.	
    - Uso: Links.
  - `date`: Abre um seletor de data.		
    - Uso: Data de nascimento.
  - `time`: Abre um seletor de horário.			
    - Uso: 	Horário de encontro.
  - `file`: Permite o upload de arquivos.	
    - Uso: Envio de documentos ou imagens.
  - `checkbox`: Permite seleção de múltiplas opções em um grupo.	
    - Uso: Preferências ou consentimentos.
  - `radio`: Permite a seleção de apenas uma opção dentro de um grupo
    - Uso: Escolha de gênero, status, etc.
  - `range`: Cria um controle deslizante para valores numéricos.		
    - Uso: Ajuste de volume ou preço.
  - `color`: Permite selecionar uma cor.			
    - Uso: 	Paleta de cores.
  - `hidden`: Campo invisível, usado para enviar valores no background.
    - Uso: IDs de sessão ou parâmetros ocultos.
  - Exemplo Completo:
    ```html
      <form action="/enviar-dados" method="post">
        <label for="nome">Nome:</label>
        <input type="text" id="nome" name="nome" required>

        <label for="email">Email:</label>
        <input type="email" id="email" name="email" required>

        <label for="senha">Senha:</label>
        <input type="password" id="senha" name="senha" required>

        <label for="idade">Idade:</label>
        <input type="number" id="idade" name="idade" min="0" max="100" required>

        <label for="cor">Escolha uma cor:</label>
        <input type="color" id="cor" name="cor">

        <label for="arquivo">Envie um arquivo:</label>
        <input type="file" id="arquivo" name="arquivo">

        <button type="submit">Enviar</button>
      </form>
    ```
## 2.3. Atributos Comuns dos Campos

  - **`id`**: Identifica o campo unicamente.	
  
    - Uso: 	`id`="nome"
  
  - **`name`**: Nome do campo, usado na submissão dos dados.
  
    - Uso: `name`="email"
  
  - **`placeholder`**: Texto exibido dentro do campo enquanto está vazio.
  
    - Uso: `placeholder`="Seu nome"
  
  - **`value`**: Valor padrão do campo.		
  	
    - Uso: `value`="João"
  
  - **`required`**: Torna o preenchimento obrigatório.
  
    - Uso: `required`
  
  - **`readonly`**: O campo pode ser visualizado, mas não editado.	
  
    - Uso: `readonly`
  
  - **`disabled`**: O campo fica desativado e não pode ser enviado.	
  
    - Uso: `disabled`
  
  - **`min / max`**: 	Define valores mínimo e máximo para entrada numérica.
  
    - Uso: `min`="0" `max`="100"
  
  - **`step`**: Define o intervalo de incremento para entradas numéricas ou de intervalo.	
  
    - Uso: 	`step`="5"
  
  - **`autocomplete`**: Controla se o navegador deve preencher automaticamente os campos (`on` ou `off`)	
  
    - Uso: 	`autocomplete`="on"

# 3. Media Queries 

- São uma funcionalidade poderosa do CSS3 que permite criar layouts responsivos, adaptando estilos de acordo com características do dispositivo ou do viewport do usuário.


## 3.1. Media Types
- Os **Media Types** especificam o tipo de dispositivo para o qual os estilos são aplicados. Exemplos:
- **`all`**: Para todos os dispositivos (padrão).
- **`screen`**: Para telas como monitores, smartphones e tablets.
- **`print`**: Para visualização e impressão de documentos.
- **`speech`**: Para dispositivos de leitura de texto.
- Exemplo de Uso:
  
  ```css
  @media screen {
    body {
      font-family: Arial, sans-serif;
    }
  }
  ```

## 3.2. Media Features
- As Media Features permitem aplicar estilos baseados em características específicas do dispositivo, como largura da tela, orientação e densidade de pixels.

- Principais Media Features:
  - **`min-width`** e **`max-width`**: Especificam larguras mínima e máxima.
  - **`min-height`** e **`max-height`**: Definem alturas mínima e máxima.
  - **`orientation`**: Define a orientação da tela:
    - **`portrait`**: Quando a altura é maior que a largura.
    - **`landscape`**: Quando a largura é maior que a altura.
    - **`resolution`**: Especifica a densidade de pixels (dpi ou dppx).
  - Exemplo de Uso:
  
    ```css
    /* Modo retrato (portrait) */
    @media (orientation: portrait) {
      body {
        background-color: lightpink;
      }
    }

    /* Modo paisagem (landscape) */
    @media (orientation: landscape) {
      body {
        background-color: lightblue;
      }
    }
    ```

## 3.3. Mobile First
- O conceito de Mobile First sugere que os estilos base sejam criados para dispositivos móveis e sejam progressivamente adaptados para telas maiores usando Media Queries.
- Exemplo de Uso:
  
  ```css
  /* Estilo base (Mobile First) */
  body {
    font-size: 16px;
  }

  /* Adaptação para telas maiores */
  @media (min-width: 768px) {
    body {
      font-size: 18px;
    }
  }
  ```

## 3.4. Device Breakpoints
- Os Breakpoints definem pontos de interrupção onde o layout muda para melhorar a experiência em diferentes dispositivos.
  
- Pequenas telas: Até **600px**
- Celulares: De **600px** a **768px**
- Tablets: De **768px** a **992px** 
- Desktop: De **992px** a **1200px**
- Grandes telas: Acima de **1200px**

- Exemplo de Uso:
  ```css
  /* Pequenas telas: Até 600px */
  @media (max-width: 600px) {
    body {
      background-color: lightcoral;
    }
  }

  /* Celulares: De 600px a 768px */
  @media (min-width: 600px) and (max-width: 768px) {
    body {
      background-color: lightgreen;
    }
  }

  /* Tablets: De 768px a 992px */
  @media (min-width: 768px) and (max-width: 992px) {
    body {
      background-color: lightblue;
    }
  }

  /* Desktop: De 992px a 1200px */
  @media (min-width: 992px) and (max-width: 1200px) {
    body {
      background-color: lightgoldenrodyellow;
    }
  }

  /* Grandes telas: Acima de 1200px */
  @media (min-width: 1200px) {
    body {
      background-color: lightgray;
    }
  }
  ```
  
## 3.5. Propriedades e Atributos em Media Queries
- **`<media-type>`**: Tipo de mídia  
  
  - Ex: screen.
  
- **`<media-feature>`**: Características específicas 
  
  - Ex: min-width, orientation.
  
  - Sintaxe Geral:
  
    ```css
    @media <media-type> and (<media-feature>) {
      /* Estilos aplicados aqui */
    }

    ```
  - Exemplo de Uso: 
    ```css
    @media screen and (min-width: 768px) and (orientation: landscape) {
      body {
        background-color: lightpink;
      }
    }

    ```