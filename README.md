# ESTRUTURA DE DADOS

## 3.1 Introdução

### Estrutura de dados clássicas: maneira como a informação é armazenada.
<ul>
  <li>Pilhas;</li>
  <li>Filas;</li>
  <li>Listas.</li>
</ul>

### Estruturas de dados de busca e classificação: para classificar e organizar a recuperação da informação.
<ul>
  <li>Algoritmos de ordenação.</li>
</ul>

## 3.2	Pilhas I

O vetor (ou array) é uma variável que permite uma série de valores por vez;
<ul>
  <li>Serve para empilhar dados: é como um armário em que você coloca várias caixinhas. Para encontrar algo, você se refere ao armário e à prateleira.</li>
</ul>

Pilha está relacionado a empilhar valores. 
<ul>
  <li>Para empilhar você coloca em uma ordem e para retirar um dado, você faz a ordem inversa.</li>
  <li>A estrutura é vista de cima para baixo e você enxerga apenas o que está no topo.</li>
</ul>

Exemplo: você tem uma loja de material de construção. O preço da areia estava R$ 10/m³, porém veio um último caminhão trazendo 2 m³ e cobrou R$ 12/m³. O comerciante vai calcular o preço baseado no último lote que chegou para não ter prejuízo e depois pode retornar a vender pelo preço antigo. 

Existem regras para como inserir valores dentro da estrutura.
<ul>
  <li>Push (empurrar): inserir elementos; Ex: 3 2 4 1</li> 
  <li>Pop: retirar elementos; Ex: 1 4 2 3</li>
</ul>


## 3.3	Pilhas II

Exemplo prático:
<ul>
  <li>Abrir o VS Code</li>
  <li>Criar um arquivo “pilha.js”</li>
</ul>
  
<p>var elementos = [];</p>
<p>var topo = -1;</p>
<p>const max = 10;</p>
<br>
<p>function push(num) {</p>
	<p>if (topo < max) {</p>
		<p>topo = topo + 1;</p>
		<p>elementos[topo] = num;</p>
<p>} else {</p>
	<p>console.log(“Pilha está cheia.”);</p>
<p>}</p>
<p>}</p>
<br>
<p>function pop(num) {</p>
	<p>if (topo != -1) {</p>
		<p>let num = elementos[topo];</p>
		<p>topo = topo – 1;</p>
		<p>return num;</p>
<p>} else {</p>
	<p>console.log(“Pilha está vazia.”);</p>
<p>}</p>
<p>}</p>
<br>
<p>function estaVazia() {</p>
<p>return topo === -1;</p>
<p>}</p>
<br>
// para inserir elementos na pilha

push(10);</p>
push(20);</p>
push(30);</p>

<br>
// para visualizar como ficou o Array
<br>
console.log(elementos);
<br>
// para retirar elementos da pilha
<br>
console.log(pop());
<br>
console.log(pop());
<br>
console.log(pop());
<br>
<p>//usando como exemplo o número 10</p>
<p>var numDecimal = 10;</p>
<p>var resto;</p>
<br>
<p>console.log(“Hora de empilhar!!”);</p>
<p>while (numDecimal != 0) {</p>
	<p>resto = parseInt(numDecimal % 2);</p>
	<p>push(resto);</p>
	<p>numDecimal = parseInt(numDecimal / 2);</p>
<p>}</p>
<br>
<p>console.log(“Desempilhando tudo...”);</p>
<p>while (!estaVazia()){</p>
	<p>console.log(pop());</p>
<p>}</p>


## 3.4	Filas e Listas


## 3.5	Busca I


## 3.6	Busca II


## 3.7	Algoritimos de Ordenação I


## 3.8	Algoritimos de Ordenação II


