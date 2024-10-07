# Exercice Null Safety
1) corriger le code pour que la variable a accepte la valeur null
```dart
void main() {
  int a;
  a = null;
  print('a is $a.');
}
```
2) corriger le code : on veut  déclarer une liste qui peut être null et une liste qui peut avoir des valeurs null
```dart
void main() {
  List<String> aListOfStrings = ['one', 'two', 'three'];
  List<String> aNullableListOfStrings;
  List<String> aListOfNullableStrings = ['one', null, 'three'];

  print('aListOfStrings is $aListOfStrings.');
  print('aNullableListOfStrings is $aNullableListOfStrings.');
  print('aListOfNullableStrings is $aListOfNullableStrings.');
}
```
3) ajouter des points d'exclamation pour corriger le code suivant
```dart
int? couldReturnNullButDoesnt() => -3;
void main() {
  int? couldBeNullButIsnt = 1;
  List<int?> listThatCouldHoldNulls = [2, null, 4];

  int a = couldBeNullButIsnt;
  int b = listThatCouldHoldNulls.first; // first item in the list
  int c = couldReturnNullButDoesnt().abs(); // absolute value

  print('a is $a.');
  print('b is $b.');
  print('c is $c.');
}
```
# Les fonctions
## Les paramètres nommés
1) Crée une fonction showIdentity avec des paramètres nommés optionnels (nom, age) pour les informations suivantes :
    nom (String)
    âge (int)
    pays (String)
2) Tester la fonction avec ou son paramètre
3) définir la meme fonction en utilisant les paramètres nommés de position (nom, age)
4) Définir avec la forme Arrow fonction
## Exercice Arrow functions
1) terminer ce code avec des fonctions Arrow Syntax
```dart
class MyClass {
  int value1 = 2;
  int value2 = 3;
  int value3 = 5;
  
  // Returns the product of the above values:
  int get product => TODO();
  
  // Adds 1 to value1:
  void incrementValue1() => TODO();
  
  // Returns a string containing each item in the
  // list, separated by commas (e.g. 'a,b,c'): 
  String joinWithCommas(List<String> strings) => TODO();
}
```

# Exercice Setter et getter
soit la classe ShoppingCart, on veut ajouter un get total qui retourne la somme de notre liste de prix __prices__ et un setter qui change la valeur de la liste par une liste de réels >0 
```dart
class ShoppingCart {
  List<double> _prices = [];
  
  // Add a "total" getter here:

  // Add a "prices" setter here:
}
```
# Exercice les filtres 
1) implémenter la méthode ilterOutUnder21 qui retourne les users dont l'age <21
2) implémenter la méthode findFirstShortNamed qui retourne le premier  user dont la longueur de son nom <3 
```dart
Iterable<User>? filterOutUnder21(Iterable<User> users) {
  TODO('Implement this method');
}

User? findFirstShortNamed(Iterable<User> users) {
  TODO('Implement this method');
}
class User {
  String name;
  int age;

  User(
    this.name,
    this.age,
  );
}
```
# Carnet de contact Dart 
1) définir une classe Contact(name,,surname,address,_email,_mobileTel,_homeTel)
homeTel et address peuvent être null (définir un constructeur simple et un constructeur  _homeTel)
2)ajouter un get nameSurname qui retourne une chaine contenant le name et le surname.
3) ajouter une méthode privée validateEmail(email) qui teste si un email est valide ou non
4) ajouter 2 méthodes privées validateMobileTel(mobileTel) et validatehomeTel(homeTel )
5) ajouter un set email qui permet de modifier l'email avec un email valide
6) ajouter les setters mobileTel et homeTel
7) définir une Classe CarnetContact(List<Contact> listContact)
8) définir la méthode addContact qui permet d'ajouter un contact à la liste de contact
9) définir la méthode deleteContact qui permet de supprimer un contact de la liste de contacts
10) définir searchContact(String contact) qui cherche et retourne tous les contacts contenant une chaine quelconque contact

# Combat 
# Combat 
1. Créer une classe abstraite Enemy
   Attributs: 
  String name : Nom de l'ennemi 
  int health : Points de vie 
  double speed : Vitesse de déplacement 
  Méthodes abstraites: 
  void attack(): Méthode pour définir l'attaque de l'ennemi 
  void takeDamage(int damage): Méthode pour infliger des dégâts à l'ennemi
2. Créer de mixins pour les comportements spécifiques
  Mixin Flying:
  Méthode fly()
  Mixin Ranged:
  Méthode shoot()
  Mixin Melee:
  Méthode meleeAttack()
3. Créer de classes d'ennemis concrètes
  Enemy1: Un ennemi volant qui tire des lasers
  Enemy2: Un ennemi au corps à corps rapide
  Enemy3: Un ennemi volant et tirant des projectiles
4. Créer une liste d'ennemis de différents types.
5. Boucler sur la liste et appeler les méthodes attack() et takeDamage() pour simuler des combats.
6. Créer de classes d'ennemis concrètes
Enemy1: Un ennemi volant qui tire des lasers
Enemy2: Un ennemi au corps à corps rapide
Enemy3: Un ennemi volant et tirant des projectiles
4. Créer une liste d'ennemis de différents types.
Boucler sur la liste et appeler les méthodes attack() et takeDamage() pour simuler des combats.
