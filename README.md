# BookShelf

Petit projet Java qui simule une étagère de livres avec une API simple pour ajouter et consulter des livres.

## Fonctionnalités

- Ajouter un ou plusieurs livres à l'étagère
- Récupérer la liste des livres
- Empêcher la modification de la liste retournée (immutabilité côté client)

## Structure

### `BookShelf.java`

Classe principale qui contient :
- Une liste interne de livres
- La méthode `add(String... booksToAdd)` pour ajouter des livres
- La méthode `books()` qui retourne une vue non modifiable de la liste

### `BookShelfSpec.java`

Tests unitaires JUnit 5 qui vérifient :
- Une étagère vide au départ
- L’ajout de plusieurs livres
- Le comportement de `add()` sans arguments
- L’immutabilité de la liste retournée

