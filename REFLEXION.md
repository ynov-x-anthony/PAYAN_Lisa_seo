# REFLEXION.md : à compléter

1. `robots.txt` empêche-t-il, à lui seul, le duplicate content entre
   `/produits?tri=prix` et `/produits?tri=prix-asc` ? Pourquoi ?

   Non car ce fichier gère uniquement l'exploration, il ne s'occupe pas de l'indexation.

2. Pourquoi la balise canonique est-elle l'outil adapté ici, plutôt que
   `robots.txt` ou une meta `noindex` ?

   C'est l'outil adapté car elle indique à Google la version de référence. `robots.txt` bloque les craxl. Et `noindex` retire la page de l'index.

3. Si demain `/admin` existe sur ce site et ne doit jamais être exploré par
   Google, quelle ligne ajoutes-tu dans `robots.txt` ?

   Il faudra ajouter `Disallow: /admin/`.
