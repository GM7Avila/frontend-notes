# Display

> https://www.w3schools.com/css/css_display_visibility.asp#

## Display block
- Sempre começa em uma nova linha e ocupa toda a largura disponível;
	- ``<div>``
	- ``<h1> - <h6>``
	- ``<p>``
	- ``<form>``
	- ``<header>``
	- ``<footer>``
	- ``<section>``

## Display inline
- Não começa em uma nova linha e ocupa apenas a largura necessária.
	- `<a>`
	- `<img>`
	- `<span>`

## Display none
- Usado com o JS para ocultar e mostrar elementos sem precisar excluí-los ou recriá-los. O `<script>` usa `display: none` como default;

## Display inline-block
- "Bloco embutido";

- A principal diferença para o ``display: inline``, é a possibilidade do ``display inline-block`` permitir a definição de *altura* e *largura* no elemento; além de terem suas margens respeitadas (enquanto no ``display: inline`` não);
- Em comparação ao display: block, a principal diferença é que não há quebra de linha após o elemento;

```html
<body>

<h1>The display Property</h1>

<h2>display: inline</h2>
<div>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum consequat scelerisque elit sit amet consequat. Aliquam erat volutpat. <span class="a">Aliquam</span> <span class="a">venenatis</span> gravida nisl sit amet facilisis. Nullam cursus fermentum velit sed laoreet. </div>

<h2>display: inline-block</h2>
<div>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum consequat scelerisque elit sit amet consequat. Aliquam erat volutpat. <span class="b">Aliquam</span> <span class="b">venenatis</span> gravida nisl sit amet facilisis. Nullam cursus fermentum velit sed laoreet. </div>

<h2>display: block</h2>
<div>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum consequat scelerisque elit sit amet consequat. Aliquam erat volutpat. <span class="c">Aliquam</span> <span class="c">venenatis</span> gravida nisl sit amet facilisis. Nullam cursus fermentum velit sed laoreet. </div>

</body>
```

```css
span.a {  display: inline; /* the default for span */  
  width: 100px;  
  height: 100px;  
  padding: 5px;  
  border: 1px solid blue;  
  background-color: yellow;}  
  
span.b {  display: inline-block;  
  width: 100px;  
  height: 100px;  
  padding: 5px;  
  border: 1px solid blue;  
  background-color: yellow;}  
  
span.c {  display: block;  
  width: 100px;  
  height: 100px;  
  padding: 5px;  
  border: 1px solid blue;  
  background-color: yellow;}
```

> W3: https://www.w3schools.com/css/tryit.asp?filename=trycss_inline-block_span1

![[Pasted image 20230208182403.png]]
