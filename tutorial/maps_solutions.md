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

6.
```dart
void main() {
  final items = <String, double>{
    "pen": 1.5, 
    "notebook": 3.0, 
    "eraser": 0.5, 
    "ruler": 2.0,
  };
  
  final results = items.entries.where((me) => me.value > 2);
  
  final resultMap = <String, double>{};
  
  resultMap.addEntries(results);
  
  print(resultMap);
}
```

7.
```dart
void main() {
  final items = <String, double>{
    "pen": 1.5, 
    "notebook": 3.0, 
    "eraser": 0.5, 
  };
  
  print(items);
  
  final discounts = items.map((k, v) => MapEntry(k, v - v * 0.1));
  
  print(discounts);
}
```

8.
```dart
void main() {
  final names = <String, int>{"John": 25, "Emma": 30, "Sophia": 22};
  
  print(names.length);
}
```

9.
```dart
void main() {
  final map1 = <String, int>{"a": 1, "b": 2};
  final map2 = <String, int>{"c": 3, "d": 4};
  
  final result = <String, int>{...map1, ...map2};
  
  print(result);
}
```

10.
```dart
void main() {
  final states = <String, int>{"US": 1, "IN": 91, "UK": 44};
  
  final results = states.entries.where((me) => me.value == 91);
  
  for(final result in results){
    print(result.key);
  }
}
```

