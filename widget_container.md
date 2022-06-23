# Container

## Why you need this widget?

1. It help your widget to get background style (color, shape, size etc), padding, margin.
2. It help you compose, decoreate, and position child widgets.

## How to use it.

- If you wrap your container widget without any parameter, it would not do anything => You will not see any differernce in appearance.
- And container size itself to child size.

```js
container(
    child: Text('Hello World')
)
```

## Adding background color to container child

- Use `color` property.

```js
container(
    child: Text('Hello World'),
    color: Colors.blue
)
```

## Add Space between child widget and container boundary

- Use `padding` property.

```js
    Container(
      color: Colors.blue,
      padding: const EdgeInsets.all(20.0),
      child: const Text('Hello World'),
    );
```

## Add Empty space around the container

- Use `margin` property.

```js
    Container(
      color: Colors.blue,
      padding: const EdgeInsets.all(20.0),
      margin: const EdgeInsets.all(20.0),
      child: const Text('Hello World'),
    );
```

## Add shape to your container

- Use `decoration` property.
- Color property can't be used when you use decoration property.
- It's by defaule sized to container child.

```js
    Container(
      // color: Colors.blue,
      padding: const EdgeInsets.all(20.0),
      margin: const EdgeInsets.all(20.0),
      decoration: const BoxDecoration(
        color: Colors.blue,
        shape: BoxShape.rectangle,
      ),
      child: const Text('Hello World'),
    );
```

## Align the child within container

- Use `alignment` property.
- When you set the alignment, container will **expand** to fit it's parent height and width.
- We can **override** this by setting height and width of the container **OR** use **box** layout model.

```js

    Container(
      // color: Colors.blue,
      padding: const EdgeInsets.all(40.0),
      margin: const EdgeInsets.all(40.0),
      // width: 200,
      // height: 200,
      constraints: const BoxConstraints.tightForFinite(width: 200, height: 200),
      alignment: Alignment.center,
      decoration: const BoxDecoration(
        color: Colors.blue,
        shape: BoxShape.circle,
      ),
      child: const Text('Hello World'),
    );

```

## Transform (e.g; rotate) container

- Use `transform` property.







# References

- https://api.flutter.dev/flutter/widgets/Container-class.html
- https://www.youtube.com/watch?v=c1xLMaTUWCY
- https://www.youtube.com/watch?v=X47zIAGIJNE