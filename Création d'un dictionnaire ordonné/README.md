L'objectif de ce prorgramme est de créer une classe, destinée à produire des objets
 conteneurs, des dictionnaires ordonnés.
 L'idée, assez simplement, est de stocker nos données dans deux listes :
 la première contenant nos clés;
 la seconde contenant les valeurs correspondantes.
 L'ordre d'ajout sera ainsi important, on pourra trier et inverser ce type de dictionnaire.
  Voici la liste des mécanismes que notre classe devra mettre en oeuvre.
 1. On doit pouvoir créer le dictionnaire de plusieurs façons :
 Vide : on appelle le constructeur sans lui passer aucun paramètre et le diction
naire créé est donc vide.
 Copié depuis un dictionnaire : on passe en paramètre du constructeur un dictionnaire que l'on copie par la suite dans notre objet. On peut ainsi écrire
 constructeur(dictionnaire) et les clés et valeurs contenues dans le dictionnaire sont copiées dans l'objet construit.
 Pré-rempli grâce à des clés et valeurs passées en paramètre : comme les dictionnaires usuels, on doit ici avoir la possibilité de pré-remplir notre objet avec
 des couples clés-valeurs passés en paramètre (constructeur(cle1 = valeur1,
 cle2 = valeur2, ...)).
 2. Les clés et valeurs doivent être couplées. Autrement dit, si on cherche à suppri
mer une clé, la valeur correspondante doit également être supprimée. Les clés et
 valeurs se trouvant dans des listes de même taille, il suffira de prendre l'indice
 dans une liste pour savoir quel objet lui correspond dans l'autre. Par exemple, la
 clé d'indice 0 est couplée avec la valeur d'indice 0.
 3. On doit pouvoir interagir avec notre objet conteneur grâce aux crochets, pour
 récupérer une valeur (objet[cle]), pour la modifier (objet[cle] = valeur) ou
 pour la supprimer (del objet[cle]).
 4. Quand on cherche à modifier une valeur, si la clé existe on écrase l'ancienne
 valeur, si elle n'existe pas on ajoute le couple clé-valeur à la fin du dictionnaire.
 5. On doit pouvoir savoir grâce au mot-clé in si une clé se trouve dans notre dic
tionnaire (cle in dictionnaire).
 6. On doit pouvoir demander la taille du dictionnaire grâce à la fonction len.
 7. On doit pouvoir afficher notre dictionnaire directement dans l'interpréteur ou
 grâce à la fonction print. L'affichage doit être similaire à celui des dictionnaires
 usuels ({cle1: valeur1, cle2: valeur2, ...}).
 8. L'objet doit défnir les méthodes sort pour le trier et reverse pour l'inverser.
 Le tri de l'objet doit se faire en fonction des clés.
 9. L'objet doit pouvoir être parcouru. Quand on écrit for cle in dictionnaire,
 on doit parcourir la liste des clés contenues dans le dictionnaire.
 10. À l'instar des dictionnaires, trois méthodes keys() (renvoyant la liste des clés),
 values() (renvoyant la liste des valeurs) et items() (renvoyant les couples (clé,
 valeur)) doivent être mises en oeuvre. 
 11. On doit pouvoir ajouter deux dictionnaires ordonnés (dico1 + dico2); les clés
 et valeurs du second dictionnaire sont ajoutées au premier.
