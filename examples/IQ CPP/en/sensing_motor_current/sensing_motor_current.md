category: sensing  
signature: Motor.current(units)  
device_class: motor  
description: Reports the amount of current a Motor or Motor Group is currently using.

# Motor Current

Reports the amount of current a VEX IQ Smart Motor or Motor Group is currently using.

```cpp
Motor.current(units)
```

## How To Use

`Motor.current` returns a decimal value (as a *double*) to report the amount of current a Motor or Motor Group is using.

The `Motor.current` command accepts **amp** (Amperes) as a valid `units` parameter.

Prints the Motor/Motor Group's current in Amperes:

```cpp
Brain.Screen.print("%f", Motor.current(amp));
```

<advanced>
</advanced>