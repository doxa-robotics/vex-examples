category: sensing  
signature: MOTOR.power()  
device_class: motor  
description: Reports the amount of power output the V5 Smart Motor or Motor Group is currently generating.

# Motor Power

Reports the amount of power output a V5 Smart Motor or the first motor of a Motor Group is currently generating.

```cpp
Motor.power(watt)
```

## How To Use

`Motor.power()` returns a decimal value (as a *double*) to report the amount of power output being generated.

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

The default unit is `watt` that returns values ranging from **0.0 to 22.0 watts**. 

```cpp
Brain.Screen.print("%f", ClawMotor.power(watt));
```

<advanced>
</advanced>