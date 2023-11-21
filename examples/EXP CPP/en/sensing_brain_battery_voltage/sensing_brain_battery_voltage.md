category: sensing  
signature: Brain.Battery.voltage()  
description: Reports the voltage of the EXP Brain's battery.  

# Brain Battery Voltage

Reports the voltage of the EXP Brain's battery.

```cpp
Brain.Battery.voltage()
```

## How To Use
Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

`Brain.Battery.voltage()` returns a decimal value (as a *double*) that reports the voltage of the EXP Brain's battery. 

The default unit is `volt`, and the command will return a value in the range of **6.0 volts to 9.0 volts**.

```cpp
Brain.Screen.print("%f", Brain.Battery.voltage());
```

<advanced>
</advanced>