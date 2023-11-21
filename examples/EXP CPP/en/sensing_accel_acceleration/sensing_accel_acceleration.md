category: sensing  
signature: ACCEL.acceleration()  
device_class: accelerometer  
description: Reports the acceleration value from one axis on the Analog Accelerometer.

# Accelerometer Acceleration

Reports the acceleration value from one axis (x, y, or z) on the Analog Accelerometer.

The X-axis reports the acceleration value from the horizontal axis and the Y-axis reports the acceleration value from the vertical axis. The Z-axis reports upward acceleration.

```cpp
Accel2G.acceleration()
```

## How To Use

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

`Accelerometer.acceleration()` returns a decimal value (as a *double*) that ranges from **-2.0 G to 2.0 G** or **-6.0 G to 6.0 G** depending upon the jumper setting on the Analog Accelerometer.

1.0 G is equivalent to 9.8 meters per second squared.

```cpp
Brain.Screen.print("%f", Accel2GB.acceleration());
```
<advanced>
</advanced>