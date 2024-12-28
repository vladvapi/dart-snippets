# Menu

```dart
void main() {
  final noodles = MenuItem("noodles", 5.99);

  final fries = MenuItem("french fries", 3.99);

  final pizza = Pizza("Pizza Diavolo", 11.99, ["pepperoni", "chilli", "cheese"]);
  
  final pizzaCasei = Pizza.acasei();

  final vanillaIce = IceCream("Vanilla Ice cream", 4.99, "Vanilla");

  print(noodles);
  print(fries);
  print(pizza);
  print(vanillaIce);
  print(pizzaCasei);
}

class MenuItem {
  String name;
  double price;

  MenuItem(this.name, this.price);

  String toString() {
    return "name: $name --> price: $price";
  }
}

class Pizza extends MenuItem {
  List<String> toppings;

  Pizza(super.name, super.price, this.toppings);

  Pizza.acasei([super.name = "Pizza Casei", super.price = 10.99,
      this.toppings = const ["mushrooms", "corn"]]);

  String toString() {
    return "${super.toString()}, toppings: $toppings";
  }
}

class IceCream extends MenuItem {
  String flavour;

  IceCream(super.name, super.price, this.flavour);

  String toString() {
    return "${super.toString()}, flavour: $flavour";
  }
}
```
