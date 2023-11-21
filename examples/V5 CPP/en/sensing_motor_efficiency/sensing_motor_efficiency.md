category: sensing  
signature: MOTOR.efficiency(percent)  
device_class: motor  
description: Reports the efficiency of the V5 Smart Motor or Motor Group.

# Motor Efficiency

Reports the efficiency of a V5 Smart Motor or the first motor of a Motor Group.

```cpp
Motor.efficiency(percent)
```

## How To Use

`Motor.efficiency()` reports the value of the power (in watts) the motor is using (input), versus the amount of power (in watts) the motor is providing (output). 

A V5 Smart Motor or Motor Group typically reaches a maximum efficiency of 65% under normal use cases.

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

`Motor.efficiency()` returns a decimal value (as a *double*) in the default unit of `percent`, and it will return a value from  **0.0% to 100.0%**.

```cpp
Brain.Screen.print("%f", Motor.efficiency(percent));
```
<advanced>
</advanced>
