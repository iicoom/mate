# mate

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://flutter.dev/docs/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://flutter.dev/docs/cookbook)

For help getting started with Flutter, view our
[online documentation](https://flutter.dev/docs), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

## StatelessWidget && StatefulWidget

## 页面结构
用到的是这个包：
```
import 'package:flutter/material.dart';
```
> 常见组件

### Scaffold(脚手架)
这个是页面的总体结构，包括了 AppBar、SafeArea、... 可以点击进去查看学习

### Container
应该是使用最频繁的组件，类似于网页设计的div。
```
Container(
  width: double.infinity,
  height: 200,
  decoration: BoxDecoration(
    color: Color.fromRGBO(253, 230, 240, 1)
  ),
  child: ListView(
    scrollDirection: Axis.horizontal,
    children: [
      card('assets/images/1.png'),
    ],
  ),
),
```

### ListView
如上在 Container 中的使用。

### SizedBox

### Button
```
leading: IconButton(
          icon: Icon(Icons.menu, color: Colors.black87,),
          onPressed: () {},
        )
```

### 图片的使用
在 pubspec.yaml 中配置：
```
flutter:

  # The following line ensures that the Material Icons font is
  # included with your application, so that you can use the icons in
  # the material Icons class.
  uses-material-design: true

  # To add assets to your application, add an assets section, like this:
  assets:
     - assets/images/
```

### image, AssetImage
```
Container(
    decoration: BoxDecoration(
    color: Colors.orange,
    borderRadius: BorderRadius.circular(20),
    image: DecorationImage(
      fit: BoxFit.cover,
      image: AssetImage(image)
    ),
),
```
更详细的参数可以点击索引查看。

## 颜色的使用
```
backgroundColor: Color.fromRGBO(244, 243, 243, 1),

backgroundColor: Colors.white,
```

## 图标的使用
https://api.flutter.dev/flutter/material/Icons-class.html

```
leading: IconButton(
          icon: Icon(Icons.menu, color: Colors.black87,),
        )
```
