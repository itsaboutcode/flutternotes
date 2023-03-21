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

- Stateless widgets are **immutable**, meaning that their properties can't change—all values are **final**.

### Stateful Widget

- Stateful widgets **maintain state** that might **change** during the lifetime of the widget.

- Implementing a stateful widget **requires** at least **two classes**, a **StatefulWidget** that creates an instance of a **State class**.

- The **StatefulWidget** object is, itself, **immutable** and can be thrown away and **regenerated**, but the **State** object **persists** over the lifetime of the widget.







  


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
