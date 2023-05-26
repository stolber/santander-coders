# Módulo 3 - CSS :art:

## 1. Introdução a CSS e História da Web

O CSS (Cascading Style Sheets) é uma linguagem de estilo utilizada para definir a apresentação visual de documentos HTML. Ele permite controlar o layout, cores, fontes e outros aspectos visuais de uma página web.

Existem três formas de utilizar o CSS em um documento HTML:

1. **CSS Inline**: É possível definir estilos diretamente nas tags HTML usando o atributo `style`. Por exemplo:

```html
<p style="color: blue;">Este é um parágrafo com estilo inline.</p>
```

2. **CSS Embutido**: Os estilos podem ser adicionados no cabeçalho do documento HTML, entre as tags `<style>` e `</style>`. Por exemplo:

```html
<head>
    <style>
        p {
            color: blue;
        }
    </style>
</head>
<body>
    <p>Este é um parágrafo com estilo embutido.</p>
</body>
```

3. **CSS Externo**: É possível criar um arquivo separado com extensão `.css` e vinculá-lo ao documento HTML usando a tag `<link>`. Por exemplo:

No arquivo `estilos.css`:

```css
p {
    color: blue;
}
```

No arquivo HTML:

```html
<head>
    <link rel="stylesheet" href="estilos.css">
</head>
<body>
    <p>Este é um parágrafo com estilo externo.</p>
</body>
```

## 2. Cores, Background e Textos :rainbow:

### Cores

As cores podem ser representadas de diferentes formas no CSS. Algumas delas são:

- Cores nomeadas: por exemplo, `red`, `blue`, `green`.
- Cores RGB: por exemplo, `rgb(255, 0, 0)` para vermelho.
- Combinação de cores: por exemplo, `#FF0000` para vermelho.

Exemplo de uso de cores:

```css
h1 {
    color: red;
    background-color: #00FF00;
}
```

### Background

As propriedades de background controlam o plano de fundo de um elemento. Algumas propriedades incluem:

- `background-color`: define a cor de fundo.
- `background-image`: define uma imagem como fundo.
- `background-size`: especifica o tamanho da imagem de fundo.
- `background-repeat`: determina como a imagem de fundo é repetida.
- `background-position`: define a posição inicial da imagem de fundo.

Exemplo de uso de background:

```css
body {
    background-color: #F2F2F2;
    background-image: url('caminho/para/imagem.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
}
```

### Texto

Algumas propriedades CSS para estilizar o texto incluem:

- `color`: define a cor do texto.
- `font-size`: especifica o tamanho da fonte.
- `font-weight`: define a espessura da fonte (por exemplo, negrito).
- `font-style`: especifica o estilo da fonte (por exemplo, itálico).
- `text-decoration`: controla a decoração do texto (por exemplo, sublinhado).
- `text-transform`: altera o formato do texto (por exemplo, maiúsculas, minúsculas).
- `text-align`: alinha o texto horizontalmente.


- `text-indent`: define o recuo da primeira linha de um parágrafo.

Exemplo de uso de propriedades de texto:

```css
p {
    color: #333333;
    font-size: 16px;
    font-weight: bold;
    text-decoration: underline;
    text-transform: uppercase;
    text-align: center;
    text-indent: 20px;
}
```

## 3. Fontes, Medidas e Links :font:

### Importando Fontes do Google Fonts

Para importar fontes do Google Fonts, você pode adicionar o seguinte trecho de código no cabeçalho do seu documento HTML:

```html
<head>
    <link href="https://fonts.googleapis.com/css2?family=Nome+da+Fonte&display=swap" rel="stylesheet">
</head>
```

Em seguida, você pode utilizar a fonte especificada no CSS:

```css
body {
    font-family: 'Nome da Fonte', sans-serif;
}
```

### Medidas

Existem várias unidades de medida disponíveis no CSS. Algumas delas são:

- `px` (pixels): unidade de medida fixa.
- `%` (porcentagem): relativa ao tamanho do elemento pai.
- `rem` (root em): relativa ao tamanho da raiz do documento (normalmente o elemento `<html>`).
- `em` (em): relativa ao tamanho do elemento pai.
- `vh` (viewport height): relativa à altura da janela de visualização.

Exemplo de uso de medidas:

```css
p {
    font-size: 16px;
    margin: 10px;
    padding: 0.5em;
    width: 50%;
    height: 100vh;
}
```

### Pseudo-classes

Pseudo-classes são seletores que especificam um estado especial de um elemento. Alguns exemplos incluem:

- `:active`: quando o elemento está sendo clicado.
- `:visited`: quando o link já foi visitado.
- `:hover`: quando o cursor está sobre o elemento.

Exemplo de uso de pseudo-classes:

```css
a:active {
    color: red;
}

a:hover {
    text-decoration: underline;
}
```

## 4. Listas, Tabelas, Box Model e Display :clipboard:

### Estilizando Tabelas

Algumas propriedades para estilizar tabelas no CSS incluem:

- `border`: define a borda de uma célula ou da tabela.
- `border-collapse`: especifica o tipo de colapso da borda.
- `first-child`: seleciona o primeiro elemento filho de um elemento pai.
- `nth-child(2n+3)`: seleciona os elementos filhos em posições específicas.

Exemplo de uso de estilização de tabelas:

```css
table {
    border: 1px solid black;
    border-collapse: collapse;
}

tr:first-child {
    font-weight: bold;
}

td:nth-child(2n+3) {
    background-color: lightgray;
}
```

### Estilizando Listas

A propriedade `list-style` controla a aparência das listas. Alguns valores possíveis são:

- `none`: remove os marcadores de lista.
- `disc`: usa um círculo sólido como marcador.
- `decimal`: usa números decimais como marcadores.

Exemplo de uso de estilização de listas:

```css
ul {
    list-style: none;
}

ol {
    list-style: decimal;
}
```

### Box Model

O box model

 é um conceito importante no CSS que define o espaço ocupado por um elemento. Algumas propriedades incluem:

- `display`: define como um elemento é exibido (`inline`, `inline-block`, `block`, etc.).
- `object-fit`: especifica como uma imagem ou vídeo se ajusta ao elemento contenedor.
- `border-radius`: define o arredondamento dos cantos de um elemento.
- `width`: define a largura do elemento.
- `height`: define a altura do elemento.
- `margin`: define as margens ao redor do elemento.
- `padding`: define o preenchimento interno do elemento.
- `box-sizing`: especifica como as dimensões do elemento são calculadas.

Exemplo de uso de box model:

```css
div {
    display: block;
    object-fit: cover;
    border-radius: 5px;
    width: 300px;
    height: 200px;
    margin: 10px;
    padding: 20px;
    box-sizing: border-box;
}
```

## 5. Position e Introdução a Flexbox :pushpin:

### Posicionamento

A propriedade `position` controla como um elemento é posicionado em relação aos outros elementos. Alguns valores incluem:

- `relative`: posicionamento relativo ao elemento pai.
- `absolute`: posicionamento absoluto em relação ao elemento pai mais próximo posicionado.
- `static`: posicionamento normal, seguindo o fluxo do documento.
- `fixed`: posicionamento fixo em relação à janela de visualização.
- `sticky`: posicionamento relativo até que o usuário role além de um ponto específico.

Exemplo de uso de posicionamento:

```css
div {
    position: relative;
    top: 50px;
    left: 20px;
    z-index: 1;
}
```

## 6. Flexbox e Alinhamentos :raised_hands:

O flexbox é um modelo de layout flexível que permite organizar elementos em uma única direção (horizontal ou vertical). Algumas propriedades incluem:

- `flex-wrap`: controla a quebra de linha dos itens flexíveis.
- `flex-direction`: define a direção do fluxo dos itens (`row`, `column`, `row-reverse`, `column-reverse`).
- `flex-flow`: propriedade de atalho para `flex-direction` e `flex-wrap`.
- `flex`: especifica como os itens flexíveis se expandem ou encolhem para preencher o espaço disponível.
- `gap`: define o espaçamento entre os itens flexíveis.
- `justify-content`: alinha os itens horizontalmente.
- `align-items`: alinha os itens verticalmente.
- `align-content`: controla o espaçamento vertical entre as linhas de itens.

Exemplo de uso de flexbox:

```css
.container {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
}

.item {
    flex: 1 0 200px;
    margin: 10px;
}
```

## 7. Seletores, Responsividade e Animações :raised_hands:

### Seletores

Os seletores no CSS permitem selecionar elementos com base em suas características. Alguns tipos de seletores incluem:

- `id`: seleciona elementos com um ID específico.
- `class`: seleciona elementos com uma classe específica.
- `data-atribute`: seleciona elementos com um atributo de dados específico.

Exemplo de uso de seletores:

```css
#elemento-id {
    color: blue;
}



.classe-elemento {
    font-weight: bold;
}

[data-atributo="valor"] {
    text-decoration: underline;
}
```

### Responsividade

A responsividade no CSS permite criar estilos diferentes para diferentes tamanhos de tela. A regra `@media` é usada para definir estilos para condições específicas. Por exemplo:

```css
@media screen and (min-width: 768px) {
    /* Estilos para telas com largura mínima de 768 pixels */
    body {
        font-size: 18px;
    }
}

@media screen and (max-width: 480px) {
    /* Estilos para telas com largura máxima de 480 pixels */
    body {
        font-size: 14px;
    }
}
```

### Animações

As animações no CSS permitem criar transições suaves entre diferentes estados de um elemento. Algumas propriedades relacionadas à animação incluem:

- `display`: controla a visibilidade de um elemento.
- `visibility`: define se um elemento é exibido ou oculto.
- `opacity`: controla a opacidade de um elemento.
- `cursor`: define o estilo do cursor ao passar sobre um elemento.
- `transform`: permite aplicar transformações (como rotação, escala e translação) a um elemento.
- `transition`: especifica a transição suave de uma ou mais propriedades ao longo do tempo.
- `@keyframes`: define uma animação personalizada com base em etapas-chave.
- `animation`: aplica uma animação a um elemento.

Exemplo de uso de animações:

```css
button {
    display: inline-block;
    padding: 10px 20px;
    background-color: blue;
    color: white;
    transition: background-color 0.3s ease;
}

button:hover {
    background-color: red;
}

@keyframes pulse {
    0% {
        transform: scale(1);
    }
    50% {
        transform: scale(1.2);
    }
    100% {
        transform: scale(1);
    }
}

div {
    animation: pulse 2s infinite;
}
```

## 8. Grid Layout e Unidade "fr" :1234:

O Grid Layout é um sistema de layout bidimensional no CSS que permite organizar elementos em linhas e colunas. Algumas propriedades incluem:

- `display: grid`: define o elemento como um container de grid.
- `justify-content`: alinha as colunas horizontalmente.
- `grid-template-rows`: especifica o tamanho das linhas.
- `grid-template-areas`: define um layout de grade baseado em nomes de áreas.
- `grid-template-columns`: especifica o tamanho das colunas.
- `grid-column-gap`: define o espaçamento horizontal entre as colunas.
- `grid-gap`: define o espaçamento entre as células do grid.
- `grid-row-gap`: define o espaçamento vertical entre as linhas.

A unidade `fr` é usada para especificar uma fração do espaço disponível em um grid.

Exemplo de uso de Grid Layout e a unidade `fr`:

```css
.container {
    display: grid;
    grid-template-columns: 1fr 2fr 1fr;
    grid-gap: 10px;
}

.item {
    background-color: lightgray;
    padding: 20px;
}

.item:nth-child(odd) {
    background-color: darkgray;
}
```

## 9 - 10. Compilando Conceitos e Criando Projeto :rocket:

Nesta etapa do curso, vamos criar um projeto que aplicará os conhecimentos apresentados até o momento. Será uma oportunidade para praticar e consolidar o aprendizado.

Espero que este README seja útil para você! :smiley: