# Atividade-5-LP

// Função que retorna os valores maiores que a média
function valoresMaioresQueMedia(lista) {
    const media = calcularMedia(lista);
    return lista.filter(num => num > media);
}

// Função auxiliar para calcular a média dos valores na lista
function calcularMedia(lista) {
    const soma = lista.reduce((acc, num) => acc + num, 0);
    return soma / lista.length;
}

// Função que retorna o menor valor da lista
function menorValor(lista) {
    return Math.min(...lista);
}

// Função que retorna a soma dos itens da lista
function somaDosItens(lista) {
    return lista.reduce((acc, num) => acc + num, 0);
}

// Função que retorna os valores menores que 20
function valoresMenoresQueVinte(lista) {
    return lista.filter(num => num < 20);
}

// Função que retorna o primeiro e o último valor da lista
function primeiroEUltimoValor(lista) {
    const primeiro = lista[0];
    const ultimo = lista[lista.length - 1];
    return [primeiro, ultimo];
}

const lista = [64,498,89,3123,45,2,89,33,1,100,5];
