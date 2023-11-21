category: motion  
signature: motor.set_velocity(VELOCITY, UNITS)  
description: Sets the speed of a V5 Smart Motor or Motor Group.

# Set Motor Velocity

Sets the speed of a V5 Smart Motor or Motor Group.

```python 
motor.set_velocity(VELOCITY, UNITS)
```

## How To Use

This command accepts a range from **-100% to 100%** or **-600rpm to 600rpm.**

Acceptable `UNITS` parameter is either `PERCENT` or `RPM`.

**Set motor velocity** will accept a "rotations per minute" (RPM) value based on the Gear Cartridge installed in the V5 Smart Motor or Motor Group used.

* Red Cartridge: -100rpm to 100rpm
* Green Cartridge: -200rpm to 200rpm
* Blue Cartridge: -600rpm to 600rpm

Setting a V5 Smart Motor's velocity to a negative value will cause the Motor/Motor Group to spin in reverse.

Setting a V5 Smart Motor's velocity to 0 will prevent the Motor/Motor Group from spinning.

## Example

This example will set the Arm Motor to spin at 25% speed to the 90 degree position.

```python
arm_motor.set_velocity(25, PERCENT)
arm_motor.spin_to_position(90, DEGREES)
```

<advanced>
</advanced>
