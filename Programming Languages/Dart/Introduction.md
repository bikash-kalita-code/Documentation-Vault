Every app requires the top-level `main()` function, where execution starts. Functions that don’t explicitly return a value have the `void` return type.

### Variables
Even in [type-safe](https://dart.dev/language/type-system) Dart code, you can declare most variables without explicitly specifying their type using `var`. Thanks to type inference, these variables’ types are determined by their initial values:
```
var name = 'Voyager I';
var year = 1977;
var antennaDiameter = 3.7;
var flybyObjects = ['Jupiter', 'Saturn', 'Uranus', 'Neptune'];
var image = {
  'tags': ['saturn'],
  'url': '//path/to/saturn.jpg'
};
```

### Functions
```
int fibonacci(int n) {
  if (n == 0 || n == 1) return n;
  return fibonacci(n - 1) + fibonacci(n - 2);
}

var result = fibonacci(20);
```
A shorthand `=>` (_arrow_) syntax is handy for functions that contain a single statement. This syntax is especially useful when passing anonymous functions as arguments:
```
flybyObjects.where((name) => name.contains('turn')).forEach(print);
```
