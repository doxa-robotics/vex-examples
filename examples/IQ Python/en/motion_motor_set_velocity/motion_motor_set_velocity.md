category: motion  
signature: motor.set_velocity(VELOCITY, UNITS)  
description: Sets the speed of an IQ Motor or Motor Group  

# Set Motor Velocity

Sets the speed of an IQ Motor or Motor Group.

```python 
motor.set_velocity(VELOCITY, UNITS)
```

## How To Use

This command accepts a range from **-100 to 100** when used with the `PERCENT` parameter or **-127 to 127** when used with `RPM`.

Setting an IQ Motor or Motor Group's velocity to a negative value will cause the Motor/Motor Group to spin in reverse.

Setting the velocity to 0 will prevent the Motor/Motor Group from spinning.

## Example

This example will set the Arm Motor to spin at 25% speed to the 90 degree position.

```python
arm_motor.set_velocity(25, PERCENT)
arm_motor.spin_to_position(90, DEGREES)
```

<advanced>
</advanced>
