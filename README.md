# Flutter Startup Name Generator

This Flutter application is a simple name generator that allows users to discover and save interesting startup names. The application covers various Flutter concepts such as state management, navigation, theming, and interactivity.

## Table of Contents

- [Description](#description)
- [Code Explanation](#code-explanation)
  - [1. `MyApp` Class (StatelessWidget)](#1-myapp-class-statelesswidget)
  - [2. `RandomWords` Class (StatefulWidget)](#2-randomwords-class-statefulwidget)
  - [3. `_buildRow` Method](#3-_buildrow-method)
  - [4. `_buildSuggestions` Method](#4-_buildsuggestions-method)
  - [5. `_pushSaved` Method](#5-_pushsaved-method)
- [Conclusion](#conclusion)

## Description

The application generates random startup names using the English Words package. Users can tap on names to mark them as favorites, and there's a separate screen to view the saved favorites. The app is styled to look natural on both iOS and Android platforms, and its theme has been customized to use a white primary color.

## Code Explanation

### 1. `MyApp` Class (StatelessWidget)

```dart
class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Startup Name Generator',
      theme: ThemeData(
        primaryColor: Colors.white,
      ),
      home: RandomWords(),
    );
  }
}
