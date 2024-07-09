### Exercice 1 : Afficher un message
Créez un programme qui demande à l'utilisateur de saisir son nom et affiche un message de salutation.

#### Exigences :
1. Le programme demande à l'utilisateur de saisir son nom.
2. Le programme affiche un message de salutation avec le nom saisi.

#### Exemple :
```
Entrez votre nom: Alice
Bonjour, Alice !
```

### Solution :

```javascript
const readline = require('readline');

const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout
});

rl.question('Entrez votre nom: ', (name) => {
  console.log(`Bonjour, ${name} !`);
  rl.close();
});
```