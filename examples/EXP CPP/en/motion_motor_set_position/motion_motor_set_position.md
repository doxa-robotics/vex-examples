category: motion  
signature: MOTOR.setPosition(0, degrees);  
device_class: motor  
description: Sets the EXP Smart Motor or Motor Group's encoder(s) to a position.  

# Motor Set Position

Sets the EXP Smart Motor or Motor Group's encoder(s) to a specified position.

```cpp
Motor.setPosition(position, units);
```

## How To Use

The `Motor.setPosition` command can be used to set a Motor or Motor Group's position to any given positional value.

The first part of the command is the device instance.

```cpp
ClawMotor.setPosition(0, degrees);
ArmMotor.setPosition(90, degrees);
```

Usually, the `Motor.setPosition` command is used to set the position to 0 to reset a Motor or Motor Group's encoder position(s).

Provide the `units` as either **degrees** or **turns**.

## Example

This example will set the ClawMotor's position to 50 degrees.

```cpp
ClawMotor.setPosition(50, degrees);
```

<advanced>
</advanced>