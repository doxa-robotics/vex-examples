category: drivetrain
signature: drivetrain.turn_to_rotation(90, DEGREES, wait=True)
description: Turns the Drivetrain to a specific angle of rotation..  

# Turn To Rotation

Turns the Drivetrain to a specific angle of rotation.

`drivetrain.turn_to_rotation(ROTATION, DEGREES)`

## How To Use

The `drivetrain.turn_to_rotation` command can be used to turn the Drivetrain to a given positive (clockwise) or negative (counter-clockwise) value.

Based on the current rotation of the Drivetrain, `drivetrain.turn_to_rotation` will determine which direction to turn.

The `ROTATION` parameter can accept numeric values.

Numeric values are **not** limited to the range of **0 - 359.99** degrees. Turns will be absolute and may cause the robot to rotate more than once if necessary.

## Example

This example will cause the Drivetrain to make four turns:

```don
drivetrain.turn_to_rotation(90.0, DEGREES)
drivetrain.turn_to_rotation(180, DEGREES)
drivetrain.turn_to_rotation(-45, DEGREES)
drivetrain.turn_to_rotation(0, DEGREES)
```

- Right (clockwise) to 90 degrees
- Right (clockwise) to 180 degrees
- Left (counter-clockwise) to -45 degrees
- Right (clockwise) to 0 degrees

The `drivetrain.turn_to_rotation`command will by default block proceeding commands until the Drivetrain turn has completed.

## Optional Parameter

You can set a third parameter to  `wait=False` to prevent the `turn_to_rotation` command from blocking proceeding commands until the Drivetrain turn is completed.

```don
drivetrain.turn_to_rotation(180.0, DEGREES, wait=False)
```

<advanced>
</advanced>
