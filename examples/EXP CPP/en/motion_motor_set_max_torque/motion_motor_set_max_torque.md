category: motion  
signature: MOTOR.setMaxTorque(50, percent);
device_class: motor  
description: Sets the EXP Smart Motor or Motor Group's max torque.  

# Motor Set Max Torque

Sets the EXP Smart Motor or Motor Group's maximum torque output.  

```cpp
Motor.setMaxTorque(value, percent);
```

## How To Use

`Motor.setMaxTorque` accepts a range of **0% to 100%**.

The first part of the command is the device instance.

```cpp
ClawMotor.setMaxTorque(25, percent);
ArmMotor.setMaxTorque(75, percent);
```

## Example

This example will spin the ClawMotor to the 40-degree position with only 20% maximum torque. This allows the Claw to grab an object without too much force.

```cpp
ClawMotor.setMaxTorque(20, percent);
ClawMotor.spinToPosition(40, degrees);

<advanced>
</advanced>