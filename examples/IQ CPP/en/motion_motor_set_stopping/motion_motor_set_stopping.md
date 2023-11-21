category: motion  
signature: Motor.setStopping(brake);  
device_class: motor  
description: Sets the Motor or Motor Group's brake mode.  

# Motor Set Stopping

Sets the behavior of the VEX IQ Smart Motor or Motor Group once it stops moving.

```cpp
Motor.setStopping(brakeType);
```

## How To Use

The first part of the command is the device instance.

```cpp
ClawMotor.setStopping(brake);
ArmMotor.setStopping(hold);
```

Specify the Motor/Motor Group's stopping behavior:

- **brake** will cause the Motor/Motor Group to come to an immediate stop.
- **coast** will spin the Motor/Motor Group gradually to a stop.
- **hold** will cause the Motor/Motor Group to come to an immediate stop and returns it to its initial stopped position if moved.

The `Motor.setStopping` command will affect the behavior of subsequent `Motor.stop` commands until otherwise changed.

## Example

This example will spin the ArmMotor forward for 90 degrees and then will resist outside forces (like gravity) to hold its position.

```cpp
ArmMotor.setStopping(hold);
ArmMotor.spinFor(forward, 90, degrees);
```

<advanced>
</advanced>