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
