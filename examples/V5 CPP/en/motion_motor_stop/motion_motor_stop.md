category: motion  
signature: MOTOR.stop();  
device_class: motor  
description: Stops the V5 Smart Motor or Motor Group.  

# Motor Stop

Stops the V5 Smart Motor or Motor Group.

```cpp
Motor.stop();
```

## How To Use

The `Motor.stop();` command will cause the V5 Smart Motor or Motor Group to come to a complete stop and use the `Motor.setStopping();` to set either `coast`, `brake`, or `hold` its position.

## Example

This example will spin the ClawMotor open for 3 seconds before stopping.

```cpp
ClawMotor.spin(forward);
wait(3, seconds);
ClawMotor.stop();
```

<advanced>
</advanced>