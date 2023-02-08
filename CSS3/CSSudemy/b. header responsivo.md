# Header Responsivo
← [[b. flex-itens]]

## 🏷️ Tags 
#css #webdev #flex-box
#responsividade
#header #li #nav #display #first-child #last-child #breakpoint


## Passo a Passo
Primeiro ciramos um **header**, e demos a ele a proprieadede de flex-box: `display: flex;`
Utilizamos `position: absolute` para mante-lo acima da tela (absolute)
`top:` e `left:` `0` para tirar espaçamentos indesejados
`align-itens: center` centralizamos os itens de forma horizontal

```css
header {

	position: absolute; /*por cima do efeito hero*/
	top: 0; /*espaçamento do topo = 0 */
	left: 0; /*espaçamento da esquerda = 0 */

	display: flex;
    justify-content: space-between;
   
	align-items: center;
}
```

```html
<header>

        <a href="#"><img src="/img (3)/logo.png"></a>

        <nav>

            <li><a href="#">Home</a></li>
            <li><a href="#">Sobre</a></li>
            <li><a href="#">Reservas</a></li>
            <li><a href="#">Contato</a></li>

        </nav>

</header>
```

em seguida demos a ``nav`` a característica de `display: flex`, para que possamos trabalhar flex-box dentro de sua div. Com o flexbox ativado, corrigimos a `margin` no topo e nas laterais dos elementos da lista `li`; e em seguida corrigimos a margem à esquerda de "home" e à direita de "contato", utlizando #pseudo-elementos: #last-child e #first-child

```css

header img {
    width: 250px;
}

header nav {
    display: flex;
}

header li {
    margin: 0px 15px;
}

  

/*removendo as margens a esquerda de home e a direita de contato*/

  

header li:first-child{ /*first-child: home*/
    margin-left:0
}

header li:last-child{
    margin-right: 0;
}
```

![[header_responsivo_img01.png]]

Para trabalhar com a responsividade do nosso cabeçalho criaremos #breakpoint, podendo informar a situação condicional para que se realize a nova formatação, da seguinte forma:

```css
@media(max-width: 700px) {
	header{
		flex-direction: collumn;
	}
}
```

Nesse caso, estamos informando que o ==máximo permitido== durante o **redimensionamento** de página, até que seja formatado um novo modelo (responsivo) é de **700px**, para que o header receba a propriedade de  ``flex-drection: collumn;`` 

![[header_responsivo.img02.png]]

A partir de agora podemos determinar qualquer propriedade que será recebida ao atingir os 700px redimensionando a tela do navegador, como: formatar novas margens (por exemplo - dar margem ao logo da nav, dentro do elemento @media), entre outras propriedades que tornam o site responsivo.

---

→ [[b. hero image]]