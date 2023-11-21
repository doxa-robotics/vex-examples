category: drivetrain
signature: drivetrain.set_rotation(0, DEGREES)  
description: Sets the Drivetrain's Inertial or Gyro Sensor to a specified rotation  

# Set Rotation

Sets the Drivetrain's Inertial or Gyro Sensor to a specified rotation.

```python
drivetrain.set_rotation(ROTATION, DEGREES)
```

## How To Use

The Drivetrain's `Set Rotation` command can be used to set the Drivetrain's angle of rotation to any given positive or negative value.

The `ROTATION` parameter can accept numeric values.

The `ROTATION` parameter **does not** have a limit of 0-359 degrees.

## Example

This example will turn the robot a total of 210 degrees if the Drivetrain is configured with the IQ (2nd generation) Brain's Inertial Sensor.

```python
drivetrain.turn_to_rotation(120, DEGREES)
drivetrain.set_rotation(-45, DEGREES)
drivetrain.turn_to_rotation(45, DEGREES)
```

- Turn right (clockwise) to rotation 120 degrees.
- Set the robot's current position as rotation of -45 degrees.
- Turn right (clockwise) an additional 90 degrees (-45 degrees to +45 degrees) based on the set rotation value from the previous command.

<advanced>
</advanced>
