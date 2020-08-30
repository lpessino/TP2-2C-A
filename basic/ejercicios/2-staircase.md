Formar una escalera de caracteres #. 

Por ejemplo considere una escalera de tamaño n=6
Se formará la siguiente forma:

\      #

\     ##

\    ###

\   ####

\  #####

\ ######

function escalera(n){
    let char = "#";
    let space = " ";
    let charAmount = 0;
    let spaceAmount = n;

    
    while(charAmount != n){
        console.log(space.repeat(spaceAmount) + char.repeat(charAmount));
        charAmount++;
        spaceAmount--;
    }
}

let repeat = 6;
escalera(repeat);
