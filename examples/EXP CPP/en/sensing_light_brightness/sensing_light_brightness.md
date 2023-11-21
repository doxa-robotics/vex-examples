category: sensing  
signature: LIGHT.brightness()  
device_class: light  
description: Reports the amount of light detected by the Light Sensor.

# Light Brightness

Reports the amount of light detected by the Light Sensor.

```cpp
Light.brightness()
```

## How To Use

`Light.brightness()` reports a range from **0% to 100%**.

A large amount of light detected will report a high brightness value.

A small amount of light detected will report a low brightness value.

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

The default unit is `percent` that returns an integer value from **0% to 100%**.

```cpp
Brain.Screen.print("%d", LightC.brightness());
```
<advanced>
</advanced>