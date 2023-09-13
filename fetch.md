# Explication du fetch

Hello, alors pour faire simple, la méthode "fetch" provient d'une API du même nom qui permet la manipulation de requêtes HTTP(S). Cette méthode nous permet d'accéder facilement à une ressource à travers le réseau (HTTP) de manière asynchrone. Bien sûr, on peut rendre la requête synchrone, comme tu as pu le faire avec les requêtes à la BDD que j'ai pu voir lors de ton dernier exercice (async, await). Tiens, je te laisse aller voir la [documentation](https://developer.mozilla.org/fr/docs/Web/API/Fetch_API/Using_Fetch) un peu plus (c'est important pour un développeur d'aller voir les documentations des technologies).

Du coup, cette méthode te permettra de faire des requêtes en [AJAX](https://developer.mozilla.org/fr/docs/Web/Guide/AJAX) (je te laisse aller voir la documentation pour celui-là 😉) et d'éviter de rafraîchir une page entière.

Voici un exemple asynchrone que tu aurais pu utiliser lors de ton dernier exercice afin d'éviter le rechargement de la page lors de l'ajout d'une carte à un deck.

```jsx
const baseUrl = "http://locahost:1234"

fetch(`${baseuUrl}/car/add/1`)
  .then((response) => {
    console.log(response)
  })
  .then((error) => {
		console.error(error)
  });
```