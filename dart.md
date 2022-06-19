# Dart

- [Dart](#dart)
  - [Comments in Dart](#comments-in-dart)
  - [Variable](#variable)
  - [Immutable Variables: final and const](#immutable-variables-final-and-const)
    - [final keyword](#final-keyword)
    - [const keyword](#const-keyword)
  - [Characters and Strings](#characters-and-strings)
  - [Assert](#assert)
  - [The Backslash](#the-backslash)
  - [String Interpolation](#string-interpolation)
  - [Multi-Line Strings and Raw Strings](#multi-line-strings-and-raw-strings)
  - [Conditions: Boolean Algebra in Dart](#conditions-boolean-algebra-in-dart)
  - [List/Array and collection literals](#listarray-and-collection-literals)
  - [The 'for in' Loop](#the-for-in-loop)
  - [Functions](#functions)
  - [Function Parameters](#function-parameters)
    - [Positional Parameters](#positional-parameters)
    - [Named Parameters](#named-parameters)
    - [The Arrow Notation](#the-arrow-notation)
    - [Anonymous Functions and Closures](#anonymous-functions-and-closures)
  - [main Function](#main-function)
- [Reference](#reference)

Dart is a Object Oriented programming language which resemables Java.

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

- **Prefix** the variable with data type, and then variable name comes.


```js

data_type variable_name = intial_value;

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

- In flutter, string is a data type which can hold both single character, array of characters or a literal string. That's why you can enclose it in single and double quotes.


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

- `assert` terminate the execution if the condition in its parentheses isn’t true (only in testing/debug mode). 
  
- It's not effective in production code.

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


## [Functions](https://dart.dev/guides/language/language-tour#functions)

- Dart support **top level** function => you can define functions outside any class defintion that can be called from anywhere in the code.
- Dart is true OO language => Function are objects and have a type, [Function](https://api.dart.dev/stable/2.17.3/dart-core/Function-class.html)
- This means that functions can be assigned to variables or passed as arguments to other functions. 
- You can also call an instance of a Dart class as if it were a [function](https://dart.dev/guides/language/language-tour#callable-classes).

Syntax

```js

returnType functionName(parameters) {
    return returnvalue;
}

```

- If a function have `void` return type, `return` is not required.


```js
double squre(double n) {
    return n*n;
}
```

- Although return type of function should be mentiond but in dart, it's not equired.



## Function Parameters

- A function can have any number of `required positional` parameters. 
- These can be followed either by `named parameters` or by `optional positional parameters` (but not both).

### Positional Parameters

- A positional parameter is a parameter whose meaning depends on its **position** in the parameter list. 
- When you create a new Text object, the characters to be displayed must **always** come first in the list.

```js
Text("Hello world!", textScaleFactor: 4.0)  // correct
Text(textScaleFactor: 4.0, "Hello world!") // wrong
```


### Named Parameters

- Named parameters are `optional unless` they’re `explicitly` marked as `required`.
- A named parameter is a parameter whose **meaning** depends on the word before the **colon**.
- A Text constructor call can have many different named parameters, such as textScaleFactor, style, and maxLines.
- You can write the named parameters **in any order** as long as they **come after any of the positional parameters**.
- If you wrap the parameters in **curly braces**, you’ll make them **named** and **optional**.


```js
double calculate({}) {
    return value;
}

Text("Hello world!", 
    textScaleFactor: 4.0,    
    style: TextStyle(fontSize: 28.0));

```

### The Arrow Notation

- If function is composed of one instruction, you can use **the arrow** notation.

```js

int square(int n) {
    return n*n;
}

int square(int n) => n*n;

```

### Anonymous Functions and Closures

- They are functions defined as variables.

## main Function

- `main` is the function called when any kind of Dart program, including Flutter app.
- It has `void` return type, and it takes no arguments.
- It can be `async`.


# Reference
- https://dart.dev/guides/language/language-tour
