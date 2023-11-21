category: drivetrain  
signature: drivetrain.set_drive_velocity(VELOCITY, UNITS)  
description: Sets the velocity of the Drivetrain that will be used for `Drive` and `Drive For` commands  

# Set Drive Velocity

Sets the velocity of the Drivetrain for `Drive` and `Drive For` commands.

```python
drivetrain.set_drive_velocity(VELOCITY, UNITS)
```

## How To Use

`Set Drive Velocity` will set the Drivetrain's velocity when used with a `Drive` or `Drive For` command. It will not cause the Drivetrain to move when used by itself.

`Set Drive Velocity` accepts a range of values depending on what units are passed as the second parameter.

If `PERCENT` is used as the second parameter, **VELOCITY** accepts a range from **-100 to 100**.

`Set Drive Velocity` can also use `RPM` as a valid **UNITS** parameter, accepting a range from **-127 to 127**.

Setting a Drivetrain's drive velocity to a negative value will cause the Drivetrain to drive opposite of the `DIRECTION` passed into a `Drive` or `Drive For` command.

Setting a Drivetrain's drive velocity to 0 will prevent the Drivetrain from moving even if a `Drive` or `Drive For` command is used.

## Example

This example shows that the Drivetrain will go in reverse due to a negative value.

```python
drivetrain.set_drive_velocity(-100, PERCENT)
drivetrain.drive(FORWARD)
```

This example will prevent the Drivetrain from moving.

```python
drivetrain.set_drive_velocity(0, PERCENT)
drivetrain.drive(FORWARD)
```

<advanced>
</advanced>
