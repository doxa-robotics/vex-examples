category: sensing  
signature: Drivetrain.efficiency(percent)  
device_class: drivetrain  
description: Reports the efficiency of the Drivetrain.

# Drivetrain Efficiency

Reports the efficiency of the Drivetrain.

```cpp
Drivetrain.efficiency()
```

## How To Use
`Drivetrain.efficiency()` reports the value of the power (in watts) the motors powering the Drivetrain are using (input), versus the amount of power (in watts) the motors powering the Drivetrain are providing (output). 

A V5 Drivetrain typically reaches a maximum efficiency of 65% under normal use cases.

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

`Drivetrain.efficiency()` returns a decimal value (as a *double*) in the default unit of `percent`, and it will return a value from  **0.0% to 100.0%**.

```cpp
Brain.Screen.print("%f", Drivetrain.efficiency());
```
<advanced>
</advanced>