# Javascript
```js
document.write("Texto Aqui");
console.log("Texto Aqui");

const pedidos = [
    {mesa: 10, nome: "Paulo", item: "Pizza"},
    {mesa: 11, nome: "Rafael", item: "X Bacon"},
    {mesa: 12, nome: "João", item: "X tudo"},
    {mesa: 13, nome: "Marcos", item: "Hamburguer"},
]
console.table(pedidos)

```
### Variaveis
```js
var nome_1 = "Paulo Rafael";
document.write(nome_1);
```
### Constantes
```js
const nome_1 = "Paulo Rafael";
document.write(nome_1);
```
### Concatenação
```js
var Nome = "Paulo ";
var Sobrenome = "Rafael";
document.write(Nome + Sobrenome + (1+1));
```
### Alert
```js
window.alert("Ola");
var nome = "Paulo";
window.alert("Ola \n" + nome);
```
### Prompt
```js
var nome = prompt("Nome:")
document.write(nome);
```
### Confirm
```js
var res = confirm("Deseja Sair?")
console.log(res);
```
### If Else
```js
var res = 34;
if(res > 60){
document.write("Maior que 60");
}else if(res > 30){
document.write("Maior que 30");
}else{
document.write("Menor que 30");
}
```

### Switch
```js
var res = 1;
switch(res){
    case 1:
        console.log(1);
        break;
    case 2:
        console.log(2);
        break;
    default:
        console.log("Não");
        break;
}
```
### Input Ranger
```html
<input type="range" min="0" value="20" max="500" id="inputWidth">
<div id="div1" style="height: 100px;background-color: aqua;width: 10px;"></div>

<script>
    var sliderWidth = document.getElementById("inputWidth");
    sliderWidth.oninput = function() {
        div1.innerHTML = this.value;
        div1.style.width = inputWidth.value + 'px';
    }
</script>
```
### For
```js
for(cont=0;cont<10;cont++)
    console.log(cont)

var Nomes = ['Emanuel', 'Ezequiel','Paulo','Rafael'];
for(cont=0;cont<Nomes.length;cont++)
    console.log(Nomes[cont])
```
### While
```js
var num = 0
while(num < 10){
    console.log(num)
    num++;
}
```
### getElementById
```js
document.getElementById('texto').style.width = '100px'

var texto = document.getElementById('texto')
texto.style.width = '100px'
```
### getElementsByTagName
```html
<p>Teste 1</p>
<p>Teste 2</p>
<p>Teste 3</p>
<p>Teste 4</p>
<p>Teste 5</p>

<script>
    var tags = document.getElementsByTagName('p')
    console.log(tags.length)
    console.log(tags[4].innerHTML)
</script>
```
### querySelectorAll
```html
<p>Paulo</p>
<p>Emanuel</p>
<p>Ezequiel</p>
<p>Rafael</p>
<script>
    var p = document.querySelectorAll('p')
    for(cont=0;cont<p.length;cont++)
        console.log(p[cont].innerHTML)
</script>
```
### Editor de Código Online
```html
<style>*{font-family: Arial, Helvetica, sans-serif;}</style>

<pre id="text"></pre>
<textarea id="input" cols="100" rows="10"></textarea>
<h3>Editor de Código Online</h3>
<script>
    var text = document.getElementById('text')
    var input = document.getElementById('input')
    input.oninput = function(){
        text.innerHTML = this.value
    }
</script>
```
### Funções
```js
n1 = 10
n2 = 20
soma(n1,n2)
function soma(n1,n2){
    console.log(n1+n2)
}
```

### addEventListener
```js
var btn = document.getElementById('btn')
        
btn.addEventListener("click",function (){
    alert('teste')
})

btn.addEventListener("click",msg)
        
function msg(){
    alert('teste')
}
```

### addEventListener P2 (keydown)
```js
var div = document.getElementById('div');
document.addEventListener('keydown',function(event){
    var tecla = event.keyCode;
    if(tecla == 37){
        div.style.background = 'green' ;
    }
    else if(tecla == 39){
        div.style.background = 'black' ;
    }
})
```

### Pegando o valor da Tecla Digitada com addEventListener
```js
document.addEventListener('keydown',function(event){
    var tecla = event.keyCode;
    if(tecla == tecla){
        alert(tecla)
    }
})
```

### setInterval(funcao,tempoMili)
```js
var div = document.getElementById('div')
function azul(){
    div.style.background = 'blue'
    console.log(Math.random())
}
setInterval(azul,1000)
```
