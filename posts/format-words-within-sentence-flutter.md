---
title: How to use multiple text styles in Flutter
publish_date: 2022-11-11
---

User Flutter's built-in `RichText` widget to display text with multiple different styles.

```dart
RichText(
  text: TextSpan(
    text: 'Hello ',
    style: DefaultTextStyle.of(context).style,
    children: const <TextSpan>[
      TextSpan(text: 'Blue & Bold', style: TextStyle(fontWeight: FontWeight.bold, color: Colors.red)),
      TextSpan(text: ' world!'),
    ],
  ),
)
```

Output:

![Red & Bold text example](/assets/post/rich-text.png)

More info: [RichText Class](https://api.flutter.dev/flutter/widgets/RichText-class.html)
