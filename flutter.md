- [Flutter](#flutter)
  - [Introduction to widgets](#introduction-to-widgets)
    - [Stateless Widget](#stateless-widget)
    - [Stateful Widget](#stateful-widget)
  - [State Management](#state-management)
- [References](#references)
  - [Opensource Projects](#opensource-projects)

# Flutter

- Flutter is **Google's UI toolkit** for building beautiful, **natively compiled applications** for mobile, web, and desktop from a single codebase.

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

- https://github.com/invoiceninja/admin-portal
- https://github.com/Solido/awesome-flutter
- https://github.com/tortuvshin/open-source-flutter-apps