Every app requires the top-level `main()` function, where execution starts. Functions that don’t explicitly return a value have the `void` return type.

### Variables
Even in [type-safe](https://dart.dev/language/type-system) Dart code, you can declare most variables without explicitly specifying their type using `var`. Thanks to type inference, these variables’ types are determined by their initial values: