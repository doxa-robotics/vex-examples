category: drivetrain  
signature: drivetrain.set_drive_velocity(VELOCITY, PRECENT)  
description: Sets the velocity of the Drivetrain that will be used for drive() and drive_for() commands.

# Set Drive Velocity

Sets the velocity of the Drivetrain for `drive` and `drive_for` commands.

```python
drivetrain.set_drive_velocity(VELOCITY, UNITS)
```

## How To Use

`drivetrain.set_drive_velocity` will set the Drivetrain's velocity when used with a `drive` or `drive_for` command. It will not cause the Drivetrain to move when used by itself.

`drivetrain.set_drive_velocity` accepts a range of values depending on what units are passed as the second parameter.

If `PERCENT` is used as the second parameter, **VELOCITY** accepts a range from **-100 to 100**.

`drivetrain.set_drive_velocity` can also use `RPM` as a valid **UNITS** parameter. Based on the Gear Cartridge installed in the V5 Smart Motors used in the Drivetrain, the range of acceptable **VELOCITY** values can vary.

* Red Cartridge: -100rpm to 100rpm
* Green Cartridge: -200rpm to 200rpm
* Blue Cartridge: -600rpm to 600rpm

Setting a Drivetrain's drive velocity to a negative value will cause the Drivetrain to drive opposite of the `DIRECTION` passed into a `drive` or `drive_for` command.

Setting a Drivetrain's drive velocity to 0 will prevent the Drivetrain from moving even if a `drive` or `drive_for` command is used.

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
