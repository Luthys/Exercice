### Exercice 5 : Compter les occurrences d'un élément dans un tableau
Créez un programme qui compte et affiche le nombre d'occurrences d'un élément donné dans un tableau.

#### Exemple de sortie :
```
L'élément 1 apparaît 4 fois dans le tableau.
```

#### Solution :

```javascript
const array = [1, 2, 3, 4, 1, 2, 1, 5, 1];
const element = 1;
let count = 0;

for (let i = 0; i < array.length; i++) {
  if (array[i] === element) {
    count++;
  }
}

console.log(`L'élément ${element} apparaît ${count} fois dans le tableau.`);
```