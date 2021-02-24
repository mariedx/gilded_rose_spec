## Mise en place des tests unitaires avec Jasmine ⚙

Fonctionnement de l'app : 

- Tous les éléments ont une valeur `sellIn` qui désigne le nombre de jours restant pour vendre l'article.
- Tous les articles ont une valeur `quality` qui dénote combien l'article est précieux.
A la fin de chaque journée, notre système diminue ces deux valeurs pour chaque produit.
- Une fois que la date de péremption est passée, la qualité se dégrade deux fois plus rapidement.
- La qualité (`quality`) d'un produit ne peut jamais être négative.
- "Aged Brie" augmente sa qualité (`quality`) plus le temps passe.
- La qualité d'un produit n'est jamais de plus de 50.
- "Sulfuras", étant un objet légendaire, n'a pas de date de péremption et ne perd jamais en qualité (`quality`)
- "Backstage passes", comme le "Aged Brie", augmente sa qualité (`quality`) plus le temps passe (`sellIn`) ; La qualité augmente de 2 quand il reste 10 jours ou moins et de 3 quand il reste 5 jours ou moins, mais la qualité tombe à 0 après le concert.
- les éléments "`Conjured`" voient leur qualité se dégrader deux fois plus vite que les objets normaux.
- "`Conjured`" est un préfixe au nom des éléments cela signifie que tu dois identifier quels éléments en sont (exemple: "Conjured Dark Blade", "Conjured Magic Stick")

Pour lancer l'app :
- Git clone https://github.com/mariedx/gilded_rose_spec.git
- npm i
- npm test 

# ✅