category: sensing  
signature: MOTOR.current()  
device_class: motor  
description: Reports the amount of current a EXP Smart Motor or Motor Group is currently using in amperes (amps).

# Motor Current

Reports the amount of current a EXP Smart Motor or Motor Group is currently using in amperes (amps).

```cpp
Motor.current(amp)
```

## How To Use

`Motor.current()` returns a decimal value (as a *double*) to report the amount of current a EXP Smart Motor or Motor Group is currently using.

The default unit is amps (`amp`) that returns a value from **0.0 to 2.5 amps**.

```cpp
Brain.Screen.print("%f", ClawMotor.current(amp));
```

<advanced>
</advanced>