- [Flutter](#flutter)
  - [Flutter Command Line](#flutter-command-line)
  - [Introduction to widgets](#introduction-to-widgets)
    - [Stateless Widget](#stateless-widget)
    - [Stateful Widget](#stateful-widget)
  - [State Management](#state-management)
- [References](#references)
  - [Opensource Projects](#opensource-projects)

# Flutter

- Flutter is **Google's UI toolkit** for building beautiful, **natively compiled applications** for mobile, web, and desktop from a single codebase.

- Flutter has a hot reload feature that helps you quickly and easily experiment, build UIs, add features, and fix bugs. Hot reload works by injecting updated source code files into the running Dart Virtual Machine (VM). After the VM updates classes with the new versions of fields and functions, the Flutter framework automatically rebuilds the widget tree, allowing you to quickly view the effects of your changes.

- Flutter provides static analysis which allows you to find problems before executing a single line of code. It’s a powerful tool used to prevent bugs and ensure that the code conforms to style guidelines.

- Dart has an AOT (Ahead of Time) compiler, which compiles to fast, predictable, native code that allows almost all of Flutter to be written in Dart. This not only makes Flutter fast but ensures that virtually everything (including all the widgets) can be customized.

## [Flutter Command Line](flutter_cli.md)


## Introduction to widgets

- The central idea is that you build your UI out of widgets. 

- `Widget` is a component user see on the screen.
  
- Widgets describe what their **view should look like** given their **current configuration and state**. 

- In flutter, almost every object `is a` instance of `Widget` class in one way or the other.

- In flutter, views are created by compsition, one object is composed of many different smaller object. It created a `has a` relationship.

- A chain of things connected by the **has a** relationship is called a **composition hierarchy**.
  
- The chain of things connected by the **is a** relationship is called the **inheritance hierarchy**.

### Stateless Widget

- Stateless widgets are **immutable**, meaning that their properties can't change. All values are **final**. It doesn’t preserve its `state`.

- Stateless widget is `drawn only once`, and it can not be redrawn at a later time.

- Stateless widget’s `build()` method is called only once.

### Stateful Widget

- A Stateful widget is mutable. It keeps track of the state.

- Stateful widgets **maintain state** that might **change** during the lifetime of the widget.

- Implementing a stateful widget **requires** at least **two classes**, a **StatefulWidget** that creates an instance of a **State class**.

- It rebuilds several times over its lifetime.

- The **StatefulWidget** object is, itself, **immutable** and can be thrown away and **regenerated**, but the **State** object **persists** over the lifetime of the widget.

- A Stateful widget’s build() method is called multiple times.



## Flutter Project Default Structure


<img width="343" alt="Screenshot 2023-04-01 at 6 06 27 PM" src="https://user-images.githubusercontent.com/204423/229290820-570ecf3d-4356-43b6-b8f2-a798e8139ab8.png">


- `android/:` This folder contains native Android code.

- `iOS/:` This folder contains native iOS code.

- `Linux/:` This folder contains native Linux code.

- `macOS/:` This folder contains native macOS code.

- `windows/:` This folder contains native windows code.

- `web/:` This folder contains web code.

- `lib/:` This folder contains all Dart files. This is a shared code across all platforms like iOS, Web, Desktop, and embedded devices. However, we are focusing only on the Android platform in this course.

- `test/:` This folder contains all unit testing classes.

- `pubspec.yaml file:` This is the dependency management and configuration file for the Flutter application.

## Weidgets

- [MaterialApp](https://api.flutter.dev/flutter/material/MaterialApp-class.html)

- [SafeArea](https://api.flutter.dev/flutter/widgets/SafeArea-class.html)

- [Center](https://api.flutter.dev/flutter/widgets/Center-class.html)

- [Scaffold](https://api.flutter.dev/flutter/material/Scaffold-class.html)

- [AppBar](https://api.flutter.dev/flutter/material/AppBar-class.html)

- [Container](https://api.flutter.dev/flutter/widgets/Container-class.html)


  

## State Management


# References

- https://flutter.dev/
- https://gallery.flutter.dev/#/
- https://pub.dev/
- https://hillel.dev/
- https://api.flutter.dev/index.html
- https://material.io/design
- https://fonts.google.com/

## Opensource Projects

- https://github.com/authpass/authpass
- https://github.com/invoiceninja/admin-portal
- https://github.com/AppFlowy-IO/AppFlowy
- https://github.com/Solido/awesome-flutter
- https://github.com/tortuvshin/open-source-flutter-apps
