category: sensing  
signature: MOTOR.isDone()  
device_class: motor  
description: Reports if the EXP Smart Motor or Motor Group has completed its movement.

# Motor Is Done

Reports if the EXP Smart Motor or Motor Group has completed its movement.

```cpp
Motor.isDone()
```

## How To Use

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

`Motor.isDone()` reports **true** when the specified Motor or Motor Group has completed its movement.

`Motor.isDone()` reports **false** when the specified Motor or Motor Group has not completed its movement.

```cpp
waitUntil(ClawMotor.isDone());
```
<advanced>
</advanced>