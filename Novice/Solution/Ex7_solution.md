### Exercice 7 : Calculer la moyenne des éléments d'un tableau
Créez un programme qui calcule et affiche la moyenne des éléments d'un tableau donné.

#### Exemple de sortie :
```
La moyenne des éléments du tableau est 3.
```

#### Solution :

```javascript
const array = [1, 2, 3, 4, 5];
let sum = 0;

for (let i = 0; i < array.length; i++) {
  sum += array[i];
}

const average = sum / array.length;
console.log(`La moyenne des éléments du tableau est ${average}.`);
```