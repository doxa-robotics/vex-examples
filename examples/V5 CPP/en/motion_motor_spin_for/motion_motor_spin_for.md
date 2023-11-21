category: motion  
signature: MOTOR.spinFor(forward, 90, degrees);  
device_class: motor  
description: Spins the V5 Smart Motor or Motor Group for a given distance.  

# Motor Spin For

Spins the V5 Smart Motor or Motor Group in a given direction for a specific amount of rotation.

```cpp
Motor.spinFor(directionType, rotation, units);
```

## How To Use

`Motor.spinFor();` will tell a Motor or Motor Group to travel in a given direction (`forward` or  `reverse`), for a given distance, from where it is currently located.

The `Motor.spinFor();` accepts numeric values for `rotation`.

Set the distance to travel by providing the `rotation` to any number. 

You can specify the units of the rotation in either `degrees` or `turns`. 

The **spinFor** command will block other commands until the V5 Smart Motor or Motor Group movement has completed.

## Optional Parameters

You can set `false` as the last parameter to tell the **spinFor** command to not block the program until the movement has completed.

```cpp
Motor.spinFor(forward, 360, degrees, false);
```

<advanced>
</advanced>
