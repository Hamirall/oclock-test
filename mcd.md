# MCD

Voici le MCD que tu m'as envoyé pour la création d'un site e-commerce.

![mcd_apprenant.png](screen/mcd_apprenant.png)

Au vu de ce que tu as fait, ton MCD me paraît plutôt cohérent par rapport à la consigne juste au-dessus. Mais j'ai une petite erreur au niveau des cardinalités entre un "User" et un "Produit".

Si on reste avec ta logique "Un utilisateur ne peut aimer qu'un seul produit, et un produit ne peut être aimé que par un seul utilisateur", alors un utilisateur pourra aimer plusieurs produits s'il le souhaite et un produit pourra être aimé par plusieurs utilisateurs.

Cardinalité à corriger :

- Utilisateur ⇒ 0,n
- Produit ⇒ 1, n

En conclusion, le MCD présenté pour la création d'un site e-commerce est plutôt cohérent par rapport à la consigne. Cependant, il y avait une petite erreur de cardinalité qui a été corrigée. Dans l'ensemble, le document est facilement compréhensible. En cas de besoin, je reste disponible pour répondre à des questions ou apporter des conseils supplémentaires. 🙂