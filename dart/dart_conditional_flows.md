- [Conditional Flows](#conditional-flows)
  - [`If` and `Else`](#if-and-else)
  - [`for` loops](#for-loops)
  - [`while` and `do-while` loops](#while-and-do-while-loops)
  - [`break` and `continue`](#break-and-continue)
  - [`switch` and `case`](#switch-and-case)
  - [`assert`](#assert)
  - [Exceptions](#exceptions)
- [Reference](#reference)

# [Conditional Flows](https://dart.dev/guides/language/language-tour#control-flow-statements)

## `If` and `Else`

```js
if (isRaining()) {
  you.bringRainCoat();
} else if (isSnowing()) {
  you.wearJacket();
} else {
  car.putTopDown();
}
```


## `for` loops

```js
var message = StringBuffer('Dart is fun');
for (var i = 0; i < 5; i++) {
  message.write('!');
}
```

- If the object that you are iterating over is an `Iterable (such as List or Set)` and 
- if you `don’t need to know the current iteration counter`, you can use the `for-in`
  

```js
for (final candidate in candidates) {
  candidate.interview();
}
```

- Iterable `classes` also have a `forEach()` method as another option.

```js
var collection = [1, 2, 3];
collection.forEach(print); // 1 2 3
```


## `while` and `do-while` loops


```js

while (!isDone()) {
  doSomething();
}
```

```js
do {
  printLine();
} while (!atEndOfPage());
```


## `break` and `continue`

- `break` stop looping.

```js
while (true) {
  if (shutDownRequested()) break;
  processIncomingRequests();
}
```

- `continue` skip to the next loop iteration.

```js
for (int i = 0; i < candidates.length; i++) {
  var candidate = candidates[i];
  if (candidate.yearsExperience < 5) {
    continue;
  }
  candidate.interview();
}
```

## `switch` and `case`

- Switch statements in Dart compare `integer, string, or compile-time` constants using `==`.

- The compared objects must all be `instances of the same class` (and not of any of its subtypes), 
- and the class `must not` override ==.

## `assert`

- `assert` terminates the execution if the condition in its parentheses isn’t true (only in testing/debug mode). 
  
- It's not effective in production code.

## [Exceptions](dart_exceptions.md)

- You can also affect the control flow using try-catch and throw.

# Reference

- https://dart.dev/guides/language/language-tour#control-flow-statements