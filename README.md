# PO001 : Découverte de l'orienté objet

> L'ensemble de cet exercice est à réaliser en JavaScript. 

## Tout d'abord un peu de pratique
Réalisez les exercices présents sur le site [https://www.khanacademy.org/computing/computer-programming/programming/object-oriented/p/object-types](ici).

## Exercice : Générer des apprenants de la Code Académie

Nous allons créer un algorithme qui va générer toute un groupe d'apprenants de la code académie. 
Ces derniers seront des personnes allant de 16 à 50 ans. Avec en moyenne 25% de représentation féminine.

### Modélisation d'un apprenant

#### Création de l'objet


Créer la classe Apprenant, ayant les attributs suivants:

* lastName (string)
* firstName (string)
* gender (Enum : H/F/A)
* birthDate: (date)
* allergies (int)

#### Génération d'une promotion

Réaliser un script qui génèrera un tableau de 24 apprenants aléatoirement. Sachant que l'entier attendu pour les allergies est une valeur entre 0 et 255.

### Implémenter des méthodes additionnelles sur l'objet

La notation requise pour les allergies est un nombre numerique représentant l'ensemble des allergies de l'apprenant.

La liste des allergènes connus par votre application (et leurs valeurs associées)  sont les suivantes :

 * oeuf (1)
 * cacahuette (2)
 * coquillage (4)
 * fraise (8)
 * tomate (16)
 * chocolat (32)
 * pollen (64)
 * chat (128)

Ainsi, si Thomas est allergique aux cacahuettes et au chocolat, il aura un numéro d'allergie de 34.

Ajouter au sein de la classe apprenant une méthode : 
 * isAllergicTo(int allergen) : bool
 * getAge() : int

### Affichage et valeurs

1) Affichez au sein de votre page web les informations suivantes : 
 * Un pourcentage de représentation féminine au sein de la promo
 * L'age du plus jeune apprenant
 * L'age moyen d'un apprenant
 * L'age de l'apprenant le plus agé
 * Un tableau avec toute la promotion et les informations correspondates

2) Réalisez une liste de choix contenant l'ensemble des allergènes connus. après sélection d'un champ au sein de cette liste de choix, affichez au sein du tableau uniquement les apprenants concernés.

### Refactoring Allergènes 

Il a été detecté de nombreux nouveaux allergènes. Trouver une méthode afin de pouvoir les intégrer sur votre site plus facilement : 
 * lait (256)
 * acarien  (512)

N'oubliez pas de mettre à  jour votre génération aléatoire.

### Unit tests
Ecrivez des tests unitaires Jasmine



>  Si vous avez terminé cet exercice, essayez de générer la promotion d'apprenants dans un autre langage (TypeScript/Python/PHP...)