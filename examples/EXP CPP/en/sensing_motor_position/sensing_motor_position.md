category: sensing  
signature: MOTOR.position()  
device_class: motor  
description: Reports the distance the EXP Smart Motor or Motor Group has traveled.

# Motor Position

Reports the distance a EXP Smart Motor or the first motor of a Motor Group has traveled.

```cpp
Motor.position(degrees)
```

## How To Use

`Motor.position()` returns a decimal value (as a *double*) to report the distance the Shaft Encoder in a Motor has rotated.

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

Values can be returned in `degrees`.

```cpp
Brain.Screen.print("%f", ArmMotor.position(degrees));
```

Values can be returned in `turns`.

```cpp
Brain.Screen.print("%f", ArmMotor.position(turns));
```
<advanced>
</advanced> 