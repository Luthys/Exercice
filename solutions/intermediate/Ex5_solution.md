### Exercice 5 : Inverser une chaîne de caractères
Créez un programme qui demande à l'utilisateur de saisir une chaîne de caractères et affiche la chaîne inversée.

#### Exigences :
1. Le programme demande à l'utilisateur de saisir une chaîne de caractères.
2. Le programme affiche la chaîne de caractères inversée.

#### Exemple :
```
Entrez une chaîne de caractères: OpenAI
La chaîne inversée est: IAnepO
```

### Solution :

```javascript
const readline = require('readline');

const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout
});

rl.question('Entrez une chaîne de caractères: ', (str) => {
  const reversedStr = str.split('').reverse().join('');
  console.log(`La chaîne inversée est: ${reversedStr}`);
  rl.close();
});
```