category: motion  
signature: MOTOR.setStopping(brake);  
device_class: motor  
description: Sets the V5 Smart Motor or or Motor Group's brake mode.  

# Motor Set Stopping

Sets the V5 Smart Motor or or Motor Group's brake mode. 

```cpp
Motor.setStopping(brakeType);
```

## How To Use

Here are possible `brakeType` inputs that you can specify: 

* `brake` will cause the Motor or Motor Group to come to an immediate stop, and will not correct for outside forces.
* `coast` lets the Motor or Motor Group to spin gradually to a stop.
* `hold` will cause the Motor or Motor Group to come to an immediate stop, and returns it to its stopped position if moved by an outside force, by using the built-in encoder.

## Example

This example will make the ArmMotor move forward for 90 degrees and then will resist outside forces (like gravity) to hold its position.

```cpp
ArmMotor.setStopping(hold);
ArmMotor.spinFor(90, degrees);
```

<advanced>
</advanced>