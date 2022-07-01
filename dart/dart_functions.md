- [Functions](#functions)
  - [Function Parameters](#function-parameters)
    - [Positional Parameters](#positional-parameters)
    - [Named Parameters](#named-parameters)
    - [The Arrow Notation](#the-arrow-notation)
    - [Anonymous Functions and Closures](#anonymous-functions-and-closures)
  - [main Function](#main-function)
- [Reference](#reference)

# [Functions](https://dart.dev/guides/language/language-tour#functions)

- Dart support **top level** function => you can define functions outside any class definition that can be called from anywhere in the code.

- Dart is true OO language => Function are objects and have a type, [Function](https://api.dart.dev/stable/2.17.3/dart-core/Function-class.html)

- This means that functions can be assigned to variables or passed as arguments to other functions. 

- You can also call an instance of a Dart class as if it were a [function](https://dart.dev/guides/language/language-tour#callable-classes).

Syntax

```js

returnType functionName(parameters) {
    return returnvalue;
}

```

- If a function has a `void` return type, `return` is not required.


```js
double square(double n) {
    return n*n;
}
```

- Although the return type of function should be mentioned but in dart, it's not required.


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

- If a function is composed of one instruction, you can use **the arrow** notation.

```js

int square(int n) {
    return n*n;
}

int square(int n) => n*n;

```

### Anonymous Functions and Closures

- They are functions defined as variables.

## main Function

- The special, **required**, top-level function where app execution starts.
- `main` is the function called when any kind of Dart program, including Flutter app.
- It has a `void` return type, and it takes no arguments.
- It can be `async`.

# Reference