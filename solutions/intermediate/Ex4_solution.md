### Exercice 4 : Compter les voyelles
Créez un programme qui demande à l'utilisateur de saisir une phrase et compte le nombre de voyelles dans la phrase.

#### Exigences :
1. Le programme demande à l'utilisateur de saisir une phrase.
2. Le programme compte et affiche le nombre de voyelles dans la phrase.

#### Exemple :
```
Entrez une phrase: Bonjour tout le monde
Il y a 8 voyelles dans la phrase.
```

### Solution :

```javascript
const readline = require('readline');

const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout
});

rl.question('Entrez une phrase: ', (phrase) => {
  const vowels = 'aeiouAEIOU';
  let count = 0;

  for (let char of phrase) {
    if (vowels.includes(char)) {
      count++;
    }
  }

  console.log(`Il y a ${count} voyelles dans la phrase.`);
  rl.close();
});
```