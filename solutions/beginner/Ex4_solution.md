### Exercice 4 : Inverser un tableau
Créez un programme qui inverse un tableau donné et affiche le tableau inversé.

#### Exemple de sortie :
```
Tableau inversé : [5, 4, 3, 2, 1]
```

#### Solution :

```javascript
const array = [1, 2, 3, 4, 5];
const reversedArray = [];

for (let i = array.length - 1; i >= 0; i--) {
  reversedArray.push(array[i]);
}

console.log('Tableau inversé :', reversedArray);
```