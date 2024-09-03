# Trabalho FlexBox 
<div align="center">
<img src="https://github.com/user-attachments/assets/5a7d2c71-cbfb-44c7-bfa1-cf1665900bee" width="1000px">
</div>
<h1 align="center">Explicando o Flexbox do CSS</h1>
<p align="center"> Projeto para explicar o flexbox. Cada propriedade, como funciona e como usar.</p>

## Flex Container
<img style="float: left" src="https://github.com/user-attachments/assets/c8566934-388d-4e10-bba6-50307963cfc2" width="500px">

São os elementos filhos de um Flex Container . se colocar display: flex; em um contêiner, todos os elementos  dentro dele se tornam Flex Items.

```css
.flex-container {
           display: flex; /* Define o contêiner como flexível */
            flex-direction: row; /* Eixo principal é horizontal */
            justify-content: space-between; /* Espaço igual entre os itens */
            align-items: center; /* Itens alinhados ao centro verticalmente */
            height: 100px;
            background-color: lightgray;
        }
```



### flex-direction
Ele serve como uma direção dos itens dentro do flex container. por padrão ele é row (linha) por isso quando o display: flex; é adicionado, os elementos ficam em linha, um do lado do outro.
Para estilos medias queries mobile geralmente usa column , para que o conteúdo seja mostrado em uma única coluna.
Tipos 
row (padrão):
Os itens são dispostos em uma linha horizontal, da esquerda para a direita (em linguagens de escrita de esquerda para a direita).
O eixo principal é horizontal, e o eixo cruzado é vertical.

row-reverse:
Os itens são dispostos em uma linha horizontal, mas da direita para a esquerda.
O eixo principal continua sendo horizontal, mas os itens são invertidos.

column:
Os itens são dispostos em uma coluna vertical, de cima para baixo.
O eixo principal é vertical, e o eixo cruzado é horizontal.

column-reverse:
Os itens são dispostos em uma coluna vertical, mas de baixo para cima.
O eixo principal continua sendo vertical, mas os itens são invertidos.

<img  src="https://github.com/user-attachments/assets/cb339389-679c-4d04-ad17-176d20e170be" width="500px">

[ Código... ](Projetos/flex-cont.css)


### justify-content
justify-content
no Flexbox controla como os itens flexíveis são alinhados ao longo do eixo principal do contêiner.A propriedade só funciona se os itens atuais não ocuparem todo o container, ou seja , ao definir um flex 1 : ela não tera mais função . Tipos  : 
Se flex-direction for row ou row-reverse, o eixo principal é horizontal.
Se flex-direction for column ou column-reverse, o eixo principal é vertical.
Valores :

justify-content: flex-start;  Alinha os itens ao início do container. 

justify-content: flex-end; Alinha os itens ao final do container 

justify-content: center; Alinha os itens ao centro do container.

justify-content: space-between; Cria um espaçamento igual entre os elementos. Mantendo o primeiro grudado no início e o último no final. 

justify-content: space-around; Cria um espaçamento entre os elementos. Os espaçamentos do meio são duas vezes maiores que o inicial e final. 

<img src="https://github.com/user-attachments/assets/0bb6565b-ed41-4935-9442-5c76f63745a6" width="500px">

[ Código... ](Projetos/style.css)

### align-items
align-items
Pelo próprio nome ele alinha itens de acordo com o eixo cruzado  do container , ela permite alinhamento central no eixo vertical.

 Valor padrão, ele que faz com que os flex itens cresçam igualmente.

Alinha os itens ao início.
align-items: flex-start;


 Alinha os itens ao final.
align-items: flex-end;



Alinha os itens ao centro.
align-items: center;

<img  src="https://github.com/user-attachments/assets/cb099ff7-c4ac-4c38-b519-1c5890eb48e4" width="500px">

[ Código... ](Projetos/style2.css)

### align-content
é usada para controlar o alinhamento das linhas em um contêiner flexível quando há espaço extra no eixo cruzado , só vai ser usada quando temos varias linha de itens, quando são mais de uma linha usa o flex-wrap , tipos :
flex-start:As linhas são agrupadas no início do contêiner (ao topo, se o eixo cruzado for vertical).

flex-end:
As linhas são agrupadas no final do contêiner (à base, se o eixo cruzado for vertical).

center:
As linhas são centralizadas ao longo do eixo cruzado.

space-between:
As linhas são distribuídas uniformemente, com a primeira linha no início do contêiner e a última linha no final.

space-around:
As linhas são distribuídas com espaço igual ao redor de cada linha.

space-evenly:
As linhas são distribuídas com espaço igual entre elas e as bordas do contêiner.

stretch (padrão):
As linhas são esticadas para preencher todo o espaço disponível ao longo do eixo cruzado.


<img  src="https://github.com/user-attachments/assets/c39d49ae-b820-47b1-9a55-f92a1fb6c028" width="500px">

[ Código... ](Projetos/style3.css)

### gap,row-gap,column-gap


## Flex Items 
São os elementos filhos de um Flex Container . se colocar display: flex; em um contêiner, todos os elementos  dentro dele se tornam Flex Items.

<img  src="https://github.com/user-attachments/assets/51b5824e-24dc-4c59-9ffe-8ebdd70003bc" width="500px">

```css
.flex-container {
  display: flex; /* Transforma o contêiner em um Flex Container */
}

.item {
  background-color: lightblue;
  padding: 20px;
  margin: 10px;
  text-align: center;
}
```
O item possui suas propriedades como Oder , Flex-grow, Flex-shrink, Flex-basis, Align-self

### order





