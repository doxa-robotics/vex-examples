category: sensing  
signature: MOTOR.direction()  
device_class: motor  
description: Reports the direction a EXP Smart Motor is currently spinning.

# Motor.direction()

Reports the direction a EXP Smart Motor is currently spinning.

```cpp
Motor.direction()
```

## How To Use

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

`Motor.current()` returns a **directionType** value, so it will return either `forward` or `reverse`.


```cpp
if (LeftMotor.direction() == forward) {
    Brain.Screen.print("Left Motor is spinning forward!");
}
```
**Note:** The semicolon in the example above is used by the `print` command.
<advanced>
</advanced>