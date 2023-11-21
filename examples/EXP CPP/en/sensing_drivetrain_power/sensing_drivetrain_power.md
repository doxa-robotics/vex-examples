category: sensing  
signature: Drivetrain.power()  
device_class: drivetrain  
description: Reports the amount of power output the Drivetrain is currently generating.

# Drivetrain Power

Reports the amount of power output the Drivetrain is currently generating.

```cpp
Drivetrain.power()
```

## How To Use
`Drivetrain.power()` returns a decimal value (as a *double*) to report the amount of power output the Drivetrain is currently generating.

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

The default value is `watt` that returns values ranging from **0.0 to 22.0 watts**. 


```cpp
Brain.Screen.print("%f", Drivetrain.power());
```
<advanced>
</advanced>