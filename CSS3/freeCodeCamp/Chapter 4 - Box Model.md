# Box Model

![[Pasted image 20230208132813.png]]

- Atentar aos estilos padrões (Styles ->"user agent stylesheet")
- Uma box sempre apresentará valores iniciais de margin, border e padding; é necessário utilizar um css reset ``*{}``

- margin: top, right, left, bottom;
- padding: top, right, left, bottom;

## 📦box-sizing
- modifica a maneira de exibir o tamanho de uma box;
- padrão: ``content-box``;

- ``box-sizing: border-box;`` determina o tamanho da box a partir da box (100% -  padding + border);
- não inclui a margem (lado de fora);

- possíveis problemas a se resolverem: text box overflowing (usar propriedade overflow)

para todos os elementos: ``*{ box-sizing: border-box}`` 