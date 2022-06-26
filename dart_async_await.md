# Async/concurrent Coding in Dart

- Dart is a single threaded language.
  
- It still support, future, async/await, streams, and background work to work in modern aysnc envinment and in reactive way.

- Dart supports concurrent programming with `async-await`, `isolates`, and classes such as `Future` and `Stream`.


## [Isolates](https://dart.dev/guides/language/concurrency)

- In Dart, all code runs in an `isolate`.

- Each Dart isolate has a `single thread` of execution and `shares no mutable objects` with other isolates.

- To `communicate` with each other, isolates use `message passing`.

- Many Dart apps use only **one isolate** (the `main` isolate)

- You can create **additional** isolates, enabling parallel code execution on multiple processor cores.


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




