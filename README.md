# javascript-2
// Fonctions de manipulation de chaînes

 Inverser une chaîne
 
function reverseString(str) {
    return str.split('').reverse().join('');
}

 Compter les caractères
 
function countCharacters(str) {
    return str.length;
}

 Mettre les mots en majuscule
 
function capitalizeWords(sentence) {
    return sentence.split(' ').map(word => word.charAt(0).toUpperCase() + word.slice(1)).join(' ');
}

 Fonctions de tableau

 Rechercher le maximum
 
function findMax(arr) {
    return Math.max(...arr);
}

 Rechercher le minimum
 
function findMin(arr) {
    return Math.min(...arr);
}

Somme d'un tableau

function sumArray(arr) {
    return arr.reduce((sum, num) => sum + num, 0);
}

 Filtrer le tableau
 
function filterArray(arr, conditionFn) {
    return arr.filter(conditionFn);
}

LES FONCTIONS MATHEMATHIQUES.

Factorielle

function factorial(n) {
    if(n < 0) {
       return "la factorielle n'est pas definie pour les nombres negatifs";
       }
    if (n === 0 ) {
        return 0 ;
        }
    let result= 1;
    for (let i = 1; i <= n; i++){
        result *= i;
}
  return result;
  }
  

Vérification des nombres premiers

function isPrime(num) {
    if (num <= 1) return false;
    for (let i = 2; i <= Math.sqrt(num); i++) {
        if (num % i === 0) return false;
    }
    return true;
}

     SUITE DE FIBONACCI
     
function Fibonacci(n) {
    if (n <= 0) {
    return [];
    }
    if (n === 2){ 
    return [0, 1];
    }
    const result = [0, 1];
    for (let i = 2; i < n; i++) {
        result.push(result [i-1 ] + result[i - 2]);
    }
    return result;
}
