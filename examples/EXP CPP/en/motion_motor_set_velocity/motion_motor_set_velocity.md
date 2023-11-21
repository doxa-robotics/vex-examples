category: motion  
signature: MOTOR.setVelocity(50, percent);  
device_class: motor  
description: Sets the EXP Motor or Motor Group's velocity.  

# Motor Set Velocity

Sets the speed of an EXP Smart Motor or Motor Group.

```cpp
Motor.setVelocity(velocity, units);
```

## How To Use

`Motor.setVelocity` accepts a range of **-100% to 100%** or **-127rpm to 127rpm**.

Setting a Motor or Motor Group's velocity to a negative value will cause the Motor/Motor Group to spin in reverse.

Setting a Motor or Motor Group's velocity to 0 will cause the Motor/Motor Group to stop.

The first part of the command is the device instance.

```cpp
ClawMotor.setVelocity(25, percent);
ArmMotor.setVelocity(75, percent);
```

Specify if the velocity `units` is set to either **percent** or **rpm** (revolutions per minute).

## Example

This example will set the ClawMotor to spin at 25% speed to the 90-degree position.

```cpp
ClawMotor.setVelocity(25, percent);
ClawMotor.spinToPosition(90, degrees);
```


<advanced>
</advanced>