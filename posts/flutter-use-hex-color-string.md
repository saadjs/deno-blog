---
title: Use Hex color strings ("#808080") instead of ARGB integer (0xFF808080)
publish_date: 2023-01-30
---

## Extend `Color` class

```dart
class HexColor extends Color {
  static int _contructARBG(String hexStr) {
    hexStr = hexStr.replaceAll("#", "");
    if (hexStr.length == 6) {
      hexStr = "FF$hexStr";
    }
    return int.parse(hexStr, radix: 16);
  }

  HexColor(final String hexStr) : super(_contructARBG(hexStr));
}
```

## Usage

```dart
Color gray = HexColor("808080");
// OR
Color gray = HexColor("#808080");
```
