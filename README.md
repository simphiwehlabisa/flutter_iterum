# Flutter Iterum

Easily restart your application from scratch.

## Usage

Wrap you App widget in the `Iterum` widget.

```dart
void main() {
  runApp(
    Iterum(
      child: App(),
    ),
  );
}
```

Call the `revive` static method when you want to restart your application (rebuild the entire widget from scratch).

```dart
Iterum.revive(context);
```
>**Disclaimer :** 
<br><br>Iterum restarts your application at the application level, rebuilding your application widget tree from scratch, losing any previous state.
<br><br>Iterum does not fully restart your application process at the OS level.

## Use cases 

Here is a non-exhaustive list of use cases where `Iterum` can help :

- restart the app after a logout
- restart the app after a failed app initialization process
- restart the app after a specific event in the app occurs
- ...

## Installation

### Dependency
Add the package as a dependency in your pubspec.yaml file.
```yaml
dependencies:
  flutter_Iterum: "^1.0.0"
```

### Import
Import the package in your code file.
```dart
import 'package:flutter_Iterum/flutter_Iterum.dart';
```

## License

Flutter Iterum is released under the [MIT License](LICENSE)