# Constructors

```dart
import 'dart:math';

void main() {
  final rectangle = Rectangle(10, 12);
  final square = Rectangle.square(7);

  print(rectangle);
  print(square);

  final cu = Circle.unit();
  final c2 = Circle.fromDiameter(10.5);

  print(cu);
  print(c2);

  final triangle = Triangle(4, 5, 6);
  final equi = Triangle.equilateral(5);
  final right = Triangle.right(3, 4);

  print(triangle);
  print(equi);
  print(right);
}

class Triangle {
  double side1;
  double side2;
  double side3;

  Triangle(this.side1, this.side2, this.side3);
  Triangle.equilateral(double side)
      : side1 = side,
        side2 = side,
        side3 = side;
  Triangle.right(double leg1, double leg2)
      : side1 = leg1,
        side2 = leg2,
        side3 = sqrt(leg1 * leg1 + leg2 * leg2);

  @override
  String toString() => "Triangle(side1: $side1, side2: $side2, side3: $side3)";
}

class Circle {
  double radius;

  Circle(this.radius);
  Circle.unit() : radius = 1;
  Circle.fromDiameter(double diameter) : radius = diameter / 2;

  @override
  String toString() => "Circle(radius: $radius)";
}

class Rectangle {
  int width;
  int height;

  Rectangle(this.width, this.height);
  Rectangle.square(int size)
      : height = size,
        width = size;

  @override
  String toString() => "Rectangle(width: $width, height: $height)";
}


```

Am definit tipul piont cu 2 date membre, coordonatele punctului, x si y.
Am definit unnamed constructor care initializeaza x si y.
In dart putem avea cel mult un **unnamed constructor**.

Am mai definit doi **named constructors** `Point.origin` si `Point.unit`.
Retine sintaxa cum am initializat x si y in acesti constructori.

Am rescris functia `toString()` ca sa afiseze numele tipului si datele membre.
Retine annotarea `@override`.

In `main()` am creeat obiecte de tip **point** folosind toate tipurile de constructori create.

```dart
void main() {
  final p = Point(5, 3);
  final o = Point.origin();
  final u = Point.unit();

  print(p);
  print(o);
  print(u);
}

class Point {
  int x;
  int y;

  // unnamed constructor
  Point(this.x, this.y);
  Point.origin()
      : x = 0,
        y = 0;
  Point.unit()
      : x = 1,
        y = 1;

  @override
  String toString() => "Point(x: $x, y: $y)";
}
```

## Positional optional arguments

* Optional arguments se pun intotdeauna dupa required arguments.
* Daca dau valoare pt un argument optional trebuie sa dau valoare pt toate argumentele pozitionale de dinainte. (ex: daca la person dau si grade trebuie neaparat sa pun si age)

```dart
void main() {
  final p1 = Person("Alice", 25);
  final p2 = Person("Bob");
  
  print(p1);
  print(p2);
}

class Person {
  String name;
  int age;
// int? age;
  int? grade;
  
  Person(this.name, [this.age = 18, this.grade]);
// Person(this.name, [this.age]);
  
  String toString() => "Person(name: $name, age: $age, grade: $grade)";
}
```

## Named arguments (optional and required)

```dart
void main() {
  final p1 = Person(name: "Alice",age: 25);
  final p2 = Person(grade: 10, name: "Bob");
  
  print(p1);
  print(p2);
}

class Person {
  String name;
  int age;
  int? grade;
  
  Person({required this.name, this.age = 18, this.grade});
  
  String toString() => "Person(name: $name, age: $age, grade: $grade)";
}
```
