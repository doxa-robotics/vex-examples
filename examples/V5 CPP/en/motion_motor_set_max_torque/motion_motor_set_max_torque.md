category: motion  
signature: MOTOR.setMaxTorque(50, percent);
device_class: motor  
description: Sets the V5 Smart Motor or Motor Group's max torque.  

# Motor Set Max Torque

Sets the V5 Smart Motor or Motor Group's maximum torque output.  

```cpp
Motor.setMaxTorque(value, units);
```

## How To Use

`Motor.setMaxTorque();` accepts a torque range of **0 to 100** using `percent` units.

## Example

This example will spin the ClawMotor to the 40 degree position with only 20% maximum torque. This allows the claw to grab an object without damaging it with too much force.

```cpp
ClawMotor.setMaxTorque(20, percent);
ClawMotor.spinToPosition(40, degrees);
```

<advanced>
</advanced>