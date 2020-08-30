### Problema
Dados 5 enteros positivos, encuentre el minimo y maximo valor que puede ser calculado por sumar exactamente 4 de los 5 enteros. Luego imprima respectivamente el minimo y maximo.

#### Ejemplo

> arr = [1,3,5,7,9]

La suma minima es 1 + 3 + 5 + 7 = 16

La suma maxima es 3 + 5 + 7 + 9 = 24

function sumaMenosUno(array){
    let i = 0;
    let suma = 0;
    while(i < array.length-1){
        suma = suma + array[i];
        i++;
    }

    return suma;
}

let arr1 = [1,3,5,7,9];

arr1.sort(function(a,b){return a-b}); //Ascending order.

console.log("Numero minimo: " + sumaMenosUno(arr1));

arr1.sort(function(a,b){return b-a});

console.log("Numero maximo: " + sumaMenosUno(arr1)); //Descending.