# Flex-container ✨
## 🏷️ Tags
#css #webdev #flex-box
#flex-container #container 
#flex-direction #flex-wrap
#flex-flow #justify-content
#align-itens

https://caniuse.com/flexbox


## Propriedades de Container
Utilização de #container 
`container { display: flex }` 

![[flex_img04.png]]


==Código 001==
```html
<section class="container">


        <article class="item article-01">
            Article 01
        </article>


        <article class="item article-01">
            Article 02
        </article>


        <article class="item article-01">
            Article 03
        </article>


</section>
```

### Flex-Direction 
1) definindo #container como flex: ``display: flex`` 
2) por padrão todos os elementos possuem ``flex-direction: row`` 
``flex-direction`` pode assumir:
- row
- collumn
- row-reverse / collumn-reverse

![[flex_img03.png]]

### Flex-wrap
1) define se os items possuem quebra de linha ou não (wordwrap)
2) por padrão todos os elementos possuem ``flex-wrap: nowrap;`` 

Exemplo
- Fazer com que os blocos do ==Código 001== ocupem 50% de width.
```css
.container{
	flex-wrap: wrap;
}

.item{
	padding:20px;
	margin: 5px;

	width:50%;
}
```

Dessa forma, estamos definindo que cada item ocupara 50% da largura, e que serão orientados por quebra de linhas (flex-wrap). 

![[flex_img01.png]]

### Flex-flow
União do `flex-direction` com o `flex-wrap` 

`flex-flow: row wrap`
*flex-flow: valor do flex diretction - valor do flex wrap*

### Justify-content
1) Alinha os elementos de forma ==horizontal==
2) Valor padrão `justify-content: flex-start;` 
- `flex-start` alinha os elementos horizontalmente da esquerda para a direita
- `flex-end` alinha os elementos horizontalmente da direita para a esquerda
- `center` alinha horizontalmente no centro
- `space-between` alinha horizontalmente os itens, com espaçamento entre eles
- `space-around` espaçamentos iguais entre itens e extremidade

![[flex_img05.png]]

### Align-itens
1) Alinha os elementos de forma ==vertical==
2) Valor padrão ``align-itens: stretch;`` 
- `stretch` define o crescimento vertical uniforme entre os itens.
- `flex-start` alinha os itens no topo (início)
- `flex-end` alinha os itens na base (final)
- `center` alinha os itens no centro da coluna
- `baseline` alinhamento baseado no conteúdo de cada coluna

![[flex_img02.png]]

### Align-content
1) Alinhamento vertical, quandos os itens estiverem em quebra (wrap)
2) Valor padrão ``align-content: stretch
- ``flex-start`` faz o alinhamento dos itens wrap pelo topo
- ``flex-end`` faz o alinhamento dos itens wrap na base
- ``center`` alinhamento ao centro
- ``space-between`` espaçamento entre os itens
- `space-around` entre os itens e extremidades
- `stretch` itens esticados

---
→ [[b. flex-itens]]