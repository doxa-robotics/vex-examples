category: drive 
signature: Drivetrain.turnToRotation(90, degrees);  
device_class: smartdrive  
description: Turns a Drivetrain to a specific angle of rotation when configured with a 3-Wire Gyro Sensor or V5 Inertial Sensor.  

# Drivetrain Turn To Rotation

Turns a Drivetrain to a specific angle of rotation when configured with a 3-Wire Gyro Sensor or V5 Inertial Sensor.

`Drivetrain.turnToRotation(rotation, units);`

## How To Use

The `Drivetrain.turnToRotation();` command can be used to turn the Drivetrain to a given positive (clockwise) or negative (counter-clockwise) value.

Based on the current **rotation** value of the Drivetrain, `Drivetrain.turnToRotation();` will determine which direction to turn.

`Drivetrain.turnToRotation();` can accept decimals, integers, or numeric units.

`Drivetrain.turnToRotation();` is **not** limited to 0-359.99 degrees. Turns will be absolute and may cause the robot to rotate more than once if necessary.

## Example

This example will cause the Drivetrain to make four turns:

```cpp
Drivetrain.turnToRotation(90.0, degrees);
Drivetrain.turnToRotation(180, degrees);
Drivetrain.turnTorotation(-45, degrees);
Drivetrain.turnToRotation(0, degrees);
```

- Right (clockwise) to 90 degrees
- Right (clockwise) to 180 degrees
- Left (counter-clockwise) to -45 degrees
- Right (clockwise) to 0 degrees

The `Drivetrain.turnToRotation();`command will block other commands until the Drivetrain turn has completed.

## Optional Parameters

You can set `false` as the last parameter to tell the `Drivetrain.turnToRotation();` command to not block the program until the movement has completed.

```cpp
Drivetrain.turnToRotation(180.0, degrees, false);
```

<advanced>
</advanced>