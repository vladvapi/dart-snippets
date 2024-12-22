# Maps solutions

1.
```dart
void main() {
  final countries = <String, String>{
    "Romania": "Bucharest",
    "Bulgaria": "Sofia",
    "France": "Paris",
    "Germany": "Berlin",
    "Italy": "Rome",
  };
  
  print(countries);

//  or:
  for(final me in countries.entries){
    print("${me.key}: ${me.value}");
  }
// or:
  for(final k in countries.keys){
    print("$k: ${countries[k]}");
  }
}
```

2.
```dart
void main() {
  final fruits = <String, int>{"apple": 2, "banana": 1, "cherry": 3};
  
  print(fruits["banana"]);
}
```

3.
```dart
void main() {
  final numbers = <String, int>{};
  
  numbers.addAll({"one": 1, "two": 2, "three" : 3});
  
  numbers.remove("two");
  
  print(numbers);
}
```

4.
```dart
void main() {
  final students = <String, int>{
    "Alice": 85,
    "Bob": 90,
    "Charlie": 78,
  };

  for (final me in students.entries) {
    print("${me.key}: ${me.value}");
  }
}
```

5.
```dart
void main() {
  final products = <String, int>{
    "laptop": 10, 
    "phone": 15, 
    "tablet": 5,
  };
  
  if(products.containsKey("tablet")){
    print("exists");
  }else {
    print("doesn't exist");
  }
}
```
