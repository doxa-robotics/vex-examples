category: sensing  
signature: Drivetrain.current()  
device_class: drivetrain  
description: Reports the amount of current that the Drivetrain is currently using.

# Drivetrain Current

Reports the amount of current that the Drivetrain is currently using.

```cpp
Drivetrain.current(amp)
```

## How To Use
`Drivetrain.current(amp)` returns a decimal value (as a *double*) to report the amount of current a V5 Drivetrain is currently using.

The default unit is amps (`amp`) that returns a value from **0.0 to 2.5 amps**.

```cpp
Brain.Screen.print("%f", Drivetrain.current(amp));
```

<advanced>
</advanced>