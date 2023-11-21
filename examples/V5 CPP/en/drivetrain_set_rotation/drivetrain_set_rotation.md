category: drive
signature: Drivetrain.setRotation(90, degrees);  
device_class: smartdrive  
description: Sets the Drivetrain's angle of rotation when configured with a 3-Wire Gyro Sensor or V5 Inertial Sensor.

# Drivetrain Set Rotation

Sets the Drivetrain's angle of rotation when configured with a 3-Wire Gyro Sensor or V5 Inertial Sensor.

```cpp
Drivetrain.setRotation(rotation, degrees);
```

## How To Use

The `Drivetrain.setRotation()` command can be used to set the Drivetrain's angle of rotation to any given positive or negative value.

The `Drivetrain.setRotation()` command can accept integers or numeric commands

The `Drivetrain.setRotation()` command **does not** have a limit of 0-359 degrees.

This example will turn the robot a total of 210 degrees:

```cpp
Drivetrain.turnToRotation(120, degrees);
Drivetrain.setRotation(-45, degrees);
Drivetrain.turnToRotation(45, degrees);
```

- Turn right (clockwise) to rotation 120 degrees.
- Set the robot's current position as rotation of -45 degrees.
- Turn right (clockwise) an additional 90 degrees (-45 degrees to +45 degrees) based on the set rotation value from the previous command.

<advanced>
</advanced>
