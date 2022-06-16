# Dart

Dart is a programming language resemables Java.

## Comments in Dart

- Single-line comments are created by adding // before the comment
- Multi-line comments are created by adding /* before the comment and */ after it.

```js
// this is a comment

int a = 3; // this is also a comment

/* this is also
a long, long
comment */

```


## Variable

Just like Java, by **prefixing** the variable name with the data type.


```js
variable_type variable_name = intial_value;

int a = 3;

var a = 3;
```

## Immutable Variables: final and const

### final keyword

- You initialize it with a value and that value is stored there forever.

```js
final String greeting = "Hi!";
```

### const keyword

- **const** is used to create **compile-time** constants: the compiler will evaluate the value of the constant when you build your app.
- You can’t have const **arguments**.

```js
const a = 3;
```

## Characters and Strings

In flutter, string is a data type which can hold both single character, array of characters or a literal string. That's why you can enclose it in single and double quotes.


```js
String char = "H";
var string = 'Hello WOrld';
```

You can concatinate two strings with + operator.

```js
var hello = 'Hi' + "!";
assert(hello == 'Hi!');
```

## Assert

`assert` terminate the execution if the condition in its parentheses isn’t true (only in testing/debug mode). It's not effective in production code.

## The Backslash

The backslash can be used to **escape** some characters or **insert** special characters.

For example if you wanted to print " in a string, you have 2 methods

1. Create literal string in '' and add "" inside it

```js
'Hello "World"'
```

2. escape the quotes

```js
"Hello \"World\""
```

3. Adding special character to add next line, escate \n.

```js

"First Line\nSecond Line"

```

4. Escaping \ itself

```js
"Hello \\ World" => Hello \ World
```

## String Interpolation

- String interpolation allows you to **insert** one or more **variables** value into a string. 

- By prefixing a variable’s name with $ you can insert its value into the string.”


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


# Reference
- https://dart.dev/
