category: sensing  
signature: INERTIAL.rotation(degrees)  
device_class: inertial
description: Reports the EXP Inertial Sensor's current angle of rotation in degrees.

# Inertial Rotation

Reports the EXP Inertial Sensor's current angle of rotation in degrees.

```cpp
Inertial.rotation(degrees)
```

## How To Use

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

The `Inertial.rotation(degrees)` reports a **positive** value when the Inertial Sensor turns in the **clockwise** direction.

`Inertial.rotation(degrees)` reports a **negative** value when the Inertial Sensor turns in the **counter-clockwise** direction.

```cpp
waitUntil(Inertial20.rotation(degrees) > 180);
```
<advanced>
</advanced>
