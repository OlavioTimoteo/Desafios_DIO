# Desafios_DIO
Resolução dos desafios do bootcamp HTML Web Developer DIO


\\Desafios de Fundamentos aritméticos//

01 -  Quantidade de Números Positivos

Resolução: 
numero = Array(6);

numero[0] = gets();
numero[1] = gets();
numero[2] = gets();
numero[3] = gets();
numero[4] = gets();
numero[5] = gets();

positivos = numero.filter(value => value > 0);

console.log(positivos.length + " valores positivos");

//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

02 - Exibindo Números Pares

Resolução:
let numero = gets();

let par = 2;

while (par <= numero) {
  
  console.log(par);
  par += 2;

}

//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
03 - Análise de Números

Resolução:
numero = Array(5);

numero[0] = gets();
numero[1] = gets();
numero[2] = gets();
numero[3] = gets();
numero[4] = gets();

pares = numero.filter(value => value % 2 == 0);
impares = numero.filter(value => value % 2 != 0);

positivos = numero.filter(value => value > 0);
negativos = numero.filter(value => value < 0);

console.log(pares.length + " valor(es) par(es)");
console.log(impares.length + " valor(es) impar(es)");

console.log(positivos.length + " valor(es) positivo(s)");
console.log(negativos.length + " valor(es) negativo(s)");

//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
04 - Contagem de Cédulas

Resolução:
let notas = [100, 50, 20, 10, 5, 2, 1];
let nnotas = [0, 0, 0, 0, 0, 0, 0];

let quantia = parseInt(gets());

let resto = quantia;

while (resto >= 1) {
  
  nota = notas.findIndex(value => value <= resto);
  nnotas[nota] = Math.trunc(resto / notas[nota]);
  resto = resto % notas[nota];

}

console.log(quantia);
console.log(nnotas[0] + " nota(s) de R$ 100,00");
console.log(nnotas[1] + " nota(s) de R$ 50,00");
console.log(nnotas[2] + " nota(s) de R$ 20,00");
console.log(nnotas[3] + " nota(s) de R$ 10,00");
console.log(nnotas[4] + " nota(s) de R$ 5,00");
console.log(nnotas[5] + " nota(s) de R$ 2,00");
console.log(nnotas[6] + " nota(s) de R$ 1,00");

//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
05 -Consumo Médio do Automóvel

Resolução:
let X = parseInt(gets());
let Y = parseFloat(gets());

let consumoMedio = parseFloat(X / Y).toFixed(3);

console.log(consumoMedio + " km/l");

//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

Desafios de Problemas Aritméticos

01 - Soma Simples

Resolução:
var A = parseInt(gets());
var B = parseInt(gets());

let soma = (A + B);

console.log("SOMA = " + soma);

//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
\\ Desafios Introdução a Programação//

01 - Dividindo x por y

Resolução:let limit = parseInt(gets());

for (let i = 0; i < limit; i++) {
    
    let line = gets().split(" ");
    let X = parseInt(line[0]);
    let Y = parseInt(line[1]);
    
    if (Y == 0) {
        console.log("divisao impossivel");
    } else {
        let divisao = parseFloat(X / Y).toFixed(1);
        console.log(divisao);
    }
}

//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
02 - Distância

Resolução:
let quilometros = parseInt(gets());
 let minutos = quilometros * 2;  
 
 console.log(minutos + " minutos");

//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
02 - Quanta Mandioca?

Resolução:
let chico = 300 * parseInt(gets());
let bento = 1500 * parseInt(gets());
let bernardo = 600 * parseInt(gets());
let marina = 1000 * parseInt(gets());
let iara = 150 * parseInt(gets());
let marlene = 225;
let total = chico + bento + bernardo + marina + iara + marlene;

console.log(total); 