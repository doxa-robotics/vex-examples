category: drivetrain
signature: drivetrain.set_turn_velocity(VELOCITY, PERCENT)  
description: Sets the Drivetrain's turn velocity.

# Set Turn Velocity

Sets the Drivetrain's turn velocity.

```python
drivetrain.set_turn_velocity(VELOCITY, UNITS)
```

## How To Use

`drivetrain.set_turn_velocity` will set the velocity of the Drivetrain when turning, but will not cause the Drivetrain to move when used without a `turn` or `turn_for` command.

`drivetrain.set_turn_velocity` accepts a range of values depending on what units are passed as the second parameter.

If `PERCENT` is used as the second parameter, **VELOCITY** accepts a range from **-100 to 100**.

Alternatively, `drivetrain.set_turn_velocity` can also use `RPM` as a valid **UNITS** parameter. Based on the Gear Cartridge installed in the V5 Smart Motors used in the Drivetrain, the range of acceptable **VELOCITY** values can vary.

* Red Cartridge: -100rpm to 100rpm
* Green Cartridge: -200rpm to 200rpm
* Blue Cartridge: -600rpm to 600rpm

Setting a Drivetrain's turn velocity to a negative value will cause the Drivetrain to turn in the opposite of the direction passed into any following turn commands.

Setting a Drivetrain's turn velocity to 0 will prevent the Drivetrain from turning, even when using a `turn` or `turn_for` command.

## Example

In this example, the Drivetrain will turn in the opposite direction (LEFT) due to a negative value.

```python
drivetrain.set_turn_velocity(-100, PERCENT)
drivetrain.turn(RIGHT)
```

<advanced>
</advanced>
