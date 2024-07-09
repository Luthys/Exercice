### Exercice 6 : Filtrer les nombres pairs d'un tableau
Créez un programme qui filtre et affiche uniquement les nombres pairs d'un tableau donné.

#### Exemple de sortie :
```
Nombres pairs dans le tableau : [2, 4, 6, 8, 10]
```

#### Solution :

```javascript
const array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
const evenNumbers = [];

for (let i = 0; i < array.length; i++) {
  if (array[i] % 2 === 0) {
    evenNumbers.push(array[i]);
  }
}

console.log('Nombres pairs dans le tableau :', evenNumbers);
```