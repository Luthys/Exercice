### Exercice 3 : Trouver le nombre maximum dans un tableau
Créez un programme qui trouve et affiche le nombre maximum dans un tableau donné.

#### Exemple de sortie :
```
Le nombre maximum dans le tableau est 89.
```

#### Solution :

```javascript
const numbers = [3, 56, 23, 89, 12, 45, 67];
let max = numbers[0];

for (let i = 1; i < numbers.length; i++) {
  if (numbers[i] > max) {
    max = numbers[i];
  }
}

console.log(`Le nombre maximum dans le tableau est ${max}.`);
```