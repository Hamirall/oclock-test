# Apprenant 1

**Étape 1: Détail d’une carte**

Peut-être ajouter une condition quand l’élément d’une carte est vide ou nan, ça serait plus jolie je pense

![Capture d’écran 2023-09-13 à 15.15.08.png](screen/Capture_decran_2023-09-13_a_15.15.08.png)

**Étape 2: Recherche**

Quand on recherche par élément on peu voir un “NaN”, s’afficher sur la page. Ce qui peux perdre l’utilisateur.

- Route: [http://localhost:1234/search/element?element=glace](http://localhost:1234/search/element?element=glace)
    
    ![Capture d’écran 2023-09-12 à 18.35.30.png](screen/Capture_decran_2023-09-12_a_18.35.30.png)
    

Si le code est finit, il faut bien penser à retirer son code commenté, pour rendre ce dernier plus lisible( voir screen si dessus). Code commenté = code inutilisé donc à supprimer.

![Capture d’écran 2023-09-12 à 18.41.56.png](screen/Capture_decran_2023-09-12_a_18.41.56.png)

**Étape 3: Construire un deck**

Le cahier des charges est bien respectés, les cartes s’ajoutent bien comme il faut, on ne peut pas en mettre plus de 5 et pas possible d’ajouter deux fois la même cartes. Et la suppression fonctionne très bien donc bravo.

**Étape Bonus:**

- Route: [http://localhost:1234/search/values?direction=north&value=0](http://localhost:1234/search/values?direction=north&value=0)
    - Quand il n’y a pas de valeur peut-être personnalisé un peu la message à la place d’un “empty”, pour afficher un message plus clair et en Français.
        
        ![Capture d’écran 2023-09-12 à 18.38.03.png](screen/Capture_decran_2023-09-12_a_18.38.03.png)
        

**Conclusion:**

Dans l’ensemble le cahier des charges à bien été respecté donc félicitation. 

Mais dans un esprit de perfectionnement on pourrai améliorer certains petits éléments dans le code.

**Exemple:**

- Si j’essaie de contourner un peu le système en mettant une chaîne de caractères dans l’URL: [http://localhost:1234/deck/add/hbskjdfhsdkfjdsf](http://localhost:1234/deck/add/hbskjdfhsdkfjdsf).
    
    ![Capture d’écran 2023-09-12 à 18.58.27.png](screen/Capture_decran_2023-09-12_a_18.58.27.png)
    

- Et Il faut faudrait potentiellement mettre un try catch sur le cast de la variable

```jsx
const cardId = Number(req.params.id);

// Propositions
try {
	const cardId = Number(req.params.id);
} catch (error) {
	throw "Error cast params"
}
```