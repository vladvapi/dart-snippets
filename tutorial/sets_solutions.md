# Sets Solutions

1.
```dart
void main() {
  final numbers = <int>{1, 2, 3, 4, 5};
  
  print(numbers);
}
```

2.
```dart
void main() {
  final fruits = <String>{};
  
  fruits.addAll({"apple", "banana", "cherry"});
  fruits.remove("banana");
  
  print(fruits);
}
```

3.
```dart
void main() {
  final numbers = <int>{10, 15, 20, 25, 30};
  
  final bigNr = numbers.where((nr) => nr > 20).toSet();
  
  print(bigNr);
}
```

4.
```dart
void main() {
  final numbers = <int>{1, 2, 3, 4};
  
  final squared = numbers.map((nr) => nr * nr).toSet();
  
  print(squared);
}
```

5.
```dart
void main() {
  final numbers1 = <int>{1, 2, 3, 4};
  final numbers2 = <int>{3, 4, 5, 6};
  
  print(numbers1.intersection(numbers2));
}
```

6.
```dart
void main() {
  final numbers1 = <int>{1, 2, 3};
  final numbers2 = <int>{4, 5, 6};
  
  print(numbers1.union(numbers2));
}
```

7.
```dart
void main() {
  final numbers1 = <int>{1, 2, 3, 4};
  final numbers2 = <int>{3, 4, 5, 6};
  
  print(numbers1.difference(numbers2));
}
```

8.
```dart
void main() {
  final numbers1 = <int>{1, 2, 3};
  final numbers2 = <int>{1, 2, 3, 4, 5};
  
  final isSubset = numbers2.containsAll(numbers1);
  
  print(isSubset);
}
```

9.
```dart
void main() {
  final numbers1 = <int>[1, 2, 2, 3, 4, 4, 5];
  
  final setNumbers = numbers1.toSet();
  
  print(setNumbers);
}
```

10.
```dart
void main() {
  final fruits = <String>{"apple", "banana", "cherry"};
  
  print(fruits.contains("banana"));
}
```