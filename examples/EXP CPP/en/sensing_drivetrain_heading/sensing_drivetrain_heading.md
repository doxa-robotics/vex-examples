category: sensing  
signature: Drivetrain.heading()  
device_class: smartdrive  
description: Reports the 3-Wire Gyro Sensor or EXP Inertial Sensor's current heading in degrees.

# Drivetrain Heading

Reports the 3-Wire Gyro Sensor or EXP Inertial Sensor's current heading in degrees.

```cpp
Drivetrain.heading()
```

## How To Use
Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

The `Drivetrain.heading()` command reports an increase in heading when rotating clockwise.

`Drivetrain.heading()` reports a range from **0.00 to 359.99**.

```cpp
waitUntil(Drivetrain.heading() > 180);
```
<advanced>
</advanced>
