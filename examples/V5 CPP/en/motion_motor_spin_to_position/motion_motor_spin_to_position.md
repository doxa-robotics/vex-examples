category: motion  
signature: MOTOR.spinToPosition(90, degrees);  
device_class: motor  
description: Spins the V5 Smart Motor or Motor Group to a position.  

# Motor Spin To Position

Spins the V5 Smart Motor or Motor Group to a specific rotational position.

```cpp
Motor3.spinToPosition(rotation, units);
```

## How To Use

`Motor.spinToPosition();` will tell a Motor or Motor Group to travel to a specific position. Based on the current position of the Motor or Motor Group, `Motor.spinToPosition();` will determine the direction to rotate.

The `Motor.spinToPosition();` accepts numeric values for `rotation`.

Set the position to travel to by providing the `rotation` to any number. 

You can specify the units of the rotation in either `degrees` or `turns`. 

The **spinToPosition** command will block other commands until the V5 Smart Motor or Motor Group movement has completed.

## Optional Parameters

You can set `false` as the last parameter to tell the **spinToPosition** command to not block the program until the movement has completed.

```cpp
Motor.spinToPosition(360, degrees, false);
```

<advanced>
</advanced>