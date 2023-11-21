category: motion  
signature: Motor.stop();  
device_class: motor  
description: Stops a Motor or Motor Group.  

# Stop Motor

Stops a VEX IQ Smart Motor or Motor Group.

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