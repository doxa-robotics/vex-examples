category: sensing  
signature: MOTOR.torque()  
device_class: motor  
description: Reports the amount of torque (rotational force) a EXP Smart Motor or Motor Group is currently using.

# Motor Torque

Reports the amount of torque (rotational force) a EXP Smart Motor or the first motor of a Motor Group is currently using.

```cpp
Motor.torque(Nm)
```

## How To Use

`Motor.torque()` returns a decimal value (as a *double*) to report the amount of torque (rotational force) a EXP Smart Motor or the first motor of a Motor Group is currently using.

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

Values can be returned in Newton-meters(`Nm`) which ranges from **0.0 to 2.1 Newton-meters (Nm)**.

```cpp
Brain.Screen.print("%f", ArmMotor.torque(Nm));
```

Values can be returned in inch-pounds(`InLb`) which ranges from **0.0 to 18.6 inch-pounds (InLb)**. 

```cpp
Brain.Screen.print("%f", ArmMotor.torque(InLb));
```
<advanced>
</advanced>