### Exercice 2 : Calculer la somme des nombres de 1 à 100
Créez un programme qui calcule et affiche la somme des nombres de 1 à 100.

#### Exemple de sortie :
```
La somme des nombres de 1 à 100 est 5050.
```

#### Solution :

```javascript
let sum = 0;
for (let i = 1; i <= 100; i++) {
  sum += i;
}
console.log(`La somme des nombres de 1 à 100 est ${sum}.`);
```