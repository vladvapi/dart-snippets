# List exercises solutions:
1.
```dart
void main() {
  List<String> colors = ["blue", "red", "white"];
  
  print(colors);
}
```
2.
```dart
void main() {
  List<int> numbers = [];
  
  numbers.add(5);
  numbers.addAll([10, 15, 20]);
  
  numbers.remove(10);
  
  print(numbers);
}
```
3.
```dart
void main() {
  List<String> days = [
    "Monday",
    "Tuesday",
    "Wednesday",
    "Thursday",
    "Friday",
    "Saturday",
    "Sunday"
  ];

  print(days.first);
  print(days.last);
}
```

4.
```dart
void main() {
  List<int> numbers = [3, 6, 9, 12, 15];

  print(numbers.length);
}
```

5.
```dart
void main() {
  List<String> fruits = ["apple", "banana", "cherry", "date"];

  for(String fruit in fruits){
    print(fruit);
  }
}
```

6.
```dart
void main() {
  List<int> numbers = [1, 2 ,3 , 4, 5];
  
  numbers = numbers.reversed.toList();
  
  print(numbers);
}
```

7.
```dart
void main() {
  List<int> numbers = [45, 3, 67, 1, 23];
  
  numbers.sort();
  
  print(numbers);
  
  numbers.sort((a,b) => -(a-b));
  
  print(numbers);
}
```

8.
```dart
void main() {
  List<int> numbers = [2, 7, 10, 15, 18, 21];
  
  numbers = numbers.where((nr) => nr > 10).toList();
  
  print(numbers);
}
```

9.
```dart
void main() {
  List<int> numbers = [1, 2, 3, 4];
  
  final doubles = numbers.map((a) => a * 2).toList();
  
  print(doubles);
}
```

10.
```dart
void main() {
  List<String> animals = ["cat", "dog", "bird", "fish"];
  
  print(animals.contains("dog"));
}
```

11.
```dart
void main() {
  final numbers = <int>[1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
 
  final even = numbers.where((nr) => nr % 2 == 0).toList();
  
  print(even);
}
```

12.
```dart
void main() {
  final words = <String>["apple", "bat", "cherry", "dog", "elephant"];
 
  final bigWords = words.where((e) => e.length > 3).toList();
  
  print(bigWords);
}
```

13.
```dart
void main() {
  final numbers = <int>[3, 6, 9, 12, 15, 18];
 
  final div = numbers.firstWhere((nr) => nr % 4 == 0);
  
  print(div);
}
```

14.
```dart
void main() {
  List<int> numbers = [1, 2, 3, 4];
  
  final doubles = numbers.map((a) => a * a).toList();
  
  print(doubles);
}
```

15.
```dart
void main() {
  final numbers = <int>[10, 20, 30, 40, 50];
 
  final sum = numbers.reduce((s, e) => s + e);
  
  print(sum);
}
```

16.
```dart
void main() {
  final fruits = <String>["grape", "apple", "banana", "kiwi", "cherry"];
  
  fruits.sort((a, b) => -(a.length.compareTo(b.length)));
  
//   or:
//   fruits.sort((a, b) => b.length.compareTo(a.length));
  
  print(fruits);
}
```

17.
```dart
void main() {
  final numbers = <int>[2, 4, 6, 8, 10];
  
  final allEven = numbers.every((nr) => nr % 2 == 0);
  
  print(allEven);
}
```

18.
```dart
void main() {
  final numbers = <int>[3, 5, 7, 9, 12];
  
  final anyEven = numbers.any((nr) => nr % 2 == 0);
  
  print(anyEven);
}
```

19.
```dart
void main() {
  final numbers1 = <int>[1, 2, 3];
  final numbers2 = <int>[4, 5, 6];
  
  final combinedList = [numbers1, numbers2].expand((list) => list).toList();
//   or (simpler):
//   final combinedList = [...numbers1, ...numbers2];
  
  print(combinedList);
}
```

20.
```dart
import 'package:collection/collection.dart';

void main() {
  final words = <String>["bat", "cat", "ball", "apple", "ant"];
  
  final groups = groupBy(words, (s) => s[0]);
  
  print(groups);
}
```
