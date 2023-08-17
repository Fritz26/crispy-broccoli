# crispy-broccoli

# packagenpm

Obtenez une liste des référentiels Github du nom d'utilisateur spécifié triés par nombre d'étoiles dans l'ordre décroissant et l'heure de la dernière mise à jour

## Installation

```js
# en utilisant npm
npm install packagenpm

# utiliser du yarn
yarn add packagenpm
```

## Utilisation

```js
# utilisation de require
const { getRepos } = require('packagenpm');

# utiliser l'import
import { getRepos } from 'packagenpm' ;
```

## Exemple

### Utilisation des promesses :

```js
getRepos({
  nom d'utilisateur : 'gaearon', // fournir le nom d'utilisateur GitHub ici
  page : 1, // propriété facultative : la valeur par défaut est 1
  per_page : 50 // propriété facultative : la valeur par défaut est 30
}).then((repositories) => console.log(repositories));
```

### Utilisation de async/await :

```js
const getRepositories = fonction async () {
  Repositories const =await getRepos({
    nom d'utilisateur : 'gaearon', // fournir le nom d'utilisateur GitHub ici
    page : 1, // propriété facultative : la valeur par défaut est 1
    per_page : 50 // propriété facultative : la valeur par défaut est 30
  });
  console.log(Repositories);
} ;

getRepositories();
```
