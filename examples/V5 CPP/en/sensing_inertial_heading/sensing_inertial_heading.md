category: sensing  
signature: INERTIAL.heading(degrees)  
device_class: inertial  
description: Reports the V5 Inertial Sensor's current heading in degrees.

# Inertial Heading

Reports the V5 Inertial Sensor's current heading in degrees.

```cpp
Inertial.heading(degrees)
```

## How To Use

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon

The `Inertial.heading(degrees)` command reports an increase in heading when rotating clockwise.

`Inertial.heading(degrees)` reports a range from **0.00 to 359.99 degrees**

```cpp
waitUntil(Inertial.heading(degrees) > 180);
```
<advanced>
</advanced>
