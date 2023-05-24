# Introdução ao HTML 

## 🌐 1. Introdução

HTML (HyperText Markup Language) é a linguagem padrão para criação de páginas web. É uma linguagem de marcação que define a estrutura e o conteúdo de uma página, permitindo a organização lógica e a formatação dos elementos.

🎨 Front-End refere-se à parte visual e interativa de um website. Envolve a criação de elementos gráficos e a aplicação de estilos para tornar a página atrativa e fácil de usar.

Nesta documentação, vamos explorar os elementos mais básicos do HTML, aprender a criar uma página HTML, conhecer as principais tags e entender como elas são utilizadas.

## 🏁 2. Criando a Primeira Página HTML

Vamos começar criando a estrutura básica de uma página HTML. Cada página HTML começa com a tag `<html>` e possui um cabeçalho `<head>` e um corpo `<body>`. O cabeçalho é onde colocamos metadados e referências a arquivos externos, como folhas de estilo e scripts.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Minha Primeira Página</title>
</head>
<body>
    <!-- Aqui você pode inserir o conteúdo da página -->
</body>
</html>
```

Dentro do corpo da página, podemos adicionar diversos elementos para exibir conteúdo.

## 🏷️ 3. Principais Tags HTML

### Cabeçalhos

Os cabeçalhos são usados para definir os títulos e subtítulos de uma página. Eles vão de `<h1>` a `<h6>`, sendo `<h1>` o maior e `<h6>` o menor.

```html
<h1>Título</h1>
<h2>Subtítulo</h2>
...
<h6>Subtítulo Menor</h6>
```

### Parágrafos

O parágrafo é usado para agrupar e formatar blocos de texto.

```html
<p>Este é um parágrafo de exemplo.</p>
```

### Divisor de Linha

A tag `<br>` é usada para criar uma quebra de linha dentro de um parágrafo ou outro elemento.

```html
<p>Linha 1<br>Linha 2</p>
```

### Links

Os links são usados para criar hiperlinks para outras páginas ou recursos na web.

```html
<a href="https://www.example.com">Visitar exemplo</a>
```

Podemos definir o atributo `target` para determinar como o link deve ser aberto. Os valores mais comuns são `_self`, `_blank` e `_parent`.

## 🏷️ 4. Principais Tags HTML - Parte 2

### Imagens

Podemos inserir imagens usando a tag `<img>`, especificando o caminho da imagem no atributo `src`. O atributo `alt` fornece um texto alternativo para ser exibido caso a imagem não possa ser carregada.

```html
<img src="caminho/para/imagem.jpg" alt="Descrição da Imagem">
```

### Listas

Podemos criar listas não numeradas (unordered) usando a tag `<ul>` e listas numeradas (ordered) usando a tag `<ol>`. Os itens da lista são definidos com a tag `<li>`.

```html
<ul>
    <li>Item 1</li>
    <li>Item 2</li>
</ul>

<ol>
    <li>Item 1</li>
    <li>Item 2</li>
</ol>
```

### Tag de Uso Genérico

A tag `<span>` é usada para agrupar elementos em linha, enquanto a tag `<div>` é usada para agrupar elementos em bloco.

```html
<span>Texto em linha</span>
<div>Texto em bloco</div>
```

## ✒️ 5. Tags de Formatação de Texto

Existem várias tags HTML que permitem formatar o texto em sua página.

- **Negrito**: `<b>` ou `<strong>`
- **Itálico**: `<i>` ou `<em>`
- **Sublinhado**: `<u>`
- **Riscado**: `<s>`
- **Texto Marcado**: `<mark>`
- **Texto Pré-formatado**: `<pre>`
- **Código**: `<code>`
- **Citação**: `<cite>` ou `<blockquote>`
- **Subscrito**: `<sup>` (em cima)
- **Sobrescrito**: `<sub>` (em baixo)

## 🌐 6. Elementos Semânticos

HTML5 introduziu uma série de elementos semânticos que ajudam a estruturar o conteúdo da página de forma mais significativa. Alguns desses elementos são:

- `<header>`: Define o cabeçalho da página ou de uma seção.
- `<main>`: Define o conteúdo principal da página.
- `<aside>`: Define um conteúdo lateral, como uma barra lateral ou assunto não relacionado ao conteúdo.
- `<footer>`: Define o rodapé da página ou de uma seção.
- `<section>`: Define uma seção dentro de um documento.
- `<article>`: Define um conteúdo independente e autossuficiente.
- `<figure>`: Define uma figura ilustrativa para o conteúdo.
- `<nav>`: Define uma seção de navegação.

## 🚀 7. Construindo uma Barra de Navegação

Podemos criar uma barra de navegação usando a tag `<nav>`, juntamente com uma imagem e uma lista de links.

```html
<nav>
    <img src="caminho/para/logo.png" alt="Logo">
    <ul>
        <li><a href="#">Página Inicial</a></li>
        <li><a href="#">Sobre Nós</a></li>
        <li><a href="#">Serviços</a></li>
    </ul>
</nav>
```

## 📊 8. Tabelas

As tabelas são usadas para exibir dados em formato de linhas e colunas. Elas são construídas utilizando as tags `<table>`, `<thead>`, `<tbody>`, `<tr>`, `<th>` e `<td>`.

```html
<table>
    <thead>
        <tr>
            <th>Primeira Coluna</th>
            <th>Segunda Coluna</th>
            <th>Terceira Coluna</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Dado 1</td>
            <td>Dado 2</td>
            <td>Dado 3</td>
        </tr>
        <tr>
            <td>Dado 1</td>
            <td>Dado 2</td>
            <td>Dado 3</td>
        </tr>
    </tbody>
</table>
```

## 📝 9. Formulários

Os formulários são usados para coletar informações dos usuários. Podemos criar formulários usando a tag `<form>` e adicionar diferentes tipos de campos de entrada, como `<input>`, `<textarea>` e `<select>`.

```html
<form>
    <input type="text" name="nome" placeholder="Nome Completo">
    <input type="email" name="email" placeholder="E-mail">
    <input type="password" name="senha" placeholder="Senha">
    <textarea name="mensagem" placeholder="Digite sua mensagem"></textarea>
    <input type="submit" value="Enviar">
</form>
```

## 💅 10. Integração com CSS

Podemos integrar o CSS em nossas páginas HTML usando as classes e IDs. As classes são usadas para estilizar um ou mais elementos, enquanto os IDs são usados para estilizar um elemento específico.

```html
<div class="destaque">Texto em Destaque</div>
<p id="paragrafo">Um parágrafo com ID</p>
```

No CSS, podemos estilizar os elementos selecionando suas classes e IDs correspondentes.

```css
.destaque {
    color: red;
}

#paragrafo {
    font-size: 16px;
}
```

Espero que este guia introdutório ao HTML e aos elementos mais básicos seja útil para você começar a criar suas próprias páginas web. Continue explorando e aprimorando suas habilidades em HTML e Front-End! 😊✨