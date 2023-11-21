category: sensing  
signature: Drivetrain.torque(Nm)  
device_class: drivetrain  
description: Reports the amount of torque (rotational force) the Drivetrain is currently using.

# Drivetrain Torque

Reports the amount of torque (rotational force) the Drivetrain is currently using.

```cpp
Drivetrain.torque(Nm)
```

## How To Use
`Drivetrain.torque(Nm)` returns a decimal as a (*double*) to report the amount of torque (rotational force) the Drivetrain is currently using. 

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

The default return value is Newton-meters(`Nm`) which ranges from **0.0 to 2.1 Newton-meters (Nm)**.

Alternatively, values can only be returned in Inch-pounds(`InLb`).

```cpp
Brain.Screen.print("%f", Drivetrain.torque(Nm));
Brain.Screen.print("%f", Drivetrain.torque(InLb));
```
<advanced>
</advanced>