# Units & Sizes
Conceitos de Unidades e Tamanhos em CSS.

>https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Values_and_units

## Numbers, lenghts and percentages
- *integer*;
- *number* - may represents decimal number;
- *dimension* - number + unit attached to it;
- *percentage* - relative to another quantity.

## Units
-  ``px`` - pixels na tela;
-  `%` - porcentagem referente ao tamanaho do elemento;
- ``rem`` - referente ao elemento root (raiz - html); elemento definido como padrão pelo navegador (1rem - 1x elemento raiz; 2rem - 2x elemento raiz);
- ``em`` - referente ao elemento pai;
- ``ch`` - media em caracteres;
- ``vh`` e ``vw `` - view height e view width (0-100);   

```css
h1{
	border: 2px dashed red;
	width: 50%;
	font-size: 3rem; //"3x o root"
	padding: 1em; //"1x o elemento font-size"
}
```