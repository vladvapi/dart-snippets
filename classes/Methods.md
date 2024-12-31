# Methods

* Getters (aria, perimeter, width, height); 
* Setters (width, height);
* `_` creates private fields (that are not accesible outside the current library);

```dart
void main() {
  final r1 = Rectangle(4, 5);
  r1.width = 6;
  
  print(r1.aria);
  print(r1.perimeter);
  
  print(r1.width);
}

class Rectangle {
  double _width;
  double _height;
  
  Rectangle(this._width, this._height);
  
  double get aria => _width * _height;
  
  double get perimeter => 2 * (_width + _height);
  
  double get width => _width;
  
  set width(double value) => _width = value;
  
  double get height => _height;
  
  set height(double value) => _height = value;
}
```
