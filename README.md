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
  
var elementos = [];
var topo = -1;
const max = 10;

function push(num) {
	if (topo < max) {
		topo = topo + 1;
		elementos[topo] = num;
} else {
	console.log(“Pilha está cheia.”);
}
}

function pop(num) {
	if (topo != -1) {
		let num = elementos[topo];
		topo = topo – 1;
		return num;
} else {
	console.log(“Pilha está vazia.”);
}
}

function estaVazia() {
return topo === -1;
}

// para inserir elementos na pilha
push(10);
push(20);
push(30);

// para visualizar como ficou o Array
console.log(elementos);

// para retirar elementos da pilha
console.log(pop());
console.log(pop());
console.log(pop());

//usando como exemplo o número 10
var numDecimal = 10;
var resto;

console.log(“Hora de empilhar!!”);
while (numDecimal != 0) {
	resto = parseInt(numDecimal % 2);
	push(resto);
	numDecimal = parseInt(numDecimal / 2);
}

console.log(“Desempilhando tudo...”);
while (!estaVazia()){
	console.log(pop());
}


## 3.4	Filas e Listas


## 3.5	Busca I


## 3.6	Busca II


## 3.7	Algoritimos de Ordenação I


## 3.8	Algoritimos de Ordenação II


