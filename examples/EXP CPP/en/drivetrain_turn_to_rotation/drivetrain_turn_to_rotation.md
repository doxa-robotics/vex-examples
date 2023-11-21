category: drive 
signature: Drivetrain.turnToRotation(90, degrees);  
device_class: smartdrive  
description: Turns a Drivetrain to a specific angle of rotation when configured with a 3-Wire Gyro Sensor or Inertial Sensor.  

# Drivetrain Turn To Rotation

Turns a Drivetrain to a specific angle of rotation when configured with a 3-Wire Gyro Sensor, Inertial Sensor BrainInertial.

`Drivetrain.turnToRotation(rotation, units);`

## How To Use

The Drivetrain will have a clockwise-positive rotation, meaning that rotation will increase as the Drivetrain turns right.

Based on the current rotation of the Drivetrain, `Drivetrain.turnToRotation` will determine which direction to turn.

The `rotation` parameter is **not** limited to **0 to 359.99 degrees**. Turns will be absolute and may cause the robot to rotate more than once if necessary.

## Example

This example will cause the Drivetrain to make four turns:

```cpp
Drivetrain.turnToRotation(90.0, degrees);
Drivetrain.turnToRotation(180, degrees);
Drivetrain.turnToRotation(-45, degrees);
Drivetrain.turnToRotation(0, degrees);
```

- Right to 90 degrees
- Right to 180 degrees
- Left to -45 degrees
- Right to 0 degrees

The `Drivetrain.turnToRotation`command will by default block other commands until the Drivetrain turn has completed.

## Optional Parameters

You can set `false` as the last parameter to prevent the `Drivetrain.turnToRotation` command from blocking the program until the turn has completed.

```cpp
Drivetrain.turnToRotation(180.0, degrees, false);
```


<advanced>
</advanced>