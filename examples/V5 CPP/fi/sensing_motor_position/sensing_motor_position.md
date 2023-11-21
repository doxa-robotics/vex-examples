category: sensing  
signature: MOTOR.position()  
device_class: motor  
description: Reports the distance the V5 Smart Motor has traveled.

# Motor Position

Reports the distance the V5 Smart Motor has traveled.

```cpp
Motor.position(degrees)
```

## How To Use

`Motor.position()` returns a decimal value (as a *double*) to report the distance the Shaft Encoder has rotated.


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