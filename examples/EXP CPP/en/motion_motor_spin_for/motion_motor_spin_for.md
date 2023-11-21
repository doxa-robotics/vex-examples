category: motion  
signature: MOTOR.spinFor(forward, 90, degrees);  
device_class: motor  
description: Spins the EXP Smart Motor or Motor Group for a given distance.  

# Motor Spin For

Spins an EXP Smart Motor or Motor Group for a given distance.

```cpp
Motor.spinFor(direction, rotation, units);
```

## How To Use

`Motor.spinFor` will spin an EXP Smart Motor or Motor Group in the given direction for a given distance.

Possible arguments:

- `direction` accepts either **forward** or **reverse**
- `rotation` accepts numeric values
- `units` accepts either **degrees** or **turns**

The `Motor.spinFor` command will block other commands until the motor movement has completed.

## Optional Parameters

You can set `false` as the last parameter to tell the `Motor.spinFor` command to not block the program until the movement has completed.

```cpp
Motor.spinFor(reverse, 360, degrees, false);
```

<advanced>
</advanced>
