# SeparatedRow

<img alt="Pub" src="https://img.shields.io/pub/v/separated_row.svg">

Flutter package for rendering separated Row children.

## Usage

The only difference between `SeparatedRow` and `Row` is the `separatorBuilder` property.

```dart
SeparatedRow(
  children: <Widget>[
    IconButton(
      onPressed: () {},
      icon: Icon(Icons.favorite),
    ),
    IconButton(
      onPressed: () {},
      icon: Icon(Icons.favorite_border),
    ),
    IconButton(
      onPressed: () {},
      icon: Icon(Icons.check),
    ),
    IconButton(
      onPressed: () {},
      icon: Icon(Icons.close),
    ),
  ],
  separatorBuilder: (BuildContext context, int index) {
    return Container(
      width: 1.0,
      height: 15.0,
      color: Colors.grey,
    );
  },
  mainAxisAlignment: MainAxisAlignment.spaceEvenly,
)
```