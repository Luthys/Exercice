### Exercice 1 : Afficher les nombres pairs de 1 à 20
Créez un programme qui affiche tous les nombres pairs de 1 à 20.

#### Exemple de sortie :
```
2
4
6
8
10
12
14
16
18
20
```

#### Solution :

```javascript
for (let i = 1; i <= 20; i++) {
  if (i % 2 === 0) {
    console.log(i);
  }
}
```