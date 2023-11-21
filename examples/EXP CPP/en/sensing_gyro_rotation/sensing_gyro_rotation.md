category: sensing  
signature: GYRO.rotation(degrees)  
device_class: gyro  
description: Reports the 3-Wire Gyro Sensor's current angle of rotation in degrees.

# Gyro Rotation

Reports the 3-Wire Gyro Sensor's current angle of rotation in degrees.

```cpp
Gyro.rotation(degrees)
```

## How To Use

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

The `Gyro.rotation(degrees)` command reports a **positive** value when the Gyro turns in a **clockwise** direction.

`Gyro.rotation(degrees)` reports a **negative** value when the Gyro Sensor turns in the **counter-clockwise** direction.

```cpp
waitUntil(Gyro.rotation(degrees) > 180);
```
<advanced>
</advanced>
