## REPONSES :
1. Peut-on modifier l'âge d'un chien une fois qu'il a été créé (essayez de donner 10 ans à chien3 pour vérifier) ? 

VOTRE REPONSE ICI
Non, l'attribut age est privé et il n'y a pas de méthode pour le modifier après la création du chien. Pour changer l'âge, il faudrait ajouter une méthode setAge().

2. Que se passe-t-il si on modifie le nom de chien2 ?

VOTRE REPONSE ICI
Tous les chiens auront le même nom, car l'attribut nom est statique. Il est partagé par tous les objets Chien, donc si vous changez le nom d'un chien, il change pour tous.

3. Pourquoi tous les chiens ont tous le même nom ?

VOTRE REPONSE ICI
Tous les chiens ont le même nom parce que nom est une variable statique. Les variables statiques sont partagées par tous les objets de la classe. Pour que chaque chien ait son propre nom, il faut rendre nom non statique.

4. Observez avec attention les lignes N°20 à N°26 du main() et réfléchissez : par quel miracle le chien3 à la ligne N°26 s'affiche correctement ?
   Répondez à cette question en expliquant avec précision ce qui se passe et pourquoi.

VOTRE REPONSE ICI
Quand vous affichez chien3 sans utiliser toString(), Java appelle automatiquement la méthode toString() de l'objet. Cette méthode retourne une chaîne avec le nom et l'âge du chien. Mais comme nom est statique, tous les chiens partageront le même nom affiché.

