---
title: How to remove all routes from the Navigator in Flutter
publish_date: 2022-11-10
---

### Helpful for designing functionality of a Logout button

```dart
Navigator.of(context).pushNamedAndRemoveUntil(
    '/desiredNamedRoute',
    (Route<dynamic> route) => false,
  );
```
