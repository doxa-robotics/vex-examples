category: sensing  
signature: Drivetrain.rotation()  
device_class: smartdrive  
description: Reports the Drivetrain's angle of rotation when configured with a 3-Wire Gyro Sensor or EXP Inertial Sensor.

# Drivetrain Rotation

Reports the Drivetrain's angle of rotation when configured with a 3-Wire Gyro Sensor, EXP Inertial Sensor or EXP BrainInertial Sensor.

```cpp
Drivetrain.rotation()
```

## How To Use

`Drivetrain.rotation()`reports a **positive** value when the Drivetrain turns in a **clockwise** direction.

`Drivetrain.rotation()` reports a **negative** value when the Drivetrain turns in a **counter-clockwise** direction.

```cpp
waitUntil(Drivetrain.rotation() > 180);
```
<advanced>
</advanced>
