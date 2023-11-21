category: sensing  
signature: GYRO.heading(degrees)  
device_class: gyro  
description: Reports the 3-Wire Gyro Sensor's current heading in degrees.

# Gyro Heading

Reports the 3-Wire Gyro Sensor's current heading in degrees.

```cpp
Gyro.heading(degrees)
```

## How To Use
Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

The `Gyro.heading(degrees)` command reports an increase in heading when rotating clockwise.

`Gyro.heading(degrees)` reports a range from **0.00 to 359.99**.

```cpp
waitUntil(Gyro.heading(degrees) > 180);
```
<advanced>
</advanced>