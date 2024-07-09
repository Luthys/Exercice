### Exercice 3 : Vérifier la parité d'un nombre
Créez un programme qui demande à l'utilisateur de saisir un nombre et vérifie s'il est pair ou impair.

#### Exigences :
1. Le programme demande à l'utilisateur de saisir un nombre.
2. Le programme vérifie et affiche si le nombre est pair ou impair.

#### Exemple :
```
Entrez un nombre: 4
Le nombre 4 est pair.

Entrez un nombre: 7
Le nombre 7 est impair.
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
    if (num % 2 === 0) {
      console.log(`Le nombre ${num} est pair.`);
    } else {
      console.log(`Le nombre ${num} est impair.`);
    }
  }

  rl.close();
});
```