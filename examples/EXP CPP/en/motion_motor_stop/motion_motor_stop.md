category: motion  
signature: MOTOR.stop();  
device_class: motor  
description: Stops the EXP Smart Motor or Motor Group.  

# Motor Stop

Stops the EXP Smart Motor or Motor Group.

```cpp
Motor.stop();
```

## How To Use

The first part of the command is the device instance.

```cpp
ClawMotor.stop();
ArmMotor.stop();
``` 

## Example

This example will spin the ClawMotor open for 3 seconds before stopping.

```cpp
ClawMotor.spin(forward);
wait(3, seconds);
ClawMotor.stop();
```

<advanced>
</advanced>