category: sensing  
signature: INERTIAL.rotation(degrees)  
device_class: inertial
description: Reports the IQ (2nd generation) Brain Inertial Sensor's current angle of rotation in degrees.

# Inertial Rotation

Reports the IQ (2nd generation) Brain Inertial Sensor's current angle of rotation in degrees.

```cpp
BrainInertial.rotation(degrees)
```

## How To Use

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

The `BrainInertial.rotation(degrees)` command reports an increasingly **positive** value when the Inertial Sensor turns in the **clockwise** direction.

`BrainInertial.rotation(degrees)` reports an increasingly **negative** value when the Inertial Sensor turns in the **counter-clockwise** direction.

```cpp
Drivetrain.turn(right);
waitUntil(BrainInertial.rotation(degrees) > 180);
Drivetrain.stop();
```

<advanced>
</advanced>
