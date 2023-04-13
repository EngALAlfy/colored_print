Flutter library to print objects to console with colors

## Features

- colors support

## Getting started

TODO: List prerequisites and provide or point to information on how to
start using the package.

## Usage

### Import package
```dart
import 'colored_print/flutter_colored_print.dart' as c_l;
```

### Use it to print anything
Use `log` method to control type as `LogType` and color as `LogColor`
```dart
c_l.log("This is test colored log to console" ,type: LogType.info , color: LogColor.cyan);
```

#### Output
<pre style="color: cyan">
[Info] This is test colored log to console
</pre>

If you set `allColored` to `true` (as default) whole message will colored

#### set `allColored` to  `false`

```dart
c_l.log("This is test colored log to console" ,type: LogType.info , color: LogColor.blue , allColored:false);
```
#### Output
<pre style="color: blue">
<span style="color:cyan;">[Info]</span> This is test colored log to console
</pre>

### Or use typed methods
```dart
c_l.error("This is error");

c_l.info("This is info");

c_l.warn("This is warning");

c_l.primary("This is primary");
```

<pre >
    <p style="color: red;margin: 0;padding: 0">[Error] This is error</p>
    <p style="color: cyan;margin: 0;padding: 0">[Info] This is info</p>
    <p style="color: yellow;margin: 0;padding: 0">[Warning] This is warning</p>
    <p style="color: blue;margin: 0;padding: 0">[Primary] This is primary</p>
</pre>