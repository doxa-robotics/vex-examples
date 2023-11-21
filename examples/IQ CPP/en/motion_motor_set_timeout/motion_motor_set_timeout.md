category: motion  
signature: Motor.setTimeout(1, seconds);  
device_class: motor  
description: Sets the Motor or Motor Group's timeout to stop if a blocking command never reaches its target.  

# Motor Set Timeout

Sets a VEX IQ Smart Motor or Motor Group's timeout to stop if a blocking command never reaches its target.  

```cpp
Motor.setTimeout(time, seconds);
```

## How To Use

The `Motor.setTimeout` command is used to prevent Motor movements that do not reach their intended position from preventing other commands in the program from running. 

An example of a Motor not reaching its position is an Arm or Claw that reaches its mechanical limit and cannot complete its movement.

Set the timeout by specifying the amount of time in **seconds**.

## Example

This example will end the `Motor.spinToPosition` command after 2 seconds if the ClawMotor has not reached the intended position of 270 degrees. 

Once the timeout or target is reached, the ArmMotor will spin to 90 degrees.

```cpp
ClawMotor.setTimeout(2, seconds);
ClawMotor.spinToPosition(270, degrees);
ArmMotor.spinToPosition(90, degrees);
```

<advanced>
</advanced>