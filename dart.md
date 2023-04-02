- [Dart](#dart)
  - [Comments](#comments)
  - [Data Types](#data-types)
  - [Variable](#variable)
  - [Null safety](#null-safety)
  - [String Interpolation and The Backslash](#string-interpolation-and-the-backslash)
  - [Multi-Line Strings and Raw Strings](#multi-line-strings-and-raw-strings)
  - [Conditions: Boolean Algebra in Dart](#conditions-boolean-algebra-in-dart)
  - [List/Array and collection literals](#listarray-and-collection-literals)
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

- Dart 1.0 was released on November 14th, 2013

- It covers client, server, and now mobile, web, desktop with Flutter.

- It has virtual machine, core libraries and package management repository.

- Instead of threads, all Dart code runs inside of `isolates`. Each isolate has its own memory heap, ensuring that no isolate’s state is accessible from any other isolate.

- Dart has an `AOT (Ahead of Time) compiler`, which compiles to fast, predictable, native code that allows almost all of Flutter to be written in Dart. This not only makes Flutter fast but ensures that virtually everything (including all the widgets) can be customized.

- In dart, all `statements` end with a semicolon `;`.

## Dart program entry point

- All dart programs e.g; flutter, the compiler look for an entry point.
- In dart, this entry point is `main` method.

```
main(){
  // Insert Code Here
}
```

- If compiler don't find this, it will raise an error and application will not run.

## Print method

- This method is used to print something on the console

```
print("Hello World");
```

## Importing a library in dart

```import 'dart:io';```


- You can take the input from user with following command 

```stdin.readLineSync()```

## [final Keyword](https://www.educative.io/answers/what-is-the-final-keyword-in-dart)

- `final` keyword is used to define `immutable` constants or objects
- It's `runtime` constant value

```
// Without datatype
final variable_name;

// With datatype
final data_type  variable_name;
```

```
final y = DateTime.now(); // initialized at runtime

Class User {
 final String firstName;
 final String lastName;

 User(this.firstName, this.lastName);

}

```

## [const keyword]

- `const` variables are `compile-time constants`.
- it means their values are determined at compile-time rather than runtime. 
- They must be initialized with a constant value (i.e., a value that can be determined at compile-time) and cannot be changed later. 
- const variables are also implicitly final, which means they cannot be reassigned after initialization.


```
const x = 5; // compile-time constant
```

## Imperative Programming

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

## [Control Flow Statements](dart/dart_conditional_flows.md)

## [Exceptions](dart/dart_exceptions.md)

## [Functions](dart/dart_functions.md)

## [Classes](dart/dart_classes.md)

## [Async Coding in Dart](dart/dart_async_await.md)

## [Exception Handling](dart/dart_exceptions.md)

# Reference
- https://dart.dev/guides/language/language-tour
