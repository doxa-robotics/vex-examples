category: motion  
signature: motor.set_max_torque(50, PERCENT)  
description: Sets the strength of an IQ Motor or Motor Group  

# Set Motor Torque

Sets the strength of an IQ Motor or Motor Group.

```python
motor.set_max_torque(AMOUNT, PERCENT)
```

## How To Use

This command accepts a range of **0 to 100** for the **AMOUNT** parameter.

The `Set Max Torque` command can accept decimals, integers, or numeric values.

## Example

This example will spin the Claw Motor to the 40 degree position with only 20% maximum torque. This allows the claw to grab an object without damaging it with too much force.

```python
claw_motor.set_max_torque(20, PERCENT)
claw_motor.spin_to_position(40, DEGREES)
```

<advanced>
</advanced>
