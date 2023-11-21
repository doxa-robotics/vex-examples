category: sensing  
signature: Brain.Battery.current()
description: Reports the current of the V5 Brain's battery.

# Brain Battery Current

Reports the current of the V5 Brain's battery.

```cpp
Brain.Battery.current()
```

## How To Use
Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

`Brain.Battery.current()` returns a decimal value (as a *double*) to report the current of the V5 Brain's battery.

The default unit is amps (`amp`) that returns a value from **0.0 to 20.0 amps**.

```cpp
Brain.Screen.print("%f", Brain.Battery.current());
```
<advanced>
</advanced>