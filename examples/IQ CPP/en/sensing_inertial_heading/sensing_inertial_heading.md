category: sensing  
signature: INERTIAL.heading(degrees)  
device_class: inertial  
description: Reports the IQ (2nd generation) Brain Inertial Sensor's current heading in degrees.

# Inertial Heading

Reports the IQ (2nd generation) Brain Inertial Sensor's current heading in degrees.

```cpp
BrainInertial.heading(degrees)
```

## How To Use

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon

The `BrainInertial.heading(degrees)` command reports an increase in heading when rotating clockwise.

`BrainInertial.heading(degrees)` reports a range from **0.00 to 359.99 degrees**

```cpp
Drivetrain.turn(right);
waitUntil(BrainInertial.heading(degrees) > 180);
Drivetrain.stop();
```
<advanced>
</advanced>
