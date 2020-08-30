### Problema
John trabaja en una tienda de medias. Tiene una larga pila de medias que tiene que aparear por color. Dado un array de numeros enteros que representan el color de cada media, determine cuantos pares de medias (segun color) hay.

#### Ejemplo
> #### Ejemplo de entrada
> 9
> 
>  [10, 20, 20, 20, 20, 30, 50, 10, 20]

> #### Ejemplo de salida
> 3

![](https://s3.amazonaws.com/hr-challenge-images/25168/1474122392-c7b9097430-sock.png)


let arr1 =  [10, 20, 20, 20, 20, 30, 50, 10, 20];

function countPairs(array){
    let count = 0;
    for (let i = 0; i < array.length-1; i++) {
        if(array[i] === array[i+1]){
            count++;
        }
        
    }
    return count;
}

console.log(countPairs(arr1));