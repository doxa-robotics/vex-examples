category: drive 
signature: Drivetrain.turnToRotation(90, degrees);  
device_class: smartdrive  
description: Turns a Drivetrain to a specific angle of rotation when configured with a VEX IQ Gyro or Brain Inertial Sensor.

# Turn To Rotation

Turns a Drivetrain to a specific angle of rotation when configured with a VEX IQ Gyro or Brain Inertial Sensor.

```cpp
Drivetrain.turnToRotation(rotation, degrees);
```

## How To Use

### IQ (1st generation) Brain

The `Drivetrain.turnToRotation` command can be used to turn the Drivetrain to a given positive (counter-clockwise) or negative (clockwise) value.

### IQ (2nd generation) Brain

The `Drivetrain.turnToRotation` command can be used to turn the Drivetrain either in a counter-clockwise or clockwise rotation depending on whether the integrated inertial or a gyro sensor is configured in the Drivetrain configuration.

If the Drivetrain is configured with the integrated inertial sensor, the Drivetrain will have a clockwise-positive rotation, meaning that rotation will increase as the Drivetrain turns right.

Alternatively, if the Drivetrain is configured with a gyro sensor, the Drivetrain will have a counter-clockwise-positive rotation, meaning that rotation will increase as the Drivetrain turns left.

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

- Left (counter-clockwise) to 90 degrees
- Left (counter-clockwise) to 180 degrees
- Right (clockwise) to -45 degrees
- Left (counter-clockwise) to 0 degrees

(The clockwise/counter-clockwise motions described above are based on an IQ (1st generation) Brain + Drivetrain configuration, or an IQ (2nd generation) Brain + Drivetrain configuration with a gyro sensor)

The `Drivetrain.turnToRotation`command will by default block other commands until the Drivetrain turn has completed.

## Optional Parameters

You can set `false` as the last parameter to prevent the `Drivetrain.turnToRotation` command from blocking the program until the turn has completed.

```cpp
Drivetrain.turnToRotation(180.0, degrees, false);
```

<advanced>
</advanced>
