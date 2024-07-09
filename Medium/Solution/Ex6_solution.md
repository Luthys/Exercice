### Exercice 6 : Calculer la somme des chiffres
Créez un programme qui demande à l'utilisateur de saisir un nombre et calcule la somme de ses chiffres.

#### Exigences :
1. Le programme demande à l'utilisateur de saisir un nombre.
2. Le programme calcule et affiche la somme des chiffres du nombre.

#### Exemple :
```
Entrez un nombre: 1234
La somme des chiffres de 1234 est 10.
```

### Solution :

```javascript
const readline = require('readline');

const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout
});

rl.question('Entrez un nombre: ', (num) => {
  num = parseInt(num);

  if (isNaN(num)) {
    console.log('Veuillez entrer un nombre valide.');
  } else {
    let sum = 0;
    while (num > 0) {
      sum += num % 10;
      num = Math.floor(num / 10);
    }
    console.log(`La somme des chiffres est ${sum}.`);
  }

  rl.close();
});
```