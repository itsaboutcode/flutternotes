- [The Backslah](#the-backslah)
- [String Interpolation](#string-interpolation)

# The Backslah

- The backslash can be used to **escape** some characters or **insert** special characters.

For example if you wanted to print `"` in a string, you have 2 options.

1. Create literal string in `''` and add `""` inside it.

```js
'Hello "World"'
```

2. Escape the quotes using `\"`.

```js
"Hello \"World\""
// Output will be
// Hello "World" 
```

3. Adding a special character to add the next line, escape `\n`.

```js

"First Line\nSecond Line"
// Output will be 
// First Line
// Second Line
```

4. Escaping \ itself

```js
"Hello \\ World" 
// Output 
// Hello \ World
```

# String Interpolation

- String interpolation allows you to **insert** one or more **variables** values into a string. 

- By prefixing a variable’s name with **$**, you can insert its value into the string.


```js

int times = 5;
int more = 10;

"You clicked on this button $times times. To complete this challenge, click $more more times"

// Output
// You clicked on this button 5 times. To complete this challenge, click 10 more times.
```

- If you need to access an element of a List, the member of a class, or write any kind of expression, you need to enclose the statement in **curly braces**.

```js

List numbers = [1, 2, 3];

"There are ${numbers.length} elements and second element is number ${numbers[1]}"

// Output
// There are 3 elements and second element is number 2

```