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
<br>O modelo da pilha é <strong>last in, first out (o último que entra é o primeiro que sai)</strong>.
<br>

## 3.3	Pilhas II

Exemplo prático:
<ul>
  <li>Abrir o VS Code</li>
  <li>Criar um arquivo “pilha.js”</li>
</ul>
var elementos = [];
<br>var topo = -1;
<br>const max = 10;
<br>
<br>function push(num) {
	<br>if (topo < max) {
		<br>topo = topo + 1;
		<br>elementos[topo] = num;
<br>} else {
	<br>console.log(“Pilha está cheia.”);
<br>}
<br>}
<br>
<br>function pop(num) {
	<br>if (topo != -1) {
		<br>let num = elementos[topo];
		<br>topo = topo – 1;
		<br>return num;
<br>} else {
	<br>console.log(“Pilha está vazia.”);
<br>}
<br>}
<br>
<br>function estaVazia() {
<br>return topo === -1;
<br>}
<br>
<br>// para inserir elementos na pilha
<br>push(10);
<br>push(20);
<br>push(30);
<br>
<br>// para visualizar como ficou o Array
<br>
console.log(elementos);
<br>
<br>// para retirar elementos da pilha
<br>console.log(pop());
<br>console.log(pop());
<br>console.log(pop());
<br>
<br>//usando como exemplo o número 10
<br>var numDecimal = 10;
<br>var resto;
<br>
<br>console.log(“Hora de empilhar!!”);
<br>while (numDecimal != 0) {
	<br>resto = parseInt(numDecimal % 2);
	<br>push(resto);
	<br>numDecimal = parseInt(numDecimal / 2);
<br>}
<br>
<br>console.log(“Desempilhando tudo...”);
<br>while (!estaVazia()){
	<br>console.log(pop());
<br>}
<br>

## 3.4	Filas e Listas

### Filas
Para nós é um modelo bastante intuitivo, pois podemos pensar na fila do banco, fila de prioridade no aeroporto, fila da padaria. 
<br>
<br>O modelo da fila é <strong>first in, first out (o primeiro que entra é o primeiro que sai)</strong>:
<ul>
	<li>o próximo elemento a entrar: vai entrar na última posição;</li>
	<li>o próximo elemento a sair: vai ser o que está na primeira posição.</li>
</ul>
Ex: você atende a fila normal depois que tiver atendido a fila prioritária.
<br>
<br>Para as pilhas e filas, em geral, se trabalha no modelo de vetor com tamanhos limitados (capacidade máxima) para facilitar a implementação.

### Listas

As listas são conceitos para valores que são armazenados em conjuntos de tamanho “infinito”. Você pode ocupar o quanto tiver de memória e não o valor máximo que pré-estipulou. 
<br>
<br>Ex: ordem alfabética, ordem crescente, ordem decrescente.

## 3.5	Busca I

A busca de elementos é feita por meio dos conjuntos;
<br>
<br>Busca sequencial:
<ul>
	<li>A partir de um determinado conjunto de valores, quero encontrar em que posição está um valor específico;</li>
	<li>Se não encontrar o valor, retornar um valor inválido;</li>
</ul>
Exemplo:
<br> var valores = [5, 8, 10, 22, 45, 38];
<br> 
<br> function busca(num) {
<br> 	for (i = 0; i < 6; i++) {
<br> 		if (num == valores[i]) {
<br> 			return i;
<br> 		}
<br> 	}
<br> 	return -1;
<br> }
<br> 
<br> console.log(busca(10));
<br> console.log(busca(50));

## 3.6	Busca II


## 3.7	Algoritimos de Ordenação I


## 3.8	Algoritimos de Ordenação II


