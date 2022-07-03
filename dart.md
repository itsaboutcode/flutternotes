- [Dart](#dart)
  - [Comments](#comments)
  - [Data Types](#data-types)
  - [Variable](#variable)
  - [Null safety](#null-safety)
  - [String Interpolation and The Backslash](#string-interpolation-and-the-backslash)
  - [Multi-Line Strings and Raw Strings](#multi-line-strings-and-raw-strings)
  - [Conditions: Boolean Algebra in Dart](#conditions-boolean-algebra-in-dart)
  - [List/Array and collection literals](#listarray-and-collection-literals)
  - [The 'for in' Loop](#the-for-in-loop)
  - [Control Flow Statements](#control-flow-statements)
  - [Exceptions](#exceptions)
  - [Functions](#functions)
  - [Classes](#classes)
  - [Async Coding in Dart](#async-coding-in-dart)
  - [Exception Handling](#exception-handling)
- [Reference](#reference)

# Dart

- Dart is an Object Oriented programming language which resembles Java.
- Dart is a single threaded language.

## [Comments](dart/dart_commends.md)

## [Data Types](dart/dart_data_types.md)

## [Variable](dart/dart_variables.md)

## [Null safety](dart/dart_null_safety.md)

## [String Interpolation and The Backslash](dart/dart_backslash.md)




## Multi-Line Strings and Raw Strings

- You can make multi-line strings by using **triple** quotes.

```js
"""
Hello
World
"""
```

## Conditions: Boolean Algebra in Dart

- You can use ==, !=, >, <, <= and >= to **compare values**, and you use `&&` as the **AND** operator, `||` as the **OR** operator and `!` as the **NOT** operator.


## List/Array and collection literals

- List is an ordered collection of data.
- Elements of the list are indexed from 0 to length-1.
- Length of List is the number of elements it contains.
- It can be initialized with `list literal`, which is a comma-separated list of values enclosed in square brackets.

```js

var list = [10,20,30];

assert(list[0] == 30);

```

## The 'for in' Loop

It's a special kind of loop which **iterates** over the element of a list.

```js
var names = ["Adil", "Muhammad", "Bushra", "Shaukat"];

for (var name in names) {
    print(name);
}
```

---

## [Control Flow Statements](dart/dart_conditional_flows.md)

## [Exceptions](dart/dart_exceptions.md)

## [Functions](dart/dart_functions.md)

## [Classes](dart/dart_classes.md)

## [Async Coding in Dart](dart/dart_async_await.md)

## [Exception Handling](dart/dart_exceptions.md)

# Reference
- https://dart.dev/guides/language/language-tour
