- [Variables](#variables)
  - [Variable declarion syntax](#variable-declarion-syntax)
  - [Final and const Variables](#final-and-const-variables)
    - [Final Variables](#final-variables)
    - [Const Variables](#const-variables)
    - [Const Value](#const-value)
    - [Note](#note)
  - [Immutable Variables: final and const](#immutable-variables-final-and-const)
    - [final keyword](#final-keyword)
    - [const keyword](#const-keyword)
- [Reference](#reference)

# [Variables](https://dart.dev/guides/language/language-tour#variables)

- Dart supports **top-level** variables, as well as variables tied to a class (**static** variables) or object (**instance** variables). 

- **Instance** variables are sometimes known as `fields or properties`.

- When you want to explicitly say that any type is allowed, use the type **Object?** (if you’ve enabled **null safety**), **Object**, or—if you must defer type checking until runtime—the special type dynamic.

- Everything you can place in a variable is an **object**, and every object is an instance of a class. 

- Even numbers, functions, and null are objects. 
  
- With the exception of null (if you enable sound null safety), all objects inherit from the **Object** class.
  
  
## Variable declarion syntax

- **Prefix** the variable with data type, and then variable name comes.

```js
data_type variable_name = intial_value;
int a = 3;
var a = 3;
```

## [Final and const Variables](https://dart.dev/guides/language/language-tour#final-and-const)

- If you never intend to change a variable, use `final or const`. These unchangeable variables are known as **immutable**.

### Final Variables

- `final` means single-assignment: a final variable or field *must* have an `initializer`.
   
- Once assigned a value, a final variable's value `cannot` be changed.

- A `final` variable can be **set only once**. 
  
- They are **runtime constant** (value of these variables are known when program is running e.g; you are getting the value from the server or it's the timestamp value etc)

```js
final hoursSinceMidnight = DateTime.now().hour;

final name = 'Bob'; // Without a type annotation
final String nickname = 'Bobby';

name = 'Alice'; // Error: a final variable can only be set once.
```

### Const Variables


- A `const` variable is a `compile-time` constant (Const variables are **implicitly** `final`) - (value that can be determined by the compiler **before** the program ever starts running.)

```js
const bar = 1000000; // Unit of pressure (dynes/cm2)
const double atm = 1.01325 * bar; // Standard atmosphere
```

- If you can’t create a `const` variable because you don’t know its value at compile time, then you must use the `final` keyword to make it a `runtime constant`.

### Const Value

- You have learned about `const variables`, but dart introduce the concept of `const values`.

- You can use it when creating **collections**, like `const [1, 2, 3]`, and when **constructing objects** (instead of new) like `const Point(2, 3).`

- Here, const means that the object's **entire deep state** can be determined entirely at compile time and that the object will be frozen and completely immutable.

- You `can't change` the value `assigned to variable` but you can `assign new value` to the variable.

```
var foo = const [];
final bar = const [];
const baz = []; // Equivalent to `const []`

foo = [1, 2, 3];    // ALLOWED because foo is not not declare const
foo.add(4);         // NOT ALLOWED because values is declared constant.
```

### Note

- A `final` **object** cannot be modified, its fields can be changed. 
  
- A `const` object and its fields **cannot** be changed: they’re **immutable**.

- `Instance variables` can be final but **not const**.

- You can define constants that use [type checks and casts (is and as)](https://dart.dev/guides/language/language-tour#type-test-operators), [collection if](https://dart.dev/guides/language/language-tour#collection-operators), and [spread operators (... and ...?)](https://dart.dev/guides/language/language-tour#spread-operator)


// NOTE: Need more explaination

```js
const Object i = 3; // Where i is a const Object with an int value...
const list = [i as int]; // Use a typecast.
const map = {if (i is int) i: 'int'}; // Use is and collection if.
const set = {if (list is List<int>) ...list}; // ...and a spread.
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


# Reference

- https://dart.dev/guides/language/language-tour#variables
- https://news.dartlang.org/2012/06/const-static-final-oh-my.html

