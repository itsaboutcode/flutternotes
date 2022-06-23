# Dart

- [Dart](#dart)
  - [Comments](#comments)
    - [Single-line comments](#single-line-comments)
    - [Multi-line comments](#multi-line-comments)
    - [Documentation comments](#documentation-comments)
  - [Data Types](#data-types)
    - [Void](#void)
    - [var](#var)
  - [Variable](#variable)
    - [Variable declarion syntax](#variable-declarion-syntax)
  - [Null safety](#null-safety)
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
  - [Control flow statements](#control-flow-statements)
    - [If and else](#if-and-else)
    - [For loops](#for-loops)
    - [While and do-while](#while-and-do-while)
    - [Break and continue](#break-and-continue)
    - [Switch and case](#switch-and-case)
    - [Assert](#assert-1)
  - [Exceptions](#exceptions)
    - [Throw](#throw)
    - [Catch](#catch)
    - [Finally](#finally)
  - [Functions](#functions)
  - [Function Parameters](#function-parameters)
    - [Positional Parameters](#positional-parameters)
    - [Named Parameters](#named-parameters)
    - [The Arrow Notation](#the-arrow-notation)
    - [Anonymous Functions and Closures](#anonymous-functions-and-closures)
  - [main Function](#main-function)
  - [Classes](#classes)
    - [Using class members](#using-class-members)
    - [Using constructors](#using-constructors)
    - [Class variables and methods](#class-variables-and-methods)
      - [Static variables](#static-variables)
      - [Static methods](#static-methods)
  - [Async Coding in Dart](#async-coding-in-dart)
- [Reference](#reference)

Dart is a Object Oriented programming language which resemables Java.

## Comments

- Dart supports single-line comments, multi-line comments, and documentation comments.

### Single-line comments

- A single-line comment begins with //. 
  
- Everything between // and the end of line is ignored by the Dart compiler.

```js
void main() {
  // TODO: refactor into an AbstractLlamaGreetingFactory?
  print('Welcome to my Llama farm!');   // This is a comment
}
```

### Multi-line comments

- A multi-line comment begins with /* and ends with */. 

- Everything between /* and */ is ignored by the Dart compiler

```js

void main() {
  /*
   * This is a lot of work. Consider raising chickens.

  Llama larry = Llama();
  larry.feed();
  larry.exercise();
  larry.clean();
   */
}

```

### Documentation comments

- Documentation comments are multi-line or single-line comments that begin with /// or /**. 

- Using /// on consecutive lines has the same effect as a multi-line doc comment.


```js
/// A domesticated South American camelid (Lama glama).
///
/// Andean cultures have used llamas as meat and pack
/// animals since pre-Hispanic times.
///
/// Just like any other animal, llamas need to eat,
/// so don't forget to [feed] them some [Food].
```


---


## Data Types

### Void
- A special type that indicates a value that’s never used. 

### var
- A way to declare a variable without specifying its type.


## Variable

- Dart supports **top-level** variables, as well as variables tied to a class or object (**static** and **instance** variables). 

- Instance variables are sometimes known as fields or properties.

- When you want to explicitly say that any type is allowed, use the type **Object?** (if you’ve enabled **null safety**), **Object**, or—if you must defer type checking until runtime—the special type dynamic.

= Everything you can place in a variable is an **object**, and every object is an instance of a class. 

- Even numbers, functions, and null are objects. 
  
- With the exception of null (if you enable sound null safety), all objects inherit from the **Object** class.
  
  
### Variable declarion syntax

- **Prefix** the variable with data type, and then variable name comes.

```js

data_type variable_name = intial_value;

int a = 3;

var a = 3;
```

## [Null safety](https://dart.dev/null-safety)

- If you enable **null safety**, variables can’t contain null unless you say they can. 

- You can make a variable **nullable** by putting a **question mark (?)** at the end of its type. For example, a variable of type **int?** might be an integer, or it might be null. 

- If you know that an expression never evaluates to null but Dart disagrees, you can add **!** to assert that it isn’t null (and to throw an exception if it is). An example: **int x = nullableButNotNullInt!**

- **Uninitialized** variables that have a **nullable type** have an initial value of **null**. 

- https://www.youtube.com/watch?v=iYhOU9AuaFs&list=PLjxrf2q8roU3wk7CDw4RfV3mEwOJbjx1k&index=10

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

---

## Control flow statements

### If and else

### For loops

### While and do-while

### Break and continue

### Switch and case

### Assert

---

## Exceptions

### Throw

### Catch

### Finally

---

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

- The special, **required**, top-level function where app execution starts.
- `main` is the function called when any kind of Dart program, including Flutter app.
- It has `void` return type, and it takes no arguments.
- It can be `async`.

---


## Classes

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

---




## [Async Coding in Dart](dart_async_await.md)

# Reference
- https://dart.dev/guides/language/language-tour
