category: sensing  
signature: Drivetrain.velocity(units)  
device_class: drivetrain  
description: Reports the current velocity of the Drivetrain.

# Drivetrain Velocity

Reports the current velocity of the Drivetrain.

```cpp
Drivetrain.velocity(units)
```

## How to Use
`Drivetrain.velocity` returns a decimal value (as a *double*) to report the current velocity of the Drivetrain. 

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

Acceptable `units` are **percent** and **rpm**.

If the provided `units` parameter is **percent**, the reported values ranges between **-100% to 100%**.

Alternatively, if the provided `units` is **rpm**, the range of reported values vary based on the Gear Catridge installed in the V5 Smart Motors used in the Drivetrain.

* Red Catridge: -100rpm to 100rpm
* Green Catridge: -200rpm to 200rpm
* Blue Catridge: -600rpm to 600rpm

```cpp
Brain.Screen.print("%f", Drivetrain.velocity(percent));
```
<advanced>
</advanced>