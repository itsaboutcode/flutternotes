- [Comments](#comments)
  - [Single-line comments](#single-line-comments)
  - [Multi-line comments](#multi-line-comments)
  - [Documentation comments](#documentation-comments)
- [Reference](#reference)

# [Comments](https://dart.dev/guides/language/language-tour#comments)

- Dart supports single-line comments, multi-line comments, and documentation comments.

## Single-line comments

- A single-line comment begins with //. 
  
- Everything between // and the end of line is ignored by the Dart compiler.

```js
void main() {
  // TODO: refactor into an AbstractLlamaGreetingFactory?
  print('Welcome to my Llama farm!');   // This is a comment
}
```

## Multi-line comments

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

## Documentation comments

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


# Reference