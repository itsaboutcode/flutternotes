- [Dart](#dart)
  - [Comments](#comments)
  - [Data Types](#data-types)
  - [Variable](#variable)
  - [Null safety](#null-safety)
  - [The Backslash](#the-backslash)
  - [String Interpolation](#string-interpolation)
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

- Dart is a Object Oriented programming language which resemables Java.
- Dart is a single threaded language.

## [Comments](dart/dart_commends.md)

## [Data Types](dart/dart_data_types.md)

## [Variable](dart/dart_variables.md)

## [Null safety](dart/dart_null_safety.md)

## The Backslash

- The backslash can be used to **escape** some characters or **insert** special characters.

For example if you wanted to print " in a string, you have 2 options

1. Create literal string in '' and add "" inside it

```js
'Hello "World"'
```

2. Escape the quotes using \"

```js
"Hello \"World\""
```

3. Adding special character to add next line, escape \n.

```js

"First Line\nSecond Line"

```

4. Escaping \ itself

```js
"Hello \\ World" => Hello \ World
```

## String Interpolation

- String interpolation allows you to **insert** one or more **variables** value into a string. 

- By prefixing a variable’s name with **$**, you can insert its value into the string.”


```js

int times = 5;
int more = 10;

"You clicked on this button $times times. To complete this challenge, click $more more times"

// Output
You clicked on this button 5 times. To complete this challenge, click 10 more times.
```

- If you need to access an element of a List, the member of a class, or write any kind of expression, you need to enclose the statement in **curly braces**.

```js

List numbers = [1, 2, 3];

"There are ${numbers.length} and second element is number ${numbers[1]}"

```


## Multi-Line Strings and Raw Strings

- You can make multi-line strings by using **triple** quotes.

```js
"""
Hello
World
"""
```

## Conditions: Boolean Algebra in Dart

- You can use ==, !=, >, <, <= and >= to **compare values**, and you use && as the **AND** operator, || as the **OR** operator and ! as the **NOT** operator.


## List/Array and collection literals

- List is an ordered collection of data.
- Elements of list are indexed from 0 to length-1.
- Length of List is the number of elements it contains.
- It can be initialized with `list literal`, which is comma-seperated list of values enclosed in square brackets.

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
