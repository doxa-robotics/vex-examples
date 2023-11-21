category: motion  
signature: MOTOR.setTimeout(1, seconds);  
device_class: motor  
description: Sets the V5 Smart Motor or or Motor Group's timeout to stop if a blocking command never reaches its target.  

# Motor Set Timeout

Sets the V5 Smart Motor or Motor Group's timeout to stop if a blocking command never reaches its target.  

```cpp
Motor.setTimeout(time, seconds);
```

## How To Use

The `Motor.setTimeout();` is used to prevent movement commands that do not reach their position from preventing other commands in the stack from running. An example of a Motor not reaching its position is an arm or claw that reaches its mechanical limit and cannot complete its movement.

Set the timeout by specifying the amount of time in `seconds`.

## Example

This example will end the `Motor.spinToPosition();` command after 2 second if the ClawMotor has not reached the position of 270 degrees. 

Once the time limit or target is reached, the ClawMotor will move to position 0 degrees.

```cpp
ClawMotor.setTimeout(2, seconds);
ClawMotor.spinToPosition(270, degrees);
ClawMotor.spinToPosition(0, degrees);
```

<advanced>
</advanced>