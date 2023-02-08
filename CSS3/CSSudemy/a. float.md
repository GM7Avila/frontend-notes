# Float

← [[a. boxmodel]]

## 🏷️ Tags
#css #webdev  #elementos_flutuantes #boxmodel

## Elemento float
O #float_css é usado para tornar um objeto flutuante, sendo possível 

*Os exemplos usam o código html anterior, com o incremento de um terceiro contentes.*

```CSS 

.contents{

    background: blue;

    border: 1px solid rgb(216, 216, 57);

    width: 200px;

    height: 200px;

    margin-bottom: 10px;

}

  

.contents1{

    background: red;

    border: 1px solid rgb(216, 216, 57);

    width: 150px;

    height: 150px;
    


    float: left

  

}

```

O objeto Contents 1 fica em um fluxo diferente, que chamamos de ==fluxo flutuante== de forma flutuante e a esquerda da página, como indicado no código acima.

![[float_img01.png]]

Caso os 3 contents tivessem a propriedade `float: left`  , os blocos ficariam um ao lado do outro, e não ocupariam o mesmo espaço.
![[float_img04.png]]

Opções para valores em float:
![[float_img02.png]]

note o exemplo de `float: right` , o contents 1 não influencia o comportamento dos outros contents, pois ele está flutuando, e à direita.
![[float_img03.png]]

caso todos possuam a propriedade `float: right` eles também ficaram um ao lado do outro, sem ocupar o mesmo espaço.
![[float_img05.png]]

tirando a propriedade `float` de contents 1, os elementos continuam flutuando, e ocupam todo o espaço á direita.
![[float_img06.png]]

→ [[a. clear]]
