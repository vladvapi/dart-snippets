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
