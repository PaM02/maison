la fonction suivante extraire les categires dan le tableaux
    const categories = plantList.reduce(
        (acc, plant) =>
            acc.includes(plant.category) ? acc : acc.concat(plant.category),
        []
    )
***************************************
avant ça le fonctionnement de reduce
const array1 = [1, 2, 3, 4];

// 0 + 1 + 2 + 3 + 4
const initialValue = 0;
const sumWithInitial = array1.reduce(
  (previousValue, currentValue) =>previousValue + currentValue ,
  initialValue
);

console.log(sumWithInitial);
// expected output: 10    
***********************************
syntaxe
arr.reduce(callback)
arr.reduce(callback, valeurInitiale)

explication ans ce lien
https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce

*********************************
const array1 = [1, 2, 3];

console.log(array1.includes(2));
// expected output: true

const pets = ['cat', 'dog', 'bat'];

console.log(pets.includes('cat'));
// expected output: true

console.log(pets.includes('at'));
// expected output: false
explication sur ce lien
https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/Array/includes

******************************
const array1 = ['a', 'b', 'c'];
const array2 = ['d', 'e', 'f'];
const array3 = array1.concat(array2);

console.log(array3);
// expected output: Array ["a", "b", "c", "d", "e", "f"]

https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/Array/concat