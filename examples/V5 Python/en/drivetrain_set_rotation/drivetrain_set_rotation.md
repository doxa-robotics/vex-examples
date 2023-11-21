category: drivetrain
signature: drivetrain.set_rotation(0, DEGREES)  
description: Sets the Drivetrain's angle of rotation with a Gyro Sensor.

# Set Rotation

Sets the drivetrain's angle of rotation with a Gyro Sensor.

```don
drivetrain.set_rotation(ROTATION, UNITS)
```

## How To Use

The `drivetrain.set_rotation` command can be used to set the Drivetrain's angle of rotation to any given positive or negative value.

The `ROTATION` parameter can accept numeric values.

The `ROTATION` parameter **does not** have a limit of 0-359 degrees.

## Example

This example will turn the robot a total of 210 degrees:

```don
drivetrain.turn_to_rotation(120, DEGREES)
drivetrain.set_rotation(-45, DEGREES)
drivetrain.turn_to_rotation(45, DEGREES)
```

- Turn right (clockwise) to rotation 120 degrees.
- Set the robot's current position as rotation of -45 degrees.
- Turn right (clockwise) an additional 90 degrees (-45 degrees to +45 degrees) based on the set rotation value from the previous command.

<advanced>
</advanced>
