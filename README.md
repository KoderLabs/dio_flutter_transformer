# dio_flutter_transformer [![Pub](https://img.shields.io/pub/v/dio_flutter_transformer.svg?style=flat-square)](https://pub.dartlang.org/packages/dio_flutter_transformer)

A [dio](https://github.com/flutterchina/dio) transformer especially for flutter, by which the json decoding will be in background with [compute] function.

> Through practical experience, we find that although using `compute` can make tasks go on in the background, it may lead to slow task execution. So please think carefully before using it.


## Install

```yaml
dio_flutter_transformer:
    git:
      url: https://github.com/KoderLabs/dio_flutter_transformer
      ref: master
```

## Usage

Import the package:

```dart
import 'package:dio/dio.dart';
import 'package:dio_flutter_transformer/dio_flutter_transformer.dart';
```

Then replace dio default transformer: 

```dart

var dio=Dio();
dio.transformer = FlutterTransformer(); // replace dio default transformer
dio.get(...);
```

