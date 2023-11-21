category: motion  
signature: MOTOR.spin(forward);  
device_class: motor  
description: Spins a EXP Smart Motor or Motor Group in a direction until stopped.  

# Motor Spin
Spins an EXP Smart Motor or Motor Group in a direction until stopped.

```cpp
Motor.spin(direction);
```

## How To Use

The `Motor.spin` command will spin an EXP Smart Motor or Motor Group forever until a new motion command is used or the program is stopped.

- **forward** spins the Motor forward.
- **reverse** spins the Motor in reverse.

```cpp
Motor.spin(forward);
Motor.spin(reverse);
```

<advanced>
</advanced>