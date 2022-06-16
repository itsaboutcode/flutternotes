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

2. Escate the quotes

```js
"Hello \"World\""
```




# Reference
- https://dart.dev/
