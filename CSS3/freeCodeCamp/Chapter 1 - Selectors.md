# Seletor de Elemento
- class selector - existe mais de um;
- ID selector - existe apenas uma vez no documento (menos uso);

## group selectors
```css 
h1, h2 {      // h1 e h2 recebem essa propriedade
	color: blue;
}

p span{      // span dentro de p
	text-transform: uppercase;
	background-color: gold; 
}
```

note que ``p span`` poderia facilmente ser substituido por uma classe com a função de marcador de texto (chamaremos de highlight):
```css
.highlight{
	text-transform: uppercase;
	background-color: gold;
}
```

- *universal selector* : seleciona todos os elementos da página; formatação ``*{}``
```css
*{
	font-size: 22px;
}
```

## ordem de prioridade de selector
```css
p {
	color: purple;
}
p {
	color: red;
}
// a cor do paragrafo sera roxa pois foi inserida primeiro
```

## CSS specificity
> https://specificity.keegan.st/

### inherit
``ìnherit`` faz com que o elemento obtenha o valor computado da propriedade de seu elemento pai. Ele pode ser aplicado a qualquer propriedade CSS, incluindo a propriedade abreviada CSS all.

*Nota*: A herança é sempre do elemento pai na árvore do documento, mesmo quando o elemento pai não é o bloco que o contém.

