#### 1°Lista de exercícios - js ###

# Desafio 1
# Alice e Bob criaram um problema cada para o HackerRank. Um revisor avalia os dois desafios, atribuindo pontos em uma escala de 1 a 100 para três categorias: clareza do problema , originalidade e dificuldade .
# A classificação para o desafio de Alice é o tripleto a = (a[0], a[1], a[2]) , e a classificação para o desafio de Bob é o tripleto b = (b[0], b[1], b[2]) .
# A tarefa é calcular seus pontos de comparação comparando cada categoria:
# Se a[i] > b[i] , então Alice ganha 1 ponto.
# Se a[i] < b[i] , então Bob ganha 1 ponto.
# Se a[i] = b[i] , então nenhuma das pessoas recebe um ponto.
# FUNÇÃO:
function compareTriplets(a, b) {
 let alice = 0;
 let bob = 0;
    
    for(let i = 0; i < a.length; i++){
        if(a[i]> b[i]){
            alice++;
        }else if(a[i]< b[i]){
            bob++;
        }
}
    return [alice, bob];
}

# Desafio 2
# Neste desafio, você precisa calcular e imprimir a soma dos elementos de um array, considerando que alguns números inteiros podem ser muito grandes.
# Função:
function aVeryBigSum(ar) {
    // Write your code here
    let soma = 0;
    for(let i = 0; i <ar.length; i++){
        soma = soma + ar[i];
    }
    return soma;
}

# Desafio 3
# Dado um conjunto de inteiros, calcule as proporções de seus elementos que são,, e. Imprima o valor decimal de cada fração em uma nova linha com 6 casas decimais.
# Função: 
function plusMinus(arr) {
    // Write your code here
    let positivos = 0;
    let negativos = 0;
    let zeros = 0;
  
    
    for(let i = 0; i < arr.length; i++){
        if(arr[i] > 0 ){
            positivos++;
        }else if(arr[i] < 0 ){
            negativos++;
        }else{
            zeros++;
        }
    }
    let calc1 = (positivos / arr.length).toFixed(6);
    let calc2 = (negativos / arr.length).toFixed(6);
    let calc3 = (zeros / arr.length).toFixed(6);

    console.log(calc1);
    console.log(calc2);
    console.log(calc3);
}

# Desafio 4
# Dado um conjunto de inteiros, calcule as proporções de seus elementos que são,, e. Imprima o valor decimal de cada fração em uma nova linha com 6 casas decimais.
# Função:
function plusMinus(arr) {
    // Write your code here
    let positivos = 0;
    let negativos = 0;
    let zeros = 0;
  
    
    for(let i = 0; i < arr.length; i++){
        if(arr[i] > 0 ){
            positivos++;
        }else if(arr[i] < 0 ){
            negativos++;
        }else{
            zeros++;
        }
    }
    let calc1 = (positivos / arr.length).toFixed(6);
    let calc2 = (negativos / arr.length).toFixed(6);
    let calc3 = (zeros / arr.length).toFixed(6);

    console.log(calc1);
    console.log(calc2);
    console.log(calc3);
}

# Desafio 5
# Dados cinco inteiros positivos, encontre os valores mínimo e máximo que podem ser calculados somando exatamente quatro dos cinco inteiros. Em seguida, imprima os respectivos valores mínimo e máximo como uma única linha de dois inteiros longos separados por espaços.
# Função: 
function miniMaxSum(arr) {
    // Write your code here
    let maior = arr[0];
    let menor = arr[0];
    let somaT = 0;
    
    for(let i = 0; i< arr.length; i++){
        if(arr[i] < menor){
            menor = arr[i];
        }else if(arr[i] > maior){
            maior = arr[i];
        }
     somaT = somaT + arr[i]; 
    }
    let conta1 = somaT - maior;
    let conta2 = somaT - menor;
    console.log(`${conta1} ${conta2}`)
}
