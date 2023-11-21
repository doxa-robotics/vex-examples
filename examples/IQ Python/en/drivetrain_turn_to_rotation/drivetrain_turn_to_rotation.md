category: drivetrain
signature: drivetrain.turn_to_rotation(90, DEGREES, wait=True)
description: Turns the Drivetrain to a specific angle of rotation when used with a Gyro or Inertial Sensor  

# Turn To Rotation

Turns the Drivetrain to a specific angle of rotation when used with a Gyro or Inertial Sensor.

```python
drivetrain.turn_to_rotation(ROTATION, DEGREES)
```

## How To Use

The `Turn to Rotation` command can be used to turn the Drivetrain to an absolute rotation value.

Depending on whether the Drivetrain is configured with a Gyro or Inertial Sensor, rotation values can either be counter-clockwise positive (Gyro), or clockwise positive (Inertial).

Based on the current rotation of the Drivetrain, `Turn to Rotation` will determine which direction to turn.

The `ROTATION` parameter can accept numeric values.

Numeric values are **not** limited to the range of **0 - 359.99** degrees. Turns will be absolute and may cause the robot to rotate more than once if necessary.

## Example

This example will cause the Drivetrain to make four turns:

```python
drivetrain.turn_to_rotation(90.0, DEGREES)
drivetrain.turn_to_rotation(180, DEGREES)
drivetrain.turn_to_rotation(-45, DEGREES)
drivetrain.turn_to_rotation(0, DEGREES)
```

- Right (clockwise) to 90 degrees
- Right (clockwise) to 180 degrees
- Left (counter-clockwise) to -45 degrees
- Right (clockwise) to 0 degrees

(The direction descriptions above are aligned with an IQ (2nd generation) Brain's Inertial Sensor being configured with the Drivetrain)

The `Turn to Rotation`command will by default block proceeding commands until the Drivetrain turn has completed.

## Optional Parameter

You can set a third parameter to  `wait=False` to prevent the `Turn to Rotation` command from blocking proceeding commands until the Drivetrain turn is completed.

```python
drivetrain.turn_to_rotation(180.0, DEGREES, wait=False)
```

<advanced>
</advanced>
