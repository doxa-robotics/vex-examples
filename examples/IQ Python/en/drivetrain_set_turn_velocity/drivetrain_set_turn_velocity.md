category: drivetrain
signature: drivetrain.set_turn_velocity(VELOCITY, UNITS)  
description: Sets the Drivetrain's turn velocity  

# Set Turn Velocity

Sets the Drivetrain's turn velocity.

```python
drivetrain.set_turn_velocity(VELOCITY, UNITS)
```

## How To Use

`Set Turn Velocity` will set the velocity of the Drivetrain when turning, but will not cause the Drivetrain to move when used without a `Turn` or `Turn For` command.

`Set Turn Velocity` accepts a range of values depending on what units are passed as the second parameter.

If `PERCENT` is used as the second parameter, **VELOCITY** accepts a range from **-100 to 100**.

Alternatively, `Set Turn Velocity` can also use `RPM` as a valid **UNITS** parameter, accepting a range from **-127 to 127** as the **VELOCITY** parameter.

Setting a Drivetrain's turn velocity to a negative value will cause the Drivetrain to turn in the opposite of the direction passed into any following `drivtrain.turn` commands.

Setting a Drivetrain's turn velocity to 0 will prevent the Drivetrain from turning.

## Example

In this example, the Drivetrain will turn in the opposite direction (LEFT) due to a negative turn velocity.

```python
drivetrain.set_turn_velocity(-100, PERCENT)
drivetrain.turn(RIGHT)
```

<advanced>
</advanced>
