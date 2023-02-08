# Flex Itens ✨
← [[b. flex-container]]

## 🏷️ Tags 
#css #webdev #flex-box
#flex-itens


## Propriedades de Itens
Utilizando como exemplo o seguinte código HTML:
``` HTML
<body>
    <section class="container">
    
        <article class="item article-01">
            Article 01
        </article>

        <article class="item article-02">
            Article 02
        </article>
        
        <article class="item article-03">
            Article 03
        </article>
        
        <article class="item article-04">
            Article 04
        </article>
        
    </section>
</body>
```

### Order
Alterar a ordem dos itens #order

```CSS
.article-01 {order: 3;}
.article-02 {order: 1;}
.article-03 {order: 2;}
.article-04 {order: 4;}
```

### Align-self
Alinha o próprio item no display flex utilizando #align-self
Valor padrão: `auto` 
- `auto` respeita o que foi definido no `align-itens` do #container 
- `center` alinha no centro (seguindo a flex-direction)
- `flex-start` alinha no topo/início (seguindo a flex-direction)
- `flex-end` alinha em baixo/final (seguindo a flex-direction)
- `base-line` 
- `stretch` esticado

```CSS
.container{
    background-color: #ccc;
    height: 500px;

    display: flex;

    flex-flow: row wrap; /*1*/
    justify-content: flex-start; /*2*/
    align-items: stretch; /*3*/
    align-content: stretch; /*4*/
}

.item{
    background-color: #333;
    color: #fff;

    padding: 20px;
    margin: 5px;

    width: 30px;
    height: 30px;
}


.article-01 {order: 3;}

.article-02 {order: 1; align-self: center;}

.article-03 {order:2;}

.article-04 {order:4;}
```

![[flex_img06.png]]

No exemplo acima, o item article-02 (de ordem 1) é alinhado através de `align-self` seguindo sua base estrutural` flex-direction: row` (contido em `flex-flow: row wrap;`).

### Flex-grow 
- Valor padrão de #flex-grow: `flex-grow: 0` - uniformidade da largura de colunas
- Valor: `0` todos os itens possuem larguras próprias/diferentes;
- Valor: `1` todos os itens possuem a mesma largura;
- Valor: `x` vezes a mais do `flex-grow` geral utilizado pelos outros itens;

```CSS
.container{

    background-color: #ccc;
    height: 500px;

    display: flex;

    flex-flow: row wrap;
    justify-content: flex-start;
    align-items: stretch;
    align-content: stretch;

}
.item{

    background-color: #333;
    color: #fff;

    padding: 20px;
    margin: 5px;

    height: 30px;

    flex-grow: 1; /*width igual para todos*/

}

.article-03 {flex-grow: 4;} /*4 vezes o tamanho dos itens pertencentes ao flex grow ja definido*/ 


```

Resultado:
![[float_img09.png]]

### Flex-shrik 
- Utilize o #flex-shrik para redução de largura, inverso do flex-grow.

### Flex-basis 
- O #flex-basis determina a ==largura inicial== dos itens; por exemplo: `flex-basis: 20px` determina que o item terá a largura da coluna inicial de 20px;

### Flex 
- União de #flex grow, flew-shrik, flex-basis

---

→ [[b. header responsivo]]

qUANDO A PESSOA CORTA E NÃO PARA DE SANGRAR DA [[hemofilia]] 