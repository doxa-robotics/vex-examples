category: motion  
signature: motor.set_timeout(TIME, SECONDS)  
description: Sets a time limit for the V5 Smart Motor or Motor Group movement commands.

# Set Motor Timeout

Sets a time limit for the V5 Smart Motor or Motor Group movement commands.

```python 
motor.set_timeout(TIME, SECONDS)
```

## How To Use

A Motor or Motor Group's is used to prevent motion commands that do not reach their position from preventing subsequent commands from running. 

An example of a Motor not reaching its position is an Arm or Claw that reaches its mechanical limit and cannot complete its movement.

## Example

This example will set the timeout of the `spin_to_position` commands to 2 seconds.

If the Claw Motor has not reached the position of 270 degrees after 2 seconds, the Claw Motor will stop spinning.

```python
claw_motor.set_timeout(2, SECONDS)
claw_motor.spin_to_position(270, DEGREES)
```

<advanced>
</advanced>
