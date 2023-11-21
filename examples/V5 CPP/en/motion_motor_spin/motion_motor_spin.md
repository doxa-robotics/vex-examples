category: motion  
signature: MOTOR.spin(forward);  
device_class: motor  
description: Spins a V5 Smart Motor or Motor Group in a direction until stopped.  

# Motor Spin
Spins a V5 Smart Motor or Motor Group in a direction until stopped.

```cpp
Motor.spin(directionType);
```

## How To Use

The `Motor.spin();` can run a V5 Smart Motor or Motor Group forever until a new motor command is used or the program is stopped.

Use the `forward` parameter to drive the V5 Smart Motor or Motor Group in the forward direction.

```cpp
Motor.spin(forward);
```

Use the `reverse` parameter to drive the V5 Smart Motor or Motor Group in the reverse direction.

```cpp
Motor.spin(reverse);
```

<advanced>
</advanced>