category: motion  
signature: MOTOR.spinToPosition(90, degrees);  
device_class: motor  
description: Spins the EXP Smart Motor or Motor Group to a position.  

# Motor Spin To Position

Spins the EXP Smart Motor or Motor Group to a specific rotational position.

```cpp
Motor3.spinToPosition(rotation, units);
```

## How To Use

`Motor.spinToPosition` will tell an EXP Smart Motor or Motor Group to spin to a specific position.

Based on the current position of the Motor/Motor Group, `Motor.spinToPosition` will determine the direction to spin.

The `Motor.spinToPosition` command accepts numeric values for `rotation`.

You can specify the `units` of the rotation in either **degrees** or **turns**. 

The `Motor.spinToPosition` command will block other commands until the motor movement has completed.

## Optional Parameters

You can set `false` as the last parameter to tell the `Motor.spinToPosition` command to not block the program until the movement has completed.

```cpp
Motor.spinToPosition(360, degrees, false);
```

<advanced>
</advanced>