### Exercice 8 : Vérifier un palindrome
Créez un programme qui demande à l'utilisateur de saisir une chaîne de caractères et vérifie si elle est un palindrome.

#### Exigences :
1. Le programme demande à l'utilisateur de saisir une chaîne de caractères.
2. Le programme vérifie et affiche si la chaîne est un palindrome.

#### Exemple :
```
Entrez une chaîne de caractères: radar
"radar" est un palindrome.

Entrez une chaîne de caractères: hello
"hello" n'est pas un palindrome.
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
  if (str === reversedStr) {
    console.log(`"${str}" est un palindrome.`);
  } else {
    console.log(`"${str}" n'est pas un palindrome.`);
  }
  rl.close();
});
```
