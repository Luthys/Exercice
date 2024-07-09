### Exercice 2 : Addition de deux nombres
Créez un programme qui demande à l'utilisateur de saisir deux nombres et affiche leur somme.

#### Exigences :
1. Le programme demande à l'utilisateur de saisir deux nombres.
2. Le programme calcule et affiche la somme des deux nombres.

#### Exemple :
```
Entrez le premier nombre: 3
Entrez le deuxième nombre: 5
La somme de 3 et 5 est 8.
```

### Solution :

```javascript
const readline = require('readline');

const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout
});

rl.question('Entrez le premier nombre: ', (num1) => {
  rl.question('Entrez le deuxième nombre: ', (num2) => {
    const sum = parseFloat(num1) + parseFloat(num2);
    console.log(`La somme de ${num1} et ${num2} est ${sum}.`);
    rl.close();
  });
});
```