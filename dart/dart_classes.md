- [Classes](#classes)
    - [Using class members](#using-class-members)
    - [Using constructors](#using-constructors)
    - [Class variables and methods](#class-variables-and-methods)
      - [Static variables](#static-variables)
      - [Static methods](#static-methods)
    - [Private Member of the class](#private-member-of-the-class)
- [Reference](#reference)

# Classes

- Dart is an object-oriented language with classes and **mixin-based** inheritance.
  
- **Mixin-based** inheritance means that although every class (except for the top class, Object?) has **exactly one superclass**, a class body can be reused in multiple class hierarchies.

- **Extension methods** are a way to add functionality to a class without changing the class or creating a subclass.

### Using class members

- Objects have members consisting of **functions and data** (**methods and instance variables**, respectively).

- When you call a method, you **invoke** it on an object: the method has **access** to that object’s functions and data.

- Use a **dot (.)** to refer to an instance variable or method:

```js

var p = Point(2, 2);

// Get the value of y.
assert(p.y == 2);

// Invoke distanceTo() on p.
double distance = p.distanceTo(Point(4, 4));

```

- Use `?.` instead of `.` to avoid an exception when the leftmost operand is null:

```js
// If p is non-null, set a variable equal to its y value.
var a = p?.y;
```

### Using constructors



### Class variables and methods

- Use the `static` keyword to implement **class-wide** variables and methods.

#### Static variables

- Static/class variables are useful for class-wide **state** and **constants**.
- Static variables **aren’t initialized** until they’re used.

```js

class Queue {
  static const initialCapacity = 16;
}

void main() {
  assert(Queue.initialCapacity == 16);
}

```

#### Static methods

- Static/Class methods **don’t** operate on an **instance**, and thus **don’t** have access to **this**.
- They do, however, have **access to static** variables.


### Private Member of the class

- Unlike Java, Dart **doesn’t have** the keywords `public, protected, and private`. 
  
- If an identifier starts with an `underscore (_)`, it’s private to its library.


# Reference

- https://dart.dev/guides/language/language-tour#classes
- https://dart.dev/guides/language/language-tour#libraries-and-visibility

