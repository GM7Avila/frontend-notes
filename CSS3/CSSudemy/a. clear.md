# Clear 

← [[a. float]] 

## 🏷️ Tags
#css #webdev #boxmodel

## Funcionamento
- Limpar fluxo flutuante

A função clear "limpa" os objetos flutuantes de sua região. Note que no primeiro exemplo, não há a função clear na classe do texto lorem (fora dos conteúdos), já no exemplo dois, com a função clear, o texto 2 não fica na mesma região que os objetos flutuantes.

- Exemplo 1
```CSS
.contents{

    background: rgb(133, 133, 219);
    border: 1px solid rgb(216, 216, 57);

    width: 200px;
    height: 200px;
    margin: 10px;

    float: left;
}
```

```html
<body>


    <div class ="contents1"> Contents 1 </div>

    <div class="contents"> Contents 2 </div>

    <div class="contents"> Contents 3 </div>

    <div class="contents"> Contents 4 </div>

    <div class="contents"> Contents 5 </div>

    <div class="contents"> 
		Contents 6
	    Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquam ea odio 
		neque vitae veniam? Optio quod vero officia unde qui, rem quos molestiae 
		velit quam veritatis, asperiores inventore? Consectetur, cumque.
    </div>	

Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquam ea odio neque vitae veniam? Optio quod vero officia unde qui, rem quos molestiae velit quam veritatis, asperiores inventore? Consectetur, cumque.Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquam ea odio neque vitae veniam? Optio quod vero officia unde qui, rem quos molestiae velit quam veritatis, asperiores inventore? Consectetur, cumque.

</body>

```

![[clear_img001.png]]

- Exemplo 2
``` CSS
.contents{

    background: rgb(133, 133, 219);
    border: 1px solid rgb(216, 216, 57);

    width: 200px;
    height: 200px;
    margin: 10px;

    float: left;
}

  

.clear {
    clear: both;
}


```
utlização da ==class clear==
```HTML
<body>


    <div class ="contents1"> Contents 1 </div>

    <div class="contents"> Contents 2 </div>

    <div class="contents"> Contents 3 </div>

    <div class="contents"> Contents 4 </div>

    <div class="contents"> Contents 5 </div>

    <div class="contents"> 
		Contents 6
	    Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquam ea odio 
		neque vitae veniam? Optio quod vero officia unde qui, rem quos molestiae 
		velit quam veritatis, asperiores inventore? Consectetur, cumque.
    </div>



	<div class="clear">

Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquam ea odio neque vitae veniam? Optio quod vero officia unde qui, rem quos molestiae velit quam veritatis, asperiores inventore? Consectetur, cumque.Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquam ea odio neque vitae veniam? Optio quod vero officia unde qui, rem quos molestiae velit quam veritatis, asperiores inventore? Consectetur, cumque.

    </div>

  

</body>
```

![[clear_img02.png]]

-------
