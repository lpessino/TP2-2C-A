### Suma de array simple
Considere un array de enteros, encontrar la suma de los elementos. 

Por ejemplo si el array ar = [1,2,3] 
1 + 2 + 3 = 6 

retorna 6.

arr1 = [1,2,5,7,20,44,80,92,69];

function sumarArray(array){
    let i = 0;
    let suma = 0;
    while(i < array.length){
        suma = suma + array[i];
        i++;
    } 
    
    return suma;
}

let total = sumarArray(arr1);

console.log(total);