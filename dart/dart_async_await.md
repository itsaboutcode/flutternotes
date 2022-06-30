- [Async/concurrent Coding in Dart](#asyncconcurrent-coding-in-dart)
  - [Isolates](#isolates)
  - [Future Functions](#future-functions)
    - [Handling Future Functions](#handling-future-functions)
      - [Async/Await Method](#asyncawait-method)
      - [.then method](#then-method)
    - [Handling Error](#handling-error)
- [References](#references)

# Async/concurrent Coding in Dart

- Dart is a single threaded language.
  
- It still supports future, async/await, streams, and background work to work in a modern async environment and in a reactive way.

- Dart supports concurrent programming with `async-await`, `isolates`, and classes such as `Future` and `Stream`.


## [Isolates](https://dart.dev/guides/language/concurrency)

- In Dart, all code runs in an `isolate`.

- Each Dart isolate has a `single thread` of execution and `shares no mutable objects` with other isolates.

- To `communicate` with each other, isolates use `message passing`.

- Many Dart apps use only **one isolate** (the `main` isolate)

- You can create **additional** isolates, enabling parallel code execution on multiple processor cores.


## [Future Functions](https://api.dart.dev/stable/2.17.5/dart-async/Future-class.html)

- These functions are **asynchronous**: they return after setting up a possibly time-consuming operation (such as I/O), without waiting for that operation to complete.

- A future is `defined` exactly like a function in dart.
  
- If the function return type is `void`, you use `Future` as return type. 
  
- If you want to return a `value` from the Future then you pass it a type.


```js
Future myVoidFuture() {}

Future<bool> myTypedFuture() {}
```

### Handling Future Functions

#### Async/Await Method

- To call Future function, you use the `await` keyword and the function `from which` you are calling this future function must be marked as `async`.

```js

Future actualCalc() {
    return 2+2
}

Future<int> calculate() async {
    return await actualCalc();
}

void main() async {

    var calc = await calculate();
    
}

```

#### .then method

```js

    calculate().then((return_value){})

```

### Handling Error


# References

- [Concurrency in Dart](https://dart.dev/guides/language/concurrency)
- [Asynchrony support](https://dart.dev/guides/language/language-tour#asynchrony-support)
- [Asynchronous programming: Streams](https://dart.dev/tutorials/language/streams)
- [Asynchronous programming: futures, async, await](https://dart.dev/codelabs/async-await)
- [Isolates and Event Loops | Flutter in Focus](https://www.youtube.com/watch?v=vl_AaCgudcY)
- [Dart Futures | Flutter in Focus](https://www.youtube.com/watch?v=OTS-ap9_aXc)
- [Dart Streams | Flutter in Focus](https://www.youtube.com/watch?v=nQBpOIHE4eE)
- [Async/Await | Flutter in Focus](https://www.youtube.com/watch?v=SmTCmDMi4BY)
- [Generator Functions | Flutter in Focus](https://www.youtube.com/watch?v=TF-TBsgIErY)
- [Async vs Isolates | Decoding Flutter](https://www.youtube.com/watch?v=5AxWC49ZMzs)




