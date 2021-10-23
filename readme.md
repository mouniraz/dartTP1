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
# Exercice fibonacci 
1) Ecrire une fonction qui calcule Fibonacci(n) n>=0 de 2 façons différentes: recursive et itérative
2) Tester la fonction dans le programme principal main
# Exercice Arrow functions
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

