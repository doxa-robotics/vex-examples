category: sensing  
signature: Drivetrain.temperature(percent)  
device_class: drivetrain  
description: Reports the temperature of the V5 Smart Motors powering the Drivetrain.

# Drivetrain Temperature

Reports the temperature of the V5 Smart Motors powering the Drivetrain.

```cpp
Drivetrain.temperature(percent)
```

## How To Use

`Drivetrain.temperature(percent)` returns a decimal value (as a *double*) to report the temperature of the V5 Smart Motors powering the Drivetrain.  

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

Set `percent` as the unit to get values ranging from **0.0% to 100.0%**. 

```cpp
Brain.Screen.print("%f", Drivetrain.temperature(percent));
```

<advanced>
</advanced>